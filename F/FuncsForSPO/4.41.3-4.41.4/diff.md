# Comparing `tmp/FuncsForSPO-4.41.3.tar.gz` & `tmp/FuncsForSPO-4.41.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-4.41.3.tar", last modified: Mon May  8 20:39:27 2023, max compression
+gzip compressed data, was "FuncsForSPO-4.41.4.tar", last modified: Mon May  8 20:47:16 2023, max compression
```

## Comparing `FuncsForSPO-4.41.3.tar` & `FuncsForSPO-4.41.4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 20:39:27.627084 FuncsForSPO-4.41.3/
-drwxrwxrwx   0        0        0        0 2023-05-08 20:39:26.897325 FuncsForSPO-4.41.3/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-05-08 20:39:27.165467 FuncsForSPO-4.41.3/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-4.41.3/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-4.41.3/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-05-08 20:39:27.187546 FuncsForSPO-4.41.3/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.3/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-4.41.3/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-08 20:39:27.205495 FuncsForSPO-4.41.3/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.3/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-4.41.3/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-05-08 20:39:27.240732 FuncsForSPO-4.41.3/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.3/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-4.41.3/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-05-08 20:39:26.881096 FuncsForSPO-4.41.3/FuncsForSPO/fpdf/
-drwxrwxrwx   0        0        0        0 2023-05-08 20:39:27.279026 FuncsForSPO-4.41.3/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-4.41.3/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.41.3/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-4.41.3/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-05-08 20:39:27.309079 FuncsForSPO-4.41.3/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-4.41.3/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.41.3/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-4.41.3/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-05-08 20:39:27.322319 FuncsForSPO-4.41.3/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-4.41.3/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-05-08 20:39:27.362832 FuncsForSPO-4.41.3/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-4.41.3/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-4.41.3/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     5030 2023-05-08 20:20:01.000000 FuncsForSPO-4.41.3/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-05-08 20:39:27.386034 FuncsForSPO-4.41.3/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.3/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-4.41.3/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-05-08 20:39:27.402203 FuncsForSPO-4.41.3/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.3/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    69597 2023-03-17 17:54:18.000000 FuncsForSPO-4.41.3/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-05-08 20:39:27.421185 FuncsForSPO-4.41.3/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.3/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-4.41.3/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-05-08 20:39:27.438668 FuncsForSPO-4.41.3/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.3/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    38180 2023-03-31 19:28:24.000000 FuncsForSPO-4.41.3/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-05-08 20:39:27.458376 FuncsForSPO-4.41.3/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.3/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-4.41.3/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-08 20:39:27.475871 FuncsForSPO-4.41.3/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-4.41.3/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-4.41.3/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-05-08 20:39:27.488600 FuncsForSPO-4.41.3/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-4.41.3/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 20:39:27.091718 FuncsForSPO-4.41.3/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8027 2023-05-08 20:39:26.000000 FuncsForSPO-4.41.3/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1331 2023-05-08 20:39:26.000000 FuncsForSPO-4.41.3/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 20:39:26.000000 FuncsForSPO-4.41.3/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2023-05-08 20:39:26.000000 FuncsForSPO-4.41.3/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      350 2023-05-08 20:39:26.000000 FuncsForSPO-4.41.3/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-4.41.3/LICENSE
--rw-rw-rw-   0        0        0     8027 2023-05-08 20:39:27.621577 FuncsForSPO-4.41.3/PKG-INFO
--rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-4.41.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-08 20:39:27.628105 FuncsForSPO-4.41.3/setup.cfg
--rw-rw-rw-   0        0        0     2150 2023-05-08 20:39:14.000000 FuncsForSPO-4.41.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:47:16.568738 FuncsForSPO-4.41.4/
+drwxrwxrwx   0        0        0        0 2023-05-08 20:47:15.977635 FuncsForSPO-4.41.4/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-05-08 20:47:16.085526 FuncsForSPO-4.41.4/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-4.41.4/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-4.41.4/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:47:16.098961 FuncsForSPO-4.41.4/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.4/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-4.41.4/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:47:16.121407 FuncsForSPO-4.41.4/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.4/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-4.41.4/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:47:16.140488 FuncsForSPO-4.41.4/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.4/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-4.41.4/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:47:15.943683 FuncsForSPO-4.41.4/FuncsForSPO/fpdf/
+drwxrwxrwx   0        0        0        0 2023-05-08 20:47:16.184678 FuncsForSPO-4.41.4/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-4.41.4/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.41.4/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-4.41.4/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:47:16.239722 FuncsForSPO-4.41.4/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-4.41.4/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.41.4/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-4.41.4/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:47:16.255826 FuncsForSPO-4.41.4/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-4.41.4/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:47:16.294757 FuncsForSPO-4.41.4/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-4.41.4/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-4.41.4/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     5017 2023-05-08 20:46:58.000000 FuncsForSPO-4.41.4/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:47:16.314268 FuncsForSPO-4.41.4/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.4/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-4.41.4/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:47:16.330533 FuncsForSPO-4.41.4/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.4/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    69597 2023-03-17 17:54:18.000000 FuncsForSPO-4.41.4/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:47:16.352779 FuncsForSPO-4.41.4/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.4/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-4.41.4/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:47:16.368745 FuncsForSPO-4.41.4/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.4/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    38180 2023-03-31 19:28:24.000000 FuncsForSPO-4.41.4/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:47:16.392263 FuncsForSPO-4.41.4/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.4/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-4.41.4/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:47:16.410413 FuncsForSPO-4.41.4/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-4.41.4/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-4.41.4/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:47:16.425395 FuncsForSPO-4.41.4/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-4.41.4/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:47:16.059169 FuncsForSPO-4.41.4/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8027 2023-05-08 20:47:15.000000 FuncsForSPO-4.41.4/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1331 2023-05-08 20:47:15.000000 FuncsForSPO-4.41.4/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 20:47:15.000000 FuncsForSPO-4.41.4/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2023-05-08 20:47:15.000000 FuncsForSPO-4.41.4/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      350 2023-05-08 20:47:15.000000 FuncsForSPO-4.41.4/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-4.41.4/LICENSE
+-rw-rw-rw-   0        0        0     8027 2023-05-08 20:47:16.564710 FuncsForSPO-4.41.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-4.41.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 20:47:16.568738 FuncsForSPO-4.41.4/setup.cfg
+-rw-rw-rw-   0        0        0     2150 2023-05-08 20:47:05.000000 FuncsForSPO-4.41.4/setup.py
```

### Comparing `FuncsForSPO-4.41.3/FuncsForSPO/femails/femails.py` & `FuncsForSPO-4.41.4/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.3/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-4.41.4/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.3/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-4.41.4/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.3/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-4.41.4/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.3/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-4.41.4/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.3/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-4.41.4/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.3/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-4.41.4/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.3/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-4.41.4/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.3/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-4.41.4/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.3/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-4.41.4/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.3/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-4.41.4/FuncsForSPO/fpdf/focr/orc.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from FuncsForSPO.fpython.functions_for_py import *
 import requests
 import json
 import os
 import base64
 
 class ErroAPI(Exception):
-    return 'ErrorAPi'
+    pass
 
 def faz_ocr_em_pdf(file_pdf: str, dir_exit: str='output', get_text_into_code: bool=True, headless: bool=True, prints=False) -> str:
     """
     ## DIREITOS RESERVADOS / RIGHTS RESERVED / DERECHOS RESERVADOS
 
     ## https://online2pdf.com/pt/converter-pdf-para-txt-com-ocr
```

### Comparing `FuncsForSPO-4.41.3/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-4.41.4/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.3/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-4.41.4/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.3/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-4.41.4/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.3/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-4.41.4/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.3/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-4.41.4/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.3/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-4.41.4/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.3/FuncsForSPO/utils/utils.py` & `FuncsForSPO-4.41.4/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.3/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-4.41.4/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 4.41.3
+Version: 4.41.4
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-4.41.3/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-4.41.4/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.3/LICENSE` & `FuncsForSPO-4.41.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.3/PKG-INFO` & `FuncsForSPO-4.41.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 4.41.3
+Version: 4.41.4
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-4.41.3/README.md` & `FuncsForSPO-4.41.4/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.3/setup.py` & `FuncsForSPO-4.41.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '4.41.3'
+version = '4.41.4'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
```

