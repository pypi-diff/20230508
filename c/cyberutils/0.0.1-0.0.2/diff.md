# Comparing `tmp/cyberutils-0.0.1.tar.gz` & `tmp/cyberutils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberutils-0.0.1.tar", max compression
+gzip compressed data, was "cyberutils-0.0.2.tar", max compression
```

## Comparing `cyberutils-0.0.1.tar` & `cyberutils-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1075 2023-05-03 03:06:56.801482 cyberutils-0.0.1/LICENSE
--rw-r--r--   0        0        0       12 2023-05-03 03:06:56.801482 cyberutils-0.0.1/README.md
--rw-r--r--   0        0        0      166 2023-05-03 03:06:56.801482 cyberutils-0.0.1/cyberutils/__init__.py
--rw-r--r--   0        0        0       77 2023-05-03 03:06:56.801482 cyberutils-0.0.1/cyberutils/bash/__init__.py
--rw-r--r--   0        0        0     2268 2023-05-03 03:06:56.801482 cyberutils-0.0.1/cyberutils/bash/execution.py
--rw-r--r--   0        0        0       40 2023-05-03 03:06:56.801482 cyberutils-0.0.1/cyberutils/contract/__init__.py
--rw-r--r--   0        0        0     1698 2023-05-03 03:06:56.801482 cyberutils-0.0.1/cyberutils/contract/execution.py
--rw-r--r--   0        0        0     1749 2023-05-03 03:06:56.801482 cyberutils-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 cyberutils-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-08 05:28:37.655197 cyberutils-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2523 2023-05-08 05:28:37.655197 cyberutils-0.0.2/README.md
+-rw-r--r--   0        0        0      166 2023-05-08 05:28:37.655197 cyberutils-0.0.2/cyberutils/__init__.py
+-rw-r--r--   0        0        0       77 2023-05-08 05:28:37.655197 cyberutils-0.0.2/cyberutils/bash/__init__.py
+-rw-r--r--   0        0        0     2268 2023-05-08 05:28:37.655197 cyberutils-0.0.2/cyberutils/bash/execution.py
+-rw-r--r--   0        0        0       40 2023-05-08 05:28:37.655197 cyberutils-0.0.2/cyberutils/contract/__init__.py
+-rw-r--r--   0        0        0     1671 2023-05-08 05:28:37.655197 cyberutils-0.0.2/cyberutils/contract/execution.py
+-rw-r--r--   0        0        0       39 2023-05-08 05:28:37.655197 cyberutils-0.0.2/cyberutils/graphql/__init__.py
+-rw-r--r--   0        0        0      757 2023-05-08 05:28:37.655197 cyberutils-0.0.2/cyberutils/graphql/execution.py
+-rw-r--r--   0        0        0     1818 2023-05-08 05:28:37.655197 cyberutils-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3958 1970-01-01 00:00:00.000000 cyberutils-0.0.2/PKG-INFO
```

### Comparing `cyberutils-0.0.1/LICENSE` & `cyberutils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberutils-0.0.1/cyberutils/bash/execution.py` & `cyberutils-0.0.2/cyberutils/bash/execution.py`

 * *Files identical despite different names*

### Comparing `cyberutils-0.0.1/cyberutils/contract/execution.py` & `cyberutils-0.0.2/cyberutils/contract/execution.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,27 +20,26 @@
     :param gas: amount of gas
     :param fee_amount: fee amount
     :param fee_denom: fee denom
     :param memo: note(memo) of a transaction
     :return: transaction result
     """
 
-    _create_links_msgs = \
+    _msgs = \
         [MsgExecuteContract(
             sender=wallet.key.acc_address,
             contract=AccAddress(contract_address),
             execute_msg=execute_msg) for execute_msg in execute_msgs]
 
     _tx_signed = wallet.create_and_sign_tx(
         CreateTxOptions(
-            msgs=_create_links_msgs,
+            msgs=_msgs,
             memo=memo,
             fee=Fee(gas, Coins([Coin(amount=fee_amount, denom=fee_denom)]))
         ))
 
     try:
         _tx_broadcasted = lcd_client.tx.broadcast(_tx_signed)
         return _tx_broadcasted
-
     except LCDResponseError as _e:
         print(f'LCDResponseError: {_e}')
         return None
```

### Comparing `cyberutils-0.0.1/pyproject.toml` & `cyberutils-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,34 +6,35 @@
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-description = "The Toolset for cyber protocol"
+description = "The Toolset for cyber protocol and cosmos ecosystem"
 documentation = "https://github.com/Snedashkovsky/cyberutils"
 homepage = "https://github.com/Snedashkovsky/cyberutils"
 keywords = ["bostrom", "cyber", "knowledge-graph", "dex", "swap", "defi", "crypto", "blockchain", ]
 license = "MIT"
 packages = [{ include = "cyberutils" }]
 readme = "README.md"
 repository = "https://github.com/Snedashkovsky/cyberutils.git"
-version = "0.0.1"
+version = "0.0.2"
 
 [tool.poetry.dependencies]
 pandas = "^1.0.0"
 numpy = "^1.0.0"
 python-dotenv = "^0.20.0"
 tqdm = "^4.0.0"
 ipython = "^8.0.0"
 pandarallel = "^1.6.0"
 multiprocess = "^0.70.14"
 python = "^3.9"
 cyber_sdk = "^1.1.2"
+gql = { version = "^3.0.0", extras = ["all"] }
 
 [tool.poetry.dev-dependencies]
 aioresponses = "^0.7.2"
 asynctest = "^0.13.0"
 pytest-cov = "^3.0.0"
 pytest = "^7.0.1"
 pip = "^22.0.3"
@@ -60,8 +61,8 @@
 
 [tool.flake8]
 max-line-length = 88
 extend-ignore = "E203"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
-requires = ["poetry-core>=1.1.0"]
+requires = ["poetry-core>=1.1.0"]
```

