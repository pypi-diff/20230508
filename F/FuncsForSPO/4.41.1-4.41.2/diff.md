# Comparing `tmp/FuncsForSPO-4.41.1.tar.gz` & `tmp/FuncsForSPO-4.41.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-4.41.1.tar", last modified: Fri Apr 28 12:56:51 2023, max compression
+gzip compressed data, was "FuncsForSPO-4.41.2.tar", last modified: Mon May  8 16:18:56 2023, max compression
```

## Comparing `FuncsForSPO-4.41.1.tar` & `FuncsForSPO-4.41.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 12:56:51.564394 FuncsForSPO-4.41.1/
-drwxrwxrwx   0        0        0        0 2023-04-28 12:56:51.265701 FuncsForSPO-4.41.1/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-04-28 12:56:51.312856 FuncsForSPO-4.41.1/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-4.41.1/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-4.41.1/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-04-28 12:56:51.323010 FuncsForSPO-4.41.1/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.1/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-4.41.1/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-28 12:56:51.330583 FuncsForSPO-4.41.1/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.1/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-4.41.1/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-04-28 12:56:51.339753 FuncsForSPO-4.41.1/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.1/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-4.41.1/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-04-28 12:56:51.259558 FuncsForSPO-4.41.1/FuncsForSPO/fpdf/
-drwxrwxrwx   0        0        0        0 2023-04-28 12:56:51.355476 FuncsForSPO-4.41.1/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-4.41.1/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.41.1/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-4.41.1/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-04-28 12:56:51.370335 FuncsForSPO-4.41.1/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-4.41.1/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.41.1/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-4.41.1/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-04-28 12:56:51.374350 FuncsForSPO-4.41.1/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-4.41.1/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-04-28 12:56:51.393876 FuncsForSPO-4.41.1/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-4.41.1/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-4.41.1/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     4962 2023-04-28 12:55:20.000000 FuncsForSPO-4.41.1/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-04-28 12:56:51.410967 FuncsForSPO-4.41.1/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.1/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-4.41.1/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-04-28 12:56:51.421006 FuncsForSPO-4.41.1/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.1/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    69597 2023-03-17 17:54:18.000000 FuncsForSPO-4.41.1/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-04-28 12:56:51.430230 FuncsForSPO-4.41.1/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.1/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-4.41.1/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-04-28 12:56:51.441421 FuncsForSPO-4.41.1/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.1/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    38180 2023-03-31 19:28:24.000000 FuncsForSPO-4.41.1/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-04-28 12:56:51.452063 FuncsForSPO-4.41.1/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.1/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-4.41.1/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-04-28 12:56:51.459821 FuncsForSPO-4.41.1/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-4.41.1/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-4.41.1/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-04-28 12:56:51.464933 FuncsForSPO-4.41.1/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-4.41.1/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-28 12:56:51.305505 FuncsForSPO-4.41.1/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8027 2023-04-28 12:56:51.000000 FuncsForSPO-4.41.1/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1331 2023-04-28 12:56:51.000000 FuncsForSPO-4.41.1/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 12:56:51.000000 FuncsForSPO-4.41.1/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2023-04-28 12:56:51.000000 FuncsForSPO-4.41.1/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      350 2023-04-28 12:56:51.000000 FuncsForSPO-4.41.1/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-4.41.1/LICENSE
--rw-rw-rw-   0        0        0     8027 2023-04-28 12:56:51.559683 FuncsForSPO-4.41.1/PKG-INFO
--rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-4.41.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-28 12:56:51.565311 FuncsForSPO-4.41.1/setup.cfg
--rw-rw-rw-   0        0        0     2150 2023-04-28 12:56:25.000000 FuncsForSPO-4.41.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:18:56.884089 FuncsForSPO-4.41.2/
+drwxrwxrwx   0        0        0        0 2023-05-08 16:18:56.528115 FuncsForSPO-4.41.2/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-05-08 16:18:56.633123 FuncsForSPO-4.41.2/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-4.41.2/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-4.41.2/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:18:56.646058 FuncsForSPO-4.41.2/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.2/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-4.41.2/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:18:56.655538 FuncsForSPO-4.41.2/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.2/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-4.41.2/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:18:56.667931 FuncsForSPO-4.41.2/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.2/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-4.41.2/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:18:56.519086 FuncsForSPO-4.41.2/FuncsForSPO/fpdf/
+drwxrwxrwx   0        0        0        0 2023-05-08 16:18:56.684051 FuncsForSPO-4.41.2/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-4.41.2/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.41.2/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-4.41.2/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:18:56.698480 FuncsForSPO-4.41.2/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-4.41.2/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.41.2/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-4.41.2/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:18:56.703995 FuncsForSPO-4.41.2/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-4.41.2/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:18:56.720673 FuncsForSPO-4.41.2/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-4.41.2/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-4.41.2/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     4990 2023-05-08 16:18:16.000000 FuncsForSPO-4.41.2/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:18:56.731005 FuncsForSPO-4.41.2/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.2/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-4.41.2/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:18:56.739920 FuncsForSPO-4.41.2/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.2/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    69597 2023-03-17 17:54:18.000000 FuncsForSPO-4.41.2/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:18:56.753126 FuncsForSPO-4.41.2/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.2/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-4.41.2/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:18:56.762398 FuncsForSPO-4.41.2/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.2/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    38180 2023-03-31 19:28:24.000000 FuncsForSPO-4.41.2/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:18:56.773230 FuncsForSPO-4.41.2/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.2/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-4.41.2/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:18:56.783110 FuncsForSPO-4.41.2/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-4.41.2/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-4.41.2/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:18:56.788697 FuncsForSPO-4.41.2/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-4.41.2/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:18:56.618032 FuncsForSPO-4.41.2/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8027 2023-05-08 16:18:56.000000 FuncsForSPO-4.41.2/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1331 2023-05-08 16:18:56.000000 FuncsForSPO-4.41.2/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 16:18:56.000000 FuncsForSPO-4.41.2/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2023-05-08 16:18:56.000000 FuncsForSPO-4.41.2/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      350 2023-05-08 16:18:56.000000 FuncsForSPO-4.41.2/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-4.41.2/LICENSE
+-rw-rw-rw-   0        0        0     8027 2023-05-08 16:18:56.878565 FuncsForSPO-4.41.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-4.41.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 16:18:56.885091 FuncsForSPO-4.41.2/setup.cfg
+-rw-rw-rw-   0        0        0     2150 2023-05-08 16:18:44.000000 FuncsForSPO-4.41.2/setup.py
```

### Comparing `FuncsForSPO-4.41.1/FuncsForSPO/femails/femails.py` & `FuncsForSPO-4.41.2/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.1/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-4.41.2/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.1/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-4.41.2/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.1/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-4.41.2/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.1/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-4.41.2/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.1/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-4.41.2/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.1/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-4.41.2/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.1/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-4.41.2/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.1/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-4.41.2/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.1/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-4.41.2/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.1/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-4.41.2/FuncsForSPO/fpdf/focr/orc.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,13 +126,13 @@
             response = requests.post(url, data=data, headers={'Content-Type': 'application/json'})
 
             # Extrai o texto da resposta JSON
             try:
                 response_json = response.json()
             except Exception as e:
                 print(e)
-                continue
+                ocr_paycon(pdf_path, user, password)
             if response_json.get('status') == 'finalizado':
                 return response_json.get('result')
             else:
                 print(response_json.get('status'))
                 sleep(1)
```

### Comparing `FuncsForSPO-4.41.1/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-4.41.2/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.1/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-4.41.2/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.1/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-4.41.2/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.1/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-4.41.2/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.1/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-4.41.2/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.1/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-4.41.2/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.1/FuncsForSPO/utils/utils.py` & `FuncsForSPO-4.41.2/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.1/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-4.41.2/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 4.41.1
+Version: 4.41.2
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-4.41.1/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-4.41.2/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.1/LICENSE` & `FuncsForSPO-4.41.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.1/PKG-INFO` & `FuncsForSPO-4.41.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 4.41.1
+Version: 4.41.2
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-4.41.1/README.md` & `FuncsForSPO-4.41.2/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.1/setup.py` & `FuncsForSPO-4.41.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '4.41.1'
+version = '4.41.2'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
```

