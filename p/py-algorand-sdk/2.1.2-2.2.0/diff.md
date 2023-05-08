# Comparing `tmp/py-algorand-sdk-2.1.2.tar.gz` & `tmp/py-algorand-sdk-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-algorand-sdk-2.1.2.tar", last modified: Thu Mar 23 20:08:28 2023, max compression
+gzip compressed data, was "py-algorand-sdk-2.2.0.tar", last modified: Mon May  8 14:09:50 2023, max compression
```

## Comparing `py-algorand-sdk-2.1.2.tar` & `py-algorand-sdk-2.2.0.tar`

### file list

```diff
@@ -1,73 +1,90 @@
-drwxr-xr-x   0 arthurkepler   (502) staff       (20)        0 2023-03-23 20:08:28.071702 py-algorand-sdk-2.1.2/
--rw-r--r--   0 arthurkepler   (502) staff       (20)     1065 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/LICENSE
--rw-r--r--   0 arthurkepler   (502) staff       (20)       44 2023-01-03 23:38:30.000000 py-algorand-sdk-2.1.2/MANIFEST.in
--rw-r--r--   0 arthurkepler   (502) staff       (20)     4289 2023-03-23 20:08:28.071530 py-algorand-sdk-2.1.2/PKG-INFO
--rw-r--r--   0 arthurkepler   (502) staff       (20)     3923 2023-03-23 16:56:34.000000 py-algorand-sdk-2.1.2/README.md
-drwxr-xr-x   0 arthurkepler   (502) staff       (20)        0 2023-03-23 20:08:28.064581 py-algorand-sdk-2.1.2/algosdk/
--rw-r--r--   0 arthurkepler   (502) staff       (20)      745 2023-03-23 16:56:34.000000 py-algorand-sdk-2.1.2/algosdk/__init__.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     1115 2023-03-23 16:56:34.000000 py-algorand-sdk-2.1.2/algosdk/__init__.pyi
-drwxr-xr-x   0 arthurkepler   (502) staff       (20)        0 2023-03-23 20:08:28.067265 py-algorand-sdk-2.1.2/algosdk/abi/
--rw-r--r--   0 arthurkepler   (502) staff       (20)     1284 2023-03-23 16:56:34.000000 py-algorand-sdk-2.1.2/algosdk/abi/__init__.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     2711 2023-01-03 23:38:30.000000 py-algorand-sdk-2.1.2/algosdk/abi/address_type.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     3243 2023-01-03 23:38:30.000000 py-algorand-sdk-2.1.2/algosdk/abi/array_dynamic_type.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     3675 2023-01-03 23:38:30.000000 py-algorand-sdk-2.1.2/algosdk/abi/array_static_type.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     4709 2023-01-03 23:38:30.000000 py-algorand-sdk-2.1.2/algosdk/abi/base_type.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     1936 2023-01-03 23:38:30.000000 py-algorand-sdk-2.1.2/algosdk/abi/bool_type.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     1651 2023-01-03 23:38:30.000000 py-algorand-sdk-2.1.2/algosdk/abi/byte_type.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     3072 2023-01-03 23:38:30.000000 py-algorand-sdk-2.1.2/algosdk/abi/contract.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     1845 2023-03-23 16:56:34.000000 py-algorand-sdk-2.1.2/algosdk/abi/interface.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     7715 2023-03-23 16:56:34.000000 py-algorand-sdk-2.1.2/algosdk/abi/method.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)      389 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/abi/reference.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     2251 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/abi/string_type.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     1076 2023-01-03 23:38:30.000000 py-algorand-sdk-2.1.2/algosdk/abi/transaction.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)    12075 2023-01-03 23:38:30.000000 py-algorand-sdk-2.1.2/algosdk/abi/tuple_type.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     3165 2023-01-03 23:38:30.000000 py-algorand-sdk-2.1.2/algosdk/abi/ufixed_type.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     2510 2023-01-03 23:38:30.000000 py-algorand-sdk-2.1.2/algosdk/abi/uint_type.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)      767 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/account.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)    35035 2023-03-23 20:06:49.000000 py-algorand-sdk-2.1.2/algosdk/atomic_transaction_composer.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     4291 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/auction.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     3289 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/box_reference.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     4695 2023-01-03 23:38:30.000000 py-algorand-sdk-2.1.2/algosdk/constants.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     6981 2023-03-23 16:56:34.000000 py-algorand-sdk-2.1.2/algosdk/dryrun_results.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     5880 2023-01-03 23:38:30.000000 py-algorand-sdk-2.1.2/algosdk/encoding.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     5623 2023-03-23 16:56:34.000000 py-algorand-sdk-2.1.2/algosdk/error.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)    13368 2023-01-03 23:38:30.000000 py-algorand-sdk-2.1.2/algosdk/kmd.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     2061 2023-01-03 23:38:30.000000 py-algorand-sdk-2.1.2/algosdk/logic.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     5033 2023-01-03 23:38:30.000000 py-algorand-sdk-2.1.2/algosdk/mnemonic.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)        0 2023-01-03 23:38:30.000000 py-algorand-sdk-2.1.2/algosdk/py.typed
--rw-r--r--   0 arthurkepler   (502) staff       (20)     2803 2023-03-23 16:56:34.000000 py-algorand-sdk-2.1.2/algosdk/source_map.py
-drwxr-xr-x   0 arthurkepler   (502) staff       (20)        0 2023-03-23 20:08:28.067513 py-algorand-sdk-2.1.2/algosdk/testing/
--rw-r--r--   0 arthurkepler   (502) staff       (20)        0 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/testing/__init__.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)    27818 2023-03-23 16:56:34.000000 py-algorand-sdk-2.1.2/algosdk/testing/dryrun.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)   109072 2023-03-23 16:56:34.000000 py-algorand-sdk-2.1.2/algosdk/transaction.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     2543 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/util.py
-drwxr-xr-x   0 arthurkepler   (502) staff       (20)        0 2023-03-23 20:08:28.068155 py-algorand-sdk-2.1.2/algosdk/v2client/
--rw-r--r--   0 arthurkepler   (502) staff       (20)       93 2023-03-23 16:56:34.000000 py-algorand-sdk-2.1.2/algosdk/v2client/__init__.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)    22050 2023-03-23 16:56:34.000000 py-algorand-sdk-2.1.2/algosdk/v2client/algod.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)    36632 2023-03-23 16:56:34.000000 py-algorand-sdk-2.1.2/algosdk/v2client/indexer.py
-drwxr-xr-x   0 arthurkepler   (502) staff       (20)        0 2023-03-23 20:08:28.070758 py-algorand-sdk-2.1.2/algosdk/v2client/models/
--rw-r--r--   0 arthurkepler   (502) staff       (20)     1416 2023-03-23 16:56:34.000000 py-algorand-sdk-2.1.2/algosdk/v2client/models/__init__.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)    17792 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/v2client/models/account.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     8562 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/v2client/models/account_participation.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     3301 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/v2client/models/application.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     4367 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/v2client/models/application_local_state.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     7927 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/v2client/models/application_params.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     3782 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/v2client/models/application_state_schema.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     3255 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/v2client/models/asset.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     5346 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/v2client/models/asset_holding.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)    12993 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/v2client/models/asset_params.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     7734 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/v2client/models/dryrun_request.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     5163 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/v2client/models/dryrun_source.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     3181 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/v2client/models/teal_key_value.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     3928 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/v2client/models/teal_value.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)     7486 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/wallet.py
--rw-r--r--   0 arthurkepler   (502) staff       (20)    13267 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/algosdk/wordlist.py
-drwxr-xr-x   0 arthurkepler   (502) staff       (20)        0 2023-03-23 20:08:28.071358 py-algorand-sdk-2.1.2/py_algorand_sdk.egg-info/
--rw-r--r--   0 arthurkepler   (502) staff       (20)     4289 2023-03-23 20:08:28.000000 py-algorand-sdk-2.1.2/py_algorand_sdk.egg-info/PKG-INFO
--rw-r--r--   0 arthurkepler   (502) staff       (20)     1786 2023-03-23 20:08:28.000000 py-algorand-sdk-2.1.2/py_algorand_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 arthurkepler   (502) staff       (20)        1 2023-03-23 20:08:28.000000 py-algorand-sdk-2.1.2/py_algorand_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 arthurkepler   (502) staff       (20)       59 2023-03-23 20:08:28.000000 py-algorand-sdk-2.1.2/py_algorand_sdk.egg-info/requires.txt
--rw-r--r--   0 arthurkepler   (502) staff       (20)        8 2023-03-23 20:08:28.000000 py-algorand-sdk-2.1.2/py_algorand_sdk.egg-info/top_level.txt
--rw-r--r--   0 arthurkepler   (502) staff       (20)       30 2023-01-03 17:46:37.000000 py-algorand-sdk-2.1.2/pyproject.toml
--rw-r--r--   0 arthurkepler   (502) staff       (20)       38 2023-03-23 20:08:28.071741 py-algorand-sdk-2.1.2/setup.cfg
--rw-r--r--   0 arthurkepler   (502) staff       (20)      871 2023-03-23 20:07:10.000000 py-algorand-sdk-2.1.2/setup.py
+drwxr-xr-x   0 barbara    (502) staff       (20)        0 2023-05-08 14:09:50.463777 py-algorand-sdk-2.2.0/
+-rw-r--r--   0 barbara    (502) staff       (20)     1065 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/LICENSE
+-rw-r--r--   0 barbara    (502) staff       (20)       44 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/MANIFEST.in
+-rw-r--r--   0 barbara    (502) staff       (20)     4289 2023-05-08 14:09:50.463379 py-algorand-sdk-2.2.0/PKG-INFO
+-rw-r--r--   0 barbara    (502) staff       (20)     3923 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/README.md
+drwxr-xr-x   0 barbara    (502) staff       (20)        0 2023-05-08 14:09:50.422193 py-algorand-sdk-2.2.0/algosdk/
+-rw-r--r--   0 barbara    (502) staff       (20)      745 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/__init__.py
+-rw-r--r--   0 barbara    (502) staff       (20)     1115 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/__init__.pyi
+drwxr-xr-x   0 barbara    (502) staff       (20)        0 2023-05-08 14:09:50.432890 py-algorand-sdk-2.2.0/algosdk/abi/
+-rw-r--r--   0 barbara    (502) staff       (20)     1284 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/abi/__init__.py
+-rw-r--r--   0 barbara    (502) staff       (20)     2711 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/address_type.py
+-rw-r--r--   0 barbara    (502) staff       (20)     3243 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/array_dynamic_type.py
+-rw-r--r--   0 barbara    (502) staff       (20)     3675 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/array_static_type.py
+-rw-r--r--   0 barbara    (502) staff       (20)     4709 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/base_type.py
+-rw-r--r--   0 barbara    (502) staff       (20)     1936 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/bool_type.py
+-rw-r--r--   0 barbara    (502) staff       (20)     1651 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/byte_type.py
+-rw-r--r--   0 barbara    (502) staff       (20)     3072 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/contract.py
+-rw-r--r--   0 barbara    (502) staff       (20)     1845 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/abi/interface.py
+-rw-r--r--   0 barbara    (502) staff       (20)     7715 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/abi/method.py
+-rw-r--r--   0 barbara    (502) staff       (20)      389 2022-01-14 15:35:40.000000 py-algorand-sdk-2.2.0/algosdk/abi/reference.py
+-rw-r--r--   0 barbara    (502) staff       (20)     2251 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/string_type.py
+-rw-r--r--   0 barbara    (502) staff       (20)     1076 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/transaction.py
+-rw-r--r--   0 barbara    (502) staff       (20)    12075 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/tuple_type.py
+-rw-r--r--   0 barbara    (502) staff       (20)     3165 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/ufixed_type.py
+-rw-r--r--   0 barbara    (502) staff       (20)     2510 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/uint_type.py
+-rw-r--r--   0 barbara    (502) staff       (20)      767 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/account.py
+-rw-r--r--   0 barbara    (502) staff       (20)    36921 2023-05-08 14:08:12.000000 py-algorand-sdk-2.2.0/algosdk/atomic_transaction_composer.py
+-rw-r--r--   0 barbara    (502) staff       (20)     4291 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/auction.py
+-rw-r--r--   0 barbara    (502) staff       (20)     3289 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/box_reference.py
+-rw-r--r--   0 barbara    (502) staff       (20)     4705 2023-05-08 14:08:12.000000 py-algorand-sdk-2.2.0/algosdk/constants.py
+-rw-r--r--   0 barbara    (502) staff       (20)     6981 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/dryrun_results.py
+-rw-r--r--   0 barbara    (502) staff       (20)     5880 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/encoding.py
+-rw-r--r--   0 barbara    (502) staff       (20)     5623 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/error.py
+-rw-r--r--   0 barbara    (502) staff       (20)    13562 2023-05-08 14:08:12.000000 py-algorand-sdk-2.2.0/algosdk/kmd.py
+-rw-r--r--   0 barbara    (502) staff       (20)     2061 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/logic.py
+-rw-r--r--   0 barbara    (502) staff       (20)     5033 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/mnemonic.py
+-rw-r--r--   0 barbara    (502) staff       (20)        0 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/py.typed
+-rw-r--r--   0 barbara    (502) staff       (20)     2803 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/source_map.py
+drwxr-xr-x   0 barbara    (502) staff       (20)        0 2023-05-08 14:09:50.433963 py-algorand-sdk-2.2.0/algosdk/testing/
+-rw-r--r--   0 barbara    (502) staff       (20)        0 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/testing/__init__.py
+-rw-r--r--   0 barbara    (502) staff       (20)    27818 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/testing/dryrun.py
+-rw-r--r--   0 barbara    (502) staff       (20)   109053 2023-05-08 14:08:12.000000 py-algorand-sdk-2.2.0/algosdk/transaction.py
+-rw-r--r--   0 barbara    (502) staff       (20)     2543 2022-08-18 18:15:50.000000 py-algorand-sdk-2.2.0/algosdk/util.py
+drwxr-xr-x   0 barbara    (502) staff       (20)        0 2023-05-08 14:09:50.436761 py-algorand-sdk-2.2.0/algosdk/v2client/
+-rw-r--r--   0 barbara    (502) staff       (20)       93 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/v2client/__init__.py
+-rw-r--r--   0 barbara    (502) staff       (20)    24540 2023-05-08 14:08:12.000000 py-algorand-sdk-2.2.0/algosdk/v2client/algod.py
+-rw-r--r--   0 barbara    (502) staff       (20)    36632 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/v2client/indexer.py
+drwxr-xr-x   0 barbara    (502) staff       (20)        0 2023-05-08 14:09:50.448548 py-algorand-sdk-2.2.0/algosdk/v2client/models/
+-rw-r--r--   0 barbara    (502) staff       (20)     1612 2023-05-08 14:08:12.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/__init__.py
+-rw-r--r--   0 barbara    (502) staff       (20)    17792 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/account.py
+-rw-r--r--   0 barbara    (502) staff       (20)     8562 2022-02-15 21:52:01.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/account_participation.py
+-rw-r--r--   0 barbara    (502) staff       (20)     3301 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/application.py
+-rw-r--r--   0 barbara    (502) staff       (20)     4367 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/application_local_state.py
+-rw-r--r--   0 barbara    (502) staff       (20)     7927 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/application_params.py
+-rw-r--r--   0 barbara    (502) staff       (20)     3782 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/application_state_schema.py
+-rw-r--r--   0 barbara    (502) staff       (20)     3255 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/asset.py
+-rw-r--r--   0 barbara    (502) staff       (20)     5346 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/asset_holding.py
+-rw-r--r--   0 barbara    (502) staff       (20)    12993 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/asset_params.py
+-rw-r--r--   0 barbara    (502) staff       (20)     7734 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/dryrun_request.py
+-rw-r--r--   0 barbara    (502) staff       (20)     5163 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/dryrun_source.py
+-rw-r--r--   0 barbara    (502) staff       (20)     1238 2023-05-08 14:08:12.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/simulate_request.py
+-rw-r--r--   0 barbara    (502) staff       (20)     3181 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/teal_key_value.py
+-rw-r--r--   0 barbara    (502) staff       (20)     3928 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/teal_value.py
+-rw-r--r--   0 barbara    (502) staff       (20)     7486 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/wallet.py
+-rw-r--r--   0 barbara    (502) staff       (20)    13267 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/wordlist.py
+drwxr-xr-x   0 barbara    (502) staff       (20)        0 2023-05-08 14:09:50.452674 py-algorand-sdk-2.2.0/py_algorand_sdk.egg-info/
+-rw-r--r--   0 barbara    (502) staff       (20)     4289 2023-05-08 14:09:50.000000 py-algorand-sdk-2.2.0/py_algorand_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 barbara    (502) staff       (20)     2204 2023-05-08 14:09:50.000000 py-algorand-sdk-2.2.0/py_algorand_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 barbara    (502) staff       (20)        1 2023-05-08 14:09:50.000000 py-algorand-sdk-2.2.0/py_algorand_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 barbara    (502) staff       (20)       59 2023-05-08 14:09:50.000000 py-algorand-sdk-2.2.0/py_algorand_sdk.egg-info/requires.txt
+-rw-r--r--   0 barbara    (502) staff       (20)        8 2023-05-08 14:09:50.000000 py-algorand-sdk-2.2.0/py_algorand_sdk.egg-info/top_level.txt
+-rw-r--r--   0 barbara    (502) staff       (20)       30 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/pyproject.toml
+-rw-r--r--   0 barbara    (502) staff       (20)       38 2023-05-08 14:09:50.463880 py-algorand-sdk-2.2.0/setup.cfg
+-rw-r--r--   0 barbara    (502) staff       (20)      871 2023-05-08 14:08:22.000000 py-algorand-sdk-2.2.0/setup.py
+drwxr-xr-x   0 barbara    (502) staff       (20)        0 2023-05-08 14:09:50.453833 py-algorand-sdk-2.2.0/tests/
+-rw-r--r--   0 barbara    (502) staff       (20)        0 2022-08-18 18:15:50.000000 py-algorand-sdk-2.2.0/tests/__init__.py
+-rw-r--r--   0 barbara    (502) staff       (20)     4770 2023-05-08 14:08:12.000000 py-algorand-sdk-2.2.0/tests/environment.py
+drwxr-xr-x   0 barbara    (502) staff       (20)        0 2023-05-08 14:09:50.457853 py-algorand-sdk-2.2.0/tests/steps/
+-rw-r--r--   0 barbara    (502) staff       (20)        0 2022-08-18 18:15:50.000000 py-algorand-sdk-2.2.0/tests/steps/__init__.py
+-rw-r--r--   0 barbara    (502) staff       (20)     9561 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/tests/steps/account_v2_steps.py
+-rw-r--r--   0 barbara    (502) staff       (20)    44018 2023-05-05 20:18:25.000000 py-algorand-sdk-2.2.0/tests/steps/application_v2_steps.py
+-rw-r--r--   0 barbara    (502) staff       (20)    49356 2023-05-08 14:08:12.000000 py-algorand-sdk-2.2.0/tests/steps/other_v2_steps.py
+-rw-r--r--   0 barbara    (502) staff       (20)    26804 2023-05-08 14:08:12.000000 py-algorand-sdk-2.2.0/tests/steps/steps.py
+drwxr-xr-x   0 barbara    (502) staff       (20)        0 2023-05-08 14:09:50.462402 py-algorand-sdk-2.2.0/tests/unit_tests/
+-rw-r--r--   0 barbara    (502) staff       (20)        0 2022-08-18 18:15:50.000000 py-algorand-sdk-2.2.0/tests/unit_tests/__init__.py
+-rw-r--r--   0 barbara    (502) staff       (20)    26719 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/tests/unit_tests/test_abi.py
+-rw-r--r--   0 barbara    (502) staff       (20)    19987 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/tests/unit_tests/test_dryrun.py
+-rw-r--r--   0 barbara    (502) staff       (20)    40826 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/tests/unit_tests/test_logicsig.py
+-rw-r--r--   0 barbara    (502) staff       (20)    30241 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/tests/unit_tests/test_other.py
+-rw-r--r--   0 barbara    (502) staff       (20)    59966 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/tests/unit_tests/test_transaction.py
```

### Comparing `py-algorand-sdk-2.1.2/LICENSE` & `py-algorand-sdk-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/PKG-INFO` & `py-algorand-sdk-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-algorand-sdk
-Version: 2.1.2
+Version: 2.2.0
 Summary: Algorand SDK in Python
 Home-page: https://github.com/algorand/py-algorand-sdk
 Author: Algorand
 Author-email: pypiservice@algorand.com
 License: MIT
 Project-URL: Source, https://github.com/algorand/py-algorand-sdk
 Requires-Python: >=3.8
```

### Comparing `py-algorand-sdk-2.1.2/README.md` & `py-algorand-sdk-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/__init__.py` & `py-algorand-sdk-2.2.0/algosdk/__init__.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/__init__.pyi` & `py-algorand-sdk-2.2.0/algosdk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/abi/__init__.py` & `py-algorand-sdk-2.2.0/algosdk/abi/__init__.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/abi/address_type.py` & `py-algorand-sdk-2.2.0/algosdk/abi/address_type.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/abi/array_dynamic_type.py` & `py-algorand-sdk-2.2.0/algosdk/abi/array_dynamic_type.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/abi/array_static_type.py` & `py-algorand-sdk-2.2.0/algosdk/abi/array_static_type.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/abi/base_type.py` & `py-algorand-sdk-2.2.0/algosdk/abi/base_type.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/abi/bool_type.py` & `py-algorand-sdk-2.2.0/algosdk/abi/bool_type.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/abi/byte_type.py` & `py-algorand-sdk-2.2.0/algosdk/abi/byte_type.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/abi/contract.py` & `py-algorand-sdk-2.2.0/algosdk/abi/contract.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/abi/interface.py` & `py-algorand-sdk-2.2.0/algosdk/abi/interface.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/abi/method.py` & `py-algorand-sdk-2.2.0/algosdk/abi/method.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/abi/string_type.py` & `py-algorand-sdk-2.2.0/algosdk/abi/string_type.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/abi/transaction.py` & `py-algorand-sdk-2.2.0/algosdk/abi/transaction.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/abi/tuple_type.py` & `py-algorand-sdk-2.2.0/algosdk/abi/tuple_type.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/abi/ufixed_type.py` & `py-algorand-sdk-2.2.0/algosdk/abi/ufixed_type.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/abi/uint_type.py` & `py-algorand-sdk-2.2.0/algosdk/abi/uint_type.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/account.py` & `py-algorand-sdk-2.2.0/algosdk/account.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/atomic_transaction_composer.py` & `py-algorand-sdk-2.2.0/algosdk/atomic_transaction_composer.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     Union,
     cast,
 )
 
 from algosdk import abi, error, transaction
 from algosdk.transaction import GenericSignedTransaction
 from algosdk.abi.address_type import AddressType
-from algosdk.v2client import algod
+from algosdk.v2client import algod, models
+
 
 # The first four bytes of an ABI method call return must have this hash
 ABI_RETURN_HASH = b"\x15\x1f\x7c\x75"
 # Support for generic typing
 T = TypeVar("T")
 
 
@@ -251,43 +252,75 @@
         self,
         tx_id: str,
         raw_value: bytes,
         return_value: Any,
         decode_error: Optional[Exception],
         tx_info: dict,
         method: abi.Method,
-        missing_signature: bool,
     ) -> None:
         self.tx_id = tx_id
         self.raw_value = raw_value
         self.return_value = return_value
         self.decode_error = decode_error
         self.tx_info = tx_info
         self.method = method
-        self.missing_signature = missing_signature
+
+
+class SimulateEvalOverrides:
+    def __init__(
+        self,
+        *,
+        max_log_calls: Optional[int] = None,
+        max_log_size: Optional[int] = None,
+        allow_empty_signatures: Optional[bool] = None,
+    ) -> None:
+        self.max_log_calls = max_log_calls
+        self.max_log_size = max_log_size
+        self.allow_empty_signatures = allow_empty_signatures
+
+    @staticmethod
+    def from_simulation_result(
+        simulation_result: Dict[str, Any]
+    ) -> Optional["SimulateEvalOverrides"]:
+        if "eval-overrides" not in simulation_result:
+            return None
+
+        eval_override_dict = simulation_result.get("eval-overrides", dict())
+        eval_override = SimulateEvalOverrides()
+
+        if "max-log-calls" in eval_override_dict:
+            eval_override.max_log_calls = eval_override_dict["max-log-calls"]
+        if "max-log-size" in eval_override_dict:
+            eval_override.max_log_size = eval_override_dict["max-log-size"]
+        if "allow-empty-signatures" in eval_override_dict:
+            eval_override.allow_empty_signatures = eval_override_dict[
+                "allow-empty-signatures"
+            ]
+
+        return eval_override
 
 
 class SimulateAtomicTransactionResponse:
     def __init__(
         self,
         version: int,
-        would_succeed: bool,
         failure_message: str,
         failed_at: Optional[List[int]],
         simulate_response: Dict[str, Any],
         tx_ids: List[str],
         results: List[SimulateABIResult],
+        eval_overrides: Optional[SimulateEvalOverrides] = None,
     ) -> None:
         self.version = version
-        self.would_succeed = would_succeed
         self.failure_message = failure_message
         self.failed_at = failed_at
         self.simulate_response = simulate_response
         self.tx_ids = tx_ids
         self.abi_results = results
+        self.eval_overrides = eval_overrides
 
 
 class AtomicTransactionComposer:
     """
     Constructs an atomic transaction group which may contain a combination of
     Transactions and ABI Method calls.
 
@@ -491,23 +524,26 @@
         # First app arg must be the selector of the method
         app_args.append(method.get_selector())
 
         # Iterate through the method arguments and either pack a transaction
         # or encode a ABI value.
         for i, arg in enumerate(method.args):
             if abi.is_abi_transaction_type(arg.type):
-                if not isinstance(
-                    method_args[i], TransactionWithSigner
-                ) or not abi.check_abi_transaction_type(
+                if not isinstance(method_args[i], TransactionWithSigner):
+                    raise error.AtomicTransactionComposerError(
+                        "expected TransactionWithSigner as method argument, "
+                        f"but received: {method_args[i]}"
+                    )
+
+                if not abi.check_abi_transaction_type(
                     arg.type, method_args[i].txn
                 ):
                     raise error.AtomicTransactionComposerError(
-                        "expected TransactionWithSigner as method argument, but received: {}".format(
-                            method_args[i]
-                        )
+                        f"expected Transaction type {arg.type} as method argument, "
+                        f"but received: {method_args[i].txn.type}"
                     )
                 txn_list.append(method_args[i])
             else:
                 if abi.is_abi_reference_type(arg.type):
                     current_type: Union[str, abi.ABIType] = abi.UintType(8)
                     if arg.type == abi.ABIReferenceType.ACCOUNT:
                         address_type = AddressType()
@@ -679,24 +715,28 @@
             )
 
         client.send_transactions(self.signed_txns)
         self.status = AtomicTransactionComposerStatus.SUBMITTED
         return self.tx_ids
 
     def simulate(
-        self, client: algod.AlgodClient
+        self,
+        client: algod.AlgodClient,
+        request: Optional[models.SimulateRequest] = None,
     ) -> SimulateAtomicTransactionResponse:
         """
         Send the transaction group to the `simulate` endpoint and wait for results.
         An error will be thrown if submission or execution fails.
         The composer's status must be SUBMITTED or lower before calling this method,
         since execution is only allowed once.
 
         Args:
             client (AlgodClient): Algod V2 client
+            request (models.SimulateRequest): SimulateRequest with options in simulation.
+                The request's transaction group will be overrwritten by the composer's group, only simulation related options will be used.
 
         Returns:
             SimulateAtomicTransactionResponse: Object with simulation results for this
                 transaction group, a list of txIDs of the simulated transactions,
                 an array of results for each method call transaction in this group.
                 If a method has no return value (void), then the method results array
                 will contain None for that method's return value.
@@ -706,17 +746,26 @@
             self.gather_signatures()
         else:
             raise error.AtomicTransactionComposerError(
                 "AtomicTransactionComposerStatus must be submitted or "
                 "lower to simulate a group"
             )
 
+        current_simulation_request = (
+            request if request else models.SimulateRequest(txn_groups=list())
+        )
+        current_simulation_request.txn_groups = [
+            models.SimulateRequestTransactionGroup(txns=self.signed_txns)
+        ]
+
         simulation_result = cast(
-            Dict[str, Any], client.simulate_transactions(self.signed_txns)
+            Dict[str, Any],
+            client.simulate_transactions(current_simulation_request),
         )
+
         # Only take the first group in the simulate response
         txn_group: Dict[str, Any] = simulation_result["txn-groups"][0]
 
         # Parse out abi results
         txn_results = [t["txn-result"] for t in txn_group["txn-results"]]
         method_results: List[ABIResult] = []
         for method_index, method in self.method_dict.items():
@@ -747,26 +796,27 @@
                 SimulateABIResult(
                     tx_id=result.tx_id,
                     raw_value=result.raw_value,
                     return_value=result.return_value,
                     decode_error=result.decode_error,
                     tx_info=result.tx_info,
                     method=result.method,
-                    missing_signature=sim_txn.get("missing-signature", False),
                 )
             )
 
         return SimulateAtomicTransactionResponse(
             version=simulation_result.get("version", 0),
-            would_succeed=simulation_result.get("would-succeed", False),
             failure_message=txn_group.get("failure-message", ""),
             failed_at=txn_group.get("failed-at"),
             simulate_response=simulation_result,
             tx_ids=self.tx_ids,
             results=sim_results,
+            eval_overrides=SimulateEvalOverrides.from_simulation_result(
+                simulation_result
+            ),
         )
 
     def execute(
         self, client: algod.AlgodClient, wait_rounds: int
     ) -> AtomicTransactionResponse:
         """
         Send the transaction group to the network and wait until it's committed
```

### Comparing `py-algorand-sdk-2.1.2/algosdk/auction.py` & `py-algorand-sdk-2.2.0/algosdk/auction.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/box_reference.py` & `py-algorand-sdk-2.2.0/algosdk/box_reference.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/constants.py` & `py-algorand-sdk-2.2.0/algosdk/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 KMD_AUTH_HEADER = "X-KMD-API-Token"
 """str: header key for kmd requests"""
 ALGOD_AUTH_HEADER = "X-Algo-API-Token"
 """str: header key for algod requests"""
 INDEXER_AUTH_HEADER = "X-Indexer-API-Token"
 """str: header key for indexer requests"""
-UNVERSIONED_PATHS = ["/health", "/versions", "/metrics", "/genesis"]
+UNVERSIONED_PATHS = ["/health", "/versions", "/metrics", "/genesis", "/ready"]
 """str[]: paths that don't use the version path prefix"""
 NO_AUTH: List[str] = []
 """str[]: requests that don't require authentication"""
 
 
 # transaction types
 PAYMENT_TXN = "pay"
```

### Comparing `py-algorand-sdk-2.1.2/algosdk/dryrun_results.py` & `py-algorand-sdk-2.2.0/algosdk/dryrun_results.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/encoding.py` & `py-algorand-sdk-2.2.0/algosdk/encoding.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/error.py` & `py-algorand-sdk-2.2.0/algosdk/error.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/kmd.py` & `py-algorand-sdk-2.2.0/algosdk/kmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -429,11 +429,16 @@
         query = {
             "wallet_handle_token": handle,
             "wallet_password": password,
             "transaction": txn,
             "public_key": public_key,
             "partial_multisig": partial,
         }
+
+        if hasattr(mtx, "auth_addr") and mtx.auth_addr is not None:
+            signer = base64.b64encode(encoding.decode_address(mtx.auth_addr))
+            query["signer"] = signer.decode()
+
         result = self.kmd_request("POST", req, data=query)["multisig"]
         msig = encoding.msgpack_decode(result)
         mtx.multisig = msig
         return mtx
```

### Comparing `py-algorand-sdk-2.1.2/algosdk/logic.py` & `py-algorand-sdk-2.2.0/algosdk/logic.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/mnemonic.py` & `py-algorand-sdk-2.2.0/algosdk/mnemonic.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/source_map.py` & `py-algorand-sdk-2.2.0/algosdk/source_map.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/testing/dryrun.py` & `py-algorand-sdk-2.2.0/algosdk/testing/dryrun.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/transaction.py` & `py-algorand-sdk-2.2.0/algosdk/transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -3229,15 +3229,15 @@
 
 
 defaultAppId = 1380011588
 
 
 def create_dryrun(
     client: algod.AlgodClient,
-    txns: List[Union[SignedTransaction, LogicSigTransaction]],
+    txns: List["GenericSignedTransaction"],
     protocol_version=None,
     latest_timestamp=None,
     round=None,
 ) -> models.DryrunRequest:
     """
     Create DryrunRequest object from a client and list of signed transactions
```

### Comparing `py-algorand-sdk-2.1.2/algosdk/util.py` & `py-algorand-sdk-2.2.0/algosdk/util.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/v2client/algod.py` & `py-algorand-sdk-2.2.0/algosdk/v2client/algod.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     cast,
 )
 import urllib.error
 from urllib import parse
 from urllib.request import Request, urlopen
 
 from algosdk import constants, encoding, error, transaction, util
+from algosdk.v2client import models
 
 AlgodResponseType = Union[Dict[str, Any], bytes]
 
 # for compatibility with urllib.parse.urlencode
 ParamsType = Union[Mapping[str, Any], Sequence[Tuple[str, Any]]]
 
 api_version_path_prefix = "/v2"
@@ -108,14 +109,19 @@
                 e = json.loads(es)["message"]
             finally:
                 raise error.AlgodHTTPError(e, code)
         if response_format == "json":
             try:
                 return json.load(resp)
             except Exception as e:
+                # Some algod responses currently return a 200 OK
+                # but have an empty response.
+                # Do not return an error, and just return an empty response.
+                if resp.status == 200 and resp.length == 0:
+                    return {}
                 raise error.AlgodResponseError(
                     "Failed to parse JSON response from algod"
                 ) from e
         else:
             return resp.read()
 
     @classmethod
@@ -303,21 +309,21 @@
         """
         req = "/status/wait-for-block-after/" + _specify_round_string(
             block_num, round_num
         )
         return self.algod_request("GET", req, **kwargs)
 
     def send_transaction(
-        self, txn: "transaction.Transaction", **kwargs: Any
+        self, txn: "transaction.GenericSignedTransaction", **kwargs: Any
     ) -> str:
         """
         Broadcast a signed transaction object to the network.
 
         Args:
-            txn (SignedTransaction or MultisigTransaction): transaction to send
+            txn (SignedTransaction, LogicSigTransaction, or MultisigTransaction): transaction to send
             request_header (dict, optional): additional header for request
 
         Returns:
             str: transaction ID
         """
         assert not isinstance(
             txn, transaction.Transaction
@@ -594,56 +600,127 @@
             round_num (int): The round in which the transaction appears.
         """
         req = "/blocks/{}/hash".format(round_num)
         return self.algod_request("GET", req, **kwargs)
 
     def simulate_transactions(
         self,
-        txns: "Iterable[transaction.GenericSignedTransaction]",
+        request: models.SimulateRequest,
         **kwargs: Any,
     ) -> AlgodResponseType:
         """
-        Simulate a list of a signed transaction objects being sent to the network.
+        Simulate transactions being sent to the network.
 
         Args:
-            txns (SignedTransaction[] or MultisigTransaction[]):
-                transactions to send
-            request_header (dict, optional): additional header for request
+            request (models.SimulateRequest): Simulation request object
+            headers (dict, optional): additional header for request
 
         Returns:
-            Dict[str, Any]: results from simulation of transaction group
+            Dict[str, Any]: results from simulation of transactions
         """
-        serialized = []
-        for txn in txns:
-            serialized.append(base64.b64decode(encoding.msgpack_encode(txn)))
-
-        return self.simulate_raw_transaction(
-            base64.b64encode(b"".join(serialized)), **kwargs
+        body = base64.b64decode(encoding.msgpack_encode(request))
+        req = "/transactions/simulate"
+        headers = util.build_headers_from(
+            kwargs.get("headers", False),
+            {"Content-Type": "application/msgpack"},
         )
+        kwargs["headers"] = headers
+        return self.algod_request("POST", req, data=body, **kwargs)
 
-    def simulate_raw_transaction(self, txn, **kwargs):
+    def simulate_raw_transactions(
+        self, txns: "Sequence[transaction.GenericSignedTransaction]", **kwargs
+    ):
         """
-        Simulate a transaction group
+        Simulate a transaction group being sent to the network.
 
         Args:
-            txn (str): transaction to send, encoded in base64
-            request_header (dict, optional): additional header for request
+            txns (Sequence[transaction.GenericSignedTransaction]): transaction group to simulate
+            headers (dict, optional): additional header for request
 
         Returns:
-            Dict[str, Any]: results from simulation of transaction group
+            Dict[str, Any]: results from simulation of transactions
         """
-        txn = base64.b64decode(txn)
-        req = "/transactions/simulate"
-        headers = util.build_headers_from(
-            kwargs.get("headers", False),
-            {"Content-Type": "application/x-binary"},
+        request = models.SimulateRequest(
+            txn_groups=[
+                models.SimulateRequestTransactionGroup(txns=list(txns))
+            ]
         )
-        kwargs["headers"] = headers
+        return self.simulate_transactions(request, **kwargs)
+
+    def get_sync_round(self, **kwargs: Any) -> AlgodResponseType:
+        """
+        Get the minimum sync round for the ledger.
+
+        Returns:
+            Dict[str, Any]: Response from algod
+        """
+        req = "/ledger/sync"
+        return self.algod_request("GET", req, **kwargs)
+
+    def set_sync_round(self, round: int, **kwargs: Any) -> AlgodResponseType:
+        """
+        Set the minimum sync round for the ledger.
 
-        return self.algod_request("POST", req, data=txn, **kwargs)
+        Args:
+            round (int): Sync round
+
+        Returns:
+            Dict[str, Any]: Response from algod
+        """
+        req = f"/ledger/sync/{round}"
+        return self.algod_request("POST", req, **kwargs)
+
+    def unset_sync_round(self, **kwargs: Any) -> AlgodResponseType:
+        """
+        Unset the minimum sync round for the ledger.
+
+        Returns:
+            Dict[str, Any]: Response from algod
+        """
+        req = "/ledger/sync"
+        return self.algod_request("DELETE", req, **kwargs)
+
+    def ready(self, **kwargs: Any) -> AlgodResponseType:
+        """
+        Returns OK if the node is healthy and fully caught up.
+
+        Returns:
+            Dict[str, Any]: Response from algod
+        """
+        req = "/ready"
+        return self.algod_request("GET", req, **kwargs)
+
+    def get_timestamp_offset(self, **kwargs: Any) -> AlgodResponseType:
+        """
+        Get the timestamp offset in block headers.
+        This feature is only available in dev mode networks.
+
+        Returns:
+            Dict[str, Any]: Response from algod
+        """
+        req = "/devmode/blocks/offset"
+        return self.algod_request("GET", req, **kwargs)
+
+    def set_timestamp_offset(
+        self,
+        offset: int,
+        **kwargs: Any,
+    ) -> AlgodResponseType:
+        """
+        Set the timestamp offset in block headers.
+        This feature is only available in dev mode networks.
+
+        Args:
+            offset (int): Block timestamp offset
+
+        Returns:
+            Dict[str, Any]: Response from algod
+        """
+        req = f"/devmode/blocks/offset/{offset}"
+        return self.algod_request("POST", req, **kwargs)
 
 
 def _specify_round_string(
     block: Union[int, None], round_num: Union[int, None]
 ) -> str:
     """
     Return the round number specified in either 'block' or 'round_num'.
```

### Comparing `py-algorand-sdk-2.1.2/algosdk/v2client/indexer.py` & `py-algorand-sdk-2.2.0/algosdk/v2client/indexer.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/v2client/models/__init__.py` & `py-algorand-sdk-2.2.0/algosdk/v2client/models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,22 +27,29 @@
 from algosdk.v2client.models.asset import Asset
 from algosdk.v2client.models.asset_holding import AssetHolding
 from algosdk.v2client.models.asset_params import AssetParams
 from algosdk.v2client.models.dryrun_request import DryrunRequest
 from algosdk.v2client.models.dryrun_source import DryrunSource
 from algosdk.v2client.models.teal_key_value import TealKeyValue
 from algosdk.v2client.models.teal_value import TealValue
+from algosdk.v2client.models.simulate_request import (
+    SimulateRequest,
+    SimulateRequestTransactionGroup,
+)
 
 __all__ = [
     "Account",
     "AccountParticipation",
+    "Application",
     "ApplicationLocalState",
     "ApplicationParams",
     "ApplicationStateSchema",
     "Asset",
     "AssetHolding",
     "AssetParams",
     "DryrunRequest",
     "DryrunSource",
     "TealKeyValue",
     "TealValue",
+    "SimulateRequest",
+    "SimulateRequestTransactionGroup",
 ]
```

### Comparing `py-algorand-sdk-2.1.2/algosdk/v2client/models/account.py` & `py-algorand-sdk-2.2.0/algosdk/v2client/models/account.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/v2client/models/account_participation.py` & `py-algorand-sdk-2.2.0/algosdk/v2client/models/account_participation.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/v2client/models/application.py` & `py-algorand-sdk-2.2.0/algosdk/v2client/models/application.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/v2client/models/application_local_state.py` & `py-algorand-sdk-2.2.0/algosdk/v2client/models/application_local_state.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/v2client/models/application_params.py` & `py-algorand-sdk-2.2.0/algosdk/v2client/models/application_params.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/v2client/models/application_state_schema.py` & `py-algorand-sdk-2.2.0/algosdk/v2client/models/application_state_schema.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/v2client/models/asset.py` & `py-algorand-sdk-2.2.0/algosdk/v2client/models/asset.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/v2client/models/asset_holding.py` & `py-algorand-sdk-2.2.0/algosdk/v2client/models/asset_holding.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/v2client/models/asset_params.py` & `py-algorand-sdk-2.2.0/algosdk/v2client/models/asset_params.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/v2client/models/dryrun_request.py` & `py-algorand-sdk-2.2.0/algosdk/v2client/models/dryrun_request.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/v2client/models/dryrun_source.py` & `py-algorand-sdk-2.2.0/algosdk/v2client/models/dryrun_source.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/v2client/models/teal_key_value.py` & `py-algorand-sdk-2.2.0/algosdk/v2client/models/teal_key_value.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/v2client/models/teal_value.py` & `py-algorand-sdk-2.2.0/algosdk/v2client/models/teal_value.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/wallet.py` & `py-algorand-sdk-2.2.0/algosdk/wallet.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/algosdk/wordlist.py` & `py-algorand-sdk-2.2.0/algosdk/wordlist.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.1.2/py_algorand_sdk.egg-info/PKG-INFO` & `py-algorand-sdk-2.2.0/py_algorand_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-algorand-sdk
-Version: 2.1.2
+Version: 2.2.0
 Summary: Algorand SDK in Python
 Home-page: https://github.com/algorand/py-algorand-sdk
 Author: Algorand
 Author-email: pypiservice@algorand.com
 License: MIT
 Project-URL: Source, https://github.com/algorand/py-algorand-sdk
 Requires-Python: >=3.8
```

### Comparing `py-algorand-sdk-2.1.2/py_algorand_sdk.egg-info/SOURCES.txt` & `py-algorand-sdk-2.2.0/py_algorand_sdk.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -51,14 +51,28 @@
 algosdk/v2client/models/application_params.py
 algosdk/v2client/models/application_state_schema.py
 algosdk/v2client/models/asset.py
 algosdk/v2client/models/asset_holding.py
 algosdk/v2client/models/asset_params.py
 algosdk/v2client/models/dryrun_request.py
 algosdk/v2client/models/dryrun_source.py
+algosdk/v2client/models/simulate_request.py
 algosdk/v2client/models/teal_key_value.py
 algosdk/v2client/models/teal_value.py
 py_algorand_sdk.egg-info/PKG-INFO
 py_algorand_sdk.egg-info/SOURCES.txt
 py_algorand_sdk.egg-info/dependency_links.txt
 py_algorand_sdk.egg-info/requires.txt
-py_algorand_sdk.egg-info/top_level.txt
+py_algorand_sdk.egg-info/top_level.txt
+tests/__init__.py
+tests/environment.py
+tests/steps/__init__.py
+tests/steps/account_v2_steps.py
+tests/steps/application_v2_steps.py
+tests/steps/other_v2_steps.py
+tests/steps/steps.py
+tests/unit_tests/__init__.py
+tests/unit_tests/test_abi.py
+tests/unit_tests/test_dryrun.py
+tests/unit_tests/test_logicsig.py
+tests/unit_tests/test_other.py
+tests/unit_tests/test_transaction.py
```

### Comparing `py-algorand-sdk-2.1.2/setup.py` & `py-algorand-sdk-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = f.read()
 
 setuptools.setup(
     name="py-algorand-sdk",
     description="Algorand SDK in Python",
     author="Algorand",
     author_email="pypiservice@algorand.com",
-    version="2.1.2",
+    version="2.2.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/algorand/py-algorand-sdk",
     license="MIT",
     project_urls={
         "Source": "https://github.com/algorand/py-algorand-sdk",
     },
```

