# Comparing `tmp/spotON_sdk-0.0.1.4.tar.gz` & `tmp/spotON_sdk-0.0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.1.4.tar", last modified: Sat May  6 22:56:43 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.1.5.tar", last modified: Sat May  6 23:33:50 2023, max compression
```

## Comparing `spotON_sdk-0.0.1.4.tar` & `spotON_sdk-0.0.1.5.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     6171 2023-05-06 14:09:02.618269 spotON_sdk-0.0.1.4/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.1.4/LICENSE
--rw-r--r--   0        0        0      317 2023-05-06 22:56:31.734624 spotON_sdk-0.0.1.4/pyproject.toml
--rw-r--r--   0        0        0      390 2023-05-06 22:55:40.247203 spotON_sdk-0.0.1.4/spotON_sdk/__init__.py
--rw-r--r--   0        0        0     2786 2023-05-06 22:41:04.021539 spotON_sdk-0.0.1.4/spotON_sdk/logic/Config.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     6171 2023-05-06 14:09:02.618269 spotON_sdk-0.0.1.5/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.1.5/LICENSE
+-rw-r--r--   0        0        0      317 2023-05-06 23:30:48.724788 spotON_sdk-0.0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      449 2023-05-06 23:33:41.090094 spotON_sdk-0.0.1.5/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      570 2023-05-06 23:28:52.158935 spotON_sdk-0.0.1.5/spotON_sdk/constants/geography.py
+-rw-r--r--   0        0        0     2786 2023-05-06 22:41:04.021539 spotON_sdk-0.0.1.5/spotON_sdk/logic/Config.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.1.5/PKG-INFO
```

### Comparing `spotON_sdk-0.0.1.4/.gitignore` & `spotON_sdk-0.0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.1.4/LICENSE` & `spotON_sdk-0.0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.1.4/spotON_sdk/logic/Config.py` & `spotON_sdk-0.0.1.5/spotON_sdk/logic/Config.py`

 * *Files identical despite different names*

