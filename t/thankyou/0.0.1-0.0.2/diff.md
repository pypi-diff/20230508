# Comparing `tmp/thankyou-0.0.1.tar.gz` & `tmp/thankyou-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thankyou-0.0.1.tar", max compression
+gzip compressed data, was "thankyou-0.0.2.tar", max compression
```

## Comparing `thankyou-0.0.1.tar` & `thankyou-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    35149 2021-06-29 02:56:17.939902 thankyou-0.0.1/LICENSE
--rw-r--r--   0        0        0      187 2021-06-29 03:14:18.031643 thankyou-0.0.1/README.md
--rw-r--r--   0        0        0      730 2021-06-29 03:08:37.518729 thankyou-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      847 2021-06-29 03:03:13.817500 thankyou-0.0.1/thankyou.py
--rw-r--r--   0        0        0      712 2021-06-29 03:14:38.653824 thankyou-0.0.1/setup.py
--rw-r--r--   0        0        0      955 2021-06-29 03:14:38.654306 thankyou-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-08 08:35:27.761622 thankyou-0.0.2/LICENSE
+-rw-r--r--   0        0        0      712 2023-05-08 08:35:27.761622 thankyou-0.0.2/README.md
+-rw-r--r--   0        0        0     1185 2023-05-08 08:35:27.761622 thankyou-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-05-08 08:35:27.761622 thankyou-0.0.2/thankyou/__init__.py
+-rw-r--r--   0        0        0      131 2023-05-08 08:35:27.761622 thankyou-0.0.2/thankyou/tests.py
+-rw-r--r--   0        0        0     8940 2023-05-08 08:35:27.761622 thankyou-0.0.2/thankyou/thankyou.py
+-rw-r--r--   0        0        0     1713 1970-01-01 00:00:00.000000 thankyou-0.0.2/PKG-INFO
```

### Comparing `thankyou-0.0.1/LICENSE` & `thankyou-0.0.2/LICENSE`

 * *Files identical despite different names*

