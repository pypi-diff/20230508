# Comparing `tmp/gnssanalysis-0.0.8.tar.gz` & `tmp/gnssanalysis-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gnssanalysis-0.0.8.tar", last modified: Tue Oct 11 18:24:25 2022, max compression
+gzip compressed data, was "dist/gnssanalysis-0.0.9.tar", last modified: Tue Oct 11 19:32:15 2022, max compression
```

## Comparing `gnssanalysis-0.0.8.tar` & `gnssanalysis-0.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-11 18:24:25.000000 gnssanalysis-0.0.8/
--rw-r--r--   0 root         (0) root         (0)      244 2022-10-11 18:24:25.000000 gnssanalysis-0.0.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-11 18:24:25.000000 gnssanalysis-0.0.8/gnssanalysis/
--rw-rw-rw-   0 root         (0) root         (0)      146 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6300 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/create_erp_file.py
--rw-rw-rw-   0 root         (0) root         (0)     8315 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_aux.py
--rw-rw-rw-   0 root         (0) root         (0)     8211 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_combi.py
--rw-rw-rw-   0 root         (0) root         (0)     3980 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_const.py
--rw-rw-rw-   0 root         (0) root         (0)     9526 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_datetime.py
--rw-rw-rw-   0 root         (0) root         (0)    23932 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_diffaux.py
--rw-rw-rw-   0 root         (0) root         (0)    26839 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_download.py
--rw-rw-rw-   0 root         (0) root         (0)     8403 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_frame.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-11 18:24:25.000000 gnssanalysis-0.0.8/gnssanalysis/gn_io/
--rw-rw-rw-   0 root         (0) root         (0)      382 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17825 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_io/aux_dicts.py
--rw-rw-rw-   0 root         (0) root         (0)     5228 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_io/clk.py
--rw-rw-rw-   0 root         (0) root         (0)     2469 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_io/common.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_io/discon.py
--rw-rw-rw-   0 root         (0) root         (0)    21394 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_io/igslog.py
--rw-rw-rw-   0 root         (0) root         (0)     2835 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_io/ionex.py
--rw-rw-rw-   0 root         (0) root         (0)      753 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_io/pea.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_io/pod.py
--rw-rw-rw-   0 root         (0) root         (0)      707 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_io/psd.py
--rw-rw-rw-   0 root         (0) root         (0)     3394 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_io/rinex.py
--rw-rw-rw-   0 root         (0) root         (0)    19228 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_io/sinex.py
--rw-rw-rw-   0 root         (0) root         (0)    13602 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_io/sp3.py
--rw-rw-rw-   0 root         (0) root         (0)      700 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_io/stec.py
--rw-rw-rw-   0 root         (0) root         (0)     8553 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_io/trace.py
--rw-rw-rw-   0 root         (0) root         (0)     1889 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_io/trop.py
--rw-rw-rw-   0 root         (0) root         (0)     5895 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_plot.py
--rw-rw-rw-   0 root         (0) root         (0)     8557 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_transform.py
--rw-rw-rw-   0 root         (0) root         (0)    12710 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/gnssanalysis/gn_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-11 18:24:25.000000 gnssanalysis-0.0.8/gnssanalysis.egg-info/
--rw-r--r--   0 root         (0) root         (0)      244 2022-10-11 18:24:25.000000 gnssanalysis-0.0.8/gnssanalysis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      988 2022-10-11 18:24:25.000000 gnssanalysis-0.0.8/gnssanalysis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-11 18:24:25.000000 gnssanalysis-0.0.8/gnssanalysis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      229 2022-10-11 18:24:25.000000 gnssanalysis-0.0.8/gnssanalysis.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       88 2022-10-11 18:24:25.000000 gnssanalysis-0.0.8/gnssanalysis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-10-11 18:24:25.000000 gnssanalysis-0.0.8/gnssanalysis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-11 18:24:25.000000 gnssanalysis-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      872 2022-10-11 18:24:09.000000 gnssanalysis-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)      244 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/gnssanalysis/
+-rw-rw-rw-   0 root         (0) root         (0)      146 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6300 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/create_erp_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     8315 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_aux.py
+-rw-rw-rw-   0 root         (0) root         (0)     8211 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_combi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3980 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_const.py
+-rw-rw-rw-   0 root         (0) root         (0)     9526 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_datetime.py
+-rw-rw-rw-   0 root         (0) root         (0)    23938 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_diffaux.py
+-rw-rw-rw-   0 root         (0) root         (0)    26839 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_download.py
+-rw-rw-rw-   0 root         (0) root         (0)     8403 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_frame.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17825 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/aux_dicts.py
+-rw-rw-rw-   0 root         (0) root         (0)     5228 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/clk.py
+-rw-rw-rw-   0 root         (0) root         (0)     2469 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/discon.py
+-rw-rw-rw-   0 root         (0) root         (0)    21394 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/igslog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2835 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/ionex.py
+-rw-rw-rw-   0 root         (0) root         (0)      753 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/pea.py
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/pod.py
+-rw-rw-rw-   0 root         (0) root         (0)      707 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/psd.py
+-rw-rw-rw-   0 root         (0) root         (0)     3394 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/rinex.py
+-rw-rw-rw-   0 root         (0) root         (0)    19228 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/sinex.py
+-rw-rw-rw-   0 root         (0) root         (0)    13602 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/sp3.py
+-rw-rw-rw-   0 root         (0) root         (0)      700 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/stec.py
+-rw-rw-rw-   0 root         (0) root         (0)     8553 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/trace.py
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/trop.py
+-rw-rw-rw-   0 root         (0) root         (0)     5895 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     8557 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_transform.py
+-rw-rw-rw-   0 root         (0) root         (0)    12710 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/gnssanalysis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      244 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/gnssanalysis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      988 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/gnssanalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/gnssanalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      229 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/gnssanalysis.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/gnssanalysis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/gnssanalysis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      872 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/setup.py
```

### Comparing `gnssanalysis-0.0.8/gnssanalysis/create_erp_file.py` & `gnssanalysis-0.0.9/gnssanalysis/create_erp_file.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_aux.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_aux.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_combi.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_combi.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_const.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_const.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_datetime.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_datetime.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_diffaux.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_diffaux.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
     return 0
 
 def _compare_nonsat_postfit_residuals(diffstd,log_lvl,tol=None):
     diff_count = diffstd[~diffstd.attrs['SAT_MASK']]
     if diff_count.empty: #no non-sat records found such as Zamb
         _logging.warning(f':diffutil non-SVs residuals not present. Skipping')
         return 0
-    diff_count =  diff_count.droplevel('SAT').unstack(['SITE','TYPE','BLK'])
+    diff_count =  diff_count.droplevel('SAT').unstack(['TYPE','NUM','SITE','BLK'])
     bad_nonsv_residuals = _diff2msg(diff_count,tol=tol)
     if bad_nonsv_residuals is not None:
         _logging.log(msg=f':diffutil found non-SVs residuals diffs above {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}:\n{bad_nonsv_residuals.to_string(justify="center")}\n',level=log_lvl)
         return -1
     _logging.log(msg=f':diffutil [OK] non-SVs residuals diffs within the {"extracted STDs" if tol is None else f"{tol:.1E} tolerance"}',level=_logging.INFO)
     return 0
```

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_download.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_download.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_frame.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_frame.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_io/aux_dicts.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_io/aux_dicts.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_io/clk.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_io/clk.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_io/common.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_io/common.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_io/discon.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_io/discon.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_io/igslog.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_io/igslog.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_io/ionex.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_io/ionex.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_io/pea.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_io/pea.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_io/pod.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_io/pod.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_io/psd.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_io/psd.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_io/rinex.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_io/rinex.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_io/sinex.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_io/sinex.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_io/sp3.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_io/sp3.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_io/stec.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_io/stec.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_io/trace.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_io/trace.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_io/trop.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_io/trop.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_plot.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_plot.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_transform.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_transform.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis/gn_utils.py` & `gnssanalysis-0.0.9/gnssanalysis/gn_utils.py`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/gnssanalysis.egg-info/SOURCES.txt` & `gnssanalysis-0.0.9/gnssanalysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gnssanalysis-0.0.8/setup.py` & `gnssanalysis-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     include_package_data=True,
     name="gnssanalysis",
-    version="0.0.8",
+    version="0.0.9",
     description="basic python module for gnss analysis",
     author="Geoscience Australia",
     author_email="GNSSAnalysis@ga.gov.au",
     packages=setuptools.find_packages(),
     install_requires=[
         "boto3",
         "click",
```

