# Comparing `tmp/zillionare_omicron-2.0.0a67.tar.gz` & `tmp/zillionare_omicron-2.0.0a68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zillionare_omicron-2.0.0a67.tar", max compression
+gzip compressed data, was "zillionare_omicron-2.0.0a68.tar", max compression
```

## Comparing `zillionare_omicron-2.0.0a67.tar` & `zillionare_omicron-2.0.0a68.tar`

### file list

```diff
@@ -1,124 +1,125 @@
--rw-r--r--   0        0        0      112 2023-01-24 12:41:24.903079 zillionare_omicron-2.0.0a67/AUTHORS.md
--rw-r--r--   0        0        0     1561 2023-01-24 12:41:24.903079 zillionare_omicron-2.0.0a67/HISTORY.md
--rw-r--r--   0        0        0     1068 2023-01-19 03:32:37.450696 zillionare_omicron-2.0.0a67/LICENSE
--rw-r--r--   0        0        0     1331 2023-05-07 03:30:41.208098 zillionare_omicron-2.0.0a67/README.md
--rw-r--r--   0        0        0   503846 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/_static/Omicron_Windows10.docx
--rw-r--r--   0        0        0     5620 2023-01-19 03:32:37.450696 zillionare_omicron-2.0.0a67/docs/_static/jetbrains-variant-3.svg
--rw-r--r--   0        0        0       84 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/api/dal/flux.md
--rw-r--r--   0        0        0      110 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/api/dal/influxclient.md
--rw-r--r--   0        0        0      189 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/api/dal/serialize.md
--rw-r--r--   0        0        0     5772 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/api/metrics.md
--rw-r--r--   0        0        0      203 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/api/omicron.md
--rw-r--r--   0        0        0      142 2023-05-07 03:32:06.872770 zillionare_omicron-2.0.0a67/docs/api/plotting.md
--rw-r--r--   0        0        0       68 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/api/security.md
--rw-r--r--   0        0        0       65 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/api/stock.md
--rw-r--r--   0        0        0       21 2023-05-07 03:32:19.736871 zillionare_omicron-2.0.0a67/docs/api/strategy.md
--rw-r--r--   0        0        0       58 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/api/talib.md
--rw-r--r--   0        0        0       57 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/api/timeframe.md
--rw-r--r--   0        0        0       66 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a67/docs/api/triggers.md
--rw-r--r--   0        0        0      907 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a67/docs/css/extra.css
--rw-r--r--   0        0        0     1778 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/developer.md
--rw-r--r--   0        0        0       43 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a67/docs/history.md
--rw-r--r--   0        0        0       42 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a67/docs/index.md
--rw-r--r--   0        0        0     1820 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/installation.md
--rw-r--r--   0        0        0     9823 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/usage.md
--rw-r--r--   0        0        0      920 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/omicron/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/omicron/config/__init__.py
--rw-r--r--   0        0        0    56389 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/config/calendar.json
--rw-r--r--   0        0        0      441 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/config/defaults.yaml
--rw-r--r--   0        0        0      378 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/config/dev.yaml
--rw-r--r--   0        0        0     1334 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/config/schema.py
--rw-r--r--   0        0        0      816 2023-01-19 03:32:37.458696 zillionare_omicron-2.0.0a67/omicron/config/sql/v0.6.sql
--rw-r--r--   0        0        0     2785 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/config/sql/v1.0.sql
--rw-r--r--   0        0        0       46 2023-01-19 03:32:37.458696 zillionare_omicron-2.0.0a67/omicron/core/__init__.py
--rw-r--r--   0        0        0      140 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/core/constants.py
--rw-r--r--   0        0        0     1095 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/core/errors.py
--rw-r--r--   0        0        0       46 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/core/events.py
--rw-r--r--   0        0        0     6517 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/core/triggers.py
--rw-r--r--   0        0        0       71 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/dal/__init__.py
--rw-r--r--   0        0        0     3215 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/dal/cache.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/dal/influx/__init__.py
--rw-r--r--   0        0        0      370 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/dal/influx/errors.py
--rw-r--r--   0        0        0      996 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/dal/influx/escape.py
--rw-r--r--   0        0        0    19097 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a67/omicron/dal/influx/flux.py
--rw-r--r--   0        0        0    16805 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a67/omicron/dal/influx/influxclient.py
--rw-r--r--   0        0        0    27708 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a67/omicron/dal/influx/serialize.py
--rw-r--r--   0        0        0       78 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a67/omicron/extensions/__init__.py
--rw-r--r--   0        0        0      656 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a67/omicron/extensions/decimals.py
--rw-r--r--   0        0        0    15929 2023-05-01 02:32:25.512887 zillionare_omicron-2.0.0a67/omicron/extensions/np.py
--rw-r--r--   0        0        0      492 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a67/omicron/models/__init__.py
--rw-r--r--   0        0        0     7867 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a67/omicron/models/board.py
--rw-r--r--   0        0        0    26127 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a67/omicron/models/security.py
--rw-r--r--   0        0        0    53741 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a67/omicron/models/stock.py
--rw-r--r--   0        0        0    41959 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a67/omicron/models/timeframe.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a67/omicron/notify/__init__.py
--rw-r--r--   0        0        0     5472 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a67/omicron/notify/dingtalk.py
--rw-r--r--   0        0        0     6006 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a67/omicron/notify/mail.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a67/omicron/notify/tts.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a67/omicron/plotting/__init__.py
--rw-r--r--   0        0        0    14220 2023-05-03 09:06:32.908144 zillionare_omicron-2.0.0a67/omicron/plotting/candlestick.py
--rw-r--r--   0        0        0     9039 2023-05-07 05:01:15.503704 zillionare_omicron-2.0.0a67/omicron/plotting/metrics.py
--rw-r--r--   0        0        0        0 2023-05-07 01:07:54.376952 zillionare_omicron-2.0.0a67/omicron/strategy/__init__.py
--rw-r--r--   0        0        0     8912 2023-05-07 03:40:18.247316 zillionare_omicron-2.0.0a67/omicron/strategy/base.py
--rw-r--r--   0        0        0     1099 2023-05-07 02:09:33.855184 zillionare_omicron-2.0.0a67/omicron/strategy/sma.py
--rw-r--r--   0        0        0      114 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a67/omicron/talib/__init__.py
--rw-r--r--   0        0        0     9958 2023-01-24 12:41:24.927079 zillionare_omicron-2.0.0a67/omicron/talib/core.py
--rw-r--r--   0        0        0    23141 2023-01-24 12:41:24.927079 zillionare_omicron-2.0.0a67/omicron/talib/morph.py
--rwxr-xr-x   0        0        0     3391 2023-05-07 04:10:04.992167 zillionare_omicron-2.0.0a67/pyproject.toml
--rw-r--r--   0        0        0     5556 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a67/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a67/tests/core/__init__.py
--rw-r--r--   0        0        0      297 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a67/tests/core/test_errors.py
--rw-r--r--   0        0        0     3615 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a67/tests/core/test_triggers.py
--rw-r--r--   0        0        0     1024 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/core/test_types.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/dal/__init__.py
--rw-r--r--   0        0        0      622 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/dal/influx/__init__.py
--rw-r--r--   0        0        0     1177 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/dal/influx/test_escape.py
--rw-r--r--   0        0        0     8531 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/dal/influx/test_flux.py
--rw-r--r--   0        0        0    14284 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/dal/influx/test_influxclient.py
--rw-r--r--   0        0        0    15710 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/dal/influx/test_serialize.py
--rw-r--r--   0        0        0     1253 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.15m.csv
--rw-r--r--   0        0        0      118 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.1M.csv
--rw-r--r--   0        0        0      188 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.1d.csv
--rw-r--r--   0        0        0    22206 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.1m.csv
--rw-r--r--   0        0        0      115 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.1w.csv
--rw-r--r--   0        0        0      654 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.30m.csv
--rw-r--r--   0        0        0     3633 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.5m.csv
--rw-r--r--   0        0        0      352 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.60m.csv
--rw-r--r--   0        0        0  1059606 2023-05-07 02:32:26.029160 zillionare_omicron-2.0.0a67/tests/data/000001.XSHG.1m.csv
--rw-r--r--   0        0        0     8089 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/data/000002.XSHE.1d.csv
--rw-r--r--   0        0        0    22419 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a67/tests/data/000002.XSHE.1m.csv
--rw-r--r--   0        0        0     7166 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a67/tests/data/000002.XSHE.1w.csv
--rw-r--r--   0        0        0     8096 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a67/tests/data/000002.XSHE.30m.csv
--rw-r--r--   0        0        0     7585 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a67/tests/data/000004.XSHE.1d.csv
--rw-r--r--   0        0        0    20344 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a67/tests/data/000004.XSHE.1m.csv
--rw-r--r--   0        0        0     6443 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a67/tests/data/000004.XSHE.1w.csv
--rw-r--r--   0        0        0     7688 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a67/tests/data/000004.XSHE.30m.csv
--rw-r--r--   0        0        0     4206 2023-05-07 02:31:54.553073 zillionare_omicron-2.0.0a67/tests/data/600000.XSHG.1d.csv
--rw-r--r--   0        0        0     1145 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a67/tests/data/README.md
--rw-r--r--   0        0        0     2191 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a67/tests/data/bars_1d.pkl
--rw-r--r--   0        0        0   408697 2023-01-24 12:41:24.943079 zillionare_omicron-2.0.0a67/tests/data/bars_1m.pkl
--rw-r--r--   0        0        0      713 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a67/tests/data/limits.csv
--rw-r--r--   0        0        0   164066 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a67/tests/data/stock_bars_flux_query.txt
--rw-r--r--   0        0        0     6315 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a67/tests/data/test.jpg
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a67/tests/extensions/__init__.py
--rw-r--r--   0        0        0      594 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a67/tests/extensions/test_decimals.py
--rw-r--r--   0        0        0     9864 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a67/tests/extensions/test_np.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a67/tests/models/__init__.py
--rw-r--r--   0        0        0     6802 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a67/tests/models/test_board.py
--rw-r--r--   0        0        0    11161 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a67/tests/models/test_security.py
--rw-r--r--   0        0        0    68822 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/models/test_stock.py
--rw-r--r--   0        0        0    36351 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/models/test_timeframe.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/notify/__init__.py
--rw-r--r--   0        0        0      823 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/notify/test_dingtalk.py
--rw-r--r--   0        0        0     2686 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/notify/test_mail.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/performance/influx/__init__.py
--rw-r--r--   0        0        0     3317 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/performance/influx/end2end.py
--rw-r--r--   0        0        0     4197 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/performance/influx/serialize.py
--rw-r--r--   0        0        0      294 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/performance/readme.md
--rw-r--r--   0        0        0      406 2023-01-19 03:32:37.466696 zillionare_omicron-2.0.0a67/tests/pyrightconfig.json
--rw-r--r--   0        0        0        0 2023-05-07 02:10:22.915444 zillionare_omicron-2.0.0a67/tests/strategy/__init__.py
--rw-r--r--   0        0        0     1517 2023-05-07 03:14:15.795948 zillionare_omicron-2.0.0a67/tests/strategy/test_strategy.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/talib/__init__.py
--rw-r--r--   0        0        0     2917 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/talib/test_core.py
--rw-r--r--   0        0        0    37991 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/talib/test_morph.py
--rw-r--r--   0        0        0     4334 1970-01-01 00:00:00.000000 zillionare_omicron-2.0.0a67/PKG-INFO
+-rw-r--r--   0        0        0      112 2023-01-24 12:41:24.903079 zillionare_omicron-2.0.0a68/AUTHORS.md
+-rw-r--r--   0        0        0     1663 2023-05-08 08:54:41.853890 zillionare_omicron-2.0.0a68/HISTORY.md
+-rw-r--r--   0        0        0     1068 2023-01-19 03:32:37.450696 zillionare_omicron-2.0.0a68/LICENSE
+-rw-r--r--   0        0        0     1331 2023-05-07 03:30:41.208098 zillionare_omicron-2.0.0a68/README.md
+-rw-r--r--   0        0        0   503846 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/_static/Omicron_Windows10.docx
+-rw-r--r--   0        0        0     5620 2023-01-19 03:32:37.450696 zillionare_omicron-2.0.0a68/docs/_static/jetbrains-variant-3.svg
+-rw-r--r--   0        0        0       84 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/api/dal/flux.md
+-rw-r--r--   0        0        0      110 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/api/dal/influxclient.md
+-rw-r--r--   0        0        0      189 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/api/dal/serialize.md
+-rw-r--r--   0        0        0     5772 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/api/metrics.md
+-rw-r--r--   0        0        0      203 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/api/omicron.md
+-rw-r--r--   0        0        0       73 2023-05-08 07:55:54.700078 zillionare_omicron-2.0.0a68/docs/api/plotting/candlestick.md
+-rw-r--r--   0        0        0       69 2023-05-08 07:55:45.740005 zillionare_omicron-2.0.0a68/docs/api/plotting/metrics.md
+-rw-r--r--   0        0        0       68 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/api/security.md
+-rw-r--r--   0        0        0       65 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/api/stock.md
+-rw-r--r--   0        0        0       21 2023-05-07 03:32:19.736871 zillionare_omicron-2.0.0a68/docs/api/strategy.md
+-rw-r--r--   0        0        0       58 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/api/talib.md
+-rw-r--r--   0        0        0       57 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/api/timeframe.md
+-rw-r--r--   0        0        0       66 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a68/docs/api/triggers.md
+-rw-r--r--   0        0        0      907 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a68/docs/css/extra.css
+-rw-r--r--   0        0        0     1778 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/developer.md
+-rw-r--r--   0        0        0       43 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a68/docs/history.md
+-rw-r--r--   0        0        0       42 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a68/docs/index.md
+-rw-r--r--   0        0        0     1820 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/installation.md
+-rw-r--r--   0        0        0     9823 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/usage.md
+-rw-r--r--   0        0        0      920 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/omicron/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/omicron/config/__init__.py
+-rw-r--r--   0        0        0    56389 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/config/calendar.json
+-rw-r--r--   0        0        0      441 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/config/defaults.yaml
+-rw-r--r--   0        0        0      378 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/config/dev.yaml
+-rw-r--r--   0        0        0     1334 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/config/schema.py
+-rw-r--r--   0        0        0      816 2023-01-19 03:32:37.458696 zillionare_omicron-2.0.0a68/omicron/config/sql/v0.6.sql
+-rw-r--r--   0        0        0     2785 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/config/sql/v1.0.sql
+-rw-r--r--   0        0        0       46 2023-01-19 03:32:37.458696 zillionare_omicron-2.0.0a68/omicron/core/__init__.py
+-rw-r--r--   0        0        0      140 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/core/constants.py
+-rw-r--r--   0        0        0     1095 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/core/errors.py
+-rw-r--r--   0        0        0       46 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/core/events.py
+-rw-r--r--   0        0        0     6517 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/core/triggers.py
+-rw-r--r--   0        0        0       71 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/dal/__init__.py
+-rw-r--r--   0        0        0     3215 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/dal/cache.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/dal/influx/__init__.py
+-rw-r--r--   0        0        0      370 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/dal/influx/errors.py
+-rw-r--r--   0        0        0      996 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/dal/influx/escape.py
+-rw-r--r--   0        0        0    19097 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a68/omicron/dal/influx/flux.py
+-rw-r--r--   0        0        0    16805 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a68/omicron/dal/influx/influxclient.py
+-rw-r--r--   0        0        0    27708 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a68/omicron/dal/influx/serialize.py
+-rw-r--r--   0        0        0       78 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a68/omicron/extensions/__init__.py
+-rw-r--r--   0        0        0      656 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a68/omicron/extensions/decimals.py
+-rw-r--r--   0        0        0    15929 2023-05-01 02:32:25.512887 zillionare_omicron-2.0.0a68/omicron/extensions/np.py
+-rw-r--r--   0        0        0      492 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a68/omicron/models/__init__.py
+-rw-r--r--   0        0        0     7867 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a68/omicron/models/board.py
+-rw-r--r--   0        0        0    26127 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a68/omicron/models/security.py
+-rw-r--r--   0        0        0    53741 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a68/omicron/models/stock.py
+-rw-r--r--   0        0        0    41959 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a68/omicron/models/timeframe.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a68/omicron/notify/__init__.py
+-rw-r--r--   0        0        0     5472 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a68/omicron/notify/dingtalk.py
+-rw-r--r--   0        0        0     6006 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a68/omicron/notify/mail.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a68/omicron/notify/tts.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a68/omicron/plotting/__init__.py
+-rw-r--r--   0        0        0    16523 2023-05-08 08:53:56.981283 zillionare_omicron-2.0.0a68/omicron/plotting/candlestick.py
+-rw-r--r--   0        0        0     8474 2023-05-08 08:53:20.740774 zillionare_omicron-2.0.0a68/omicron/plotting/metrics.py
+-rw-r--r--   0        0        0        0 2023-05-07 01:07:54.376952 zillionare_omicron-2.0.0a68/omicron/strategy/__init__.py
+-rw-r--r--   0        0        0     8909 2023-05-08 08:01:12.268255 zillionare_omicron-2.0.0a68/omicron/strategy/base.py
+-rw-r--r--   0        0        0     1099 2023-05-07 02:09:33.855184 zillionare_omicron-2.0.0a68/omicron/strategy/sma.py
+-rw-r--r--   0        0        0      114 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a68/omicron/talib/__init__.py
+-rw-r--r--   0        0        0     9958 2023-01-24 12:41:24.927079 zillionare_omicron-2.0.0a68/omicron/talib/core.py
+-rw-r--r--   0        0        0    23141 2023-01-24 12:41:24.927079 zillionare_omicron-2.0.0a68/omicron/talib/morph.py
+-rwxr-xr-x   0        0        0     3391 2023-05-08 07:56:23.256312 zillionare_omicron-2.0.0a68/pyproject.toml
+-rw-r--r--   0        0        0     5556 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a68/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a68/tests/core/__init__.py
+-rw-r--r--   0        0        0      297 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a68/tests/core/test_errors.py
+-rw-r--r--   0        0        0     3615 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a68/tests/core/test_triggers.py
+-rw-r--r--   0        0        0     1024 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/core/test_types.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/dal/__init__.py
+-rw-r--r--   0        0        0      622 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/dal/influx/__init__.py
+-rw-r--r--   0        0        0     1177 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/dal/influx/test_escape.py
+-rw-r--r--   0        0        0     8531 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/dal/influx/test_flux.py
+-rw-r--r--   0        0        0    14284 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/dal/influx/test_influxclient.py
+-rw-r--r--   0        0        0    15710 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/dal/influx/test_serialize.py
+-rw-r--r--   0        0        0     1253 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.15m.csv
+-rw-r--r--   0        0        0      118 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.1M.csv
+-rw-r--r--   0        0        0      188 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.1d.csv
+-rw-r--r--   0        0        0    22206 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.1m.csv
+-rw-r--r--   0        0        0      115 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.1w.csv
+-rw-r--r--   0        0        0      654 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.30m.csv
+-rw-r--r--   0        0        0     3633 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.5m.csv
+-rw-r--r--   0        0        0      352 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.60m.csv
+-rw-r--r--   0        0        0  1059606 2023-05-07 02:32:26.029160 zillionare_omicron-2.0.0a68/tests/data/000001.XSHG.1m.csv
+-rw-r--r--   0        0        0     8089 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/data/000002.XSHE.1d.csv
+-rw-r--r--   0        0        0    22419 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a68/tests/data/000002.XSHE.1m.csv
+-rw-r--r--   0        0        0     7166 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a68/tests/data/000002.XSHE.1w.csv
+-rw-r--r--   0        0        0     8096 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a68/tests/data/000002.XSHE.30m.csv
+-rw-r--r--   0        0        0     7585 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a68/tests/data/000004.XSHE.1d.csv
+-rw-r--r--   0        0        0    20344 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a68/tests/data/000004.XSHE.1m.csv
+-rw-r--r--   0        0        0     6443 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a68/tests/data/000004.XSHE.1w.csv
+-rw-r--r--   0        0        0     7688 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a68/tests/data/000004.XSHE.30m.csv
+-rw-r--r--   0        0        0     4206 2023-05-07 02:31:54.553073 zillionare_omicron-2.0.0a68/tests/data/600000.XSHG.1d.csv
+-rw-r--r--   0        0        0     1145 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a68/tests/data/README.md
+-rw-r--r--   0        0        0     2191 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a68/tests/data/bars_1d.pkl
+-rw-r--r--   0        0        0   408697 2023-01-24 12:41:24.943079 zillionare_omicron-2.0.0a68/tests/data/bars_1m.pkl
+-rw-r--r--   0        0        0      713 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a68/tests/data/limits.csv
+-rw-r--r--   0        0        0   164066 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a68/tests/data/stock_bars_flux_query.txt
+-rw-r--r--   0        0        0     6315 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a68/tests/data/test.jpg
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a68/tests/extensions/__init__.py
+-rw-r--r--   0        0        0      594 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a68/tests/extensions/test_decimals.py
+-rw-r--r--   0        0        0     9864 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a68/tests/extensions/test_np.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a68/tests/models/__init__.py
+-rw-r--r--   0        0        0     6802 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a68/tests/models/test_board.py
+-rw-r--r--   0        0        0    11161 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a68/tests/models/test_security.py
+-rw-r--r--   0        0        0    68822 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/models/test_stock.py
+-rw-r--r--   0        0        0    36351 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/models/test_timeframe.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/notify/__init__.py
+-rw-r--r--   0        0        0      823 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/notify/test_dingtalk.py
+-rw-r--r--   0        0        0     2686 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/notify/test_mail.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/performance/influx/__init__.py
+-rw-r--r--   0        0        0     3317 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/performance/influx/end2end.py
+-rw-r--r--   0        0        0     4197 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/performance/influx/serialize.py
+-rw-r--r--   0        0        0      294 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/performance/readme.md
+-rw-r--r--   0        0        0      406 2023-01-19 03:32:37.466696 zillionare_omicron-2.0.0a68/tests/pyrightconfig.json
+-rw-r--r--   0        0        0        0 2023-05-07 02:10:22.915444 zillionare_omicron-2.0.0a68/tests/strategy/__init__.py
+-rw-r--r--   0        0        0     1517 2023-05-07 03:14:15.795948 zillionare_omicron-2.0.0a68/tests/strategy/test_strategy.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/talib/__init__.py
+-rw-r--r--   0        0        0     2917 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/talib/test_core.py
+-rw-r--r--   0        0        0    37991 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/talib/test_morph.py
+-rw-r--r--   0        0        0     4334 1970-01-01 00:00:00.000000 zillionare_omicron-2.0.0a68/PKG-INFO
```

### Comparing `zillionare_omicron-2.0.0a67/HISTORY.md` & `zillionare_omicron-2.0.0a68/HISTORY.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # History
 
-
+## 2.0.0-alpha.68
+* 增加了MetricsGraph
+* 增加Strategy基类
+* Candlestick增加了布林带指标
 ## 2.0.0-alpha.49 (2022-09-16)
 * 修订了安装文档。
 * 移除了windows下对ta-lib的依赖。请参考[安装指南](docs/installation.md)以获取在windows下安装ta-lib的方法。
 * 更新了poetry.lock文件。在上一版中，该文件与pyproject.toml不同步，导致安装时进行版本锁定，延长了安装时间。
 * 修复了k线图标记顶和底时，标记离被标注的点太远的问题。
 ## 2.0.0-alpha.46 (2022-09-10)
 * [#40](https://github.com/zillionare/omicron/issues/40) 增加k线图绘制功能。
```

### Comparing `zillionare_omicron-2.0.0a67/LICENSE` & `zillionare_omicron-2.0.0a68/LICENSE`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/README.md` & `zillionare_omicron-2.0.0a68/README.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/docs/_static/Omicron_Windows10.docx` & `zillionare_omicron-2.0.0a68/docs/_static/Omicron_Windows10.docx`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/docs/_static/jetbrains-variant-3.svg` & `zillionare_omicron-2.0.0a68/docs/_static/jetbrains-variant-3.svg`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/docs/api/metrics.md` & `zillionare_omicron-2.0.0a68/docs/api/metrics.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/docs/css/extra.css` & `zillionare_omicron-2.0.0a68/docs/css/extra.css`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/docs/developer.md` & `zillionare_omicron-2.0.0a68/docs/developer.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/docs/installation.md` & `zillionare_omicron-2.0.0a68/docs/installation.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/docs/usage.md` & `zillionare_omicron-2.0.0a68/docs/usage.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/__init__.py` & `zillionare_omicron-2.0.0a68/omicron/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/config/calendar.json` & `zillionare_omicron-2.0.0a68/omicron/config/calendar.json`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/config/schema.py` & `zillionare_omicron-2.0.0a68/omicron/config/schema.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/config/sql/v0.6.sql` & `zillionare_omicron-2.0.0a68/omicron/config/sql/v0.6.sql`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/config/sql/v1.0.sql` & `zillionare_omicron-2.0.0a68/omicron/config/sql/v1.0.sql`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/core/errors.py` & `zillionare_omicron-2.0.0a68/omicron/core/errors.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/core/triggers.py` & `zillionare_omicron-2.0.0a68/omicron/core/triggers.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/dal/cache.py` & `zillionare_omicron-2.0.0a68/omicron/dal/cache.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/dal/influx/escape.py` & `zillionare_omicron-2.0.0a68/omicron/dal/influx/escape.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/dal/influx/flux.py` & `zillionare_omicron-2.0.0a68/omicron/dal/influx/flux.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/dal/influx/influxclient.py` & `zillionare_omicron-2.0.0a68/omicron/dal/influx/influxclient.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/dal/influx/serialize.py` & `zillionare_omicron-2.0.0a68/omicron/dal/influx/serialize.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/extensions/decimals.py` & `zillionare_omicron-2.0.0a68/omicron/extensions/decimals.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/extensions/np.py` & `zillionare_omicron-2.0.0a68/omicron/extensions/np.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/models/board.py` & `zillionare_omicron-2.0.0a68/omicron/models/board.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/models/security.py` & `zillionare_omicron-2.0.0a68/omicron/models/security.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/models/stock.py` & `zillionare_omicron-2.0.0a68/omicron/models/stock.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/models/timeframe.py` & `zillionare_omicron-2.0.0a68/omicron/models/timeframe.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/notify/dingtalk.py` & `zillionare_omicron-2.0.0a68/omicron/notify/dingtalk.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/notify/mail.py` & `zillionare_omicron-2.0.0a68/omicron/notify/mail.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/plotting/candlestick.py` & `zillionare_omicron-2.0.0a68/omicron/plotting/candlestick.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,89 @@
+"""绘制K线图。
+
+# 用法示例
+注意示例需要在notebook中运行，否则无法生成图。
+
+```python
+from omicron.plotting.candlestick import Candlestick
+
+bars = await Stock.get_bars("000001.XSHE", 120, FrameType.DAY)
+cs = Candlestick(bars)
+cs.plot()
+```
+
+这将生成下图：
+![](https://images.jieyu.ai/images/2023/05/20230508160941.png)
+
+默认地，将显示成交量和RSI指标两个副图。可以通过以下方式来定制：
+```python
+cs = Candlestick(bars, show_volume=True,
+    show_rsi=True,
+    show_peaks=False
+}
+cs.plot()
+```
+# 增加标记
+```python
+from omicron.plotting.candlestick import Candlestick
+
+bars = await Stock.get_bars("000001.XSHE", 120, FrameType.DAY)
+cs = Candlestick(bars, 
+        show_volume=True,
+        show_rsi=False,
+        show_peaks=True
+    )
+
+cs.add_marks([20, 50])
+cs.plot()
+```
+这将在k线上显示两个加号：
+![](https://images.jieyu.ai/images/2023/05/20230508164639.png)
+# 显示布林带
+```python
+from omicron.plotting.candlestick import Candlestick
+
+bars = await Stock.get_bars("000001.XSHE", 120, FrameType.DAY)
+cs = Candlestick(bars, 
+        show_volume=True,
+        show_rsi=False,
+        show_peaks=True
+    )
+
+cs.add_indicator("bbands")
+cs.plot()
+```
+![](https://images.jieyu.ai/images/2023/05/20230508164728.png)
+
+# 显示平台
+```python
+from omicron.plotting.candlestick import Candlestick
+
+bars = await Stock.get_bars("000001.XSHE", 120, FrameType.DAY)
+cs = Candlestick(bars, 
+        show_volume=True,
+        show_rsi=False,
+        show_peaks=True
+    )
+
+
+cs.mark_bbox()
+cs.plot()
+```
+![](https://images.jieyu.ai/images/2023/05/20230508164848.png)
+
+"""
 from collections import defaultdict
-from tkinter.messagebox import showwarning
 from typing import List, Tuple
 
 import arrow
 import numpy as np
 import plotly.graph_objects as go
 import talib
+from numpy._typing import NDArray
 from plotly.subplots import make_subplots
 
 from omicron.talib import (
     moving_average,
     peaks_and_valleys,
     plateaus,
     support_resist_lines,
@@ -127,15 +201,15 @@
         row_heights = [0.7, *([0.2] * (rows - 1))]
         cols = 1
 
         fig = make_subplots(
             rows=rows,
             cols=cols,
             shared_xaxes=True,
-            vertical_spacing=0.05,
+            vertical_spacing=0.1,
             subplot_titles=(self.title, *self.ind_traces.keys()),
             row_heights=row_heights,
             specs=specs,
         )
 
         for _, trace in self.main_traces.items():
             fig.add_trace(trace, row=1, col=1)
@@ -149,15 +223,15 @@
         fig.update_xaxes(type="category", tickangle=45, nticks=len(self.ticks) // 5)
         end = len(self.ticks)
         start = end - self.win_size
         fig.update_xaxes(range=[start, end])
 
         return fig
 
-    def _format_tick(self, tm: np.array) -> str:
+    def _format_tick(self, tm: np.array) -> NDArray:
         if tm.item(0).hour == 0:  # assume it's date
             return np.array(
                 [
                     f"{x.item().year:02}-{x.item().month:02}-{x.item().day:02}"
                     for x in tm
                 ]
             )
@@ -165,14 +239,22 @@
             return np.array(
                 [
                     f"{x.item().month:02}-{x.item().day:02} {x.item().hour:02}:{x.item().minute:02}"
                     for x in tm
                 ]
             )
 
+    def _remove_ma(self):
+        traces = {}
+        for name in self.main_traces:
+            if not name.startswith("ma"):
+                traces[name] = self.main_traces[name]
+
+        self.main_traces = traces
+
     def add_main_trace(self, trace_name: str, **kwargs):
         """add trace to main plot
 
         支持的图例类别有peaks, bbox（bounding-box), bt(回测), support_line, resist_line
         Args:
             trace_name : 图例名称
             **kwargs : 其他参数
@@ -402,23 +484,36 @@
                 y=self.bars["volume"],
                 showlegend=False,
                 marker={"color": colors},
             )
         elif indicator == "rsi":
             rsi = talib.RSI(self.bars["close"].astype(np.float64))
             trace = go.Scatter(x=self.ticks, y=rsi, showlegend=False)
+        elif indicator == "bbands":
+            self._remove_ma()
+            for name, ind in zip(
+                ["bbands-high", "bbands-mean", "bbands-low"],
+                talib.BBANDS(self.bars["close"].astype(np.float64)),
+            ):
+                trace = go.Scatter(x=self.ticks, y=ind, showlegend=True, name=name)
+                self.main_traces[name] = trace
+
+            return
         else:
             raise ValueError(f"{indicator} not supported")
 
         self.ind_traces[indicator] = trace
 
     def add_marks(self, x: List[int]):
         """向k线图中增加标记点"""
         trace = go.Scatter(
-            x=x, y=self.bars["high"][x], mode="markers", marker_symbol="cross"
+            x=self.ticks[x],
+            y=self.bars["high"][x] * 1.02,
+            mode="markers",
+            marker_symbol="cross",
         )
         self.main_traces["marks"] = trace
 
     def plot(self):
         """绘制图表"""
         fig = self.figure
```

### Comparing `zillionare_omicron-2.0.0a67/omicron/plotting/metrics.py` & `zillionare_omicron-2.0.0a68/omicron/plotting/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 # calling some strategy's backtest and get bills/metrics
 mg = MetricsGraph(bills, metrics)
 
 await mg.plot()
 ```
 注意此方法需要在notebook中调用。
+![](https://images.jieyu.ai/images/2023/05/20230508160012.png)
 
 """
 import datetime
 import logging
 from collections import defaultdict
 from copy import deepcopy
 from typing import List, Union
@@ -90,15 +91,15 @@
         elif type(frames[0]) == datetime.date:  # type: ignore
             return np.array([f"{x.year:02}-{x.month:02}-{x.day:02}" for x in frames])
         else:
             return np.array(
                 [f"{x.month:02}-{x.day:02} {x.hour:02}:{x.minute:02}" for x in frames]  # type: ignore
             )
 
-    async def _metrics_traces(self):
+    async def _metrics_trace(self):
         metric_names = {
             "start": "起始日",
             "end": "结束日",
             "window": "资产暴露窗口",
             "total_tx": "交易次数",
             "total_profit": "总利润",
             "total_profit_rate": "利润率",
@@ -106,15 +107,14 @@
             "mean_return": "日均回报",
             "sharpe": "夏普率",
             "max_drawdown": "最大回撤",
             "annual_return": "年化回报",
             "volatility": "波动率",
             "sortino": "sortino",
             "calmar": "calmar",
-            "code": "参照标的",
         }
 
         # bug: plotly go.Table.Cells format not work here
         metric_formatter = {
             "start": "{}",
             "end": "{}",
             "window": "{}",
@@ -125,62 +125,51 @@
             "mean_return": "{:.2%}",
             "sharpe": "{:.2f}",
             "max_drawdown": "{:.2%}",
             "annual_return": "{:.2%}",
             "volatility": "{:.2%}",
             "sortino": "{:.2f}",
             "calmar": "{:.2f}",
-            "code": "{}",
         }
 
         metrics = deepcopy(self.metrics)
         baseline = metrics["baseline"]
         del metrics["baseline"]
 
-        traces = []
-        traces.append(
-            go.Table(
-                header=dict(values=["指标名", "指标值"]),
-                cells=dict(
-                    values=[
-                        [metric_names[k] for k in metrics if metrics[k]],
-                        [
-                            metric_formatter[k].format(metrics[k])
-                            for k in metrics
-                            if metrics[k]
-                        ],
-                    ],
-                    font_size=10,
-                ),
-            )
-        )
-
-        if baseline:
-            baseline = {k: v for k, v in baseline.items() if v is not None}
-            if "code" in baseline:
-                baseline["code"] = await Security.alias(baseline["code"])
-
-            traces.append(
-                go.Table(
-                    header=dict(values=["指标名", "指标值"]),
-                    cells=dict(
-                        values=[
-                            [metric_names[k] for k in baseline if baseline[k]],
-                            [
-                                metric_formatter[k].format(baseline[k])
-                                for k in baseline
-                                if baseline[k]
-                            ],
-                        ],
-                        font_size=10,
-                    ),
-                )
-            )
+        if "code" in baseline:
+            baseline_name = await Security.alias(baseline["code"])
+            del baseline["code"]
+        else:
+            baseline_name = "基准"
 
-        return traces
+        metrics_formatted = []
+        for k in metric_names.keys():
+            if metrics.get(k):
+                metrics_formatted.append(metric_formatter[k].format(metrics.get(k)))
+            else:
+                metrics_formatted.append("-")
+
+        baseline_formatted = []
+        for k in metric_names.keys():
+            if baseline.get(k):
+                baseline_formatted.append(metric_formatter[k].format(baseline.get(k)))
+            else:
+                baseline_formatted.append("-")
+
+        return go.Table(
+            header=dict(values=["指标名", "策略", baseline_name]),
+            cells=dict(
+                values=[
+                    [metric_names[k] for k in metrics],
+                    metrics_formatted,
+                    baseline_formatted,
+                ],
+                font_size=10,
+            ),
+        )
 
     async def _trade_info_trace(self):
         """构建hover text 序列"""
         X = []
         Y = []
         data = []
 
@@ -222,30 +211,26 @@
         n = len(self.assets)
         bars = await Stock.get_bars(baseline_code, n, FrameType.DAY, self.end)
 
         baseline_prices = self._fill_missing_prices(bars, self.frames)
         baseline_prices /= baseline_prices[0]
 
         fig = make_subplots(
-            rows=2,
+            rows=1,
             cols=2,
             shared_xaxes=False,
             specs=[
-                [{"type": "scatter", "rowspan": 2}, {"type": "table"}],
-                [None, {"type": "table"}],
+                [{"type": "scatter"}, {"type": "table"}],
             ],
-            column_width=[0.8, 0.2],
-            row_heights=[0.63, 0.4],
+            column_width=[0.75, 0.25],
             horizontal_spacing=0.01,
-            vertical_spacing=0.07,
-            subplot_titles=("资产曲线", "策略指标", "基线指标"),
+            subplot_titles=("资产曲线", "策略指标"),
         )
 
-        for i, trace in enumerate(await self._metrics_traces()):
-            fig.add_trace(trace, row=i + 1, col=2)
+        fig.add_trace(await self._metrics_trace(), row=1, col=2)
 
         print("baseline", len(baseline_prices))
         baseline_trace = go.Scatter(
             y=baseline_prices,
             x=self.ticks,
             mode="lines",
             name="baseline",
@@ -258,9 +243,9 @@
         )
         fig.add_trace(nv_trace, row=1, col=1)
 
         trade_info_trace = await self._trade_info_trace()
         fig.add_trace(trade_info_trace, row=1, col=1)
 
         fig.update_xaxes(type="category", tickangle=45, nticks=len(self.ticks) // 5)
-        fig.update_layout(margin=dict(l=20, r=20, t=50, b=50), width=1040, height=650)
+        fig.update_layout(margin=dict(l=20, r=20, t=50, b=50), width=1040, height=435)
         fig.show()
```

### Comparing `zillionare_omicron-2.0.0a67/omicron/strategy/base.py` & `zillionare_omicron-2.0.0a68/omicron/strategy/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """策略基类
 
-## 子类派生
+# 子类派生
 
 1. 从此基类派生出一个策略子类，比如sma.py
 2. 子类需要重载`predict`方法，根据当前传入的时间帧和帧类型参数，获取数据并进行处理，评估出交易信号
 3. 子类根据交易信号，在`predict`方法里，调用基类的`buy`和`sell`方法来进行交易
 4. 子类调用`backtest`方法来进行回测，该方法将根据策略构建时指定的回测起始时间、终止时间、帧类型，逐帧生成各个时间帧，并调用子类的`predict`方法
 4. 在交易结束时，调用`plot_metrics`方法来获取如下所示的回测指标图
-![](https://images.jieyu.ai/images/2023/05/20230507112458.png)
+![](https://images.jieyu.ai/images/2023/05/20230508160012.png)
 
 如何派生子类，可以参考[sma][omicron.strategy.sma.SMAStrategy]源代码。
 
-## 回测
+# 回测
 ```python
 from omicron.strategy.sma import SMAStrategy
 sma = SMAStrategy(
     "600000.XSHG",
     url="", # the url of either backtest server, or trade server
     is_backtest=True,
     start=datetime.date(2023, 2, 3),
     end=datetime.date(2023, 4, 28),
     frame_type=FrameType.DAY,
 )
 
 await sma.backtest(stop_on_error=True)
 ```
-## 实盘
+# 实盘
 在实盘环境下，你还需要在子类中加入周期性任务(比如每分钟执行一次），在该任务中调用`predict`方法来完成交易。
 """
 import datetime
 import logging
 import uuid
 from typing import Dict, List, Optional, Union
```

### Comparing `zillionare_omicron-2.0.0a67/omicron/strategy/sma.py` & `zillionare_omicron-2.0.0a68/omicron/strategy/sma.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/talib/core.py` & `zillionare_omicron-2.0.0a68/omicron/talib/core.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/omicron/talib/morph.py` & `zillionare_omicron-2.0.0a68/omicron/talib/morph.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/pyproject.toml` & `zillionare_omicron-2.0.0a68/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.poetry.dev-dependencies]
 [tool.poetry]
 name = "zillionare-omicron"
 packages = [
     {include = "omicron"}
 ]
-version = "2.0.0a67"
+version = "2.0.0a68"
 description = "Core Library for Zillionare"
 authors = ["jieyu <code@jieyu.ai>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://zillionare-omicron.readthedocs.io"
 repository = "https://github.com/zillionare/omicron"
 documentation = "https://zillionare-omicron.readthedocs.io"
```

### Comparing `zillionare_omicron-2.0.0a67/tests/__init__.py` & `zillionare_omicron-2.0.0a68/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/core/test_triggers.py` & `zillionare_omicron-2.0.0a68/tests/core/test_triggers.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/core/test_types.py` & `zillionare_omicron-2.0.0a68/tests/core/test_types.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/dal/influx/__init__.py` & `zillionare_omicron-2.0.0a68/tests/dal/influx/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/dal/influx/test_escape.py` & `zillionare_omicron-2.0.0a68/tests/dal/influx/test_escape.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/dal/influx/test_flux.py` & `zillionare_omicron-2.0.0a68/tests/dal/influx/test_flux.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/dal/influx/test_influxclient.py` & `zillionare_omicron-2.0.0a68/tests/dal/influx/test_influxclient.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/dal/influx/test_serialize.py` & `zillionare_omicron-2.0.0a68/tests/dal/influx/test_serialize.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.15m.csv` & `zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.15m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.1m.csv` & `zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.30m.csv` & `zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.30m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.5m.csv` & `zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.5m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/data/000001.XSHG.1m.csv` & `zillionare_omicron-2.0.0a68/tests/data/000001.XSHG.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/data/000002.XSHE.1d.csv` & `zillionare_omicron-2.0.0a68/tests/data/000002.XSHE.1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/data/000002.XSHE.1m.csv` & `zillionare_omicron-2.0.0a68/tests/data/000002.XSHE.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/data/000002.XSHE.1w.csv` & `zillionare_omicron-2.0.0a68/tests/data/000002.XSHE.1w.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/data/000002.XSHE.30m.csv` & `zillionare_omicron-2.0.0a68/tests/data/000002.XSHE.30m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/data/000004.XSHE.1d.csv` & `zillionare_omicron-2.0.0a68/tests/data/000004.XSHE.1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/data/000004.XSHE.1m.csv` & `zillionare_omicron-2.0.0a68/tests/data/000004.XSHE.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/data/000004.XSHE.1w.csv` & `zillionare_omicron-2.0.0a68/tests/data/000004.XSHE.1w.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/data/000004.XSHE.30m.csv` & `zillionare_omicron-2.0.0a68/tests/data/000004.XSHE.30m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/data/600000.XSHG.1d.csv` & `zillionare_omicron-2.0.0a68/tests/data/600000.XSHG.1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/data/README.md` & `zillionare_omicron-2.0.0a68/tests/data/README.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/data/bars_1d.pkl` & `zillionare_omicron-2.0.0a68/tests/data/bars_1d.pkl`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/data/bars_1m.pkl` & `zillionare_omicron-2.0.0a68/tests/data/bars_1m.pkl`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/data/limits.csv` & `zillionare_omicron-2.0.0a68/tests/data/limits.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/data/stock_bars_flux_query.txt` & `zillionare_omicron-2.0.0a68/tests/data/stock_bars_flux_query.txt`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/data/test.jpg` & `zillionare_omicron-2.0.0a68/tests/data/test.jpg`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/extensions/test_decimals.py` & `zillionare_omicron-2.0.0a68/tests/extensions/test_decimals.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/extensions/test_np.py` & `zillionare_omicron-2.0.0a68/tests/extensions/test_np.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/models/test_board.py` & `zillionare_omicron-2.0.0a68/tests/models/test_board.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/models/test_security.py` & `zillionare_omicron-2.0.0a68/tests/models/test_security.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/models/test_stock.py` & `zillionare_omicron-2.0.0a68/tests/models/test_stock.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/models/test_timeframe.py` & `zillionare_omicron-2.0.0a68/tests/models/test_timeframe.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/notify/test_dingtalk.py` & `zillionare_omicron-2.0.0a68/tests/notify/test_dingtalk.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/notify/test_mail.py` & `zillionare_omicron-2.0.0a68/tests/notify/test_mail.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/performance/influx/end2end.py` & `zillionare_omicron-2.0.0a68/tests/performance/influx/end2end.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/performance/influx/serialize.py` & `zillionare_omicron-2.0.0a68/tests/performance/influx/serialize.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/strategy/test_strategy.py` & `zillionare_omicron-2.0.0a68/tests/strategy/test_strategy.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/talib/test_core.py` & `zillionare_omicron-2.0.0a68/tests/talib/test_core.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/tests/talib/test_morph.py` & `zillionare_omicron-2.0.0a68/tests/talib/test_morph.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a67/PKG-INFO` & `zillionare_omicron-2.0.0a68/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zillionare-omicron
-Version: 2.0.0a67
+Version: 2.0.0a68
 Summary: Core Library for Zillionare
 Home-page: https://zillionare-omicron.readthedocs.io
 License: MIT
 Keywords: AI,quant,trade,stock
 Author: jieyu
 Author-email: code@jieyu.ai
 Requires-Python: >=3.8,<3.9
```

