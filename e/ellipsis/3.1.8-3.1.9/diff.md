# Comparing `tmp/ellipsis-3.1.8.tar.gz` & `tmp/ellipsis-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellipsis-3.1.8.tar", last modified: Thu Mar 30 14:33:46 2023, max compression
+gzip compressed data, was "ellipsis-3.1.9.tar", last modified: Tue Apr  4 08:54:26 2023, max compression
```

## Comparing `ellipsis-3.1.8.tar` & `ellipsis-3.1.9.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.849508 ellipsis-3.1.8/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1074 2022-05-04 22:59:11.000000 ellipsis-3.1.8/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1411 2023-03-30 14:33:46.849508 ellipsis-3.1.8/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      939 2022-10-11 19:13:20.000000 ellipsis-3.1.8/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      232 2023-03-30 14:33:35.000000 ellipsis-3.1.8/ellipsis/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis/account/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       92 2022-10-11 19:15:57.000000 ellipsis-3.1.8/ellipsis/account/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis/account/accessToken/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       66 2022-10-10 16:42:59.000000 ellipsis-3.1.8/ellipsis/account/accessToken/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1281 2022-10-10 16:42:59.000000 ellipsis-3.1.8/ellipsis/account/accessToken/root.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1285 2022-12-08 15:07:24.000000 ellipsis-3.1.8/ellipsis/account/root.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3819 2023-03-30 13:37:14.000000 ellipsis-3.1.8/ellipsis/apiManager.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis/path/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      398 2023-02-24 15:21:36.000000 ellipsis-3.1.8/ellipsis/path/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis/path/file/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      107 2023-03-30 13:50:13.000000 ellipsis-3.1.8/ellipsis/path/file/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4417 2023-03-30 13:24:34.000000 ellipsis-3.1.8/ellipsis/path/file/root.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis/path/folder/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       91 2022-12-08 14:51:05.000000 ellipsis-3.1.8/ellipsis/path/folder/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1481 2022-12-08 18:18:49.000000 ellipsis-3.1.8/ellipsis/path/folder/root.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis/path/hashtag/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       59 2022-05-27 15:08:51.000000 ellipsis-3.1.8/ellipsis/path/hashtag/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      806 2022-05-27 15:08:51.000000 ellipsis-3.1.8/ellipsis/path/hashtag/root.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis/path/invite/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      100 2022-05-31 12:30:29.000000 ellipsis-3.1.8/ellipsis/path/invite/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1931 2022-08-31 11:10:32.000000 ellipsis-3.1.8/ellipsis/path/invite/root.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis/path/member/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       56 2022-05-27 15:08:51.000000 ellipsis-3.1.8/ellipsis/path/member/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1071 2022-05-27 15:08:51.000000 ellipsis-3.1.8/ellipsis/path/member/root.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis/path/raster/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      217 2022-12-09 22:48:00.000000 ellipsis-3.1.8/ellipsis/path/raster/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1749 2023-03-17 13:40:50.000000 ellipsis-3.1.8/ellipsis/path/raster/root.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis/path/raster/style/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       61 2022-10-10 16:42:59.000000 ellipsis-3.1.8/ellipsis/path/raster/style/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1547 2022-10-10 16:42:59.000000 ellipsis-3.1.8/ellipsis/path/raster/style/root.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis/path/raster/timestamp/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      859 2023-01-25 17:36:22.000000 ellipsis-3.1.8/ellipsis/path/raster/timestamp/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis/path/raster/timestamp/file/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       97 2023-01-25 17:16:56.000000 ellipsis-3.1.8/ellipsis/path/raster/timestamp/file/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3891 2023-03-06 10:45:44.000000 ellipsis-3.1.8/ellipsis/path/raster/timestamp/file/root.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis/path/raster/timestamp/order/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       74 2022-10-13 10:20:00.000000 ellipsis-3.1.8/ellipsis/path/raster/timestamp/order/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1176 2023-01-25 17:37:00.000000 ellipsis-3.1.8/ellipsis/path/raster/timestamp/order/root.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    12671 2022-12-13 10:39:26.000000 ellipsis-3.1.8/ellipsis/path/raster/timestamp/root.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     7609 2023-02-24 15:36:26.000000 ellipsis-3.1.8/ellipsis/path/root.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis/path/usage/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       82 2022-10-10 16:42:59.000000 ellipsis-3.1.8/ellipsis/path/usage/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1215 2022-10-10 16:42:59.000000 ellipsis-3.1.8/ellipsis/path/usage/root.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis/path/vector/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      228 2022-12-08 14:53:28.000000 ellipsis-3.1.8/ellipsis/path/vector/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis/path/vector/featureProperty/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       81 2022-10-10 16:42:59.000000 ellipsis-3.1.8/ellipsis/path/vector/featureProperty/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2128 2022-10-10 16:42:59.000000 ellipsis-3.1.8/ellipsis/path/vector/featureProperty/root.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      984 2022-12-08 14:53:07.000000 ellipsis-3.1.8/ellipsis/path/vector/root.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis/path/vector/style/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       63 2022-10-10 16:42:59.000000 ellipsis-3.1.8/ellipsis/path/vector/style/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1641 2022-10-10 16:42:59.000000 ellipsis-3.1.8/ellipsis/path/vector/style/root.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis/path/vector/timestamp/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      330 2023-01-25 17:36:38.000000 ellipsis-3.1.8/ellipsis/path/vector/timestamp/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis/path/vector/timestamp/feature/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      210 2022-10-10 16:42:59.000000 ellipsis-3.1.8/ellipsis/path/vector/timestamp/feature/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.849508 ellipsis-3.1.8/ellipsis/path/vector/timestamp/feature/message/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      100 2022-10-10 16:42:59.000000 ellipsis-3.1.8/ellipsis/path/vector/timestamp/feature/message/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3949 2022-10-11 18:30:07.000000 ellipsis-3.1.8/ellipsis/path/vector/timestamp/feature/message/root.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    13019 2023-03-01 22:29:55.000000 ellipsis-3.1.8/ellipsis/path/vector/timestamp/feature/root.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.849508 ellipsis-3.1.8/ellipsis/path/vector/timestamp/feature/series/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      107 2022-10-10 16:42:59.000000 ellipsis-3.1.8/ellipsis/path/vector/timestamp/feature/series/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     6861 2022-10-10 16:42:59.000000 ellipsis-3.1.8/ellipsis/path/vector/timestamp/feature/series/root.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.849508 ellipsis-3.1.8/ellipsis/path/vector/timestamp/file/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       73 2023-01-25 17:20:17.000000 ellipsis-3.1.8/ellipsis/path/vector/timestamp/file/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3057 2023-01-26 13:40:03.000000 ellipsis-3.1.8/ellipsis/path/vector/timestamp/file/root.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.849508 ellipsis-3.1.8/ellipsis/path/vector/timestamp/order/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       74 2022-10-13 10:20:28.000000 ellipsis-3.1.8/ellipsis/path/vector/timestamp/order/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1179 2023-01-25 17:23:52.000000 ellipsis-3.1.8/ellipsis/path/vector/timestamp/order/root.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     8620 2023-03-14 12:24:05.000000 ellipsis-3.1.8/ellipsis/path/vector/timestamp/root.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     9982 2023-03-30 12:10:00.000000 ellipsis-3.1.8/ellipsis/sanitize.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.849508 ellipsis-3.1.8/ellipsis/user/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       43 2022-05-27 15:08:51.000000 ellipsis-3.1.8/ellipsis/user/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      484 2022-05-27 15:08:51.000000 ellipsis-3.1.8/ellipsis/user/root.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.849508 ellipsis-3.1.8/ellipsis/util/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      628 2022-11-21 14:55:57.000000 ellipsis-3.1.8/ellipsis/util/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    19434 2023-03-06 10:46:09.000000 ellipsis-3.1.8/ellipsis/util/root.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.849508 ellipsis-3.1.8/ellipsis/view/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       67 2022-12-12 22:18:53.000000 ellipsis-3.1.8/ellipsis/view/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1726 2022-12-12 22:16:04.000000 ellipsis-3.1.8/ellipsis/view/root.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.845507 ellipsis-3.1.8/ellipsis.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1411 2023-03-30 14:33:46.000000 ellipsis-3.1.8/ellipsis.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2181 2023-03-30 14:33:46.000000 ellipsis-3.1.8/ellipsis.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-03-30 14:33:46.000000 ellipsis-3.1.8/ellipsis.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      127 2023-03-30 14:33:46.000000 ellipsis-3.1.8/ellipsis.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        9 2023-03-30 14:33:46.000000 ellipsis-3.1.8/ellipsis.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-03-30 14:33:46.849508 ellipsis-3.1.8/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      975 2023-03-30 14:33:26.000000 ellipsis-3.1.8/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-30 14:33:46.849508 ellipsis-3.1.8/test/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    15379 2023-03-30 13:52:35.000000 ellipsis-3.1.8/test/test.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.209630 ellipsis-3.1.9/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1074 2022-05-04 22:59:11.000000 ellipsis-3.1.9/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1411 2023-04-04 08:54:26.209630 ellipsis-3.1.9/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      939 2022-10-11 19:13:20.000000 ellipsis-3.1.9/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.201629 ellipsis-3.1.9/ellipsis/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      232 2023-04-04 08:53:33.000000 ellipsis-3.1.9/ellipsis/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.201629 ellipsis-3.1.9/ellipsis/account/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       92 2022-10-11 19:15:57.000000 ellipsis-3.1.9/ellipsis/account/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.201629 ellipsis-3.1.9/ellipsis/account/accessToken/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       66 2022-10-10 16:42:59.000000 ellipsis-3.1.9/ellipsis/account/accessToken/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1281 2022-10-10 16:42:59.000000 ellipsis-3.1.9/ellipsis/account/accessToken/root.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1285 2022-12-08 15:07:24.000000 ellipsis-3.1.9/ellipsis/account/root.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3819 2023-03-30 13:37:14.000000 ellipsis-3.1.9/ellipsis/apiManager.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.201629 ellipsis-3.1.9/ellipsis/path/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      398 2023-02-24 15:21:36.000000 ellipsis-3.1.9/ellipsis/path/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.205629 ellipsis-3.1.9/ellipsis/path/file/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      107 2023-03-30 13:50:13.000000 ellipsis-3.1.9/ellipsis/path/file/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4417 2023-03-30 13:24:34.000000 ellipsis-3.1.9/ellipsis/path/file/root.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.205629 ellipsis-3.1.9/ellipsis/path/folder/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       91 2022-12-08 14:51:05.000000 ellipsis-3.1.9/ellipsis/path/folder/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1481 2022-12-08 18:18:49.000000 ellipsis-3.1.9/ellipsis/path/folder/root.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.205629 ellipsis-3.1.9/ellipsis/path/hashtag/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       59 2022-05-27 15:08:51.000000 ellipsis-3.1.9/ellipsis/path/hashtag/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      806 2022-05-27 15:08:51.000000 ellipsis-3.1.9/ellipsis/path/hashtag/root.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.205629 ellipsis-3.1.9/ellipsis/path/invite/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      100 2022-05-31 12:30:29.000000 ellipsis-3.1.9/ellipsis/path/invite/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1931 2022-08-31 11:10:32.000000 ellipsis-3.1.9/ellipsis/path/invite/root.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.205629 ellipsis-3.1.9/ellipsis/path/member/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       56 2022-05-27 15:08:51.000000 ellipsis-3.1.9/ellipsis/path/member/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1071 2022-05-27 15:08:51.000000 ellipsis-3.1.9/ellipsis/path/member/root.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.205629 ellipsis-3.1.9/ellipsis/path/raster/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      217 2022-12-09 22:48:00.000000 ellipsis-3.1.9/ellipsis/path/raster/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1749 2023-03-17 13:40:50.000000 ellipsis-3.1.9/ellipsis/path/raster/root.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.205629 ellipsis-3.1.9/ellipsis/path/raster/style/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       61 2022-10-10 16:42:59.000000 ellipsis-3.1.9/ellipsis/path/raster/style/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1547 2022-10-10 16:42:59.000000 ellipsis-3.1.9/ellipsis/path/raster/style/root.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.205629 ellipsis-3.1.9/ellipsis/path/raster/timestamp/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      859 2023-01-25 17:36:22.000000 ellipsis-3.1.9/ellipsis/path/raster/timestamp/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.205629 ellipsis-3.1.9/ellipsis/path/raster/timestamp/file/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       97 2023-01-25 17:16:56.000000 ellipsis-3.1.9/ellipsis/path/raster/timestamp/file/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3891 2023-03-06 10:45:44.000000 ellipsis-3.1.9/ellipsis/path/raster/timestamp/file/root.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.205629 ellipsis-3.1.9/ellipsis/path/raster/timestamp/order/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       74 2022-10-13 10:20:00.000000 ellipsis-3.1.9/ellipsis/path/raster/timestamp/order/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1176 2023-01-25 17:37:00.000000 ellipsis-3.1.9/ellipsis/path/raster/timestamp/order/root.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    12671 2022-12-13 10:39:26.000000 ellipsis-3.1.9/ellipsis/path/raster/timestamp/root.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     7609 2023-02-24 15:36:26.000000 ellipsis-3.1.9/ellipsis/path/root.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.205629 ellipsis-3.1.9/ellipsis/path/usage/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       82 2022-10-10 16:42:59.000000 ellipsis-3.1.9/ellipsis/path/usage/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1215 2022-10-10 16:42:59.000000 ellipsis-3.1.9/ellipsis/path/usage/root.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.209630 ellipsis-3.1.9/ellipsis/path/vector/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      228 2022-12-08 14:53:28.000000 ellipsis-3.1.9/ellipsis/path/vector/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.209630 ellipsis-3.1.9/ellipsis/path/vector/featureProperty/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       81 2022-10-10 16:42:59.000000 ellipsis-3.1.9/ellipsis/path/vector/featureProperty/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2128 2022-10-10 16:42:59.000000 ellipsis-3.1.9/ellipsis/path/vector/featureProperty/root.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      984 2022-12-08 14:53:07.000000 ellipsis-3.1.9/ellipsis/path/vector/root.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.209630 ellipsis-3.1.9/ellipsis/path/vector/style/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       63 2022-10-10 16:42:59.000000 ellipsis-3.1.9/ellipsis/path/vector/style/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1641 2022-10-10 16:42:59.000000 ellipsis-3.1.9/ellipsis/path/vector/style/root.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.209630 ellipsis-3.1.9/ellipsis/path/vector/timestamp/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      330 2023-01-25 17:36:38.000000 ellipsis-3.1.9/ellipsis/path/vector/timestamp/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.209630 ellipsis-3.1.9/ellipsis/path/vector/timestamp/feature/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      210 2022-10-10 16:42:59.000000 ellipsis-3.1.9/ellipsis/path/vector/timestamp/feature/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.209630 ellipsis-3.1.9/ellipsis/path/vector/timestamp/feature/message/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      100 2022-10-10 16:42:59.000000 ellipsis-3.1.9/ellipsis/path/vector/timestamp/feature/message/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3949 2022-10-11 18:30:07.000000 ellipsis-3.1.9/ellipsis/path/vector/timestamp/feature/message/root.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    13019 2023-03-01 22:29:55.000000 ellipsis-3.1.9/ellipsis/path/vector/timestamp/feature/root.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.209630 ellipsis-3.1.9/ellipsis/path/vector/timestamp/feature/series/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      107 2022-10-10 16:42:59.000000 ellipsis-3.1.9/ellipsis/path/vector/timestamp/feature/series/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6861 2022-10-10 16:42:59.000000 ellipsis-3.1.9/ellipsis/path/vector/timestamp/feature/series/root.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.209630 ellipsis-3.1.9/ellipsis/path/vector/timestamp/file/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       73 2023-01-25 17:20:17.000000 ellipsis-3.1.9/ellipsis/path/vector/timestamp/file/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3057 2023-01-26 13:40:03.000000 ellipsis-3.1.9/ellipsis/path/vector/timestamp/file/root.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.209630 ellipsis-3.1.9/ellipsis/path/vector/timestamp/order/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       74 2022-10-13 10:20:28.000000 ellipsis-3.1.9/ellipsis/path/vector/timestamp/order/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1179 2023-01-25 17:23:52.000000 ellipsis-3.1.9/ellipsis/path/vector/timestamp/order/root.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     9389 2023-04-04 08:48:58.000000 ellipsis-3.1.9/ellipsis/path/vector/timestamp/root.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     9982 2023-03-30 12:10:00.000000 ellipsis-3.1.9/ellipsis/sanitize.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.209630 ellipsis-3.1.9/ellipsis/user/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       43 2022-05-27 15:08:51.000000 ellipsis-3.1.9/ellipsis/user/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      484 2022-05-27 15:08:51.000000 ellipsis-3.1.9/ellipsis/user/root.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.209630 ellipsis-3.1.9/ellipsis/util/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      628 2022-11-21 14:55:57.000000 ellipsis-3.1.9/ellipsis/util/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    19434 2023-03-06 10:46:09.000000 ellipsis-3.1.9/ellipsis/util/root.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.209630 ellipsis-3.1.9/ellipsis/view/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       67 2022-12-12 22:18:53.000000 ellipsis-3.1.9/ellipsis/view/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1726 2022-12-12 22:16:04.000000 ellipsis-3.1.9/ellipsis/view/root.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.201629 ellipsis-3.1.9/ellipsis.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1411 2023-04-04 08:54:26.000000 ellipsis-3.1.9/ellipsis.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2181 2023-04-04 08:54:26.000000 ellipsis-3.1.9/ellipsis.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-04-04 08:54:26.000000 ellipsis-3.1.9/ellipsis.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      127 2023-04-04 08:54:26.000000 ellipsis-3.1.9/ellipsis.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        9 2023-04-04 08:54:26.000000 ellipsis-3.1.9/ellipsis.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-04-04 08:54:26.209630 ellipsis-3.1.9/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      975 2023-04-04 08:54:12.000000 ellipsis-3.1.9/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-04 08:54:26.209630 ellipsis-3.1.9/test/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    15379 2023-04-04 08:53:18.000000 ellipsis-3.1.9/test/test.py
```

### Comparing `ellipsis-3.1.8/LICENSE` & `ellipsis-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/PKG-INFO` & `ellipsis-3.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellipsis
-Version: 3.1.8
+Version: 3.1.9
 Summary: Package to interact with the Ellipsis API
 Home-page: https://github.com/ellipsis-drive-internal/python-package
 Author: Daniel van der Maas
 Author-email: daniel@ellipsis-drive.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ellipsis-3.1.8/README.md` & `ellipsis-3.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/account/accessToken/root.py` & `ellipsis-3.1.9/ellipsis/account/accessToken/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/account/root.py` & `ellipsis-3.1.9/ellipsis/account/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/apiManager.py` & `ellipsis-3.1.9/ellipsis/apiManager.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/file/root.py` & `ellipsis-3.1.9/ellipsis/path/file/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/folder/root.py` & `ellipsis-3.1.9/ellipsis/path/folder/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/hashtag/root.py` & `ellipsis-3.1.9/ellipsis/path/hashtag/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/invite/root.py` & `ellipsis-3.1.9/ellipsis/path/invite/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/member/root.py` & `ellipsis-3.1.9/ellipsis/path/member/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/raster/root.py` & `ellipsis-3.1.9/ellipsis/path/raster/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/raster/style/root.py` & `ellipsis-3.1.9/ellipsis/path/raster/style/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/raster/timestamp/__init__.py` & `ellipsis-3.1.9/ellipsis/path/raster/timestamp/__init__.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/raster/timestamp/file/root.py` & `ellipsis-3.1.9/ellipsis/path/raster/timestamp/file/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/raster/timestamp/order/root.py` & `ellipsis-3.1.9/ellipsis/path/raster/timestamp/order/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/raster/timestamp/root.py` & `ellipsis-3.1.9/ellipsis/path/raster/timestamp/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/root.py` & `ellipsis-3.1.9/ellipsis/path/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/usage/root.py` & `ellipsis-3.1.9/ellipsis/path/usage/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/vector/featureProperty/root.py` & `ellipsis-3.1.9/ellipsis/path/vector/featureProperty/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/vector/root.py` & `ellipsis-3.1.9/ellipsis/path/vector/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/vector/style/root.py` & `ellipsis-3.1.9/ellipsis/path/vector/style/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/vector/timestamp/feature/message/root.py` & `ellipsis-3.1.9/ellipsis/path/vector/timestamp/feature/message/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/vector/timestamp/feature/root.py` & `ellipsis-3.1.9/ellipsis/path/vector/timestamp/feature/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/vector/timestamp/feature/series/root.py` & `ellipsis-3.1.9/ellipsis/path/vector/timestamp/feature/series/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/vector/timestamp/file/root.py` & `ellipsis-3.1.9/ellipsis/path/vector/timestamp/file/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/vector/timestamp/order/root.py` & `ellipsis-3.1.9/ellipsis/path/vector/timestamp/order/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/path/vector/timestamp/root.py` & `ellipsis-3.1.9/ellipsis/path/vector/timestamp/root.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from shapely import geometry
 import numpy as np
 
 from ellipsis.util import chunks
 from ellipsis.util import loadingBar
 from ellipsis.util.root import stringToDate
 from ellipsis.util.root import getActualExtent
-
+from ellipsis.path import get as getInfo
 
 import datetime
 
 def add(pathId,  token, properties = None, description = None, date ={'from': datetime.datetime.now(), 'to': datetime.datetime.now()}):
 
     pathId = sanitize.validUuid('pathId', pathId, True) 
     token = sanitize.validString('token', token, True)
@@ -135,34 +135,50 @@
 
         
     sh = gpd.GeoDataFrame.from_features(r['result'])    
     r['result'] = sh
     return r
     
 
-def getFeaturesByExtent(pathId, timestampId, extent, propertyFilter = None, token = None, listAll = True, pageStart = None, epsg = 4326):
+def getFeaturesByExtent(pathId, timestampId, extent, propertyFilter = None, token = None, listAll = True, pageStart = None, epsg = 4326, coordinateBuffer = None):
     pathId = sanitize.validUuid('pathId', pathId, True) 
     timestampId = sanitize.validUuid('timestampId', timestampId, True) 
     token = sanitize.validString('token', token, False)
     extent = sanitize.validBounds('extent', extent, True)
     propertyFilter = sanitize.validObject('propertyFilter', propertyFilter, False)
     listAll = sanitize.validBool('listAll', listAll, True)
     pageStart = sanitize.validObject('pageStart', pageStart, False) 
+    coordinateBuffer = sanitize.validFloat('coordinateBuffer', coordinateBuffer, False) 
+
+    if str(type(coordinateBuffer)) == str(type(None)):
+        info = getInfo(pathId, token)
+        ts = [x for x in info['vector']['timestamps'] if x['id'] == timestampId]
+        if len(ts) == 0:
+            raise ValueError('Given timestampId does not exist')
+        t = ts[0]
+        zoom = t['zoom']
+        coordinateBuffer = 0.5*360 / 2**zoom
+
 
     p = geometry.Polygon( [(extent['xMin'], extent['yMin']), (extent['xMin'], extent['yMax']),(extent['xMax'], extent['yMax']),(extent['xMax'], extent['yMin'])] )
     p = gpd.GeoDataFrame({'geometry':[p]})
 
 
     res = getActualExtent(extent['xMin'], extent['xMax'], extent['yMin'], extent['yMax'], 'EPSG:' + str(epsg))
     if res['status'] == '400':
         raise ValueError('Invalid epsg and extent combination')
         
     extent = res['message']
 
 
+    extent['xMin'] = min(-180, extent['xMin'] - coordinateBuffer)
+    extent['xMax'] = max(180, extent['xMax'] + coordinateBuffer)
+    extent['yMin'] = min(-85, extent['yMin'] - coordinateBuffer)
+    extent['yMax'] = max(85, extent['yMax'] + coordinateBuffer)
+
     try:
         p.crs = 'EPSG:' + str(epsg)
         p = p.to_crs('EPSG:4326')
     except:
         raise ValueError('Invalid crs given')
     extent = p.bounds
     extent = {'xMin': extent['minx'].values[0], 'xMax': extent['maxx'].values[0], 'yMin': extent['miny'].values[0], 'yMax': extent['maxy'].values[0] }
```

### Comparing `ellipsis-3.1.8/ellipsis/sanitize.py` & `ellipsis-3.1.9/ellipsis/sanitize.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/util/__init__.py` & `ellipsis-3.1.9/ellipsis/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/util/root.py` & `ellipsis-3.1.9/ellipsis/util/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis/view/root.py` & `ellipsis-3.1.9/ellipsis/view/root.py`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/ellipsis.egg-info/PKG-INFO` & `ellipsis-3.1.9/ellipsis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellipsis
-Version: 3.1.8
+Version: 3.1.9
 Summary: Package to interact with the Ellipsis API
 Home-page: https://github.com/ellipsis-drive-internal/python-package
 Author: Daniel van der Maas
 Author-email: daniel@ellipsis-drive.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ellipsis-3.1.8/ellipsis.egg-info/SOURCES.txt` & `ellipsis-3.1.9/ellipsis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ellipsis-3.1.8/setup.py` & `ellipsis-3.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ellipsis",
-    version="3.1.8",
+    version="3.1.9",
     author="Daniel van der Maas",
     author_email="daniel@ellipsis-drive.com",
     description="Package to interact with the Ellipsis API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ellipsis-drive-internal/python-package",
     classifiers=[
```

### Comparing `ellipsis-3.1.8/test/test.py` & `ellipsis-3.1.9/test/test.py`

 * *Files identical despite different names*

