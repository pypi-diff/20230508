# Comparing `tmp/spotON_sdk-0.0.1.6.tar.gz` & `tmp/spotON_sdk-0.0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.1.6.tar", last modified: Sun May  7 23:25:22 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.1.7.tar", last modified: Mon May  8 08:25:01 2023, max compression
```

## Comparing `spotON_sdk-0.0.1.6.tar` & `spotON_sdk-0.0.1.7.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     6171 2023-05-06 14:09:02.618269 spotON_sdk-0.0.1.6/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.1.6/LICENSE
--rw-r--r--   0        0        0      317 2023-05-06 23:30:48.724788 spotON_sdk-0.0.1.6/pyproject.toml
--rw-r--r--   0        0        0      449 2023-05-07 23:25:16.847846 spotON_sdk-0.0.1.6/spotON_sdk/__init__.py
--rw-r--r--   0        0        0     3404 2023-05-07 23:24:01.934943 spotON_sdk-0.0.1.6/spotON_sdk/constants/geography.py
--rw-r--r--   0        0        0     2786 2023-05-06 22:41:04.021539 spotON_sdk-0.0.1.6/spotON_sdk/logic/Config.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     6171 2023-05-06 14:09:02.618269 spotON_sdk-0.0.1.7/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.1.7/LICENSE
+-rw-r--r--   0        0        0      317 2023-05-06 23:30:48.724788 spotON_sdk-0.0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-08 08:24:40.645545 spotON_sdk-0.0.1.7/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0     4801 2023-05-08 08:12:43.917785 spotON_sdk-0.0.1.7/spotON_sdk/constants/countries.py
+-rw-r--r--   0        0        0     1468 2023-05-08 08:21:51.312070 spotON_sdk-0.0.1.7/spotON_sdk/constants/markets.py
+-rw-r--r--   0        0        0     2786 2023-05-06 22:41:04.021539 spotON_sdk-0.0.1.7/spotON_sdk/logic/Config.py
+-rw-r--r--   0        0        0      138 2023-05-08 08:23:54.822670 spotON_sdk-0.0.1.7/tests/test.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.1.7/PKG-INFO
```

### Comparing `spotON_sdk-0.0.1.6/.gitignore` & `spotON_sdk-0.0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.1.6/LICENSE` & `spotON_sdk-0.0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.1.6/spotON_sdk/logic/Config.py` & `spotON_sdk-0.0.1.7/spotON_sdk/logic/Config.py`

 * *Files identical despite different names*

