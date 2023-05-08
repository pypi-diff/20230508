# Comparing `tmp/shafara_tool_kit-0.1.1.tar.gz` & `tmp/shafara_tool_kit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shafara_tool_kit-0.1.1.tar", max compression
+gzip compressed data, was "shafara_tool_kit-0.2.1.tar", max compression
```

## Comparing `shafara_tool_kit-0.1.1.tar` & `shafara_tool_kit-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0      335 2023-04-20 12:43:31.366573 shafara_tool_kit-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 11:35:39.264722 shafara_tool_kit-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-20 12:39:40.438529 shafara_tool_kit-0.1.1/shafaratoolkit/__init__.py
--rw-r--r--   0        0        0      108 2023-04-20 11:41:05.406004 shafara_tool_kit-0.1.1/shafaratoolkit/props.py
--rw-r--r--   0        0        0      392 1970-01-01 00:00:00.000000 shafara_tool_kit-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    17098 2023-05-07 23:29:28.404990 shafara_tool_kit-0.2.1/LICENSE
+-rw-r--r--   0        0        0      335 2023-05-07 23:44:09.268783 shafara_tool_kit-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      667 2023-05-07 23:29:28.404990 shafara_tool_kit-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-07 23:29:28.404990 shafara_tool_kit-0.2.1/shafaratoolkit/__init__.py
+-rw-r--r--   0        0        0      108 2023-05-07 23:29:28.404990 shafara_tool_kit-0.2.1/shafaratoolkit/props.py
+-rw-r--r--   0        0        0     1324 2023-05-07 23:37:19.205311 shafara_tool_kit-0.2.1/shafaratoolkit/pytorchtools.py
+-rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 shafara_tool_kit-0.2.1/PKG-INFO
```

