# Comparing `tmp/huma_signals-0.1.1.tar.gz` & `tmp/huma_signals-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huma_signals-0.1.1.tar", max compression
+gzip compressed data, was "huma_signals-0.1.2.tar", max compression
```

## Comparing `huma_signals-0.1.1.tar` & `huma_signals-0.1.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0    34523 2023-05-06 00:10:02.616918 huma_signals-0.1.1/LICENSE
--rw-r--r--   0        0        0     2173 2023-05-06 00:10:02.617080 huma_signals-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.617555 huma_signals-0.1.1/huma_signals/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.617626 huma_signals-0.1.1/huma_signals/api/__init__.py
--rw-r--r--   0        0        0     1187 2023-05-06 00:10:02.617701 huma_signals-0.1.1/huma_signals/api/exception_handlers.py
--rw-r--r--   0        0        0      997 2023-05-06 00:10:02.617769 huma_signals-0.1.1/huma_signals/api/main.py
--rw-r--r--   0        0        0      289 2023-05-06 00:10:02.617834 huma_signals-0.1.1/huma_signals/api/models.py
--rw-r--r--   0        0        0     1114 2023-05-06 00:10:02.617904 huma_signals-0.1.1/huma_signals/api/views.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.617961 huma_signals-0.1.1/huma_signals/commons/__init__.py
--rw-r--r--   0        0        0      812 2023-05-06 00:10:02.618029 huma_signals-0.1.1/huma_signals/commons/chains.py
--rw-r--r--   0        0        0      330 2023-05-06 00:10:02.618090 huma_signals-0.1.1/huma_signals/commons/datetime_utils.py
--rw-r--r--   0        0        0      227 2023-05-06 00:10:02.618146 huma_signals-0.1.1/huma_signals/commons/pydantic_utils.py
--rw-r--r--   0        0        0      569 2023-05-06 00:10:02.618202 huma_signals-0.1.1/huma_signals/commons/string_utils.py
--rw-r--r--   0        0        0     1309 2023-05-06 00:10:02.618262 huma_signals-0.1.1/huma_signals/commons/tokens.py
--rw-r--r--   0        0        0     1078 2023-05-06 00:10:02.618330 huma_signals-0.1.1/huma_signals/commons/web3_utils.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.618388 huma_signals-0.1.1/huma_signals/domain/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.618462 huma_signals-0.1.1/huma_signals/domain/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.618534 huma_signals-0.1.1/huma_signals/domain/adapters/allowlist/__init__.py
--rw-r--r--   0        0        0     1755 2023-05-06 00:10:02.618617 huma_signals-0.1.1/huma_signals/domain/adapters/allowlist/adapter.py
--rw-r--r--   0        0        0      589 2023-05-06 00:10:02.618719 huma_signals-0.1.1/huma_signals/domain/adapters/ethereum_wallet/README.md
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.618750 huma_signals-0.1.1/huma_signals/domain/adapters/ethereum_wallet/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-06 00:27:13.844094 huma_signals-0.1.1/huma_signals/domain/adapters/ethereum_wallet/adapter.py
--rw-r--r--   0        0        0      186 2023-05-06 00:26:23.703436 huma_signals-0.1.1/huma_signals/domain/adapters/ethereum_wallet/settings.py
--rw-r--r--   0        0        0      589 2023-05-06 00:10:02.618984 huma_signals-0.1.1/huma_signals/domain/adapters/lending_pools/README.md
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.619013 huma_signals-0.1.1/huma_signals/domain/adapters/lending_pools/__init__.py
--rw-r--r--   0        0        0    23699 2023-05-06 00:10:02.619139 huma_signals-0.1.1/huma_signals/domain/adapters/lending_pools/abi/BaseCreditPool.json
--rw-r--r--   0        0        0    30632 2023-05-06 00:10:02.619304 huma_signals-0.1.1/huma_signals/domain/adapters/lending_pools/abi/BasePoolConfig.json
--rw-r--r--   0        0        0    32155 2023-05-06 00:10:02.619389 huma_signals-0.1.1/huma_signals/domain/adapters/lending_pools/abi/ReceivableFactoringPool.json
--rw-r--r--   0        0        0    30290 2023-05-06 00:10:02.619495 huma_signals-0.1.1/huma_signals/domain/adapters/lending_pools/abi/SuperfluidFactoringPool.json
--rw-r--r--   0        0        0     4740 2023-05-06 00:27:33.651253 huma_signals-0.1.1/huma_signals/domain/adapters/lending_pools/adapter.py
--rw-r--r--   0        0        0     1938 2023-05-06 00:10:02.619635 huma_signals-0.1.1/huma_signals/domain/adapters/lending_pools/registry.py
--rw-r--r--   0        0        0      158 2023-05-06 00:26:23.703674 huma_signals-0.1.1/huma_signals/domain/adapters/lending_pools/settings.py
--rw-r--r--   0        0        0      582 2023-05-06 00:10:02.619763 huma_signals-0.1.1/huma_signals/domain/adapters/models.py
--rw-r--r--   0        0        0      594 2023-05-06 00:10:02.619844 huma_signals-0.1.1/huma_signals/domain/adapters/polygon_wallet/README.md
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.619871 huma_signals-0.1.1/huma_signals/domain/adapters/polygon_wallet/__init__.py
--rw-r--r--   0        0        0     3427 2023-05-06 00:27:50.800480 huma_signals-0.1.1/huma_signals/domain/adapters/polygon_wallet/adapter.py
--rw-r--r--   0        0        0      222 2023-05-06 00:26:23.703883 huma_signals-0.1.1/huma_signals/domain/adapters/polygon_wallet/settings.py
--rw-r--r--   0        0        0     2791 2023-05-06 00:10:02.620043 huma_signals-0.1.1/huma_signals/domain/adapters/registry.py
--rw-r--r--   0        0        0      579 2023-05-06 00:10:02.620132 huma_signals-0.1.1/huma_signals/domain/adapters/request_network/README.md
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.620159 huma_signals-0.1.1/huma_signals/domain/adapters/request_network/__init__.py
--rw-r--r--   0        0        0     4372 2023-05-06 00:10:02.620235 huma_signals-0.1.1/huma_signals/domain/adapters/request_network/models.py
--rw-r--r--   0        0        0     5949 2023-05-06 00:28:18.520700 huma_signals-0.1.1/huma_signals/domain/adapters/request_network/request_invoice_adapter.py
--rw-r--r--   0        0        0     5262 2023-05-06 00:28:33.474404 huma_signals-0.1.1/huma_signals/domain/adapters/request_network/request_transaction_adapter.py
--rw-r--r--   0        0        0      284 2023-05-06 00:26:23.704224 huma_signals-0.1.1/huma_signals/domain/adapters/request_network/settings.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.620495 huma_signals-0.1.1/huma_signals/domain/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.620556 huma_signals-0.1.1/huma_signals/domain/clients/eth_client/__init__.py
--rw-r--r--   0        0        0     1434 2023-05-06 00:28:46.641667 huma_signals-0.1.1/huma_signals/domain/clients/eth_client/eth_client.py
--rw-r--r--   0        0        0      673 2023-05-06 00:10:02.620677 huma_signals-0.1.1/huma_signals/domain/clients/eth_client/eth_types.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.620728 huma_signals-0.1.1/huma_signals/domain/clients/polygon_client/__init__.py
--rw-r--r--   0        0        0     1510 2023-05-06 00:28:59.187419 huma_signals-0.1.1/huma_signals/domain/clients/polygon_client/polygon_client.py
--rw-r--r--   0        0        0      685 2023-05-06 00:10:02.620830 huma_signals-0.1.1/huma_signals/domain/clients/polygon_client/polygon_types.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.620885 huma_signals-0.1.1/huma_signals/domain/clients/request_client/__init__.py
--rw-r--r--   0        0        0     8136 2023-05-06 00:29:15.199730 huma_signals-0.1.1/huma_signals/domain/clients/request_client/request_client.py
--rw-r--r--   0        0        0      900 2023-05-06 00:10:02.621033 huma_signals-0.1.1/huma_signals/domain/clients/request_client/request_types.py
--rw-r--r--   0        0        0      499 2023-05-06 00:10:02.621121 huma_signals-0.1.1/huma_signals/dotenv/example.env
--rw-r--r--   0        0        0      946 2023-05-06 00:10:02.621175 huma_signals-0.1.1/huma_signals/exceptions.py
--rw-r--r--   0        0        0      322 2023-05-06 00:10:02.621231 huma_signals-0.1.1/huma_signals/models.py
--rw-r--r--   0        0        0     1563 2023-05-06 00:10:02.621293 huma_signals-0.1.1/huma_signals/settings.py
--rw-r--r--   0        0        0     2729 2023-05-06 01:16:30.684349 huma_signals-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3220 1970-01-01 00:00:00.000000 huma_signals-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-06 00:10:02.616918 huma_signals-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2173 2023-05-06 00:10:02.617080 huma_signals-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.617555 huma_signals-0.1.2/huma_signals/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.617626 huma_signals-0.1.2/huma_signals/api/__init__.py
+-rw-r--r--   0        0        0     1187 2023-05-06 00:10:02.617701 huma_signals-0.1.2/huma_signals/api/exception_handlers.py
+-rw-r--r--   0        0        0      997 2023-05-06 00:10:02.617769 huma_signals-0.1.2/huma_signals/api/main.py
+-rw-r--r--   0        0        0      289 2023-05-06 00:10:02.617834 huma_signals-0.1.2/huma_signals/api/models.py
+-rw-r--r--   0        0        0     1114 2023-05-06 00:10:02.617904 huma_signals-0.1.2/huma_signals/api/views.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.617961 huma_signals-0.1.2/huma_signals/commons/__init__.py
+-rw-r--r--   0        0        0      812 2023-05-06 00:10:02.618029 huma_signals-0.1.2/huma_signals/commons/chains.py
+-rw-r--r--   0        0        0      330 2023-05-06 00:10:02.618090 huma_signals-0.1.2/huma_signals/commons/datetime_utils.py
+-rw-r--r--   0        0        0      227 2023-05-06 00:10:02.618146 huma_signals-0.1.2/huma_signals/commons/pydantic_utils.py
+-rw-r--r--   0        0        0      569 2023-05-06 00:10:02.618202 huma_signals-0.1.2/huma_signals/commons/string_utils.py
+-rw-r--r--   0        0        0     1309 2023-05-06 00:10:02.618262 huma_signals-0.1.2/huma_signals/commons/tokens.py
+-rw-r--r--   0        0        0     1078 2023-05-06 00:10:02.618330 huma_signals-0.1.2/huma_signals/commons/web3_utils.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.618388 huma_signals-0.1.2/huma_signals/domain/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.618462 huma_signals-0.1.2/huma_signals/domain/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.618534 huma_signals-0.1.2/huma_signals/domain/adapters/allowlist/__init__.py
+-rw-r--r--   0        0        0     1755 2023-05-06 00:10:02.618617 huma_signals-0.1.2/huma_signals/domain/adapters/allowlist/adapter.py
+-rw-r--r--   0        0        0      589 2023-05-06 00:10:02.618719 huma_signals-0.1.2/huma_signals/domain/adapters/ethereum_wallet/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.618750 huma_signals-0.1.2/huma_signals/domain/adapters/ethereum_wallet/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-08 18:23:44.497054 huma_signals-0.1.2/huma_signals/domain/adapters/ethereum_wallet/adapter.py
+-rw-r--r--   0        0        0      186 2023-05-08 18:23:44.497148 huma_signals-0.1.2/huma_signals/domain/adapters/ethereum_wallet/settings.py
+-rw-r--r--   0        0        0      589 2023-05-06 00:10:02.618984 huma_signals-0.1.2/huma_signals/domain/adapters/lending_pools/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.619013 huma_signals-0.1.2/huma_signals/domain/adapters/lending_pools/__init__.py
+-rw-r--r--   0        0        0    23699 2023-05-06 00:10:02.619139 huma_signals-0.1.2/huma_signals/domain/adapters/lending_pools/abi/BaseCreditPool.json
+-rw-r--r--   0        0        0    30632 2023-05-06 00:10:02.619304 huma_signals-0.1.2/huma_signals/domain/adapters/lending_pools/abi/BasePoolConfig.json
+-rw-r--r--   0        0        0    32155 2023-05-06 00:10:02.619389 huma_signals-0.1.2/huma_signals/domain/adapters/lending_pools/abi/ReceivableFactoringPool.json
+-rw-r--r--   0        0        0    30290 2023-05-06 00:10:02.619495 huma_signals-0.1.2/huma_signals/domain/adapters/lending_pools/abi/SuperfluidFactoringPool.json
+-rw-r--r--   0        0        0     4740 2023-05-08 18:23:44.497330 huma_signals-0.1.2/huma_signals/domain/adapters/lending_pools/adapter.py
+-rw-r--r--   0        0        0     1938 2023-05-06 00:10:02.619635 huma_signals-0.1.2/huma_signals/domain/adapters/lending_pools/registry.py
+-rw-r--r--   0        0        0      158 2023-05-08 18:23:44.497447 huma_signals-0.1.2/huma_signals/domain/adapters/lending_pools/settings.py
+-rw-r--r--   0        0        0      582 2023-05-06 00:10:02.619763 huma_signals-0.1.2/huma_signals/domain/adapters/models.py
+-rw-r--r--   0        0        0      594 2023-05-06 00:10:02.619844 huma_signals-0.1.2/huma_signals/domain/adapters/polygon_wallet/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.619871 huma_signals-0.1.2/huma_signals/domain/adapters/polygon_wallet/__init__.py
+-rw-r--r--   0        0        0     3427 2023-05-08 18:23:44.497586 huma_signals-0.1.2/huma_signals/domain/adapters/polygon_wallet/adapter.py
+-rw-r--r--   0        0        0      222 2023-05-08 18:23:44.497661 huma_signals-0.1.2/huma_signals/domain/adapters/polygon_wallet/settings.py
+-rw-r--r--   0        0        0     2791 2023-05-06 00:10:02.620043 huma_signals-0.1.2/huma_signals/domain/adapters/registry.py
+-rw-r--r--   0        0        0      579 2023-05-06 00:10:02.620132 huma_signals-0.1.2/huma_signals/domain/adapters/request_network/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.620159 huma_signals-0.1.2/huma_signals/domain/adapters/request_network/__init__.py
+-rw-r--r--   0        0        0     4372 2023-05-06 00:10:02.620235 huma_signals-0.1.2/huma_signals/domain/adapters/request_network/models.py
+-rw-r--r--   0        0        0     5949 2023-05-08 18:23:44.497836 huma_signals-0.1.2/huma_signals/domain/adapters/request_network/request_invoice_adapter.py
+-rw-r--r--   0        0        0     5262 2023-05-08 18:23:44.497961 huma_signals-0.1.2/huma_signals/domain/adapters/request_network/request_transaction_adapter.py
+-rw-r--r--   0        0        0      284 2023-05-08 18:23:44.498031 huma_signals-0.1.2/huma_signals/domain/adapters/request_network/settings.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.620495 huma_signals-0.1.2/huma_signals/domain/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.620556 huma_signals-0.1.2/huma_signals/domain/clients/eth_client/__init__.py
+-rw-r--r--   0        0        0     1434 2023-05-08 18:23:44.498189 huma_signals-0.1.2/huma_signals/domain/clients/eth_client/eth_client.py
+-rw-r--r--   0        0        0      673 2023-05-06 00:10:02.620677 huma_signals-0.1.2/huma_signals/domain/clients/eth_client/eth_types.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.620728 huma_signals-0.1.2/huma_signals/domain/clients/polygon_client/__init__.py
+-rw-r--r--   0        0        0     1510 2023-05-08 18:23:44.498319 huma_signals-0.1.2/huma_signals/domain/clients/polygon_client/polygon_client.py
+-rw-r--r--   0        0        0      685 2023-05-06 00:10:02.620830 huma_signals-0.1.2/huma_signals/domain/clients/polygon_client/polygon_types.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.620885 huma_signals-0.1.2/huma_signals/domain/clients/request_client/__init__.py
+-rw-r--r--   0        0        0     8136 2023-05-08 18:23:44.498486 huma_signals-0.1.2/huma_signals/domain/clients/request_client/request_client.py
+-rw-r--r--   0        0        0      900 2023-05-06 00:10:02.621033 huma_signals-0.1.2/huma_signals/domain/clients/request_client/request_types.py
+-rw-r--r--   0        0        0      499 2023-05-06 00:10:02.621121 huma_signals-0.1.2/huma_signals/dotenv/example.env
+-rw-r--r--   0        0        0      946 2023-05-06 00:10:02.621175 huma_signals-0.1.2/huma_signals/exceptions.py
+-rw-r--r--   0        0        0      322 2023-05-06 00:10:02.621231 huma_signals-0.1.2/huma_signals/models.py
+-rw-r--r--   0        0        0     1563 2023-05-06 00:10:02.621293 huma_signals-0.1.2/huma_signals/settings.py
+-rw-r--r--   0        0        0     2729 2023-05-08 18:23:44.500156 huma_signals-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 huma_signals-0.1.2/PKG-INFO
```

### Comparing `huma_signals-0.1.1/LICENSE` & `huma_signals-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/README.md` & `huma_signals-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/api/exception_handlers.py` & `huma_signals-0.1.2/huma_signals/api/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/api/main.py` & `huma_signals-0.1.2/huma_signals/api/main.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/api/views.py` & `huma_signals-0.1.2/huma_signals/api/views.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/commons/chains.py` & `huma_signals-0.1.2/huma_signals/commons/chains.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/commons/string_utils.py` & `huma_signals-0.1.2/huma_signals/commons/string_utils.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/commons/tokens.py` & `huma_signals-0.1.2/huma_signals/commons/tokens.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/commons/web3_utils.py` & `huma_signals-0.1.2/huma_signals/commons/web3_utils.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/adapters/allowlist/adapter.py` & `huma_signals-0.1.2/huma_signals/domain/adapters/allowlist/adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/adapters/ethereum_wallet/README.md` & `huma_signals-0.1.2/huma_signals/domain/adapters/ethereum_wallet/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/adapters/ethereum_wallet/adapter.py` & `huma_signals-0.1.2/huma_signals/domain/adapters/ethereum_wallet/adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/adapters/lending_pools/README.md` & `huma_signals-0.1.2/huma_signals/domain/adapters/lending_pools/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/adapters/lending_pools/abi/BaseCreditPool.json` & `huma_signals-0.1.2/huma_signals/domain/adapters/lending_pools/abi/BaseCreditPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/adapters/lending_pools/abi/BasePoolConfig.json` & `huma_signals-0.1.2/huma_signals/domain/adapters/lending_pools/abi/BasePoolConfig.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/adapters/lending_pools/abi/ReceivableFactoringPool.json` & `huma_signals-0.1.2/huma_signals/domain/adapters/lending_pools/abi/ReceivableFactoringPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/adapters/lending_pools/abi/SuperfluidFactoringPool.json` & `huma_signals-0.1.2/huma_signals/domain/adapters/lending_pools/abi/SuperfluidFactoringPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/adapters/lending_pools/adapter.py` & `huma_signals-0.1.2/huma_signals/domain/adapters/lending_pools/adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/adapters/lending_pools/registry.py` & `huma_signals-0.1.2/huma_signals/domain/adapters/lending_pools/registry.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/adapters/models.py` & `huma_signals-0.1.2/huma_signals/domain/adapters/models.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/adapters/polygon_wallet/README.md` & `huma_signals-0.1.2/huma_signals/domain/adapters/polygon_wallet/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/adapters/polygon_wallet/adapter.py` & `huma_signals-0.1.2/huma_signals/domain/adapters/polygon_wallet/adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/adapters/registry.py` & `huma_signals-0.1.2/huma_signals/domain/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/adapters/request_network/README.md` & `huma_signals-0.1.2/huma_signals/domain/adapters/request_network/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/adapters/request_network/models.py` & `huma_signals-0.1.2/huma_signals/domain/adapters/request_network/models.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/adapters/request_network/request_invoice_adapter.py` & `huma_signals-0.1.2/huma_signals/domain/adapters/request_network/request_invoice_adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/adapters/request_network/request_transaction_adapter.py` & `huma_signals-0.1.2/huma_signals/domain/adapters/request_network/request_transaction_adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/clients/eth_client/eth_client.py` & `huma_signals-0.1.2/huma_signals/domain/clients/eth_client/eth_client.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/clients/eth_client/eth_types.py` & `huma_signals-0.1.2/huma_signals/domain/clients/eth_client/eth_types.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/clients/polygon_client/polygon_client.py` & `huma_signals-0.1.2/huma_signals/domain/clients/polygon_client/polygon_client.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/clients/polygon_client/polygon_types.py` & `huma_signals-0.1.2/huma_signals/domain/clients/polygon_client/polygon_types.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/clients/request_client/request_client.py` & `huma_signals-0.1.2/huma_signals/domain/clients/request_client/request_client.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/domain/clients/request_client/request_types.py` & `huma_signals-0.1.2/huma_signals/domain/clients/request_client/request_types.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/exceptions.py` & `huma_signals-0.1.2/huma_signals/exceptions.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/huma_signals/settings.py` & `huma_signals-0.1.2/huma_signals/settings.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.1/pyproject.toml` & `huma_signals-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [tool.poetry]
 name = "huma-signals"
-version = "0.1.1"
+version = "0.1.2"
 description = "Enables access to high-quality signals about a borrower's income, assets, and liabilities."
 authors = ["Jiatu Liu <jiatu@huma.finance>", "Ji Peng <ji@huma.finance>"]
 license = "AGPL v3"
 readme = "README.md"
 packages = [{include = "huma_signals"}]
 
 [tool.poetry.dependencies]
 python = "~3.10"
 fastapi = "^0.95.1"
 structlog = "^22.3.0"
 uvicorn = "^0.20.0"
 pandas = "^1.5.2"
 python-dotenv = "^0.21.0"
 web3 = "^6.1.0"
-httpx = "^0.23.3"
+httpx = "^0.24.0"
 base58 = "^2.1.1"
 ipfshttpclient = "^0.7.0"
 aiofiles = "^22.1.0"
 orjson = "^3.8.5"
-pylint-pydantic = "^0.1.6"
 ddtrace = {extras = ["opentracing"], version = "^1.7.5"}
 datadog = "^0.44.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest-describe = "^2.0.1"
 pytest = "^7.2.0"
 isort = "^5.11.3"
@@ -42,14 +41,15 @@
 vcrpy = "^4.2.1"
 pytest-spec = "^3.2.0"
 pandas-stubs = "^1.5.3.230321"
 factory-boy = "^3.2.1"
 faker = "^18.4.0"
 types-factory-boy = "^0.4.1"
 pytest-mock = "^3.10.0"
+pylint-pydantic = "^0.1.6"
 
 [tool.pytest.ini_options]
 describe_prefixes = ["describe", "if", "when", "with", "without"]
 python_functions = ["it_*", "its_*"]
 asyncio_mode = "auto"
 
 [tool.isort]
```

### Comparing `huma_signals-0.1.1/PKG-INFO` & `huma_signals-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: huma-signals
-Version: 0.1.1
+Version: 0.1.2
 Summary: Enables access to high-quality signals about a borrower's income, assets, and liabilities.
 License: AGPL v3
 Author: Jiatu Liu
 Author-email: jiatu@huma.finance
 Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: aiofiles (>=22.1.0,<23.0.0)
 Requires-Dist: base58 (>=2.1.1,<3.0.0)
 Requires-Dist: datadog (>=0.44.0,<0.45.0)
 Requires-Dist: ddtrace[opentracing] (>=1.7.5,<2.0.0)
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
-Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: ipfshttpclient (>=0.7.0,<0.8.0)
 Requires-Dist: orjson (>=3.8.5,<4.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
-Requires-Dist: pylint-pydantic (>=0.1.6,<0.2.0)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
 Requires-Dist: structlog (>=22.3.0,<23.0.0)
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0)
 Requires-Dist: web3 (>=6.1.0,<7.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: huma-signals Version: 0.1.1 Summary: Enables access
+Metadata-Version: 2.1 Name: huma-signals Version: 0.1.2 Summary: Enables access
 to high-quality signals about a borrower's income, assets, and liabilities.
 License: AGPL v3 Author: Jiatu Liu Author-email: jiatu@huma.finance Requires-
 Python: >=3.10,<3.11 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Requires-Dist: aiofiles (>=22.1.0,<23.0.0) Requires-
 Dist: base58 (>=2.1.1,<3.0.0) Requires-Dist: datadog (>=0.44.0,<0.45.0)
 Requires-Dist: ddtrace[opentracing] (>=1.7.5,<2.0.0) Requires-Dist: fastapi
-(>=0.95.1,<0.96.0) Requires-Dist: httpx (>=0.23.3,<0.24.0) Requires-Dist:
+(>=0.95.1,<0.96.0) Requires-Dist: httpx (>=0.24.0,<0.25.0) Requires-Dist:
 ipfshttpclient (>=0.7.0,<0.8.0) Requires-Dist: orjson (>=3.8.5,<4.0.0)
-Requires-Dist: pandas (>=1.5.2,<2.0.0) Requires-Dist: pylint-pydantic
-(>=0.1.6,<0.2.0) Requires-Dist: python-dotenv (>=0.21.0,<0.22.0) Requires-Dist:
-structlog (>=22.3.0,<23.0.0) Requires-Dist: uvicorn (>=0.20.0,<0.21.0)
-Requires-Dist: web3 (>=6.1.0,<7.0.0) Description-Content-Type: text/markdown
+Requires-Dist: pandas (>=1.5.2,<2.0.0) Requires-Dist: python-dotenv
+(>=0.21.0,<0.22.0) Requires-Dist: structlog (>=22.3.0,<23.0.0) Requires-Dist:
+uvicorn (>=0.20.0,<0.21.0) Requires-Dist: web3 (>=6.1.0,<7.0.0) Description-
+Content-Type: text/markdown
                                 [Huma_Finance]
                  ****** Decentralized Signal Portfolio ******
     [Action_Status] [Version] [Documentation]  [License:_AGPLv3] [Twitter:
 humafinance] The Decentralized Signal Portfolio (DSP) is an open platform that
  enables access to high-quality signals about a borrower's income, assets, and
 liabilities. These signals are collected through Signal Adapters hosted on the
  DSP, which gather data from a variety of on-chain and off-chain sources. Any
```

