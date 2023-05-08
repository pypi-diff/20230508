# Comparing `tmp/chainlib-eth-0.4.8.tar.gz` & `tmp/chainlib-eth-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlib-eth-0.4.8.tar", last modified: Wed Dec 21 08:12:44 2022, max compression
+gzip compressed data, was "chainlib-eth-0.4.9.tar", last modified: Fri Feb  3 09:18:24 2023, max compression
```

## Comparing `chainlib-eth-0.4.8.tar` & `chainlib-eth-0.4.9.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-12-21 08:12:44.072649 chainlib-eth-0.4.8/
--rw-r--r--   0 lash      (1000) lash      (1000)     2080 2022-12-16 08:29:08.000000 chainlib-eth-0.4.8/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:13:49.000000 chainlib-eth-0.4.8/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       89 2022-11-14 07:21:26.000000 chainlib-eth-0.4.8/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      731 2022-12-21 08:12:44.072649 chainlib-eth-0.4.8/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      146 2022-11-14 18:46:19.000000 chainlib-eth-0.4.8/README.md
--rw-r--r--   0 lash      (1000) lash      (1000)      872 2022-11-14 07:16:48.000000 chainlib-eth-0.4.8/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 07:16:57.000000 chainlib-eth-0.4.8/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-12-21 08:12:44.062649 chainlib-eth-0.4.8/chainlib/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-12-21 08:12:44.065983 chainlib-eth-0.4.8/chainlib/eth/
--rw-r--r--   0 lash      (1000) lash      (1000)     1029 2022-02-27 09:47:47.000000 chainlib-eth-0.4.8/chainlib/eth/address.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4296 2022-12-16 08:27:32.000000 chainlib-eth-0.4.8/chainlib/eth/block.py
--rw-r--r--   0 lash      (1000) lash      (1000)      420 2021-10-10 10:18:45.000000 chainlib-eth-0.4.8/chainlib/eth/chain.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-12-21 08:12:44.069316 chainlib-eth-0.4.8/chainlib/eth/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)       94 2021-10-18 11:32:11.000000 chainlib-eth-0.4.8/chainlib/eth/cli/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      474 2022-11-04 07:29:23.000000 chainlib-eth-0.4.8/chainlib/eth/cli/arg.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1135 2022-11-04 07:29:23.000000 chainlib-eth-0.4.8/chainlib/eth/cli/config.py
--rw-r--r--   0 lash      (1000) lash      (1000)      515 2022-11-06 10:28:58.000000 chainlib-eth-0.4.8/chainlib/eth/cli/decode.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2479 2021-12-21 14:52:18.000000 chainlib-eth-0.4.8/chainlib/eth/cli/encode.py
--rw-r--r--   0 lash      (1000) lash      (1000)       41 2022-10-13 13:18:24.000000 chainlib-eth-0.4.8/chainlib/eth/cli/log.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2362 2022-10-13 13:18:24.000000 chainlib-eth-0.4.8/chainlib/eth/cli/rpc.py
--rw-r--r--   0 lash      (1000) lash      (1000)      629 2022-10-13 13:18:24.000000 chainlib-eth-0.4.8/chainlib/eth/cli/wallet.py
--rw-r--r--   0 lash      (1000) lash      (1000)     7796 2021-12-21 14:52:18.000000 chainlib-eth-0.4.8/chainlib/eth/connection.py
--rw-r--r--   0 lash      (1000) lash      (1000)      248 2021-10-10 10:18:45.000000 chainlib-eth-0.4.8/chainlib/eth/constant.py
--rw-r--r--   0 lash      (1000) lash      (1000)    15644 2022-12-19 08:03:44.000000 chainlib-eth-0.4.8/chainlib/eth/contract.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-12-21 08:12:44.062649 chainlib-eth-0.4.8/chainlib/eth/data/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-12-21 08:12:44.069316 chainlib-eth-0.4.8/chainlib/eth/data/config/
--rw-r--r--   0 lash      (1000) lash      (1000)      275 2022-10-13 13:18:24.000000 chainlib-eth-0.4.8/chainlib/eth/data/config/config.ini
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-12-21 08:12:44.069316 chainlib-eth-0.4.8/chainlib/eth/dialect/
--rw-r--r--   0 lash      (1000) lash      (1000)      597 2022-12-16 09:15:51.000000 chainlib-eth-0.4.8/chainlib/eth/dialect/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      486 2021-10-10 10:18:45.000000 chainlib-eth-0.4.8/chainlib/eth/dialect/openethereum.py
--rw-r--r--   0 lash      (1000) lash      (1000)      578 2021-10-10 10:18:45.000000 chainlib-eth-0.4.8/chainlib/eth/error.py
--rw-r--r--   0 lash      (1000) lash      (1000)     9041 2021-12-21 14:52:18.000000 chainlib-eth-0.4.8/chainlib/eth/gas.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2080 2022-12-10 10:08:49.000000 chainlib-eth-0.4.8/chainlib/eth/jsonrpc.py
--rw-r--r--   0 lash      (1000) lash      (1000)      726 2021-10-10 10:18:45.000000 chainlib-eth-0.4.8/chainlib/eth/log.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3659 2022-10-13 13:18:24.000000 chainlib-eth-0.4.8/chainlib/eth/nonce.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-12-21 08:12:44.069316 chainlib-eth-0.4.8/chainlib/eth/pytest/
--rw-r--r--   0 lash      (1000) lash      (1000)       95 2021-10-10 10:18:45.000000 chainlib-eth-0.4.8/chainlib/eth/pytest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      296 2021-10-10 10:18:45.000000 chainlib-eth-0.4.8/chainlib/eth/pytest/fixtures_chain.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2535 2021-12-21 14:52:18.000000 chainlib-eth-0.4.8/chainlib/eth/pytest/fixtures_ethtester.py
--rw-r--r--   0 lash      (1000) lash      (1000)      310 2021-12-21 14:52:18.000000 chainlib-eth-0.4.8/chainlib/eth/pytest/fixtures_signer.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-12-21 08:12:44.072649 chainlib-eth-0.4.8/chainlib/eth/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 10:18:45.000000 chainlib-eth-0.4.8/chainlib/eth/runnable/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2815 2022-11-04 07:29:23.000000 chainlib-eth-0.4.8/chainlib/eth/runnable/balance.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4512 2022-11-06 10:28:58.000000 chainlib-eth-0.4.8/chainlib/eth/runnable/block.py
--rw-r--r--   0 lash      (1000) lash      (1000)      694 2022-11-04 07:29:23.000000 chainlib-eth-0.4.8/chainlib/eth/runnable/checksum.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2364 2022-11-04 07:29:23.000000 chainlib-eth-0.4.8/chainlib/eth/runnable/count.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2212 2022-11-06 10:28:58.000000 chainlib-eth-0.4.8/chainlib/eth/runnable/decode.py
--rw-r--r--   0 lash      (1000) lash      (1000)     7400 2022-11-06 10:28:58.000000 chainlib-eth-0.4.8/chainlib/eth/runnable/encode.py
--rw-r--r--   0 lash      (1000) lash      (1000)      996 2022-11-12 13:31:10.000000 chainlib-eth-0.4.8/chainlib/eth/runnable/flags.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6130 2022-11-06 10:28:58.000000 chainlib-eth-0.4.8/chainlib/eth/runnable/gas.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4628 2022-11-04 07:29:23.000000 chainlib-eth-0.4.8/chainlib/eth/runnable/get.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5205 2022-11-04 07:29:23.000000 chainlib-eth-0.4.8/chainlib/eth/runnable/info.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5572 2022-11-06 10:28:58.000000 chainlib-eth-0.4.8/chainlib/eth/runnable/raw.py
--rw-r--r--   0 lash      (1000) lash      (1000)      303 2021-10-10 10:18:45.000000 chainlib-eth-0.4.8/chainlib/eth/runnable/subscribe.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4102 2022-11-06 10:28:58.000000 chainlib-eth-0.4.8/chainlib/eth/runnable/wait.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5679 2022-11-04 07:29:23.000000 chainlib-eth-0.4.8/chainlib/eth/settings.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1833 2021-10-10 10:18:45.000000 chainlib-eth-0.4.8/chainlib/eth/sign.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1209 2022-11-04 07:29:23.000000 chainlib-eth-0.4.8/chainlib/eth/src.py
--rw-r--r--   0 lash      (1000) lash      (1000)    25829 2022-12-16 09:16:07.000000 chainlib-eth-0.4.8/chainlib/eth/tx.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-12-21 08:12:44.072649 chainlib-eth-0.4.8/chainlib/eth/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)     6361 2021-12-21 14:52:18.000000 chainlib-eth-0.4.8/chainlib/eth/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2551 2021-12-21 14:52:18.000000 chainlib-eth-0.4.8/chainlib/eth/unittest/ethtester.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-12-21 08:12:44.072649 chainlib-eth-0.4.8/chainlib_eth.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      731 2022-12-21 08:12:44.000000 chainlib-eth-0.4.8/chainlib_eth.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1642 2022-12-21 08:12:44.000000 chainlib-eth-0.4.8/chainlib_eth.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2022-12-21 08:12:44.000000 chainlib-eth-0.4.8/chainlib_eth.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      556 2022-12-21 08:12:44.000000 chainlib-eth-0.4.8/chainlib_eth.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      104 2022-12-21 08:12:44.000000 chainlib-eth-0.4.8/chainlib_eth.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        9 2022-12-21 08:12:44.000000 chainlib-eth-0.4.8/chainlib_eth.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      104 2022-11-04 07:31:55.000000 chainlib-eth-0.4.8/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)     1468 2022-12-21 08:12:44.075983 chainlib-eth-0.4.8/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      474 2022-11-08 10:59:04.000000 chainlib-eth-0.4.8/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       76 2021-12-21 14:52:18.000000 chainlib-eth-0.4.8/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.666658 chainlib-eth-0.4.9/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2080 2022-12-16 08:29:08.000000 chainlib-eth-0.4.9/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:13:49.000000 chainlib-eth-0.4.9/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       89 2022-11-14 07:21:26.000000 chainlib-eth-0.4.9/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      731 2023-02-03 09:18:24.666658 chainlib-eth-0.4.9/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      146 2022-11-14 18:46:19.000000 chainlib-eth-0.4.9/README.md
+-rw-r--r--   0 lash      (1000) lash      (1000)      872 2022-11-14 07:16:48.000000 chainlib-eth-0.4.9/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 07:16:57.000000 chainlib-eth-0.4.9/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.659991 chainlib-eth-0.4.9/chainlib/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.663324 chainlib-eth-0.4.9/chainlib/eth/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1029 2022-02-27 09:47:47.000000 chainlib-eth-0.4.9/chainlib/eth/address.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4296 2022-12-16 08:27:32.000000 chainlib-eth-0.4.9/chainlib/eth/block.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      420 2021-10-10 10:18:45.000000 chainlib-eth-0.4.9/chainlib/eth/chain.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.663324 chainlib-eth-0.4.9/chainlib/eth/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)       94 2021-10-18 11:32:11.000000 chainlib-eth-0.4.9/chainlib/eth/cli/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      474 2022-11-04 07:29:23.000000 chainlib-eth-0.4.9/chainlib/eth/cli/arg.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1135 2022-11-04 07:29:23.000000 chainlib-eth-0.4.9/chainlib/eth/cli/config.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      515 2022-11-06 10:28:58.000000 chainlib-eth-0.4.9/chainlib/eth/cli/decode.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2479 2021-12-21 14:52:18.000000 chainlib-eth-0.4.9/chainlib/eth/cli/encode.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       41 2022-10-13 13:18:24.000000 chainlib-eth-0.4.9/chainlib/eth/cli/log.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2362 2022-10-13 13:18:24.000000 chainlib-eth-0.4.9/chainlib/eth/cli/rpc.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      629 2022-10-13 13:18:24.000000 chainlib-eth-0.4.9/chainlib/eth/cli/wallet.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     7796 2021-12-21 14:52:18.000000 chainlib-eth-0.4.9/chainlib/eth/connection.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      248 2021-10-10 10:18:45.000000 chainlib-eth-0.4.9/chainlib/eth/constant.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    15644 2022-12-19 08:03:44.000000 chainlib-eth-0.4.9/chainlib/eth/contract.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.659991 chainlib-eth-0.4.9/chainlib/eth/data/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.663324 chainlib-eth-0.4.9/chainlib/eth/data/config/
+-rw-r--r--   0 lash      (1000) lash      (1000)      275 2022-10-13 13:18:24.000000 chainlib-eth-0.4.9/chainlib/eth/data/config/config.ini
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.663324 chainlib-eth-0.4.9/chainlib/eth/dialect/
+-rw-r--r--   0 lash      (1000) lash      (1000)      597 2022-12-16 09:15:51.000000 chainlib-eth-0.4.9/chainlib/eth/dialect/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      486 2021-10-10 10:18:45.000000 chainlib-eth-0.4.9/chainlib/eth/dialect/openethereum.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      578 2021-10-10 10:18:45.000000 chainlib-eth-0.4.9/chainlib/eth/error.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     9041 2021-12-21 14:52:18.000000 chainlib-eth-0.4.9/chainlib/eth/gas.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2080 2022-12-10 10:08:49.000000 chainlib-eth-0.4.9/chainlib/eth/jsonrpc.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      726 2021-10-10 10:18:45.000000 chainlib-eth-0.4.9/chainlib/eth/log.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3659 2022-10-13 13:18:24.000000 chainlib-eth-0.4.9/chainlib/eth/nonce.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.663324 chainlib-eth-0.4.9/chainlib/eth/pytest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       95 2021-10-10 10:18:45.000000 chainlib-eth-0.4.9/chainlib/eth/pytest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      296 2021-10-10 10:18:45.000000 chainlib-eth-0.4.9/chainlib/eth/pytest/fixtures_chain.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2535 2021-12-21 14:52:18.000000 chainlib-eth-0.4.9/chainlib/eth/pytest/fixtures_ethtester.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      310 2021-12-21 14:52:18.000000 chainlib-eth-0.4.9/chainlib/eth/pytest/fixtures_signer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.663324 chainlib-eth-0.4.9/chainlib/eth/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 10:18:45.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2815 2022-11-04 07:29:23.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/balance.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4512 2022-11-06 10:28:58.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/block.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      694 2022-11-04 07:29:23.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/checksum.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2364 2022-11-04 07:29:23.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/count.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2212 2022-11-06 10:28:58.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/decode.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     7400 2022-11-06 10:28:58.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/encode.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      996 2022-11-12 13:31:10.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/flags.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6114 2023-02-03 09:18:20.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/gas.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4628 2022-11-04 07:29:23.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/get.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5205 2022-11-04 07:29:23.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/info.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5572 2022-11-06 10:28:58.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/raw.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      303 2021-10-10 10:18:45.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/subscribe.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4102 2022-11-06 10:28:58.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/wait.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5726 2023-02-03 09:18:20.000000 chainlib-eth-0.4.9/chainlib/eth/settings.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1833 2021-10-10 10:18:45.000000 chainlib-eth-0.4.9/chainlib/eth/sign.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1209 2022-11-04 07:29:23.000000 chainlib-eth-0.4.9/chainlib/eth/src.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    25819 2023-02-03 09:18:20.000000 chainlib-eth-0.4.9/chainlib/eth/tx.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.666658 chainlib-eth-0.4.9/chainlib/eth/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)     6361 2021-12-21 14:52:18.000000 chainlib-eth-0.4.9/chainlib/eth/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2551 2021-12-21 14:52:18.000000 chainlib-eth-0.4.9/chainlib/eth/unittest/ethtester.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.666658 chainlib-eth-0.4.9/chainlib_eth.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      731 2023-02-03 09:18:24.000000 chainlib-eth-0.4.9/chainlib_eth.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1642 2023-02-03 09:18:24.000000 chainlib-eth-0.4.9/chainlib_eth.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-02-03 09:18:24.000000 chainlib-eth-0.4.9/chainlib_eth.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      556 2023-02-03 09:18:24.000000 chainlib-eth-0.4.9/chainlib_eth.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      104 2023-02-03 09:18:24.000000 chainlib-eth-0.4.9/chainlib_eth.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-02-03 09:18:24.000000 chainlib-eth-0.4.9/chainlib_eth.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      104 2022-11-04 07:31:55.000000 chainlib-eth-0.4.9/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)     1468 2023-02-03 09:18:24.666658 chainlib-eth-0.4.9/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      474 2022-11-08 10:59:04.000000 chainlib-eth-0.4.9/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       76 2021-12-21 14:52:18.000000 chainlib-eth-0.4.9/test_requirements.txt
```

### Comparing `chainlib-eth-0.4.8/CHANGELOG` & `chainlib-eth-0.4.9/CHANGELOG`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/LICENSE` & `chainlib-eth-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/PKG-INFO` & `chainlib-eth-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlib-eth
-Version: 0.4.8
+Version: 0.4.9
 Summary: Ethereum implementation of the chainlib interface
 Home-page: https://git.defalslfy.org/chainlib-eth,git
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chainlib-eth-0.4.8/WAIVER` & `chainlib-eth-0.4.9/WAIVER`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/WAIVER.asc` & `chainlib-eth-0.4.9/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/address.py` & `chainlib-eth-0.4.9/chainlib/eth/address.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/block.py` & `chainlib-eth-0.4.9/chainlib/eth/block.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/cli/config.py` & `chainlib-eth-0.4.9/chainlib/eth/cli/config.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/cli/decode.py` & `chainlib-eth-0.4.9/chainlib/eth/cli/decode.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/cli/encode.py` & `chainlib-eth-0.4.9/chainlib/eth/cli/encode.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/cli/rpc.py` & `chainlib-eth-0.4.9/chainlib/eth/cli/rpc.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/cli/wallet.py` & `chainlib-eth-0.4.9/chainlib/eth/cli/wallet.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/connection.py` & `chainlib-eth-0.4.9/chainlib/eth/connection.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/contract.py` & `chainlib-eth-0.4.9/chainlib/eth/contract.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/dialect/__init__.py` & `chainlib-eth-0.4.9/chainlib/eth/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/error.py` & `chainlib-eth-0.4.9/chainlib/eth/error.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/gas.py` & `chainlib-eth-0.4.9/chainlib/eth/gas.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/jsonrpc.py` & `chainlib-eth-0.4.9/chainlib/eth/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/log.py` & `chainlib-eth-0.4.9/chainlib/eth/log.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/nonce.py` & `chainlib-eth-0.4.9/chainlib/eth/nonce.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/pytest/fixtures_ethtester.py` & `chainlib-eth-0.4.9/chainlib/eth/pytest/fixtures_ethtester.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/runnable/balance.py` & `chainlib-eth-0.4.9/chainlib/eth/runnable/balance.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/runnable/block.py` & `chainlib-eth-0.4.9/chainlib/eth/runnable/block.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/runnable/checksum.py` & `chainlib-eth-0.4.9/chainlib/eth/runnable/checksum.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/runnable/count.py` & `chainlib-eth-0.4.9/chainlib/eth/runnable/count.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/runnable/decode.py` & `chainlib-eth-0.4.9/chainlib/eth/runnable/decode.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/runnable/encode.py` & `chainlib-eth-0.4.9/chainlib/eth/runnable/encode.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/runnable/flags.py` & `chainlib-eth-0.4.9/chainlib/eth/runnable/flags.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/runnable/gas.py` & `chainlib-eth-0.4.9/chainlib/eth/runnable/gas.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                         )
                 logg.debug('recipient {} balance before: {}'.format(settings.get('RECIPIENT'), recipient_balance))
         except urllib.error.URLError:
             pass
      
     (tx_hash_hex, o) = g.create(
             settings.get('SENDER_ADDRESS'),
-            settings.get('RECIPIENT'),
+            recipient,
             settings.get('VALUE'),
             data=settings.get('DATA'),
             id_generator=settings.get('RPC_ID_GENERATOR'),
         )
     
     logg.info('gas transfer from {} to {} value {} hash {}'.format(settings.get('SENDER_ADDRESS'), settings.get('RECIPIENT'), settings.get('VALUE'), tx_hash_hex))
```

### Comparing `chainlib-eth-0.4.8/chainlib/eth/runnable/get.py` & `chainlib-eth-0.4.9/chainlib/eth/runnable/get.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/runnable/info.py` & `chainlib-eth-0.4.9/chainlib/eth/runnable/info.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/runnable/raw.py` & `chainlib-eth-0.4.9/chainlib/eth/runnable/raw.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/runnable/wait.py` & `chainlib-eth-0.4.9/chainlib/eth/runnable/wait.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/settings.py` & `chainlib-eth-0.4.9/chainlib/eth/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 def process_settings_rpc(settings, config):
     rpc = chainlib.eth.cli.Rpc(settings.get('WALLET'))
     conn = rpc.connect_by_config(config, nonce_confirmed=True)
 
     settings.set('CONN', conn)
     settings.set('RPC_ID_GENERATOR', rpc.id_generator)
     settings.set('RPC_SEND', config.true('_RPC_SEND'))
+    settings.set('WAIT', config.true('_WAIT'))
 
     gas_oracle = rpc.get_gas_oracle()
     settings.set('GAS_ORACLE', gas_oracle)
     settings.set('FEE_ORACLE', gas_oracle)
 
     try:
         settings.set('SIGNER', rpc.get_signer())
```

### Comparing `chainlib-eth-0.4.8/chainlib/eth/sign.py` & `chainlib-eth-0.4.9/chainlib/eth/sign.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/src.py` & `chainlib-eth-0.4.9/chainlib/eth/src.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/tx.py` & `chainlib-eth-0.4.9/chainlib/eth/tx.py`

 * *Files 1% similar despite different names*

```diff
@@ -633,17 +633,17 @@
         self.gas_price = self.fee_price
         self.gas_limit = self.fee_limit
 
         address_from = self.normal(self.src['from'], SrcItem.ADDRESS)
         self.outputs = [to_checksum(address_from)]
 
         to = self.src['to']
-        if to == None:
-            to = ZERO_ADDRESS
-        self.inputs = [to_checksum(strip_0x(to))]
+        if to != None:
+            to = to_checksum(strip_0x(to))
+        self.inputs = [to]
 
         self.payload = self.normal(self.src['input'], SrcItem.PAYLOAD)
 
         try:
             self.set_wire(self.src['raw'])
         except KeyError:
             logg.debug('no inline raw tx self.src, and no raw rendering implemented, field will be "None"')
```

### Comparing `chainlib-eth-0.4.8/chainlib/eth/unittest/base.py` & `chainlib-eth-0.4.9/chainlib/eth/unittest/base.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib/eth/unittest/ethtester.py` & `chainlib-eth-0.4.9/chainlib/eth/unittest/ethtester.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib_eth.egg-info/PKG-INFO` & `chainlib-eth-0.4.9/chainlib_eth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlib-eth
-Version: 0.4.8
+Version: 0.4.9
 Summary: Ethereum implementation of the chainlib interface
 Home-page: https://git.defalslfy.org/chainlib-eth,git
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chainlib-eth-0.4.8/chainlib_eth.egg-info/SOURCES.txt` & `chainlib-eth-0.4.9/chainlib_eth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/chainlib_eth.egg-info/entry_points.txt` & `chainlib-eth-0.4.9/chainlib_eth.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.8/setup.cfg` & `chainlib-eth-0.4.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chainlib-eth
-version = 0.4.8
+version = 0.4.9
 description = Ethereum implementation of the chainlib interface
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalslfy.org/chainlib-eth,git
 keywords = 
 	dlt
 	blockchain
```

