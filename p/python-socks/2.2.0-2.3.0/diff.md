# Comparing `tmp/python-socks-2.2.0.tar.gz` & `tmp/python-socks-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-socks-2.2.0.tar", last modified: Mon Mar 13 05:54:58 2023, max compression
+gzip compressed data, was "dist/python-socks-2.3.0.tar", last modified: Mon May  8 07:13:38 2023, max compression
```

## Comparing `python-socks-2.2.0.tar` & `python-socks-2.3.0.tar`

### file list

```diff
@@ -1,110 +1,99 @@
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-03-13 05:54:58.565167 python-socks-2.2.0/
--rw-rw-r--   0 roman     (1000) roman     (1000)    11357 2021-02-13 05:38:25.000000 python-socks-2.2.0/LICENSE.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)       47 2021-02-11 14:16:51.000000 python-socks-2.2.0/MANIFEST.in
--rw-rw-r--   0 roman     (1000) roman     (1000)     6823 2023-03-13 05:54:58.565167 python-socks-2.2.0/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)     6339 2022-01-24 08:58:22.000000 python-socks-2.2.0/README.md
--rw-rw-r--   0 roman     (1000) roman     (1000)      186 2022-08-16 12:48:20.000000 python-socks-2.2.0/pyproject.toml
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-03-13 05:54:58.557167 python-socks-2.2.0/python_socks/
--rw-rw-r--   0 roman     (1000) roman     (1000)      367 2021-11-19 06:07:45.000000 python-socks-2.2.0/python_socks/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     1422 2022-12-18 05:12:18.000000 python-socks-2.2.0/python_socks/_abc.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     2130 2021-02-12 13:35:18.000000 python-socks-2.2.0/python_socks/_basic_auth.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      245 2021-02-12 08:27:58.000000 python-socks-2.2.0/python_socks/_errors.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     2544 2021-02-12 13:57:18.000000 python-socks-2.2.0/python_socks/_helpers.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-03-13 05:54:58.557167 python-socks-2.2.0/python_socks/_proto/
--rw-rw-r--   0 roman     (1000) roman     (1000)        0 2021-11-18 09:34:08.000000 python-socks-2.2.0/python_socks/_proto/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     1798 2021-11-21 07:21:29.000000 python-socks-2.2.0/python_socks/_proto/http.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      790 2021-11-21 09:25:12.000000 python-socks-2.2.0/python_socks/_proto/http_async.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      770 2021-11-21 09:25:12.000000 python-socks-2.2.0/python_socks/_proto/http_sync.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     2800 2021-11-21 07:22:14.000000 python-socks-2.2.0/python_socks/_proto/socks4.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     1151 2021-11-21 09:25:12.000000 python-socks-2.2.0/python_socks/_proto/socks4_async.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     1076 2021-11-21 09:25:12.000000 python-socks-2.2.0/python_socks/_proto/socks4_sync.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     6083 2021-11-21 07:22:14.000000 python-socks-2.2.0/python_socks/_proto/socks5.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     3090 2022-12-19 12:01:55.000000 python-socks-2.2.0/python_socks/_proto/socks5_async.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     2867 2022-12-19 12:02:27.000000 python-socks-2.2.0/python_socks/_proto/socks5_sync.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     1606 2021-11-22 07:07:19.000000 python-socks-2.2.0/python_socks/_proxy_factory.py
--rw-rw-r--   0 roman     (1000) roman     (1000)       90 2021-02-11 16:36:03.000000 python-socks-2.2.0/python_socks/_types.py
--rw-rw-r--   0 roman     (1000) roman     (1000)       49 2023-03-13 05:47:10.000000 python-socks-2.2.0/python_socks/_version.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-03-13 05:54:58.557167 python-socks-2.2.0/python_socks/async_/
--rw-rw-r--   0 roman     (1000) roman     (1000)       64 2021-11-21 07:24:05.000000 python-socks-2.2.0/python_socks/async_/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      824 2021-11-18 12:31:19.000000 python-socks-2.2.0/python_socks/async_/_proxy_chain.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-03-13 05:54:58.557167 python-socks-2.2.0/python_socks/async_/anyio/
--rw-rw-r--   0 roman     (1000) roman     (1000)       94 2021-11-21 09:47:19.000000 python-socks-2.2.0/python_socks/async_/anyio/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      895 2021-11-21 09:31:23.000000 python-socks-2.2.0/python_socks/async_/anyio/_chain.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      268 2021-11-23 10:17:21.000000 python-socks-2.2.0/python_socks/async_/anyio/_connect.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      317 2021-11-21 09:46:37.000000 python-socks-2.2.0/python_socks/async_/anyio/_factory.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     5339 2022-01-22 10:04:25.000000 python-socks-2.2.0/python_socks/async_/anyio/_proxy.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      590 2021-11-21 07:38:41.000000 python-socks-2.2.0/python_socks/async_/anyio/_resolver.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     1614 2021-11-22 12:15:15.000000 python-socks-2.2.0/python_socks/async_/anyio/_stream.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-03-13 05:54:58.561167 python-socks-2.2.0/python_socks/async_/anyio/v2/
--rw-rw-r--   0 roman     (1000) roman     (1000)      105 2023-03-12 12:58:53.000000 python-socks-2.2.0/python_socks/async_/anyio/v2/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      593 2023-03-12 12:57:05.000000 python-socks-2.2.0/python_socks/async_/anyio/v2/_chain.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      330 2023-03-12 12:07:22.000000 python-socks-2.2.0/python_socks/async_/anyio/v2/_connect.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      319 2023-03-12 12:56:26.000000 python-socks-2.2.0/python_socks/async_/anyio/v2/_factory.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     5383 2023-03-13 05:19:42.000000 python-socks-2.2.0/python_socks/async_/anyio/v2/_proxy.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     1616 2023-03-12 12:04:01.000000 python-socks-2.2.0/python_socks/async_/anyio/v2/_stream.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-03-13 05:54:58.561167 python-socks-2.2.0/python_socks/async_/asyncio/
--rw-rw-r--   0 roman     (1000) roman     (1000)      364 2021-11-21 07:25:25.000000 python-socks-2.2.0/python_socks/async_/asyncio/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     1014 2021-11-23 05:44:44.000000 python-socks-2.2.0/python_socks/async_/asyncio/_connect.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     5814 2021-11-21 13:25:47.000000 python-socks-2.2.0/python_socks/async_/asyncio/_proxy.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      681 2023-02-19 09:49:39.000000 python-socks-2.2.0/python_socks/async_/asyncio/_resolver.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     1021 2021-11-21 10:32:32.000000 python-socks-2.2.0/python_socks/async_/asyncio/_stream.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-03-13 05:54:58.561167 python-socks-2.2.0/python_socks/async_/asyncio/v2/
--rw-rw-r--   0 roman     (1000) roman     (1000)       94 2021-02-12 05:07:30.000000 python-socks-2.2.0/python_socks/async_/asyncio/v2/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      607 2023-02-18 08:09:38.000000 python-socks-2.2.0/python_socks/async_/asyncio/v2/_chain.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      587 2023-02-19 09:55:52.000000 python-socks-2.2.0/python_socks/async_/asyncio/v2/_connect.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      323 2021-02-12 08:34:01.000000 python-socks-2.2.0/python_socks/async_/asyncio/v2/_factory.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     6178 2023-03-13 05:36:17.000000 python-socks-2.2.0/python_socks/async_/asyncio/v2/_proxy.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     3465 2023-02-19 09:49:39.000000 python-socks-2.2.0/python_socks/async_/asyncio/v2/_stream.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-03-13 05:54:58.561167 python-socks-2.2.0/python_socks/async_/curio/
--rw-rw-r--   0 roman     (1000) roman     (1000)      360 2021-11-21 07:27:09.000000 python-socks-2.2.0/python_socks/async_/curio/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      328 2021-11-23 11:48:25.000000 python-socks-2.2.0/python_socks/async_/curio/_connect.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     4074 2021-11-21 13:27:47.000000 python-socks-2.2.0/python_socks/async_/curio/_proxy.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      722 2021-11-19 10:56:26.000000 python-socks-2.2.0/python_socks/async_/curio/_resolver.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      855 2021-11-20 12:52:57.000000 python-socks-2.2.0/python_socks/async_/curio/_stream.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-03-13 05:54:58.561167 python-socks-2.2.0/python_socks/async_/trio/
--rw-rw-r--   0 roman     (1000) roman     (1000)      358 2021-11-21 07:28:06.000000 python-socks-2.2.0/python_socks/async_/trio/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      783 2021-11-20 12:04:18.000000 python-socks-2.2.0/python_socks/async_/trio/_connect.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     4051 2021-11-21 13:28:46.000000 python-socks-2.2.0/python_socks/async_/trio/_proxy.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      591 2021-11-19 10:58:54.000000 python-socks-2.2.0/python_socks/async_/trio/_resolver.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     1003 2021-11-20 11:53:30.000000 python-socks-2.2.0/python_socks/async_/trio/_stream.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-03-13 05:54:58.561167 python-socks-2.2.0/python_socks/async_/trio/v2/
--rw-rw-r--   0 roman     (1000) roman     (1000)      106 2021-11-22 05:50:43.000000 python-socks-2.2.0/python_socks/async_/trio/v2/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      591 2023-02-19 10:52:16.000000 python-socks-2.2.0/python_socks/async_/trio/v2/_chain.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      379 2023-02-19 10:21:09.000000 python-socks-2.2.0/python_socks/async_/trio/v2/_connect.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      317 2021-11-21 13:18:10.000000 python-socks-2.2.0/python_socks/async_/trio/v2/_factory.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     5392 2023-03-13 05:26:26.000000 python-socks-2.2.0/python_socks/async_/trio/v2/_proxy.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     1475 2021-11-25 10:24:20.000000 python-socks-2.2.0/python_socks/async_/trio/v2/_stream.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-03-13 05:54:58.561167 python-socks-2.2.0/python_socks/sync/
--rw-rw-r--   0 roman     (1000) roman     (1000)      381 2021-11-22 10:12:27.000000 python-socks-2.2.0/python_socks/sync/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      804 2021-11-21 07:30:32.000000 python-socks-2.2.0/python_socks/sync/_chain.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      334 2021-11-21 10:31:50.000000 python-socks-2.2.0/python_socks/sync/_connect.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     3863 2021-11-21 13:24:51.000000 python-socks-2.2.0/python_socks/sync/_proxy.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      547 2021-11-19 14:35:15.000000 python-socks-2.2.0/python_socks/sync/_resolver.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      818 2021-11-20 10:28:46.000000 python-socks-2.2.0/python_socks/sync/_stream.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-03-13 05:54:58.565167 python-socks-2.2.0/python_socks/sync/v2/
--rw-rw-r--   0 roman     (1000) roman     (1000)      106 2021-11-22 10:19:17.000000 python-socks-2.2.0/python_socks/sync/v2/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      869 2021-11-22 11:47:46.000000 python-socks-2.2.0/python_socks/sync/v2/_chain.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      315 2021-11-22 07:01:15.000000 python-socks-2.2.0/python_socks/sync/v2/_factory.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     5107 2021-11-22 11:40:42.000000 python-socks-2.2.0/python_socks/sync/v2/_proxy.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     6088 2021-11-22 06:27:21.000000 python-socks-2.2.0/python_socks/sync/v2/_ssl_transport.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     1544 2021-11-25 10:17:35.000000 python-socks-2.2.0/python_socks/sync/v2/_stream.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-03-13 05:54:58.557167 python-socks-2.2.0/python_socks.egg-info/
--rw-rw-r--   0 roman     (1000) roman     (1000)     6823 2023-03-13 05:54:58.000000 python-socks-2.2.0/python_socks.egg-info/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)     3093 2023-03-13 05:54:58.000000 python-socks-2.2.0/python_socks.egg-info/SOURCES.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)        1 2023-03-13 05:54:58.000000 python-socks-2.2.0/python_socks.egg-info/dependency_links.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)       95 2023-03-13 05:54:58.000000 python-socks-2.2.0/python_socks.egg-info/requires.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)       13 2023-03-13 05:54:58.000000 python-socks-2.2.0/python_socks.egg-info/top_level.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)       38 2023-03-13 05:54:58.565167 python-socks-2.2.0/setup.cfg
--rw-rw-r--   0 roman     (1000) roman     (1000)     1722 2023-03-13 05:44:57.000000 python-socks-2.2.0/setup.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-03-13 05:54:58.565167 python-socks-2.2.0/tests/
--rw-rw-r--   0 roman     (1000) roman     (1000)      554 2021-02-12 08:48:08.000000 python-socks-2.2.0/tests/test_misc.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     6034 2022-10-02 09:34:31.000000 python-socks-2.2.0/tests/test_proxy_async_aio.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     6698 2022-12-19 11:58:50.000000 python-socks-2.2.0/tests/test_proxy_async_aio_v2.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     6674 2022-10-02 09:34:31.000000 python-socks-2.2.0/tests/test_proxy_async_anyio.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     6683 2023-03-13 05:33:27.000000 python-socks-2.2.0/tests/test_proxy_async_anyio_v2.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     7211 2022-10-02 09:34:31.000000 python-socks-2.2.0/tests/test_proxy_async_curio.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     6086 2022-10-02 09:34:31.000000 python-socks-2.2.0/tests/test_proxy_async_trio.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     6680 2022-10-02 09:34:31.000000 python-socks-2.2.0/tests/test_proxy_async_trio_v2.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     6098 2022-10-02 09:34:31.000000 python-socks-2.2.0/tests/test_proxy_sync.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     6706 2022-10-02 09:34:31.000000 python-socks-2.2.0/tests/test_proxy_sync_v2.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     2834 2021-11-21 10:21:06.000000 python-socks-2.2.0/tests/test_resolvers.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-08 07:13:38.000000 python-socks-2.3.0/
+-rw-rw-r--   0 roman     (1000) roman     (1000)    11357 2021-02-13 05:38:25.000000 python-socks-2.3.0/LICENSE.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)       47 2021-02-11 14:16:51.000000 python-socks-2.3.0/MANIFEST.in
+-rw-rw-r--   0 roman     (1000) roman     (1000)     6843 2023-05-08 07:13:38.000000 python-socks-2.3.0/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)     6339 2022-01-24 08:58:22.000000 python-socks-2.3.0/README.md
+-rw-rw-r--   0 roman     (1000) roman     (1000)      186 2022-08-16 12:48:20.000000 python-socks-2.3.0/pyproject.toml
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-08 07:13:38.000000 python-socks-2.3.0/python_socks/
+-rw-rw-r--   0 roman     (1000) roman     (1000)      367 2021-11-19 06:07:45.000000 python-socks-2.3.0/python_socks/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1422 2022-12-18 05:12:18.000000 python-socks-2.3.0/python_socks/_abc.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     2130 2021-02-12 13:35:18.000000 python-socks-2.3.0/python_socks/_basic_auth.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      245 2021-02-12 08:27:58.000000 python-socks-2.3.0/python_socks/_errors.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     2544 2021-02-12 13:57:18.000000 python-socks-2.3.0/python_socks/_helpers.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-08 07:13:38.000000 python-socks-2.3.0/python_socks/_proto/
+-rw-rw-r--   0 roman     (1000) roman     (1000)        0 2021-11-18 09:34:08.000000 python-socks-2.3.0/python_socks/_proto/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1798 2021-11-21 07:21:29.000000 python-socks-2.3.0/python_socks/_proto/http.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      790 2021-11-21 09:25:12.000000 python-socks-2.3.0/python_socks/_proto/http_async.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      770 2021-11-21 09:25:12.000000 python-socks-2.3.0/python_socks/_proto/http_sync.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     2800 2021-11-21 07:22:14.000000 python-socks-2.3.0/python_socks/_proto/socks4.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1151 2021-11-21 09:25:12.000000 python-socks-2.3.0/python_socks/_proto/socks4_async.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1076 2021-11-21 09:25:12.000000 python-socks-2.3.0/python_socks/_proto/socks4_sync.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     6083 2021-11-21 07:22:14.000000 python-socks-2.3.0/python_socks/_proto/socks5.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     3090 2022-12-19 12:01:55.000000 python-socks-2.3.0/python_socks/_proto/socks5_async.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     2867 2022-12-19 12:02:27.000000 python-socks-2.3.0/python_socks/_proto/socks5_sync.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1606 2021-11-22 07:07:19.000000 python-socks-2.3.0/python_socks/_proxy_factory.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)       90 2021-02-11 16:36:03.000000 python-socks-2.3.0/python_socks/_types.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)       49 2023-05-08 05:34:20.000000 python-socks-2.3.0/python_socks/_version.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-08 07:13:38.000000 python-socks-2.3.0/python_socks/async_/
+-rw-rw-r--   0 roman     (1000) roman     (1000)       64 2021-11-21 07:24:05.000000 python-socks-2.3.0/python_socks/async_/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      824 2021-11-18 12:31:19.000000 python-socks-2.3.0/python_socks/async_/_proxy_chain.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-08 07:13:38.000000 python-socks-2.3.0/python_socks/async_/anyio/
+-rw-rw-r--   0 roman     (1000) roman     (1000)       94 2021-11-21 09:47:19.000000 python-socks-2.3.0/python_socks/async_/anyio/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      895 2021-11-21 09:31:23.000000 python-socks-2.3.0/python_socks/async_/anyio/_chain.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      268 2021-11-23 10:17:21.000000 python-socks-2.3.0/python_socks/async_/anyio/_connect.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      317 2021-11-21 09:46:37.000000 python-socks-2.3.0/python_socks/async_/anyio/_factory.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     5339 2022-01-22 10:04:25.000000 python-socks-2.3.0/python_socks/async_/anyio/_proxy.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      590 2021-11-21 07:38:41.000000 python-socks-2.3.0/python_socks/async_/anyio/_resolver.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1614 2021-11-22 12:15:15.000000 python-socks-2.3.0/python_socks/async_/anyio/_stream.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-08 07:13:38.000000 python-socks-2.3.0/python_socks/async_/anyio/v2/
+-rw-rw-r--   0 roman     (1000) roman     (1000)      106 2023-05-08 05:17:06.000000 python-socks-2.3.0/python_socks/async_/anyio/v2/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      593 2023-03-12 12:57:05.000000 python-socks-2.3.0/python_socks/async_/anyio/v2/_chain.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      330 2023-03-12 12:07:22.000000 python-socks-2.3.0/python_socks/async_/anyio/v2/_connect.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      319 2023-03-12 12:56:26.000000 python-socks-2.3.0/python_socks/async_/anyio/v2/_factory.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     5584 2023-05-08 06:27:59.000000 python-socks-2.3.0/python_socks/async_/anyio/v2/_proxy.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1616 2023-03-12 12:04:01.000000 python-socks-2.3.0/python_socks/async_/anyio/v2/_stream.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-08 07:13:38.000000 python-socks-2.3.0/python_socks/async_/asyncio/
+-rw-rw-r--   0 roman     (1000) roman     (1000)      364 2021-11-21 07:25:25.000000 python-socks-2.3.0/python_socks/async_/asyncio/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1014 2021-11-23 05:44:44.000000 python-socks-2.3.0/python_socks/async_/asyncio/_connect.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     5814 2021-11-21 13:25:47.000000 python-socks-2.3.0/python_socks/async_/asyncio/_proxy.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      681 2023-02-19 09:49:39.000000 python-socks-2.3.0/python_socks/async_/asyncio/_resolver.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1021 2021-11-21 10:32:32.000000 python-socks-2.3.0/python_socks/async_/asyncio/_stream.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-08 07:13:38.000000 python-socks-2.3.0/python_socks/async_/asyncio/v2/
+-rw-rw-r--   0 roman     (1000) roman     (1000)       94 2021-02-12 05:07:30.000000 python-socks-2.3.0/python_socks/async_/asyncio/v2/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      607 2023-02-18 08:09:38.000000 python-socks-2.3.0/python_socks/async_/asyncio/v2/_chain.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      587 2023-02-19 09:55:52.000000 python-socks-2.3.0/python_socks/async_/asyncio/v2/_connect.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      323 2021-02-12 08:34:01.000000 python-socks-2.3.0/python_socks/async_/asyncio/v2/_factory.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     6385 2023-05-08 06:29:25.000000 python-socks-2.3.0/python_socks/async_/asyncio/v2/_proxy.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     3465 2023-02-19 09:49:39.000000 python-socks-2.3.0/python_socks/async_/asyncio/v2/_stream.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-08 07:13:38.000000 python-socks-2.3.0/python_socks/async_/curio/
+-rw-rw-r--   0 roman     (1000) roman     (1000)      360 2021-11-21 07:27:09.000000 python-socks-2.3.0/python_socks/async_/curio/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      328 2021-11-23 11:48:25.000000 python-socks-2.3.0/python_socks/async_/curio/_connect.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     4074 2021-11-21 13:27:47.000000 python-socks-2.3.0/python_socks/async_/curio/_proxy.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      722 2021-11-19 10:56:26.000000 python-socks-2.3.0/python_socks/async_/curio/_resolver.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      855 2021-11-20 12:52:57.000000 python-socks-2.3.0/python_socks/async_/curio/_stream.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-08 07:13:38.000000 python-socks-2.3.0/python_socks/async_/trio/
+-rw-rw-r--   0 roman     (1000) roman     (1000)      358 2021-11-21 07:28:06.000000 python-socks-2.3.0/python_socks/async_/trio/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      783 2021-11-20 12:04:18.000000 python-socks-2.3.0/python_socks/async_/trio/_connect.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     4051 2021-11-21 13:28:46.000000 python-socks-2.3.0/python_socks/async_/trio/_proxy.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      591 2021-11-19 10:58:54.000000 python-socks-2.3.0/python_socks/async_/trio/_resolver.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1003 2021-11-20 11:53:30.000000 python-socks-2.3.0/python_socks/async_/trio/_stream.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-08 07:13:38.000000 python-socks-2.3.0/python_socks/async_/trio/v2/
+-rw-rw-r--   0 roman     (1000) roman     (1000)      106 2021-11-22 05:50:43.000000 python-socks-2.3.0/python_socks/async_/trio/v2/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      591 2023-02-19 10:52:16.000000 python-socks-2.3.0/python_socks/async_/trio/v2/_chain.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      379 2023-02-19 10:21:09.000000 python-socks-2.3.0/python_socks/async_/trio/v2/_connect.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      317 2021-11-21 13:18:10.000000 python-socks-2.3.0/python_socks/async_/trio/v2/_factory.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     5590 2023-05-08 06:32:18.000000 python-socks-2.3.0/python_socks/async_/trio/v2/_proxy.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1475 2021-11-25 10:24:20.000000 python-socks-2.3.0/python_socks/async_/trio/v2/_stream.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-08 07:13:38.000000 python-socks-2.3.0/python_socks/sync/
+-rw-rw-r--   0 roman     (1000) roman     (1000)      381 2021-11-22 10:12:27.000000 python-socks-2.3.0/python_socks/sync/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      804 2021-11-21 07:30:32.000000 python-socks-2.3.0/python_socks/sync/_chain.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      334 2021-11-21 10:31:50.000000 python-socks-2.3.0/python_socks/sync/_connect.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     3863 2021-11-21 13:24:51.000000 python-socks-2.3.0/python_socks/sync/_proxy.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      547 2021-11-19 14:35:15.000000 python-socks-2.3.0/python_socks/sync/_resolver.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      818 2021-11-20 10:28:46.000000 python-socks-2.3.0/python_socks/sync/_stream.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-08 07:13:38.000000 python-socks-2.3.0/python_socks/sync/v2/
+-rw-rw-r--   0 roman     (1000) roman     (1000)      106 2021-11-22 10:19:17.000000 python-socks-2.3.0/python_socks/sync/v2/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      579 2023-05-08 05:02:10.000000 python-socks-2.3.0/python_socks/sync/v2/_chain.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      410 2023-05-08 04:38:42.000000 python-socks-2.3.0/python_socks/sync/v2/_connect.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      315 2021-11-22 07:01:15.000000 python-socks-2.3.0/python_socks/sync/v2/_factory.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     5234 2023-05-08 05:47:42.000000 python-socks-2.3.0/python_socks/sync/v2/_proxy.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     6088 2021-11-22 06:27:21.000000 python-socks-2.3.0/python_socks/sync/v2/_ssl_transport.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1544 2021-11-25 10:17:35.000000 python-socks-2.3.0/python_socks/sync/v2/_stream.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-08 07:13:38.000000 python-socks-2.3.0/python_socks.egg-info/
+-rw-rw-r--   0 roman     (1000) roman     (1000)     6843 2023-05-08 07:13:38.000000 python-socks-2.3.0/python_socks.egg-info/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)     2803 2023-05-08 07:13:38.000000 python-socks-2.3.0/python_socks.egg-info/SOURCES.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)        1 2023-05-08 07:13:38.000000 python-socks-2.3.0/python_socks.egg-info/dependency_links.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)       95 2023-05-08 07:13:38.000000 python-socks-2.3.0/python_socks.egg-info/requires.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)       13 2023-05-08 07:13:38.000000 python-socks-2.3.0/python_socks.egg-info/top_level.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)       38 2023-05-08 07:13:38.000000 python-socks-2.3.0/setup.cfg
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1722 2023-03-13 05:44:57.000000 python-socks-2.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `python-socks-2.2.0/LICENSE.txt` & `python-socks-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/PKG-INFO` & `python-socks-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: python-socks
-Version: 2.2.0
+Version: 2.3.0
 Summary: Core proxy (SOCKS4, SOCKS5, HTTP tunneling) functionality for Python
 Home-page: https://github.com/romis2012/python-socks
 Author: Roman Snegirev
 Author-email: snegiryev@gmail.com
 License: Apache 2
 Keywords: socks socks5 socks4 http proxy asyncio trio curio anyio
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: asyncio
 Provides-Extra: trio
 Provides-Extra: curio
 Provides-Extra: anyio
 License-File: LICENSE.txt
 
@@ -263,7 +264,9 @@
 
 
 ### and how to use it
 manager = ProxyPoolManager('socks5://user:password@127.0.0.1:1080')
 response = manager.request('GET', 'https://check-host.net/ip')
 print(response.data)
 ```
+
+
```

### Comparing `python-socks-2.2.0/README.md` & `python-socks-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/_abc.py` & `python-socks-2.3.0/python_socks/_abc.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/_basic_auth.py` & `python-socks-2.3.0/python_socks/_basic_auth.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/_helpers.py` & `python-socks-2.3.0/python_socks/_helpers.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/_proto/http.py` & `python-socks-2.3.0/python_socks/_proto/http.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/_proto/http_async.py` & `python-socks-2.3.0/python_socks/_proto/http_async.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/_proto/http_sync.py` & `python-socks-2.3.0/python_socks/_proto/http_sync.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/_proto/socks4.py` & `python-socks-2.3.0/python_socks/_proto/socks4.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/_proto/socks4_async.py` & `python-socks-2.3.0/python_socks/_proto/socks4_async.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/_proto/socks4_sync.py` & `python-socks-2.3.0/python_socks/_proto/socks4_sync.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/_proto/socks5.py` & `python-socks-2.3.0/python_socks/_proto/socks5.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/_proto/socks5_async.py` & `python-socks-2.3.0/python_socks/_proto/socks5_async.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/_proto/socks5_sync.py` & `python-socks-2.3.0/python_socks/_proto/socks5_sync.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/_proxy_factory.py` & `python-socks-2.3.0/python_socks/_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/_proxy_chain.py` & `python-socks-2.3.0/python_socks/async_/_proxy_chain.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/anyio/_chain.py` & `python-socks-2.3.0/python_socks/async_/anyio/_chain.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/anyio/_proxy.py` & `python-socks-2.3.0/python_socks/async_/anyio/_proxy.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/anyio/_resolver.py` & `python-socks-2.3.0/python_socks/async_/anyio/_resolver.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/anyio/_stream.py` & `python-socks-2.3.0/python_socks/async_/anyio/_stream.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/anyio/v2/_chain.py` & `python-socks-2.3.0/python_socks/async_/anyio/v2/_chain.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/anyio/v2/_proxy.py` & `python-socks-2.3.0/python_socks/async_/trio/v2/_proxy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 import ssl
 
-import anyio
+import trio
 
 from ._connect import connect_tcp
-from ._stream import AnyioSocketStream
+from ._stream import TrioSocketStream
 from .._resolver import Resolver
 from ...._errors import ProxyConnectionError, ProxyTimeoutError
 from ...._proto.http_async import HttpProto
 from ...._proto.socks4_async import Socks4Proto
 from ...._proto.socks5_async import Socks5Proto
 
 DEFAULT_TIMEOUT = 60
 
 
-class AnyioProxy:
+class TrioProxy:
     def __init__(
         self,
         proxy_host: str,
         proxy_port: int,
         proxy_ssl: ssl.SSLContext = None,
-        forward: 'AnyioProxy' = None,
+        forward: 'TrioProxy' = None,
     ):
         self._proxy_host = proxy_host
         self._proxy_port = proxy_port
         self._proxy_ssl = proxy_ssl
         self._forward = forward
 
         self._resolver = Resolver()
 
     async def connect(
         self,
         dest_host: str,
         dest_port: int,
         dest_ssl: ssl.SSLContext = None,
         timeout: float = None,
-    ) -> AnyioSocketStream:
+    ) -> TrioSocketStream:
         if timeout is None:
             timeout = DEFAULT_TIMEOUT
 
         try:
-            with anyio.fail_after(timeout):
+            with trio.fail_after(timeout):
                 return await self._connect(
                     dest_host=dest_host,
                     dest_port=dest_port,
                     dest_ssl=dest_ssl,
                 )
-        except TimeoutError as e:
+        except trio.TooSlowError as e:
             raise ProxyTimeoutError('Proxy connection timed out: {}'.format(timeout)) from e
 
     async def _connect(
         self,
         dest_host: str,
         dest_port: int,
         dest_ssl: ssl.SSLContext = None,
-    ) -> AnyioSocketStream:
+    ) -> TrioSocketStream:
         try:
             if self._forward is None:
                 stream = await connect_tcp(
                     host=self._proxy_host,
                     port=self._proxy_port,
                 )
             else:
@@ -85,52 +85,54 @@
             )
 
             if dest_ssl is not None:
                 stream = await stream.start_tls(
                     hostname=dest_host,
                     ssl_context=dest_ssl,
                 )
-        except BaseException:
-            with anyio.CancelScope(shield=True):
+        except BaseException:  # trio.Cancelled...
+            with trio.CancelScope(shield=True):
                 await stream.close()
             raise
 
         return stream
 
     async def _negotiate(
         self,
-        stream: AnyioSocketStream,
+        stream: TrioSocketStream,
         dest_host: str,
         dest_port: int,
     ):
-        raise NotImplementedError()
+        raise NotImplementedError
 
 
-class Socks5Proxy(AnyioProxy):
+class Socks5Proxy(TrioProxy):
     def __init__(
         self,
         proxy_host,
         proxy_port,
         username=None,
         password=None,
         rdns=None,
         proxy_ssl=None,
+        forward: 'TrioProxy' = None,
     ):
         super().__init__(
             proxy_host=proxy_host,
             proxy_port=proxy_port,
             proxy_ssl=proxy_ssl,
+            forward=forward,
         )
         self._username = username
         self._password = password
         self._rdns = rdns
 
     async def _negotiate(
         self,
-        stream: AnyioSocketStream,
+        stream: TrioSocketStream,
         dest_host: str,
         dest_port: int,
     ):
         proto = Socks5Proto(
             stream=stream,
             resolver=self._resolver,
             dest_host=dest_host,
@@ -138,68 +140,72 @@
             username=self._username,
             password=self._password,
             rdns=self._rdns,
         )
         await proto.negotiate()
 
 
-class Socks4Proxy(AnyioProxy):
+class Socks4Proxy(TrioProxy):
     def __init__(
         self,
         proxy_host,
         proxy_port,
         user_id=None,
         rdns=None,
         proxy_ssl=None,
+        forward: 'TrioProxy' = None,
     ):
         super().__init__(
             proxy_host=proxy_host,
             proxy_port=proxy_port,
             proxy_ssl=proxy_ssl,
+            forward=forward,
         )
         self._user_id = user_id
         self._rdns = rdns
 
     async def _negotiate(
         self,
-        stream: AnyioSocketStream,
+        stream: TrioSocketStream,
         dest_host: str,
         dest_port: int,
     ):
         proto = Socks4Proto(
             stream=stream,
             resolver=self._resolver,
             dest_host=dest_host,
             dest_port=dest_port,
             user_id=self._user_id,
             rdns=self._rdns,
         )
         await proto.negotiate()
 
 
-class HttpProxy(AnyioProxy):
+class HttpProxy(TrioProxy):
     def __init__(
         self,
         proxy_host,
         proxy_port,
         username=None,
         password=None,
         proxy_ssl=None,
+        forward: 'TrioProxy' = None,
     ):
         super().__init__(
             proxy_host=proxy_host,
             proxy_port=proxy_port,
             proxy_ssl=proxy_ssl,
+            forward=forward,
         )
         self._username = username
         self._password = password
 
     async def _negotiate(
         self,
-        stream: AnyioSocketStream,
+        stream: TrioSocketStream,
         dest_host: str,
         dest_port: int,
     ):
         proto = HttpProto(
             stream=stream,
             dest_host=dest_host,
             dest_port=dest_port,
```

### Comparing `python-socks-2.2.0/python_socks/async_/anyio/v2/_stream.py` & `python-socks-2.3.0/python_socks/async_/anyio/v2/_stream.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/asyncio/_connect.py` & `python-socks-2.3.0/python_socks/async_/asyncio/_connect.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/asyncio/_proxy.py` & `python-socks-2.3.0/python_socks/async_/asyncio/_proxy.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/asyncio/_resolver.py` & `python-socks-2.3.0/python_socks/async_/asyncio/_resolver.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/asyncio/_stream.py` & `python-socks-2.3.0/python_socks/async_/asyncio/_stream.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/asyncio/v2/_chain.py` & `python-socks-2.3.0/python_socks/async_/asyncio/v2/_chain.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/asyncio/v2/_connect.py` & `python-socks-2.3.0/python_socks/async_/asyncio/v2/_connect.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/asyncio/v2/_proxy.py` & `python-socks-2.3.0/python_socks/async_/asyncio/v2/_proxy.py`

 * *Files 8% similar despite different names*

```diff
@@ -128,20 +128,22 @@
         self,
         proxy_host,
         proxy_port,
         username=None,
         password=None,
         rdns=None,
         proxy_ssl=None,
+        forward: 'AsyncioProxy' = None,
         loop: asyncio.AbstractEventLoop = None,
     ):
         super().__init__(
             proxy_host=proxy_host,
             proxy_port=proxy_port,
             proxy_ssl=proxy_ssl,
+            forward=forward,
             loop=loop,
         )
         self._username = username
         self._password = password
         self._rdns = rdns
 
     async def _negotiate(
@@ -166,20 +168,22 @@
     def __init__(
         self,
         proxy_host,
         proxy_port,
         user_id=None,
         rdns=None,
         proxy_ssl=None,
+        forward: 'AsyncioProxy' = None,
         loop: asyncio.AbstractEventLoop = None,
     ):
         super().__init__(
             proxy_host=proxy_host,
             proxy_port=proxy_port,
             proxy_ssl=proxy_ssl,
+            forward=forward,
             loop=loop,
         )
         self._user_id = user_id
         self._rdns = rdns
 
     async def _negotiate(
         self,
@@ -202,20 +206,22 @@
     def __init__(
         self,
         proxy_host,
         proxy_port,
         username=None,
         password=None,
         proxy_ssl=None,
+        forward: 'AsyncioProxy' = None,
         loop: asyncio.AbstractEventLoop = None,
     ):
         super().__init__(
             proxy_host=proxy_host,
             proxy_port=proxy_port,
             proxy_ssl=proxy_ssl,
+            forward=forward,
             loop=loop,
         )
         self._username = username
         self._password = password
 
     async def _negotiate(
         self,
```

### Comparing `python-socks-2.2.0/python_socks/async_/asyncio/v2/_stream.py` & `python-socks-2.3.0/python_socks/async_/asyncio/v2/_stream.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/curio/_proxy.py` & `python-socks-2.3.0/python_socks/async_/curio/_proxy.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/curio/_resolver.py` & `python-socks-2.3.0/python_socks/async_/curio/_resolver.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/curio/_stream.py` & `python-socks-2.3.0/python_socks/async_/curio/_stream.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/trio/_connect.py` & `python-socks-2.3.0/python_socks/async_/trio/_connect.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/trio/_proxy.py` & `python-socks-2.3.0/python_socks/async_/trio/_proxy.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/trio/_resolver.py` & `python-socks-2.3.0/python_socks/async_/trio/_resolver.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/trio/_stream.py` & `python-socks-2.3.0/python_socks/async_/trio/_stream.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/trio/v2/_chain.py` & `python-socks-2.3.0/python_socks/async_/trio/v2/_chain.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/async_/trio/v2/_proxy.py` & `python-socks-2.3.0/python_socks/sync/v2/_proxy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,209 +1,206 @@
+import socket
 import ssl
 
-import trio
-
 from ._connect import connect_tcp
-from ._stream import TrioSocketStream
-from .._resolver import Resolver
-from ...._errors import ProxyConnectionError, ProxyTimeoutError
-from ...._proto.http_async import HttpProto
-from ...._proto.socks4_async import Socks4Proto
-from ...._proto.socks5_async import Socks5Proto
+from ._stream import SyncSocketStream
+from .._resolver import SyncResolver
+from ... import _abc as abc
+from ..._errors import ProxyConnectionError, ProxyTimeoutError
+from ..._proto.http_sync import HttpProto
+from ..._proto.socks4_sync import Socks4Proto
+from ..._proto.socks5_sync import Socks5Proto
 
 DEFAULT_TIMEOUT = 60
 
 
-class TrioProxy:
+class SyncProxy(abc.SyncProxy):
     def __init__(
         self,
         proxy_host: str,
         proxy_port: int,
         proxy_ssl: ssl.SSLContext = None,
-        forward: 'TrioProxy' = None,
+        forward: 'SyncProxy' = None,
     ):
         self._proxy_host = proxy_host
         self._proxy_port = proxy_port
         self._proxy_ssl = proxy_ssl
         self._forward = forward
 
-        self._resolver = Resolver()
+        self._resolver = SyncResolver()
 
-    async def connect(
+    def connect(
         self,
         dest_host: str,
         dest_port: int,
         dest_ssl: ssl.SSLContext = None,
         timeout: float = None,
-    ) -> TrioSocketStream:
+    ) -> SyncSocketStream:
         if timeout is None:
             timeout = DEFAULT_TIMEOUT
 
         try:
-            with trio.fail_after(timeout):
-                return await self._connect(
-                    dest_host=dest_host,
-                    dest_port=dest_port,
-                    dest_ssl=dest_ssl,
-                )
-        except trio.TooSlowError as e:
-            raise ProxyTimeoutError('Proxy connection timed out: {}'.format(timeout)) from e
-
-    async def _connect(
-        self,
-        dest_host: str,
-        dest_port: int,
-        dest_ssl: ssl.SSLContext = None,
-    ) -> TrioSocketStream:
-        try:
             if self._forward is None:
-                stream = await connect_tcp(
+                stream = connect_tcp(
                     host=self._proxy_host,
                     port=self._proxy_port,
+                    timeout=timeout,
                 )
             else:
-                stream = await self._forward.connect(
+                stream = self._forward.connect(
                     dest_host=self._proxy_host,
                     dest_port=self._proxy_port,
+                    timeout=timeout,
                 )
         except OSError as e:
-            raise ProxyConnectionError(
-                e.errno,
-                f"Couldn't connect to proxy {self._proxy_host}:{self._proxy_port} [{e.strerror}]",
-            ) from e
+            msg = 'Could not connect to proxy {}:{} [{}]'.format(
+                self._proxy_host,
+                self._proxy_port,
+                e.strerror,
+            )
+            raise ProxyConnectionError(e.errno, msg) from e
 
         try:
             if self._proxy_ssl is not None:
-                stream = await stream.start_tls(
+                stream = stream.start_tls(
                     hostname=self._proxy_host,
                     ssl_context=self._proxy_ssl,
                 )
 
-            await self._negotiate(
+            self._negotiate(
                 stream=stream,
                 dest_host=dest_host,
                 dest_port=dest_port,
             )
 
             if dest_ssl is not None:
-                stream = await stream.start_tls(
+                stream = stream.start_tls(
                     hostname=dest_host,
                     ssl_context=dest_ssl,
                 )
-        except BaseException:  # trio.Cancelled...
-            with trio.CancelScope(shield=True):
-                await stream.close()
-            raise
 
-        return stream
+            return stream
+
+        except socket.timeout as e:
+            stream.close()
+            raise ProxyTimeoutError('Proxy connection timed out: {}'.format(timeout)) from e
+        except Exception:
+            stream.close()
+            raise
 
-    async def _negotiate(
+    def _negotiate(
         self,
-        stream: TrioSocketStream,
+        stream: SyncSocketStream,
         dest_host: str,
         dest_port: int,
     ):
         raise NotImplementedError
 
 
-class Socks5Proxy(TrioProxy):
+class Socks5Proxy(SyncProxy):
     def __init__(
         self,
         proxy_host,
         proxy_port,
         username=None,
         password=None,
         rdns=None,
         proxy_ssl=None,
+        forward: 'SyncProxy' = None,
     ):
         super().__init__(
             proxy_host=proxy_host,
             proxy_port=proxy_port,
             proxy_ssl=proxy_ssl,
+            forward=forward,
         )
         self._username = username
         self._password = password
         self._rdns = rdns
 
-    async def _negotiate(
+    def _negotiate(
         self,
-        stream: TrioSocketStream,
+        stream: SyncSocketStream,
         dest_host: str,
         dest_port: int,
     ):
         proto = Socks5Proto(
             stream=stream,
             resolver=self._resolver,
             dest_host=dest_host,
             dest_port=dest_port,
             username=self._username,
             password=self._password,
             rdns=self._rdns,
         )
-        await proto.negotiate()
+        proto.negotiate()
 
 
-class Socks4Proxy(TrioProxy):
+class Socks4Proxy(SyncProxy):
     def __init__(
         self,
         proxy_host,
         proxy_port,
         user_id=None,
         rdns=None,
         proxy_ssl=None,
+        forward: 'SyncProxy' = None,
     ):
         super().__init__(
             proxy_host=proxy_host,
             proxy_port=proxy_port,
             proxy_ssl=proxy_ssl,
+            forward=forward,
         )
         self._user_id = user_id
         self._rdns = rdns
 
-    async def _negotiate(
+    def _negotiate(
         self,
-        stream: TrioSocketStream,
+        stream: SyncSocketStream,
         dest_host: str,
         dest_port: int,
     ):
         proto = Socks4Proto(
             stream=stream,
             resolver=self._resolver,
             dest_host=dest_host,
             dest_port=dest_port,
             user_id=self._user_id,
             rdns=self._rdns,
         )
-        await proto.negotiate()
+        proto.negotiate()
 
 
-class HttpProxy(TrioProxy):
+class HttpProxy(SyncProxy):
     def __init__(
         self,
         proxy_host,
         proxy_port,
         username=None,
         password=None,
         proxy_ssl=None,
+        forward: 'SyncProxy' = None,
     ):
         super().__init__(
             proxy_host=proxy_host,
             proxy_port=proxy_port,
             proxy_ssl=proxy_ssl,
+            forward=forward,
         )
         self._username = username
         self._password = password
 
-    async def _negotiate(
+    def _negotiate(
         self,
-        stream: TrioSocketStream,
+        stream: SyncSocketStream,
         dest_host: str,
         dest_port: int,
     ):
         proto = HttpProto(
             stream=stream,
             dest_host=dest_host,
             dest_port=dest_port,
             username=self._username,
             password=self._password,
         )
-        await proto.negotiate()
+        proto.negotiate()
```

### Comparing `python-socks-2.2.0/python_socks/async_/trio/v2/_stream.py` & `python-socks-2.3.0/python_socks/async_/trio/v2/_stream.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/sync/_chain.py` & `python-socks-2.3.0/python_socks/sync/_chain.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/sync/_proxy.py` & `python-socks-2.3.0/python_socks/sync/_proxy.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/sync/_resolver.py` & `python-socks-2.3.0/python_socks/sync/_resolver.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/sync/_stream.py` & `python-socks-2.3.0/python_socks/sync/_stream.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/sync/v2/_proxy.py` & `python-socks-2.3.0/python_socks/async_/anyio/v2/_proxy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,199 +1,215 @@
-import socket
 import ssl
-from typing import Optional
 
-from ._stream import SyncSocketStream
-from .._connect import connect_tcp
-from .._resolver import SyncResolver
-from ... import _abc as abc
-from ..._errors import ProxyConnectionError, ProxyTimeoutError
-from ..._proto.http_sync import HttpProto
-from ..._proto.socks4_sync import Socks4Proto
-from ..._proto.socks5_sync import Socks5Proto
+import anyio
 
-DEFAULT_TIMEOUT = 60
+from ._connect import connect_tcp
+from ._stream import AnyioSocketStream
+from .._resolver import Resolver
+from ...._errors import ProxyConnectionError, ProxyTimeoutError
+from ...._proto.http_async import HttpProto
+from ...._proto.socks4_async import Socks4Proto
+from ...._proto.socks5_async import Socks5Proto
 
+DEFAULT_TIMEOUT = 60
 
-class SyncProxy(abc.SyncProxy):
-    _stream: Optional[SyncSocketStream]
 
+class AnyioProxy:
     def __init__(
         self,
         proxy_host: str,
         proxy_port: int,
         proxy_ssl: ssl.SSLContext = None,
+        forward: 'AnyioProxy' = None,
     ):
         self._proxy_host = proxy_host
         self._proxy_port = proxy_port
         self._proxy_ssl = proxy_ssl
+        self._forward = forward
 
-        self._dest_host = None
-        self._dest_port = None
-        self._dest_ssl = None
-        self._timeout = None
-
-        self._stream = None
-        self._resolver = SyncResolver()
+        self._resolver = Resolver()
 
-    def connect(
+    async def connect(
         self,
         dest_host: str,
         dest_port: int,
         dest_ssl: ssl.SSLContext = None,
         timeout: float = None,
-        _stream: SyncSocketStream = None,
-    ) -> SyncSocketStream:
-
+    ) -> AnyioSocketStream:
         if timeout is None:
             timeout = DEFAULT_TIMEOUT
 
-        self._dest_host = dest_host
-        self._dest_port = dest_port
-        self._dest_ssl = dest_ssl
-        self._timeout = timeout
+        try:
+            with anyio.fail_after(timeout):
+                return await self._connect(
+                    dest_host=dest_host,
+                    dest_port=dest_port,
+                    dest_ssl=dest_ssl,
+                )
+        except TimeoutError as e:
+            raise ProxyTimeoutError('Proxy connection timed out: {}'.format(timeout)) from e
 
+    async def _connect(
+        self,
+        dest_host: str,
+        dest_port: int,
+        dest_ssl: ssl.SSLContext = None,
+    ) -> AnyioSocketStream:
         try:
-            if _stream is None:
-                sock = connect_tcp(
+            if self._forward is None:
+                stream = await connect_tcp(
                     host=self._proxy_host,
                     port=self._proxy_port,
-                    timeout=timeout,
                 )
-                self._stream = SyncSocketStream(sock)
             else:
-                self._stream = _stream
+                stream = await self._forward.connect(
+                    dest_host=self._proxy_host,
+                    dest_port=self._proxy_port,
+                )
+        except OSError as e:
+            raise ProxyConnectionError(
+                e.errno,
+                f"Couldn't connect to proxy {self._proxy_host}:{self._proxy_port} [{e.strerror}]",
+            ) from e
 
+        try:
             if self._proxy_ssl is not None:
-                self._stream = self._stream.start_tls(
+                stream = await stream.start_tls(
                     hostname=self._proxy_host,
                     ssl_context=self._proxy_ssl,
                 )
 
-            self._negotiate()
+            await self._negotiate(
+                stream=stream,
+                dest_host=dest_host,
+                dest_port=dest_port,
+            )
 
-            if self._dest_ssl is not None:
-                self._stream = self._stream.start_tls(
-                    hostname=self._dest_host,
-                    ssl_context=self._dest_ssl,
+            if dest_ssl is not None:
+                stream = await stream.start_tls(
+                    hostname=dest_host,
+                    ssl_context=dest_ssl,
                 )
-
-            return self._stream
-
-        except socket.timeout as e:
-            self._close()
-            raise ProxyTimeoutError('Proxy connection timed out: {}'.format(self._timeout)) from e
-        except OSError as e:
-            self._close()
-            msg = 'Could not connect to proxy {}:{} [{}]'.format(
-                self._proxy_host,
-                self._proxy_port,
-                e.strerror,
-            )
-            raise ProxyConnectionError(e.errno, msg) from e
-        except Exception:
-            self._close()
+        except BaseException:
+            with anyio.CancelScope(shield=True):
+                await stream.close()
             raise
 
-    def _negotiate(self):
-        raise NotImplementedError
+        return stream
 
-    def _close(self):
-        if self._stream is not None:
-            self._stream.close()
-
-    @property
-    def proxy_host(self):
-        return self._proxy_host
-
-    @property
-    def proxy_port(self):
-        return self._proxy_port
+    async def _negotiate(
+        self,
+        stream: AnyioSocketStream,
+        dest_host: str,
+        dest_port: int,
+    ):
+        raise NotImplementedError()
 
 
-class Socks5Proxy(SyncProxy):
+class Socks5Proxy(AnyioProxy):
     def __init__(
         self,
         proxy_host,
         proxy_port,
         username=None,
         password=None,
         rdns=None,
         proxy_ssl=None,
+        forward: 'AnyioProxy' = None,
     ):
         super().__init__(
             proxy_host=proxy_host,
             proxy_port=proxy_port,
             proxy_ssl=proxy_ssl,
+            forward=forward,
         )
         self._username = username
         self._password = password
         self._rdns = rdns
 
-    def _negotiate(self):
+    async def _negotiate(
+        self,
+        stream: AnyioSocketStream,
+        dest_host: str,
+        dest_port: int,
+    ):
         proto = Socks5Proto(
-            stream=self._stream,
+            stream=stream,
             resolver=self._resolver,
-            dest_host=self._dest_host,
-            dest_port=self._dest_port,
+            dest_host=dest_host,
+            dest_port=dest_port,
             username=self._username,
             password=self._password,
             rdns=self._rdns,
         )
-        proto.negotiate()
+        await proto.negotiate()
 
 
-class Socks4Proxy(SyncProxy):
+class Socks4Proxy(AnyioProxy):
     def __init__(
         self,
         proxy_host,
         proxy_port,
         user_id=None,
         rdns=None,
         proxy_ssl=None,
+        forward: 'AnyioProxy' = None,
     ):
         super().__init__(
             proxy_host=proxy_host,
             proxy_port=proxy_port,
             proxy_ssl=proxy_ssl,
+            forward=forward,
         )
         self._user_id = user_id
         self._rdns = rdns
 
-    def _negotiate(self):
+    async def _negotiate(
+        self,
+        stream: AnyioSocketStream,
+        dest_host: str,
+        dest_port: int,
+    ):
         proto = Socks4Proto(
-            stream=self._stream,
+            stream=stream,
             resolver=self._resolver,
-            dest_host=self._dest_host,
-            dest_port=self._dest_port,
+            dest_host=dest_host,
+            dest_port=dest_port,
             user_id=self._user_id,
             rdns=self._rdns,
         )
-        proto.negotiate()
+        await proto.negotiate()
 
 
-class HttpProxy(SyncProxy):
+class HttpProxy(AnyioProxy):
     def __init__(
         self,
         proxy_host,
         proxy_port,
         username=None,
         password=None,
         proxy_ssl=None,
+        forward: 'AnyioProxy' = None,
     ):
         super().__init__(
             proxy_host=proxy_host,
             proxy_port=proxy_port,
             proxy_ssl=proxy_ssl,
+            forward=forward,
         )
         self._username = username
         self._password = password
 
-    def _negotiate(self):
+    async def _negotiate(
+        self,
+        stream: AnyioSocketStream,
+        dest_host: str,
+        dest_port: int,
+    ):
         proto = HttpProto(
-            stream=self._stream,
-            dest_host=self._dest_host,
-            dest_port=self._dest_port,
+            stream=stream,
+            dest_host=dest_host,
+            dest_port=dest_port,
             username=self._username,
             password=self._password,
         )
-        proto.negotiate()
+        await proto.negotiate()
```

### Comparing `python-socks-2.2.0/python_socks/sync/v2/_ssl_transport.py` & `python-socks-2.3.0/python_socks/sync/v2/_ssl_transport.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks/sync/v2/_stream.py` & `python-socks-2.3.0/python_socks/sync/v2/_stream.py`

 * *Files identical despite different names*

### Comparing `python-socks-2.2.0/python_socks.egg-info/PKG-INFO` & `python-socks-2.3.0/python_socks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: python-socks
-Version: 2.2.0
+Version: 2.3.0
 Summary: Core proxy (SOCKS4, SOCKS5, HTTP tunneling) functionality for Python
 Home-page: https://github.com/romis2012/python-socks
 Author: Roman Snegirev
 Author-email: snegiryev@gmail.com
 License: Apache 2
 Keywords: socks socks5 socks4 http proxy asyncio trio curio anyio
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: asyncio
 Provides-Extra: trio
 Provides-Extra: curio
 Provides-Extra: anyio
 License-File: LICENSE.txt
 
@@ -263,7 +264,9 @@
 
 
 ### and how to use it
 manager = ProxyPoolManager('socks5://user:password@127.0.0.1:1080')
 response = manager.request('GET', 'https://check-host.net/ip')
 print(response.data)
 ```
+
+
```

### Comparing `python-socks-2.2.0/python_socks.egg-info/SOURCES.txt` & `python-socks-2.3.0/python_socks.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -72,22 +72,12 @@
 python_socks/sync/_chain.py
 python_socks/sync/_connect.py
 python_socks/sync/_proxy.py
 python_socks/sync/_resolver.py
 python_socks/sync/_stream.py
 python_socks/sync/v2/__init__.py
 python_socks/sync/v2/_chain.py
+python_socks/sync/v2/_connect.py
 python_socks/sync/v2/_factory.py
 python_socks/sync/v2/_proxy.py
 python_socks/sync/v2/_ssl_transport.py
-python_socks/sync/v2/_stream.py
-tests/test_misc.py
-tests/test_proxy_async_aio.py
-tests/test_proxy_async_aio_v2.py
-tests/test_proxy_async_anyio.py
-tests/test_proxy_async_anyio_v2.py
-tests/test_proxy_async_curio.py
-tests/test_proxy_async_trio.py
-tests/test_proxy_async_trio_v2.py
-tests/test_proxy_sync.py
-tests/test_proxy_sync_v2.py
-tests/test_resolvers.py
+python_socks/sync/v2/_stream.py
```

### Comparing `python-socks-2.2.0/setup.py` & `python-socks-2.3.0/setup.py`

 * *Files identical despite different names*

