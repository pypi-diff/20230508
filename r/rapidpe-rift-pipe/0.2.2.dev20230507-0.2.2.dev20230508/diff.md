# Comparing `tmp/rapidpe_rift_pipe-0.2.2.dev20230507.tar.gz` & `tmp/rapidpe_rift_pipe-0.2.2.dev20230508.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpe_rift_pipe-0.2.2.dev20230507.tar", last modified: Sun May  7 05:17:03 2023, max compression
+gzip compressed data, was "rapidpe_rift_pipe-0.2.2.dev20230508.tar", last modified: Mon May  8 05:16:11 2023, max compression
```

## Comparing `rapidpe_rift_pipe-0.2.2.dev20230507.tar` & `rapidpe_rift_pipe-0.2.2.dev20230508.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 05:17:03.659295 rapidpe_rift_pipe-0.2.2.dev20230507/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1140 2023-05-07 05:17:03.659295 rapidpe_rift_pipe-0.2.2.dev20230507/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 05:17:03.649295 rapidpe_rift_pipe-0.2.2.dev20230507/bin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 05:17:03.652295 rapidpe_rift_pipe-0.2.2.dev20230507/bin/postscripts/
--rw-rw-rw-   0 root         (0) root         (0)    10021 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/bin/postscripts/compute_posterior.py
--rwxrwxrwx   0 root         (0) root         (0)    12423 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/bin/postscripts/convert_result_to_txt.py
--rw-rw-rw-   0 root         (0) root         (0)     6342 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/bin/postscripts/cprofile_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     5579 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/bin/postscripts/create_summarypage.py
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/bin/postscripts/plot_skymap.py
--rw-rw-rw-   0 root         (0) root         (0)     1449 2023-05-07 05:17:03.660295 rapidpe_rift_pipe-0.2.2.dev20230507/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 05:17:03.649295 rapidpe_rift_pipe-0.2.2.dev20230507/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 05:17:03.655295 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    37457 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    18297 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 05:17:03.658295 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/config_files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/config_files/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 05:17:03.658295 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4536 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
--rwxrwxrwx   0 root         (0) root         (0)    31226 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/jacobians.py
--rw-rw-rw-   0 root         (0) root         (0)     9701 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/pastro.py
--rw-rw-rw-   0 root         (0) root         (0)    24280 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/postscript_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/search_bias_bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 05:17:03.659295 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/static/stylesheet.css
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/test_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-05-07 05:16:45.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 05:17:03.657295 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1140 2023-05-07 05:17:03.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1317 2023-05-07 05:17:03.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 05:17:03.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-07 05:17:03.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       96 2023-05-07 05:17:03.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-07 05:17:03.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 05:17:03.000000 rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 05:16:11.671593 rapidpe_rift_pipe-0.2.2.dev20230508/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-05-08 05:16:11.671593 rapidpe_rift_pipe-0.2.2.dev20230508/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 05:16:11.664593 rapidpe_rift_pipe-0.2.2.dev20230508/bin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 05:16:11.666593 rapidpe_rift_pipe-0.2.2.dev20230508/bin/postscripts/
+-rw-rw-rw-   0 root         (0) root         (0)    10021 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/bin/postscripts/compute_posterior.py
+-rwxrwxrwx   0 root         (0) root         (0)    12423 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/bin/postscripts/convert_result_to_txt.py
+-rw-rw-rw-   0 root         (0) root         (0)     6342 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/bin/postscripts/cprofile_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     5579 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/bin/postscripts/create_summarypage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/bin/postscripts/plot_skymap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1449 2023-05-08 05:16:11.672593 rapidpe_rift_pipe-0.2.2.dev20230508/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 05:16:11.664593 rapidpe_rift_pipe-0.2.2.dev20230508/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 05:16:11.669593 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    37457 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    18297 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 05:16:11.670593 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/config_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/config_files/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 05:16:11.670593 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4536 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
+-rwxrwxrwx   0 root         (0) root         (0)    31226 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/jacobians.py
+-rw-rw-rw-   0 root         (0) root         (0)     9701 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/pastro.py
+-rw-rw-rw-   0 root         (0) root         (0)    24280 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/postscript_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/search_bias_bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 05:16:11.671593 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/static/stylesheet.css
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/test_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-05-08 05:15:52.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 05:16:11.670593 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-05-08 05:16:11.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-05-08 05:16:11.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 05:16:11.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-08 05:16:11.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-05-08 05:16:11.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-08 05:16:11.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 05:16:11.000000 rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe.egg-info/zip-safe
```

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/COPYING` & `rapidpe_rift_pipe-0.2.2.dev20230508/COPYING`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/PKG-INFO` & `rapidpe_rift_pipe-0.2.2.dev20230508/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe_rift_pipe
-Version: 0.2.2.dev20230507
+Version: 0.2.2.dev20230508
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/bin/postscripts/compute_posterior.py` & `rapidpe_rift_pipe-0.2.2.dev20230508/bin/postscripts/compute_posterior.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/bin/postscripts/convert_result_to_txt.py` & `rapidpe_rift_pipe-0.2.2.dev20230508/bin/postscripts/convert_result_to_txt.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/bin/postscripts/cprofile_summary.py` & `rapidpe_rift_pipe-0.2.2.dev20230508/bin/postscripts/cprofile_summary.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/bin/postscripts/create_summarypage.py` & `rapidpe_rift_pipe-0.2.2.dev20230508/bin/postscripts/create_summarypage.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/bin/postscripts/plot_skymap.py` & `rapidpe_rift_pipe-0.2.2.dev20230508/bin/postscripts/plot_skymap.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/setup.cfg` & `rapidpe_rift_pipe-0.2.2.dev20230508/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -49,10 +49,10 @@
 rapidpe_rift_pipe.config_files = *.ini, *.json
 
 [options.entry_points]
 console_scripts = 
 	rapidpe-rift-pipe = rapidpe_rift_pipe.cli:main
 
 [egg_info]
-tag_build = dev.20230507
+tag_build = dev.20230508
 tag_date = 0
```

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/cli.py` & `rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/cli.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/config.py` & `rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json` & `rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/create_submit_dag_one_event.py` & `rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/create_submit_dag_one_event.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/jacobians.py` & `rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/jacobians.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/modules.py` & `rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/modules.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/pastro.py` & `rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/pastro.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/postscript_utils.py` & `rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/postscript_utils.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/profiling.py` & `rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/profiling.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/search_bias_bounds.py` & `rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/search_bias_bounds.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/static/stylesheet.css` & `rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/static/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe/test_config.py` & `rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe/test_config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe.egg-info/PKG-INFO` & `rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe-rift-pipe
-Version: 0.2.2.dev20230507
+Version: 0.2.2.dev20230508
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.2.2.dev20230507/src/rapidpe_rift_pipe.egg-info/SOURCES.txt` & `rapidpe_rift_pipe-0.2.2.dev20230508/src/rapidpe_rift_pipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

