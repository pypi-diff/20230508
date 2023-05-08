# Comparing `tmp/pymad8-2.0.0.tar.gz` & `tmp/pymad8-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymad8-2.0.0.tar", last modified: Sun Mar 19 17:23:47 2023, max compression
+gzip compressed data, was "pymad8-2.0.1.tar", last modified: Mon May  8 15:54:26 2023, max compression
```

## Comparing `pymad8-2.0.0.tar` & `pymad8-2.0.1.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-19 17:23:47.678159 pymad8-2.0.0/
--rw-r--r--   0 lnevay     (501) staff       (20)       97 2023-03-19 17:12:52.000000 pymad8-2.0.0/.gitignore
--rw-r--r--   0 lnevay     (501) staff       (20)    35149 2020-05-18 14:45:38.000000 pymad8-2.0.0/COPYING.txt
--rw-r--r--   0 lnevay     (501) staff       (20)      611 2020-05-18 14:45:38.000000 pymad8-2.0.0/LICENSE.txt
--rw-r--r--   0 lnevay     (501) staff       (20)      564 2023-02-13 16:47:29.000000 pymad8-2.0.0/Makefile
--rw-r--r--   0 lnevay     (501) staff       (20)     1217 2023-03-19 17:23:47.678245 pymad8-2.0.0/PKG-INFO
--rw-r--r--   0 lnevay     (501) staff       (20)      151 2020-05-18 14:45:38.000000 pymad8-2.0.0/README.md
--rw-r--r--   0 lnevay     (501) staff       (20)      170 2020-05-18 14:45:38.000000 pymad8-2.0.0/TODO
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-19 17:23:47.673189 pymad8-2.0.0/docs/
--rw-r--r--   0 lnevay     (501) staff       (20)      611 2020-05-18 14:45:38.000000 pymad8-2.0.0/docs/Makefile
--rw-r--r--   0 lnevay     (501) staff       (20)      808 2020-05-18 14:45:38.000000 pymad8-2.0.0/docs/make.bat
--rw-r--r--   0 lnevay     (501) staff       (20)   365545 2023-03-19 17:19:24.000000 pymad8-2.0.0/docs/pymad8.pdf
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-19 17:23:47.674650 pymad8-2.0.0/docs/source/
--rw-r--r--   0 lnevay     (501) staff       (20)      219 2022-11-01 14:50:10.000000 pymad8-2.0.0/docs/source/authorship.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     5383 2023-03-19 17:15:21.000000 pymad8-2.0.0/docs/source/conf.py
--rw-r--r--   0 lnevay     (501) staff       (20)      919 2022-11-01 14:50:10.000000 pymad8-2.0.0/docs/source/convert.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     5674 2023-02-13 16:47:29.000000 pymad8-2.0.0/docs/source/data.rst
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-19 17:23:47.674774 pymad8-2.0.0/docs/source/figures/
--rw-r--r--   0 lnevay     (501) staff       (20)    85954 2022-11-01 14:50:10.000000 pymad8-2.0.0/docs/source/figures/betas.png
--rw-r--r--   0 lnevay     (501) staff       (20)      367 2023-02-13 16:47:29.000000 pymad8-2.0.0/docs/source/index.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      540 2022-11-01 14:50:10.000000 pymad8-2.0.0/docs/source/installation.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      629 2020-05-18 14:45:38.000000 pymad8-2.0.0/docs/source/licence.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      977 2022-11-01 14:50:10.000000 pymad8-2.0.0/docs/source/moduledocs.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     4662 2023-02-13 16:47:29.000000 pymad8-2.0.0/docs/source/plot.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     3442 2023-02-13 16:47:29.000000 pymad8-2.0.0/docs/source/simulation.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      556 2020-05-18 14:45:38.000000 pymad8-2.0.0/docs/source/support.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     1382 2023-03-19 17:06:11.000000 pymad8-2.0.0/pyproject.toml
--rw-r--r--   0 lnevay     (501) staff       (20)      257 2023-03-19 17:23:47.678478 pymad8-2.0.0/setup.cfg
--rw-r--r--   0 lnevay     (501) staff       (20)       38 2023-03-19 17:08:53.000000 pymad8-2.0.0/setup.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-19 17:23:47.671640 pymad8-2.0.0/src/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-19 17:23:47.675795 pymad8-2.0.0/src/pymad8/
--rw-r--r--   0 lnevay     (501) staff       (20)     5322 2022-11-01 14:50:10.000000 pymad8-2.0.0/src/pymad8/Input.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-19 17:23:47.677166 pymad8-2.0.0/src/pymad8/Old/
--rw-r--r--   0 lnevay     (501) staff       (20)    14747 2023-02-13 16:47:29.000000 pymad8-2.0.0/src/pymad8/Old/Converter.py
--rw-r--r--   0 lnevay     (501) staff       (20)    21434 2022-11-01 14:50:10.000000 pymad8-2.0.0/src/pymad8/Old/Mad8.py
--rw-r--r--   0 lnevay     (501) staff       (20)     7250 2022-11-01 14:50:10.000000 pymad8-2.0.0/src/pymad8/Old/Mad8Converter.py
--rw-r--r--   0 lnevay     (501) staff       (20)    34234 2022-11-01 14:50:10.000000 pymad8-2.0.0/src/pymad8/Old/OutputOld.py
--rw-r--r--   0 lnevay     (501) staff       (20)    15846 2022-11-01 14:50:10.000000 pymad8-2.0.0/src/pymad8/Old/PlotOld.py
--rw-r--r--   0 lnevay     (501) staff       (20)     5372 2023-02-13 16:47:29.000000 pymad8-2.0.0/src/pymad8/Old/Saveline.py
--rw-r--r--   0 lnevay     (501) staff       (20)    25010 2023-02-13 16:47:29.000000 pymad8-2.0.0/src/pymad8/Output.py
--rw-r--r--   0 lnevay     (501) staff       (20)     8899 2023-02-13 16:47:29.000000 pymad8-2.0.0/src/pymad8/Plot.py
--rw-r--r--   0 lnevay     (501) staff       (20)    20721 2023-02-13 16:47:29.000000 pymad8-2.0.0/src/pymad8/Sim.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1538 2022-11-01 14:50:10.000000 pymad8-2.0.0/src/pymad8/Track.py
--rw-r--r--   0 lnevay     (501) staff       (20)    11057 2022-11-01 14:50:10.000000 pymad8-2.0.0/src/pymad8/Visualisation.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1304 2023-03-19 17:09:27.000000 pymad8-2.0.0/src/pymad8/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)      160 2023-03-19 17:23:47.000000 pymad8-2.0.0/src/pymad8/_version.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-19 17:23:47.676456 pymad8-2.0.0/src/pymad8.egg-info/
--rw-r--r--   0 lnevay     (501) staff       (20)     1217 2023-03-19 17:23:47.000000 pymad8-2.0.0/src/pymad8.egg-info/PKG-INFO
--rw-r--r--   0 lnevay     (501) staff       (20)     1117 2023-03-19 17:23:47.000000 pymad8-2.0.0/src/pymad8.egg-info/SOURCES.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-03-19 17:23:47.000000 pymad8-2.0.0/src/pymad8.egg-info/dependency_links.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-03-19 17:12:11.000000 pymad8-2.0.0/src/pymad8.egg-info/not-zip-safe
--rw-r--r--   0 lnevay     (501) staff       (20)       99 2023-03-19 17:23:47.000000 pymad8-2.0.0/src/pymad8.egg-info/requires.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        7 2023-03-19 17:23:47.000000 pymad8-2.0.0/src/pymad8.egg-info/top_level.txt
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-19 17:23:47.678062 pymad8-2.0.0/test/
--rw-r--r--   0 lnevay     (501) staff       (20)     1089 2023-02-13 16:47:29.000000 pymad8-2.0.0/test/T01_DRIFT.txm
--rw-r--r--   0 lnevay     (501) staff       (20)      795 2023-02-13 16:47:29.000000 pymad8-2.0.0/test/T02_QUAD.txm
--rw-r--r--   0 lnevay     (501) staff       (20)      795 2023-02-13 16:47:29.000000 pymad8-2.0.0/test/T03_SEXT.txm
--rw-r--r--   0 lnevay     (501) staff       (20)      795 2023-02-13 16:47:29.000000 pymad8-2.0.0/test/T04_OCTU.txm
--rw-r--r--   0 lnevay     (501) staff       (20)      834 2023-02-13 16:47:29.000000 pymad8-2.0.0/test/T05_SBEN.txm
--rw-r--r--   0 lnevay     (501) staff       (20)      834 2023-02-13 16:47:29.000000 pymad8-2.0.0/test/T06_RBEN.txm
--rw-r--r--   0 lnevay     (501) staff       (20)      834 2023-02-13 16:47:29.000000 pymad8-2.0.0/test/T07_MULT.txm
--rw-r--r--   0 lnevay     (501) staff       (20)      349 2022-11-01 14:50:10.000000 pymad8-2.0.0/test/test_pymad8.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 15:54:26.024834 pymad8-2.0.1/
+-rw-r--r--   0 lnevay     (501) staff       (20)       97 2023-03-19 17:12:52.000000 pymad8-2.0.1/.gitignore
+-rw-r--r--   0 lnevay     (501) staff       (20)    35149 2020-05-18 14:45:38.000000 pymad8-2.0.1/COPYING.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)      611 2020-05-18 14:45:38.000000 pymad8-2.0.1/LICENSE.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)      564 2023-02-13 16:47:29.000000 pymad8-2.0.1/Makefile
+-rw-r--r--   0 lnevay     (501) staff       (20)     1254 2023-05-08 15:54:26.025032 pymad8-2.0.1/PKG-INFO
+-rw-r--r--   0 lnevay     (501) staff       (20)      162 2023-05-08 15:49:21.000000 pymad8-2.0.1/README.md
+-rw-r--r--   0 lnevay     (501) staff       (20)      170 2020-05-18 14:45:38.000000 pymad8-2.0.1/TODO
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 15:54:26.015674 pymad8-2.0.1/docs/
+-rw-r--r--   0 lnevay     (501) staff       (20)      611 2020-05-18 14:45:38.000000 pymad8-2.0.1/docs/Makefile
+-rw-r--r--   0 lnevay     (501) staff       (20)      808 2020-05-18 14:45:38.000000 pymad8-2.0.1/docs/make.bat
+-rw-r--r--   0 lnevay     (501) staff       (20)   373831 2023-05-08 15:53:19.000000 pymad8-2.0.1/docs/pymad8.pdf
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 15:54:26.018707 pymad8-2.0.1/docs/source/
+-rw-r--r--   0 lnevay     (501) staff       (20)      219 2022-11-01 14:50:10.000000 pymad8-2.0.1/docs/source/authorship.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     5383 2023-03-19 17:15:21.000000 pymad8-2.0.1/docs/source/conf.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      919 2022-11-01 14:50:10.000000 pymad8-2.0.1/docs/source/convert.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     5674 2023-02-13 16:47:29.000000 pymad8-2.0.1/docs/source/data.rst
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 15:54:26.018982 pymad8-2.0.1/docs/source/figures/
+-rw-r--r--   0 lnevay     (501) staff       (20)    85954 2022-11-01 14:50:10.000000 pymad8-2.0.1/docs/source/figures/betas.png
+-rw-r--r--   0 lnevay     (501) staff       (20)      386 2023-05-08 15:47:39.000000 pymad8-2.0.1/docs/source/index.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      540 2022-11-01 14:50:10.000000 pymad8-2.0.1/docs/source/installation.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      629 2020-05-18 14:45:38.000000 pymad8-2.0.1/docs/source/licence.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      977 2022-11-01 14:50:10.000000 pymad8-2.0.1/docs/source/moduledocs.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     4662 2023-02-13 16:47:29.000000 pymad8-2.0.1/docs/source/plot.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     3442 2023-02-13 16:47:29.000000 pymad8-2.0.1/docs/source/simulation.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      556 2020-05-18 14:45:38.000000 pymad8-2.0.1/docs/source/support.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      130 2023-05-08 15:48:28.000000 pymad8-2.0.1/docs/source/version_history.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     1394 2023-05-03 13:39:26.000000 pymad8-2.0.1/pyproject.toml
+-rw-r--r--   0 lnevay     (501) staff       (20)      257 2023-05-08 15:54:26.025313 pymad8-2.0.1/setup.cfg
+-rw-r--r--   0 lnevay     (501) staff       (20)       38 2023-03-19 17:08:53.000000 pymad8-2.0.1/setup.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 15:54:26.012511 pymad8-2.0.1/src/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 15:54:26.021283 pymad8-2.0.1/src/pymad8/
+-rw-r--r--   0 lnevay     (501) staff       (20)     5322 2022-11-01 14:50:10.000000 pymad8-2.0.1/src/pymad8/Input.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 15:54:26.023411 pymad8-2.0.1/src/pymad8/Old/
+-rw-r--r--   0 lnevay     (501) staff       (20)    14747 2023-02-13 16:47:29.000000 pymad8-2.0.1/src/pymad8/Old/Converter.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    21434 2022-11-01 14:50:10.000000 pymad8-2.0.1/src/pymad8/Old/Mad8.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     7250 2022-11-01 14:50:10.000000 pymad8-2.0.1/src/pymad8/Old/Mad8Converter.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    34234 2022-11-01 14:50:10.000000 pymad8-2.0.1/src/pymad8/Old/OutputOld.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    15846 2022-11-01 14:50:10.000000 pymad8-2.0.1/src/pymad8/Old/PlotOld.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     5372 2023-02-13 16:47:29.000000 pymad8-2.0.1/src/pymad8/Old/Saveline.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    25413 2023-04-22 21:37:15.000000 pymad8-2.0.1/src/pymad8/Output.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     8899 2023-02-13 16:47:29.000000 pymad8-2.0.1/src/pymad8/Plot.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    33093 2023-04-22 21:37:15.000000 pymad8-2.0.1/src/pymad8/Sim.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1538 2022-11-01 14:50:10.000000 pymad8-2.0.1/src/pymad8/Track.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    11057 2022-11-01 14:50:10.000000 pymad8-2.0.1/src/pymad8/Visualisation.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1304 2023-03-19 17:09:27.000000 pymad8-2.0.1/src/pymad8/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      160 2023-05-08 15:54:25.000000 pymad8-2.0.1/src/pymad8/_version.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 15:54:26.022012 pymad8-2.0.1/src/pymad8.egg-info/
+-rw-r--r--   0 lnevay     (501) staff       (20)     1254 2023-05-08 15:54:25.000000 pymad8-2.0.1/src/pymad8.egg-info/PKG-INFO
+-rw-r--r--   0 lnevay     (501) staff       (20)     1149 2023-05-08 15:54:26.000000 pymad8-2.0.1/src/pymad8.egg-info/SOURCES.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-05-08 15:54:25.000000 pymad8-2.0.1/src/pymad8.egg-info/dependency_links.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-03-19 17:12:11.000000 pymad8-2.0.1/src/pymad8.egg-info/not-zip-safe
+-rw-r--r--   0 lnevay     (501) staff       (20)      106 2023-05-08 15:54:25.000000 pymad8-2.0.1/src/pymad8.egg-info/requires.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        7 2023-05-08 15:54:25.000000 pymad8-2.0.1/src/pymad8.egg-info/top_level.txt
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 15:54:26.024607 pymad8-2.0.1/test/
+-rw-r--r--   0 lnevay     (501) staff       (20)     1089 2023-02-13 16:47:29.000000 pymad8-2.0.1/test/T01_DRIFT.txm
+-rw-r--r--   0 lnevay     (501) staff       (20)      795 2023-02-13 16:47:29.000000 pymad8-2.0.1/test/T02_QUAD.txm
+-rw-r--r--   0 lnevay     (501) staff       (20)      795 2023-02-13 16:47:29.000000 pymad8-2.0.1/test/T03_SEXT.txm
+-rw-r--r--   0 lnevay     (501) staff       (20)      795 2023-02-13 16:47:29.000000 pymad8-2.0.1/test/T04_OCTU.txm
+-rw-r--r--   0 lnevay     (501) staff       (20)      834 2023-02-13 16:47:29.000000 pymad8-2.0.1/test/T05_SBEN.txm
+-rw-r--r--   0 lnevay     (501) staff       (20)      834 2023-02-13 16:47:29.000000 pymad8-2.0.1/test/T06_RBEN.txm
+-rw-r--r--   0 lnevay     (501) staff       (20)      834 2023-02-13 16:47:29.000000 pymad8-2.0.1/test/T07_MULT.txm
+-rw-r--r--   0 lnevay     (501) staff       (20)      349 2022-11-01 14:50:10.000000 pymad8-2.0.1/test/test_pymad8.py
```

### Comparing `pymad8-2.0.0/COPYING.txt` & `pymad8-2.0.1/COPYING.txt`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/LICENSE.txt` & `pymad8-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/Makefile` & `pymad8-2.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/PKG-INFO` & `pymad8-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymad8
-Version: 2.0.0
+Version: 2.0.1
 Summary: Write MAD8 models and load MAD8 output.
 Author-email: "JAI@RHUL" <stewart.boogert@rhul.ac.uk>
 Maintainer-email: Stewart Boogert <stewart.boogert@rhul.ac.uk>
 Project-URL: homepage, http://www.pp.rhul.ac.uk/bdsim/pymad8
 Project-URL: documentation, http://www.pp.rhul.ac.uk/bdsim/pymad8
 Project-URL: repository, https://bitbucket.org/jairhul/pymad8
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,21 +19,23 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
+License-File: COPYING.txt
 
 #pymad8#
 
 ## Authors ##
 
-L. Nevay
+M. Deniaud
 S. Boogert
+L. Nevay
 
 ## Setup ##
 
 From within the pymad8 root directory:
 
 $ make install
```

### Comparing `pymad8-2.0.0/docs/Makefile` & `pymad8-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/docs/make.bat` & `pymad8-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/docs/pymad8.pdf` & `pymad8-2.0.1/docs/pymad8.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 16% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,13 +1,13 @@
 pymad8 Documentation
-Release 2.0.0
+Release 2.0.1
 
 Royal Holloway
 
-Mar 19, 2023
+May 08, 2023
 
 CONTENTS
 
 1
 
 Licence & Disclaimer
 
@@ -94,42 +94,48 @@
 9.6 pymad8.Visualisation module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 21
 22
 22
 24
 25
-27
-27
+28
+28
 
-10 Indices and tables
+10 Version History
+10.1 v2.0.1 - 2023 / 05 / 08 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-29
+31
+31
+
+11 Indices and tables
+
+33
 
 Python Module Index
 
-31
+35
 
 Index
 
-33
+37
 
 i
 
 ii
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
 
 pymad8 is a Python package to aid in the preparation, running and validation of BDSIM models.
 
 CONTENTS
 
 1
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
 
 2
 
 CONTENTS
 
 CHAPTER
 
@@ -141,15 +147,15 @@
 This software is provided “AS IS” and any express or limit warranties, including, but not limited to, implied warranties of merchantability, of satisfactory quality, and fitness for a particular purpose or use are disclaimed. In no
 event shall Royal Holloway, University of London be liable for any direct, indirect, incidental, special, exemplary,
 or consequential damages arising in any way out of the use of this software, even if advised of the possibility of
 such damage.
 
 3
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
 
 4
 
 Chapter 1. Licence & Disclaimer
 
 CHAPTER
 
@@ -165,15 +171,15 @@
 • William Shields
 • Jochem Snuverink
 • Stuart Walker
 • Marin Deniaud
 
 5
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
 
 6
 
 Chapter 2. Authorship
 
 CHAPTER
 
@@ -195,15 +201,15 @@
 git clone http://bitbucket.org/jairhul/pymad8
 cd pymad8
 make install
 Alternatively, run make develop from the same directory to ensure that any local changes are picked up.
 
 7
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
 
 8
 
 Chapter 3. Installation
 
 CHAPTER
 
@@ -241,15 +247,15 @@
 >>> e = pymad8.Output("myEnvelopeFile", "envel")
 >>> s = pymad8.Output("mySurveyFile", "survey")
 
 Note: The import will be assumed from now on in examples.
 
 9
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
 
 4.3 Querying
 The Output class can be used to query the data in various ways.
 
 4.3.1 Basic Information
 • All data is stored in the data object inside the class
 • The number of elements is stored in nrec.
@@ -291,15 +297,15 @@
 the getIndex function, we get either an integer or a list of integers
 Note: Similar functions are avaliable to find names and types of lattice elements
 
 10
 
 Chapter 4. MAD8 File Loading & Manipulation
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
 
 4.3.3 Rows and Columns
 A row of data is an entry for a particular element. The Output class is conceptually a list of elements. Each element
 is represented by a row in the pandas dataframe that has a key for each column. The list of acceptable keys (i.e.
 names of columns) can be found in the member named ‘colums’ :
 t.data.columns #prints out list of column names
 A specific row or set of rows can be accessed using similar functions as those previously shown :
@@ -343,15 +349,15 @@
 𝐸02
 2
 𝜎𝐸
 𝐸02
 
 11
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
 
 12
 
 Chapter 4. MAD8 File Loading & Manipulation
 
 CHAPTER
 
@@ -373,15 +379,15 @@
 the machine is also produced above the graph as shown below :
 
 Other than beta, other optics plots can be made using Alpha(), Mu(), Disp() or Sigma(). These functions are
 provided as a quick utility and not the ultimate plotting script.
 
 13
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
 
 5.3 Machine lattice
 The user can make their own plot and then append a machine diagram at the end if they wish :
 f = matplotlib.pyplot.figure()
 # user plotting commands here
 pymad8.Plot.AddMachineLatticeToFigure(f, "mytwissfile")
 gcf() is a matplotlib.pyplot function to get a reference to the current matplotlib figure and can be used as the first
@@ -482,15 +488,15 @@
 envel, sigma0=LINE.SIGMA0, save, tape=ENVEL_LINE
 To make the Survey output :
 use, LINE
 survey, tape=SURVEY_LINE
 
 15
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
 
 16
 
 Chapter 6. Converting Models
 
 CHAPTER
 
@@ -523,15 +529,15 @@
 The Tracking instance is generated from Mad8 twiss and rmat files :
 tracking = pymad8.Sim.Tracking('twiss_tape', 'rmat_tape')
 Then we can add the samplers at which we want to observe the particles. Multiples samplers can be added at once
 and we can either find them by index, name or type:
 
 17
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
 
 tracking.AddSampler(10)
 # Add element with index 10 as sampler
 tracking.AddSampler('INITIAL', select='name') # Add element named 'INITIAL' as sampler
 tracking.AddSampler('QUAD', select='type')
 # Add all quadrupoles as samplers
 
@@ -581,15 +587,15 @@
 
 8.1 Feature Request
 Feature requests or proposals can be submitted to the issue tracker - select the issue type as proposal or enhancement..
 Please have a look at the existing list of proposals before submitting a new one.
 
 19
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
 
 20
 
 Chapter 8. Support
 
 CHAPTER
 
@@ -620,15 +626,15 @@
 • Sim - Perform simulations on a machine, like particle tracking
 • Track - Old particle tracking code
 • Visualisation - Old survey plotting code
 Copyright Royal Holloway, University of London 2019.
 
 21
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
 
 9.1 pymad8.Input module
 pymad8.Input.decodeFileLine(input)
 Decode line for each element type
 input : string of a mad8 line
 pymad8.Input.removeComments(input)
 Remove comment lines
@@ -662,23 +668,25 @@
 getAperture(index, defaultAperSize=0.1)
 Get aperture of an element using corresponding index
 
 22
 
 Chapter 9. Module Contents
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
 
 If none provided or is 0 : set to a default aperture of 0.1m
 getColumnsByKeys(keylist)
 Return Columns that ar in keylist
 getElementByIndex(indexlist, keylist)
 Return value of elements given their indices and for chosen columns
 getElementByNames(namelist, keylist)
 Return value of elements given their names and for chosen columns
+getElementByNearestS(s, keylist)
+Return value of elements at a given s position and for chosen columns
 getIndexByNames(namelist)
 Return Index or Index list of elements that are in namelist
 getIndexByNearestS(s)
 Return Index of the closest element in the beamline
 getIndexByTypes(typelist)
 Return Index or Index list of elements that are in typelist
 getIndexByValues(**args)
@@ -708,15 +716,15 @@
 getTypeByNearestS(s)
 Return Type of the closest element in the beamline
 
 9.2. pymad8.Output module
 
 23
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
 
 getTypesByIndex(indexlist)
 Return Type or Type list of elements that are in indexlist
 getTypesByNames(namelist)
 Return Type or Type list of elements that are in namelist
 getTypesByValues(**args)
 Return Type or Type list of elements that have certain values for a chosen column
@@ -752,15 +760,15 @@
 Mu()
 Plot the Mu functions for both planes and both Mad
 
 24
 
 Chapter 9. Module Contents
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
 
 Sigma()
 Plot the beam size and beam divergence functions for both planes and both Mad
 
 9.4 pymad8.Sim module
 pymad8.Sim.CheckUnits(coord)
 class pymad8.Sim.Track_Collection(E_0)
@@ -790,48 +798,120 @@
 AddSamplers(value, select='index')
 Add one or multiple samplers which will be used when runing the tracking
 
 9.4. pymad8.Sim module
 
 25
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
 
 By default taking the indices of the elements we want as a samplers but one can change the select
 parameter to find samplers with names or types
 GenerateSamplers(nb)
 Add multiple samplers spread evenly along the lattice
 LoadBdsimTrack(inputfilename)
 Load Bdsim root file and generate orbit files for each particle in the track collection
 Then store the data in a structure similar to the pymad8 generated one
 LoadMad8Track(inputfilename)
 Load the Mad8 track files and store it in a structure similar to the pymad8 generated data
 /!/ NOT WORKING /!/
-PlotCorrelation(index, coord, ref_index, ref_coord, linFit=False, noPlots=False)
+PlotCorrelation(S, coord, ref_S, ref_coord, linFit=False, partlimit=200, bdsimCompare=False)
 Correlation plot for a given coordinate at the closest sampler from given S
 By default the reference sampler is LUXE IP
-PlotHist(S, coord)
+PlotHist(S, coord, bins=50, bdsimCompare=False)
 Plot histogram for a given coordinate at the closest sampler from given S
-PlotPhaseSpace(S, coord, linFit=False)
+PlotPhaseSpace(S, coord, linFit=False, partlimit=200, bdsimCompare=False)
 Phase space plot for a given coordinate at the closest sampler from given S
-PlotTrajectory(particle, coord, bdsimCompare=False, relativePlots=False)
+PlotRelatTrajSTD(coord)
+STD Trajectory difference plot between Mad8 and BDSIM for a given coordinate
+PlotRelatTrajectory(particle, coord)
+Trajectory difference plot between Mad8 and BDSIM for a given coordinate and for a given particle
+number
+PlotTrajectory(particle, coord, plotLegend=True, bdsimCompare=False)
 Trajectory plot for a given coordinate and for a given particle number
 RunPymad8Tracking(track_collection, turns=1)
 Run tracking for all particles using the rmat from Mad8
 >>> track.RunPymad8Tracking(track_collection)
-reduceDFbyIndex(index)
-pymad8.Sim.setSamplersAndTrack(twissfile, rmatfile, nb_sampl)
-pymad8.Sim.setTrackCollection(nb_part, energy, paramdict)
-pymad8.Sim.testTrack(twissfile, rmatfile)
+getPlaneCoord(coord)
+getTheoryAndFit(coord, ref_S, ref_coord, initial_fit)
+class pymad8.Sim.Tracking_data(dataframe)
+Bases: object
 
 26
 
 Chapter 9. Module Contents
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
+
+Class that stores tracking data from Mad8 or from BDSIM
+Comes with a bunch of useful function to extrat data
+CalcCorrelChi2(S, coord, ref_S, ref_coord, partlimit=200)
+Calculate the chi2, slope and intercept of the correlation fit between two positions and two coordinates
+CalcResolution(ref_coord, ref_S, BPM_list, noise=1e-05)
+SVD(M, ref_Vect)
+Return the correlation coefficients from a given matrix M using a Singular Value Decomposition
+method
+SortCoeff(ref_coord, ref_S, BPM_list, noise=1e-05)
+buildBPMmatrix(ref_S, ref_coord, BPM_list=None, BPM_list_type='pos', s_range=[-inf, inf],
+noise=None, mean_sub=False)
+Build the BPM matrix M with respect to a given list of BPMs
+getChi2(coord, ref_S, ref_coord)
+Return the chi2 vector along the lattice
+getColumnsByKeys(keylist)
+Return Columns that ar in keylist
+getFirstSamplerByNearestS(s)
+Return the first sampler name that correspond to the closest s
+getRowsByNearestS(s)
+Return Rows of the closest element in the beamline
+getRowsByParticles(particle)
+Return Rows of a given partcile
+getRowsByS(s)
+Return Rows of elements with the correspondig s position
+getRowsBySamplerAndNearestS(sampler, s)
+Return Rows of elements with the corresponding sampler name and closest s position
+getRowsBySamplerAndS(sampler, s)
+Return Rows of elements with the corresponding sampler name and s position
+getRowsBySamplers(sampler)
+Return Rows of elements with the correspondig sampler name
+getRowsByValues(key=None, minValue=-inf, maxValue=inf, equalValues=None)
+Return Rows of elements that have certain values for a chosen column
+getSByNearestS(s)
+Return the s position of the closest element in the beamline
+getSBySamplers(sampler)
+Retrun the list of s positions that correspond to a given sampler name
+getSamplersByNearestS(s)
+Return the list of sampler name that correspond to the closest s
+getSamplersByS(s)
+Return the list of sampler name that correspond to a given s
+
+9.4. pymad8.Sim module
+
+27
+
+pymad8 Documentation, Release 2.0.1
+
+getVectsByNearestS(keys, s)
+Return vector of a given column and for the closest s
+getVectsByParticle(keys, particle)
+Return vector of a given column and for a given particle
+getVectsByS(keys, s)
+Return vector of a given column and for a given s
+getVectsBySampler(keys, sampler)
+Return vector of a given column and for a given sampler name
+getVectsBySamplerAndNearestS(keys, sampler, s)
+Return vector of a given column for a given sampler name and for the closest s
+getVectsBySamplerAndS(keys, sampler, s)
+Return vector of a given column for a given sampler name and for a given s
+sMax()
+Return maximal S value
+sMin()
+Return minimal S value
+pymad8.Sim.setSamplersAndTrack(twissfile, rmatfile, nb_sampl)
+pymad8.Sim.setTrackCollection(nb_part, energy, paramdict)
+pymad8.Sim.testTrack(twissfile, rmatfile)
 
 9.5 pymad8.Track module
 pymad8.Track.MakeObserveFile(elementlist, filename)
 pymad8.Track.MakeTableArchiveFile(elementlist, filename)
 pymad8.Track.MakeTableMapFile(observeElements, observeIndex, filename)
 pymad8.Track.MakeTrackCallingFile(fileNameStub)
 pymad8.Track.MakeTrackFiles(savelineFileName, line, outputFileNameStub)
@@ -843,260 +923,366 @@
 models. Elements selectable via booleans, default to true
 class pymad8.Visualisation.OneDim(survey, debug)
 Bases: object
 plot(colour=True)
 class pymad8.Visualisation.TwoDim(survey, debug=False, annotate=False, fancy=False)
 Bases: object
 plot(event=None)
+
+28
+
+Chapter 9. Module Contents
+
+pymad8 Documentation, Release 2.0.1
+
 plotUpdate(event)
 pymad8.Visualisation.testOneDim()
 pymad8.Visualisation.testTwoDim()
 pymad8.Visualisation.transformedPoly(xy, xyc, theta)
 pymad8.Visualisation.transformedRect(xyc, dx, dy, theta)
 
-9.5. pymad8.Track module
+9.6. pymad8.Visualisation module
 
-27
+29
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
 
-28
+30
 
 Chapter 9. Module Contents
 
 CHAPTER
 
 TEN
 
+VERSION HISTORY
+
+10.1 v2.0.1 - 2023 / 05 / 08
+• Fix missing pandas dependency
+
+31
+
+pymad8 Documentation, Release 2.0.1
+
+32
+
+Chapter 10. Version History
+
+CHAPTER
+
+ELEVEN
+
 INDICES AND TABLES
 
 • genindex
 • modindex
 • search
 
-29
+33
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
 
-30
+34
 
-Chapter 10. Indices and tables
+Chapter 11. Indices and tables
 
 PYTHON MODULE INDEX
 
 p
 pymad8, 21
 pymad8.Input, 22
 pymad8.Output, 22
 pymad8.Plot, 24
 pymad8.Sim, 25
-pymad8.Track, 27
-pymad8.Visualisation, 27
+pymad8.Track, 28
+pymad8.Visualisation, 28
 
-31
+35
 
-pymad8 Documentation, Release 2.0.0
+pymad8 Documentation, Release 2.0.1
 
-32
+36
 
 Python Module Index
 
 INDEX
 
 A
 
-getNamesByTypes()
-(pymad8.Output.Output
+getFirstSamplerByNearestS()
+(pymad8.Sim.Tracking_data
 method),
-23
+27
 AddAllElementsAsSamplers()
-(pygetNamesByValues()
+(pygetIndexByNames()
 (pymad8.Output.Output
 mad8.Sim.Tracking method), 25
 method),
 23
-AddMachineLatticeToFigure() (in module pygetRowByNearestS()
+AddMachineLatticeToFigure() (in module pygetIndexByNearestS()
 (pymad8.Output.Output
 mad8.Plot), 24
 method),
 23
 AddSamplers() (pymad8.Sim.Tracking method), 25
 (pymad8.Output.Output
-AddTrack() (pymad8.Sim.Track_Collection method), getRowsByFunction()
+AddTrack() (pymad8.Sim.Track_Collection method), getIndexByTypes()
 method),
 23
 25
-getRowsByIndex() (pymad8.Output.Output method),
+getIndexByValues()
+(pymad8.Output.Output
 Alpha() (pymad8.Plot.Optics method), 24
-23
-getRowsByNames() (pymad8.Output.Output method),
+method), 23
+getNameByNearestS()
+(pymad8.Output.Output
 B
-23
+method), 23
 Beta() (pymad8.Plot.Optics method), 24
-getRowsByTypes() (pymad8.Output.Output method),
-23
+getNamesByIndex()
+(pymad8.Output.Output
+buildBPMmatrix()
+(pymad8.Sim.Tracking_data
+method), 23
+method), 27
+getNamesByTypes()
+(pymad8.Output.Output
+method), 23
 C
-getRowsByValues()
+getNamesByValues()
 (pymad8.Output.Output
 calcBeamSize() (pymad8.Output.Output method), 22
 method), 23
-CheckUnits() (in module pymad8.Sim), 25
-getTypeByNearestS()
+CalcCorrelChi2()
+(pymad8.Sim.Tracking_data getPlaneCoord() (pymad8.Sim.Tracking method), 26
+method), 27
+getRowByNearestS()
 (pymad8.Output.Output
-Clear() (pymad8.Output.Output method), 22
+CalcResolution()
+(pymad8.Sim.Tracking_data
 method), 23
-getTypesByIndex()
+method), 27
+getRowsByFunction()
 (pymad8.Output.Output
-D
+CheckUnits() (in module pymad8.Sim), 25
 method), 23
+Clear() (pymad8.Output.Output method), 22
+getRowsByIndex() (pymad8.Output.Output method),
+23
+D
+getRowsByNames() (pymad8.Output.Output method),
 decodeFileLine() (in module pymad8.Input), 22
-getTypesByNames()
-(pymad8.Output.Output
+23
 Disp() (pymad8.Plot.Optics method), 24
-method), 24
-getTypesByValues()
-(pymad8.Output.Output
+getRowsByNearestS() (pymad8.Sim.Tracking_data
+method), 27
 G
-method), 24
+getRowsByParticles() (pymad8.Sim.Tracking_data
+method), 27
 GenerateNtracks() (pymad8.Sim.Track_Collection
+getRowsByS() (pymad8.Sim.Tracking_data method),
 method), 25
-L
+27
 GenerateSamplers()
-(pymad8.Sim.Tracking LoadBdsimTrack() (pymad8.Sim.Tracking method),
-method), 26
-26
-getAperture() (pymad8.Output.Output method), 22 LoadMad8Track() (pymad8.Sim.Tracking method), 26
+(pymad8.Sim.Tracking
+getRowsBySamplerAndNearestS()
+(pymethod), 26
+mad8.Sim.Tracking_data method), 27
+getAperture() (pymad8.Output.Output method), 22
+getRowsBySamplerAndS()
+(pygetChi2() (pymad8.Sim.Tracking_data method), 27
+mad8.Sim.Tracking_data method), 27
 getColumnsByKeys()
 (pymad8.Output.Output
+getRowsBySamplers() (pymad8.Sim.Tracking_data
 method), 23
-M
+method), 27
+getColumnsByKeys() (pymad8.Sim.Tracking_data
+getRowsByTypes() (pymad8.Output.Output method),
+method), 27
+23
 getElementByIndex()
 (pymad8.Output.Output
-MakeCombinedSurveyPlot() (in module pymethod), 23
-mad8.Visualisation), 27
-getElementByNames()
+getRowsByValues()
 (pymad8.Output.Output
-MakeObserveFile() (in module pymad8.Track), 27
 method), 23
-MakeTableArchiveFile()
-(in
-module
-pygetIndexByNames()
-(pymad8.Output.Output
-mad8.Track), 27
 method), 23
-MakeTableMapFile() (in module pymad8.Track), 27
-getIndexByNearestS()
-(pymad8.Output.Output
-MakeTrackCallingFile()
-(in
-module
-pymethod), 23
-mad8.Track), 27
-getIndexByTypes()
+getElementByNames()
 (pymad8.Output.Output
-MakeTrackFiles() (in module pymad8.Track), 27
+getRowsByValues()
+(pymad8.Sim.Tracking_data
 method), 23
-module
-getIndexByValues()
+method),
+27
+getElementByNearestS() (pymad8.Output.Output
+getSamplersByNearestS()
+(pymethod), 23
+
+37
+
+pymad8 Documentation, Release 2.0.1
+
+mad8.Sim.Tracking_data method), 27
+getSamplersByS()
+(pymad8.Sim.Tracking_data
+method), 27
+getSByNearestS()
+(pymad8.Sim.Tracking_data
+method), 27
+getSBySamplers()
+(pymad8.Sim.Tracking_data
+method), 27
+getTheoryAndFit() (pymad8.Sim.Tracking method),
+26
+getTypeByNearestS()
 (pymad8.Output.Output
-pymad8, 21
 method), 23
-pymad8.Input, 22
-getNameByNearestS()
+getTypesByIndex()
 (pymad8.Output.Output
-pymad8.Output, 22
 method), 23
-pymad8.Plot, 24
-getNamesByIndex()
+getTypesByNames()
 (pymad8.Output.Output
-pymad8.Sim, 25
-method), 23
-33
+method), 24
+getTypesByValues()
+(pymad8.Output.Output
+method), 24
+getVectsByNearestS() (pymad8.Sim.Tracking_data
+method), 27
+getVectsByParticle() (pymad8.Sim.Tracking_data
+method), 28
+getVectsByS() (pymad8.Sim.Tracking_data method),
+28
+getVectsBySampler() (pymad8.Sim.Tracking_data
+method), 28
+getVectsBySamplerAndNearestS()
+(pymad8.Sim.Tracking_data method), 28
+getVectsBySamplerAndS()
+(pymad8.Sim.Tracking_data method), 28
 
-pymad8 Documentation, Release 2.0.0
+L
+LoadBdsimTrack() (pymad8.Sim.Tracking method),
+26
+LoadMad8Track() (pymad8.Sim.Tracking method), 26
 
-pymad8.Track, 27
-pymad8.Visualisation, 27
-Mu() (pymad8.Plot.Optics method), 24
+M
 
-O
-OneDim (class in pymad8.Visualisation), 27
-Optics (class in pymad8.Plot), 24
 Output (class in pymad8.Output), 22
 
 P
-plot() (pymad8.Visualisation.OneDim method), 27
-plot() (pymad8.Visualisation.TwoDim method), 27
+plot() (pymad8.Visualisation.OneDim method), 28
+plot() (pymad8.Visualisation.TwoDim method), 28
 PlotCorrelation() (pymad8.Sim.Tracking method),
 26
 PlotHist() (pymad8.Sim.Tracking method), 26
 PlotPhaseSpace() (pymad8.Sim.Tracking method),
 26
+PlotRelatTrajectory()
+(pymad8.Sim.Tracking
+method), 26
+PlotRelatTrajSTD()
+(pymad8.Sim.Tracking
+method), 26
 PlotTrajectory() (pymad8.Sim.Tracking method),
 26
 plotUpdate()
 (pymad8.Visualisation.TwoDim
-method), 27
+method), 28
 plotXY() (pymad8.Output.Output method), 24
 pymad8
 module, 21
 pymad8.Input
 module, 22
 pymad8.Output
 module, 22
 pymad8.Plot
 module, 24
 pymad8.Sim
 module, 25
 pymad8.Track
-module, 27
+module, 28
 pymad8.Visualisation
-module, 27
+module, 28
+
+R
+
+removeComments() (in module pymad8.Input), 22
+removeContinuationSymbols()
+(in module pyMakeCombinedSurveyPlot() (in module pymad8.Input),
+22
+mad8.Visualisation), 28
+RunPymad8Tracking()
+(pymad8.Sim.Tracking
+MakeObserveFile() (in module pymad8.Track), 28
+method),
+26
+MakeTableArchiveFile()
+(in
+module
+pymad8.Track), 28
+MakeTableMapFile() (in module pymad8.Track), 28 S
+MakeTrackCallingFile()
+(in
+module
+py- setSamplersAndTrack() (in module pymad8.Sim),
+mad8.Track), 28
+28
+MakeTrackFiles() (in module pymad8.Track), 28
+setTrackCollection() (in module pymad8.Sim), 28
+module
+Sigma() (pymad8.Plot.Optics method), 24
+pymad8, 21
+sMax() (pymad8.Output.Output method), 24
+pymad8.Input, 22
+sMax() (pymad8.Sim.Tracking_data method), 28
+pymad8.Output, 22
+sMin() (pymad8.Output.Output method), 24
+pymad8.Plot, 24
+sMin() (pymad8.Sim.Tracking_data method), 28
+pymad8.Sim, 25
+SortCoeff() (pymad8.Sim.Tracking_data method), 27
+pymad8.Track, 28
+subline() (pymad8.Output.Output method), 24
+pymad8.Visualisation, 28
+SVD() (pymad8.Sim.Tracking_data method), 27
+Mu() (pymad8.Plot.Optics method), 24
+
+O
+OneDim (class in pymad8.Visualisation), 28
+Optics (class in pymad8.Plot), 24
+38
+
+T
+
+testOneDim() (in module pymad8.Visualisation), 29
+testTrack() (in module pymad8.Sim), 28
+testTwoDim() (in module pymad8.Visualisation), 29
+Index
+
+pymad8 Documentation, Release 2.0.1
 
-testTrack() (in module pymad8.Sim), 26
-testTwoDim() (in module pymad8.Visualisation), 27
 tidy() (in module pymad8.Input), 22
 Track_Collection (class in pymad8.Sim), 25
 Tracking (class in pymad8.Sim), 25
+Tracking_data (class in pymad8.Sim), 26
 transformedPoly()
 (in
 module
-pymad8.Visualisation), 27
+mad8.Visualisation), 29
 transformedRect()
 (in
 module
-pymad8.Visualisation), 27
-TwoDim (class in pymad8.Visualisation), 27
+mad8.Visualisation), 29
+TwoDim (class in pymad8.Visualisation), 28
+
+pypy-
 
 W
 WriteBdsimTrack() (pymad8.Sim.Track_Collection
 method), 25
 WriteMad8Track() (pymad8.Sim.Track_Collection
 method), 25
 
-R
-reduceDFbyIndex() (pymad8.Sim.Tracking method),
-26
-removeComments() (in module pymad8.Input), 22
-removeContinuationSymbols() (in module pymad8.Input), 22
-RunPymad8Tracking()
-(pymad8.Sim.Tracking
-method), 26
-
-S
-setSamplersAndTrack() (in module pymad8.Sim),
-26
-setTrackCollection() (in module pymad8.Sim), 26
-Sigma() (pymad8.Plot.Optics method), 24
-sMax() (pymad8.Output.Output method), 24
-sMin() (pymad8.Output.Output method), 24
-subline() (pymad8.Output.Output method), 24
-
-T
-testOneDim() (in module pymad8.Visualisation), 27
-
-34
-
 Index
 
+39
+
```

### Comparing `pymad8-2.0.0/docs/source/conf.py` & `pymad8-2.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/docs/source/convert.rst` & `pymad8-2.0.1/docs/source/convert.rst`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/docs/source/data.rst` & `pymad8-2.0.1/docs/source/data.rst`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/docs/source/figures/betas.png` & `pymad8-2.0.1/docs/source/figures/betas.png`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/docs/source/installation.rst` & `pymad8-2.0.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/docs/source/licence.rst` & `pymad8-2.0.1/docs/source/licence.rst`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/docs/source/moduledocs.rst` & `pymad8-2.0.1/docs/source/moduledocs.rst`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/docs/source/plot.rst` & `pymad8-2.0.1/docs/source/plot.rst`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/docs/source/simulation.rst` & `pymad8-2.0.1/docs/source/simulation.rst`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/docs/source/support.rst` & `pymad8-2.0.1/docs/source/support.rst`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/pyproject.toml` & `pymad8-2.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 authors = [
   {name = "JAI@RHUL", email = "stewart.boogert@rhul.ac.uk"}
 ]
 maintainers = [
   {name = "Stewart Boogert", email = "stewart.boogert@rhul.ac.uk"}
 ]
 dependencies = [
+  "pandas",
   "matplotlib>=3.0",
   "numpy>=1.14",
   "fortranformat",
   "importlib-metadata"
 ]
 
 [project.optional-dependencies]
```

### Comparing `pymad8-2.0.0/src/pymad8/Input.py` & `pymad8-2.0.1/src/pymad8/Input.py`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/src/pymad8/Old/Converter.py` & `pymad8-2.0.1/src/pymad8/Old/Converter.py`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/src/pymad8/Old/Mad8.py` & `pymad8-2.0.1/src/pymad8/Old/Mad8.py`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/src/pymad8/Old/Mad8Converter.py` & `pymad8-2.0.1/src/pymad8/Old/Mad8Converter.py`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/src/pymad8/Old/OutputOld.py` & `pymad8-2.0.1/src/pymad8/Old/OutputOld.py`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/src/pymad8/Old/PlotOld.py` & `pymad8-2.0.1/src/pymad8/Old/PlotOld.py`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/src/pymad8/Old/Saveline.py` & `pymad8-2.0.1/src/pymad8/Old/Saveline.py`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/src/pymad8/Output.py` & `pymad8-2.0.1/src/pymad8/Output.py`

 * *Files 5% similar despite different names*

```diff
@@ -526,20 +526,24 @@
 				return self.data.loc[column.isin(equalValues)]
 			return self.data.loc[column == equalValues]
 		return self.data.loc[column >= minValue].loc[column <= maxValue]
 
 	def getRowByNearestS(self, s):
 		"""Return Rows of the closest element in the beamline"""
 		S = self.data['S'].tolist()
-		for index in range(self.nrec):
-			if S[index - 1] <= s < S[index]:
-				if s - S[index-1] < S[index] - s:
-					return self.data.loc[[index-1]]
+		if s <= S[0]:
+			return self.data.iloc[[0]]
+		if s >= S[-1]:
+			return self.data.iloc[[-1]]
+		for index in range(self.nrec - 1):
+			if S[index] <= s < S[index + 1]:
+				if s - S[index] < S[index + 1] - s:
+					return self.data.iloc[[index]]
 				else:
-					return self.data.loc[[index]]
+					return self.data.iloc[[index + 1]]
 		raise ValueError('Closest s value not found')
 
 	def getRowsByFunction(self, f):
 		"""Return a sub-datafarme using a boolean function"""
 		return self.data.loc[f(self.data)]
 
 	####################################################################################
@@ -566,14 +570,24 @@
 		if type(keylist) != list:
 			keylist = [keylist]
 		elem = self.data.loc[self.data['NAME'].isin(namelist), keylist]
 		if elem.shape == (1, 1):
 			return elem.values[0][0]
 		return elem
 
+	def getElementByNearestS(self, s, keylist):
+		"""Return value of elements at a given s position and for chosen columns"""
+		if type(keylist) != list:
+			keylist = [keylist]
+		row = self.getRowByNearestS(s)
+		elem = row[keylist]
+		if elem.shape == (1, 1):
+			return elem.values[0][0]
+		return elem
+
 	####################################################################################
 	def getAperture(self, index, defaultAperSize=0.1):
 		"""
 		| Get aperture of an element using corresponding index
 		| If none provided or is 0 : set to a default aperture of 0.1m
 		"""
 		name = self.getNamesByIndex(index)
```

### Comparing `pymad8-2.0.0/src/pymad8/Plot.py` & `pymad8-2.0.1/src/pymad8/Plot.py`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/src/pymad8/Track.py` & `pymad8-2.0.1/src/pymad8/Track.py`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/src/pymad8/Visualisation.py` & `pymad8-2.0.1/src/pymad8/Visualisation.py`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/src/pymad8/__init__.py` & `pymad8-2.0.1/src/pymad8/__init__.py`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/src/pymad8.egg-info/PKG-INFO` & `pymad8-2.0.1/src/pymad8.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymad8
-Version: 2.0.0
+Version: 2.0.1
 Summary: Write MAD8 models and load MAD8 output.
 Author-email: "JAI@RHUL" <stewart.boogert@rhul.ac.uk>
 Maintainer-email: Stewart Boogert <stewart.boogert@rhul.ac.uk>
 Project-URL: homepage, http://www.pp.rhul.ac.uk/bdsim/pymad8
 Project-URL: documentation, http://www.pp.rhul.ac.uk/bdsim/pymad8
 Project-URL: repository, https://bitbucket.org/jairhul/pymad8
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,21 +19,23 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
+License-File: COPYING.txt
 
 #pymad8#
 
 ## Authors ##
 
-L. Nevay
+M. Deniaud
 S. Boogert
+L. Nevay
 
 ## Setup ##
 
 From within the pymad8 root directory:
 
 $ make install
```

### Comparing `pymad8-2.0.0/src/pymad8.egg-info/SOURCES.txt` & `pymad8-2.0.1/src/pymad8.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/licence.rst
 docs/source/moduledocs.rst
 docs/source/plot.rst
 docs/source/simulation.rst
 docs/source/support.rst
+docs/source/version_history.rst
 docs/source/figures/betas.png
 src/pymad8/Input.py
 src/pymad8/Output.py
 src/pymad8/Plot.py
 src/pymad8/Sim.py
 src/pymad8/Track.py
 src/pymad8/Visualisation.py
```

### Comparing `pymad8-2.0.0/test/T01_DRIFT.txm` & `pymad8-2.0.1/test/T01_DRIFT.txm`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/test/T02_QUAD.txm` & `pymad8-2.0.1/test/T02_QUAD.txm`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/test/T03_SEXT.txm` & `pymad8-2.0.1/test/T03_SEXT.txm`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/test/T04_OCTU.txm` & `pymad8-2.0.1/test/T04_OCTU.txm`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/test/T05_SBEN.txm` & `pymad8-2.0.1/test/T05_SBEN.txm`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/test/T06_RBEN.txm` & `pymad8-2.0.1/test/T06_RBEN.txm`

 * *Files identical despite different names*

### Comparing `pymad8-2.0.0/test/T07_MULT.txm` & `pymad8-2.0.1/test/T07_MULT.txm`

 * *Files identical despite different names*

