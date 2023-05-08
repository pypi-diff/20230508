# Comparing `tmp/lixinger-0.1.3.tar.gz` & `tmp/lixinger-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lixinger-0.1.3.tar", last modified: Thu May  4 14:33:31 2023, max compression
+gzip compressed data, was "lixinger-0.1.4.tar", last modified: Sun May  7 15:11:35 2023, max compression
```

## Comparing `lixinger-0.1.3.tar` & `lixinger-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,42 @@
--rw-r--r--   0        0        0      705 2023-05-03 10:11:52.615764 lixinger-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-05-01 04:05:58.277552 lixinger-0.1.3/lixinger/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:33:35.225361 lixinger-0.1.3/lixinger/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:22.152169 lixinger-0.1.3/lixinger/api/cn/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:09:36.967425 lixinger-0.1.3/lixinger/api/cn/company/__init__.py
--rw-r--r--   0        0        0     2132 2023-05-04 10:40:12.138787 lixinger-0.1.3/lixinger/api/cn/company/base.py
--rw-r--r--   0        0        0        0 2023-05-04 14:21:25.826889 lixinger-0.1.3/lixinger/api/cn/fund/__init__.py
--rw-r--r--   0        0        0     1161 2023-05-04 14:31:57.646244 lixinger-0.1.3/lixinger/api/cn/fund/total_net_value.py
--rw-r--r--   0        0        0        0 2023-05-01 05:10:55.043163 lixinger-0.1.3/lixinger/api/cn/index/__init__.py
--rw-r--r--   0        0        0     1721 2023-05-04 10:40:12.140548 lixinger-0.1.3/lixinger/api/cn/index/fundamental.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:31.838744 lixinger-0.1.3/lixinger/api/hk/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:09:00.179536 lixinger-0.1.3/lixinger/api/macro/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:44.656824 lixinger-0.1.3/lixinger/api/us/__init__.py
--rw-r--r--   0        0        0     1582 2023-05-04 10:40:12.141591 lixinger-0.1.3/lixinger/config.py
--rw-r--r--   0        0        0        0 2023-05-03 09:27:58.212202 lixinger-0.1.3/lixinger/py.typed
--rw-r--r--   0        0        0       75 2023-05-03 10:06:41.922780 lixinger-0.1.3/lixinger/settings.toml
--rw-r--r--   0        0        0      978 2023-05-04 10:40:12.142362 lixinger-0.1.3/lixinger/utils.py
--rw-r--r--   0        0        0      986 2023-05-04 14:33:31.621192 lixinger-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-01 04:43:15.660305 lixinger-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:19.505533 lixinger-0.1.3/tests/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:24.536685 lixinger-0.1.3/tests/api/cn/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:30.757795 lixinger-0.1.3/tests/api/cn/company/__init__.py
--rw-r--r--   0        0        0      127 2023-05-03 10:00:15.081563 lixinger-0.1.3/tests/api/cn/company/test_base.py
--rw-r--r--   0        0        0        0 2023-05-04 14:30:00.736254 lixinger-0.1.3/tests/api/cn/fund/__init__.py
--rw-r--r--   0        0        0      229 2023-05-04 14:32:35.703103 lixinger-0.1.3/tests/api/cn/fund/test_total_net_value.py
--rw-r--r--   0        0        0        0 2023-05-01 05:16:11.323717 lixinger-0.1.3/tests/api/cn/index/__init__.py
--rw-r--r--   0        0        0      270 2023-05-03 09:27:22.076125 lixinger-0.1.3/tests/api/cn/index/test_fundamental.py
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 lixinger-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      705 2023-05-03 10:11:52.615764 lixinger-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-01 04:05:58.277552 lixinger-0.1.4/lixinger/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:33:35.225361 lixinger-0.1.4/lixinger/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:22.152169 lixinger-0.1.4/lixinger/api/cn/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:09:36.967425 lixinger-0.1.4/lixinger/api/cn/company/__init__.py
+-rw-r--r--   0        0        0     2133 2023-05-07 15:03:30.274209 lixinger-0.1.4/lixinger/api/cn/company/base.py
+-rw-r--r--   0        0        0     1809 2023-05-07 15:03:30.267374 lixinger-0.1.4/lixinger/api/cn/company/candlestick.py
+-rw-r--r--   0        0        0     2315 2023-05-07 15:03:30.260733 lixinger-0.1.4/lixinger/api/cn/company/dividend_and_alloment.py
+-rw-r--r--   0        0        0     1369 2023-05-07 15:03:30.277996 lixinger-0.1.4/lixinger/api/cn/company/equity_change.py
+-rw-r--r--   0        0        0     1471 2023-05-07 15:02:40.594443 lixinger-0.1.4/lixinger/api/cn/company/senior_executive_shares_change.py
+-rw-r--r--   0        0        0     1205 2023-05-07 15:03:30.276496 lixinger-0.1.4/lixinger/api/cn/company/shareholders_num.py
+-rw-r--r--   0        0        0        0 2023-05-04 14:21:25.826889 lixinger-0.1.4/lixinger/api/cn/fund/__init__.py
+-rw-r--r--   0        0        0     1341 2023-05-07 15:03:30.271585 lixinger-0.1.4/lixinger/api/cn/fund/exchange_traded_close_price.py
+-rw-r--r--   0        0        0     1216 2023-05-07 15:03:30.268973 lixinger-0.1.4/lixinger/api/cn/fund/total_net_value.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:10:55.043163 lixinger-0.1.4/lixinger/api/cn/index/__init__.py
+-rw-r--r--   0        0        0     1485 2023-05-07 15:03:30.264992 lixinger-0.1.4/lixinger/api/cn/index/candlestick.py
+-rw-r--r--   0        0        0     1776 2023-05-07 15:03:30.270211 lixinger-0.1.4/lixinger/api/cn/index/fundamental.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:31.838744 lixinger-0.1.4/lixinger/api/hk/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:09:00.179536 lixinger-0.1.4/lixinger/api/macro/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:44.656824 lixinger-0.1.4/lixinger/api/us/__init__.py
+-rw-r--r--   0        0        0     1582 2023-05-04 10:40:12.141591 lixinger-0.1.4/lixinger/config.py
+-rw-r--r--   0        0        0        0 2023-05-03 09:27:58.212202 lixinger-0.1.4/lixinger/py.typed
+-rw-r--r--   0        0        0       75 2023-05-03 10:06:41.922780 lixinger-0.1.4/lixinger/settings.toml
+-rw-r--r--   0        0        0     2959 2023-05-07 15:10:46.242850 lixinger-0.1.4/lixinger/utils.py
+-rw-r--r--   0        0        0      912 2023-05-07 15:11:35.753687 lixinger-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:15.660305 lixinger-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:19.505533 lixinger-0.1.4/tests/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:24.536685 lixinger-0.1.4/tests/api/cn/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:30.757795 lixinger-0.1.4/tests/api/cn/company/__init__.py
+-rw-r--r--   0        0        0      127 2023-05-03 10:00:15.081563 lixinger-0.1.4/tests/api/cn/company/test_base.py
+-rw-r--r--   0        0        0      187 2023-05-07 03:59:49.667512 lixinger-0.1.4/tests/api/cn/company/test_candlestick.py
+-rw-r--r--   0        0        0      217 2023-05-06 05:43:46.770904 lixinger-0.1.4/tests/api/cn/company/test_dividend_and_alloment.py
+-rw-r--r--   0        0        0      170 2023-05-06 02:12:57.131245 lixinger-0.1.4/tests/api/cn/company/test_equity_change.py
+-rw-r--r--   0        0        0      235 2023-05-07 15:03:11.303695 lixinger-0.1.4/tests/api/cn/company/test_senior_executive_shares_change.py
+-rw-r--r--   0        0        0      184 2023-05-07 14:29:15.357398 lixinger-0.1.4/tests/api/cn/company/test_shareholders_num.py
+-rw-r--r--   0        0        0        0 2023-05-04 14:30:00.736254 lixinger-0.1.4/tests/api/cn/fund/__init__.py
+-rw-r--r--   0        0        0      238 2023-05-07 02:06:30.724314 lixinger-0.1.4/tests/api/cn/fund/test_exchange_traded_close_price.py
+-rw-r--r--   0        0        0      229 2023-05-04 14:32:35.703103 lixinger-0.1.4/tests/api/cn/fund/test_total_net_value.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:16:11.323717 lixinger-0.1.4/tests/api/cn/index/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-07 01:58:13.309631 lixinger-0.1.4/tests/api/cn/index/test_candlestick.py
+-rw-r--r--   0        0        0      270 2023-05-03 09:27:22.076125 lixinger-0.1.4/tests/api/cn/index/test_fundamental.py
+-rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 lixinger-0.1.4/PKG-INFO
```

### Comparing `lixinger-0.1.3/README.md` & `lixinger-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.3/lixinger/api/cn/company/base.py` & `lixinger-0.1.4/lixinger/api/cn/company/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         nullable=True
     )
 
 
 @validate_arguments
 @pa.check_types
 def get_company(
-    *,
     fs_type: Literal[
         "non_financial", "bank", "insurance", "security", "other_financial"
     ]
     | None = None,
     mutual_markets: Literal["ha"] | None = None,
     stock_codes: list[str] | None = None,
     include_delisted: bool | None = None,
@@ -52,15 +51,15 @@
     if include_delisted is not None:
         payload["includeDelisted"] = include_delisted
 
     response = requests.post(
         f"{settings.base_url}/cn/company",
         json=payload,
     )
-    df = get_response_df(response)
+    df = get_response_df(response, Output)
     df["ipo_date"] = pd.to_datetime(df["ipo_date"]).dt.tz_localize(None)
     if "delisted_date" in df.columns:
         df["delisted_date"] = pd.to_datetime(df["delisted_date"]).dt.tz_localize(None)
 
     if "mutual_markets" in df.columns:
         df["mutual_markets"] = [
             convert_column_list_to_str(column) for column in df["mutual_markets"]
```

### Comparing `lixinger-0.1.3/lixinger/api/cn/fund/total_net_value.py` & `lixinger-0.1.4/lixinger/api/cn/fund/total_net_value.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 import pandas as pd
 import pandera as pa
 import requests
 from pydantic import validate_arguments
 
 from lixinger.config import settings
-from lixinger.utils import get_response_df
+from lixinger.utils import adjust_request_date_range, get_response_df
 
 
 class Output(pa.DataFrameModel):
     date: pa.typing.Series[pa.typing.DateTime]
     total_net_value: pa.typing.Series[float]
 
 
 @validate_arguments
 @pa.check_types
+@adjust_request_date_range
 def get_total_net_value(
-    *,
     start_date: str,
+    stock_code: str,
     end_date: str | None = None,
     limit: int | None = None,
-    stock_code: str,
 ) -> pa.typing.DataFrame[Output]:
     """获取基金累计净值数据
 
     参考文档: https://www.lixinger.com/open/api/doc?api-key=cn/fund/total-net-value
     """
     payload = {
         "token": settings.token,
@@ -37,10 +37,10 @@
     if limit is not None:
         payload["limit"] = limit
 
     response = requests.post(
         f"{settings.base_url}/cn/fund/total-net-value",
         json=payload,
     )
-    df = get_response_df(response)
+    df = get_response_df(response, Output)
     df["date"] = pd.to_datetime(df["date"]).dt.tz_localize(None)
     return df
```

### Comparing `lixinger-0.1.3/lixinger/api/cn/index/fundamental.py` & `lixinger-0.1.4/lixinger/api/cn/index/fundamental.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 
 import pandas as pd
 import pandera as pa
 import requests
 from pydantic import validate_arguments
 
 from lixinger.config import settings
-from lixinger.utils import get_response_df
+from lixinger.utils import adjust_request_date_range, get_response_df
 
 
 class Output(pa.DataFrameModel):
     date: pa.typing.Series[pa.typing.DateTime]
     stock_code: pa.typing.Series[str]
 
 
 @validate_arguments
 @pa.check_types
+@adjust_request_date_range
 def get_index_fundamental(
-    *,
+    stock_codes: list[str],
+    metrics_list: list[str],
     date: str | None = None,
     start_date: str | None = None,
     end_date: str | None = None,
     adjust_forward_date: str | None = None,
     adjust_backward_date: str | None = None,
     limit: int | None = None,
-    stock_codes: list[str],
-    metrics_list: list[str],
 ) -> pa.typing.DataFrame[Output]:
     """获取基本面数据，如PE、PB等.
 
     参考文档: https://www.lixinger.com/open/api/doc?api-key=cn/index/fundamental
     """
     payload = {
         "token": settings.token,
@@ -48,11 +48,11 @@
         payload["adjustBackwardDate"] = adjust_backward_date
     if limit is not None:
         payload["limit"] = limit
     response = requests.post(
         f"{settings.base_url}/cn/index/fundamental",
         json=payload,
     )
-    df = get_response_df(response)
+    df = get_response_df(response, Output)
     df["date"] = pd.to_datetime(df["date"]).dt.tz_localize(None)
     df.sort_values(by=["date", "stock_code"], inplace=True)
     return df
```

### Comparing `lixinger-0.1.3/lixinger/config.py` & `lixinger-0.1.4/lixinger/config.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.3/pyproject.toml` & `lixinger-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=7.3.1",
+    "ipython>=8.12.2",
 ]
 
 [tool.pytest.ini_options]
 cache_dir = ".pytest_cache/"
 addopts = "-s -p no:warnings"
 asyncio_mode = "auto"
 
 [project]
 name = "lixinger"
-version = "0.1.3"
+version = "0.1.4"
 description = "Lixinger SDK for Python (Unofficial)"
 authors = [
     { name = "Chaoying", email = "chaoying2022@gmail.com" },
 ]
 dependencies = [
     "pandera>=0.14.5",
     "pydantic>=1.10.7",
     "requests>=2.29.0",
     "dynaconf>=3.1.12",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "lixinger",
 ]
 classifiers = [
-    "Topic :: Software Development :: Build Tools",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [project.license]
```

### Comparing `lixinger-0.1.3/PKG-INFO` & `lixinger-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: lixinger
-Version: 0.1.3
+Version: 0.1.4
 Summary: Lixinger SDK for Python (Unofficial)
 Keywords: lixinger
 Author-Email: Chaoying <chaoying2022@gmail.com>
 License: MIT
-Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: pandera>=0.14.5
 Requires-Dist: pydantic>=1.10.7
 Requires-Dist: requests>=2.29.0
 Requires-Dist: dynaconf>=3.1.12
 Description-Content-Type: text/markdown
 
 # lixinger
```

