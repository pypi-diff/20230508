# Comparing `tmp/ds4finance-0.1.14.tar.gz` & `tmp/ds4finance-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ds4finance-0.1.14.tar", last modified: Mon May  8 14:09:04 2023, max compression
+gzip compressed data, was "dist\ds4finance-0.1.15.tar", last modified: Mon May  8 14:17:32 2023, max compression
```

## Comparing `ds4finance-0.1.14.tar` & `ds4finance-0.1.15.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 14:09:04.264680 ds4finance-0.1.14/
--rw-rw-rw-   0        0        0     2627 2023-05-08 14:09:04.263680 ds4finance-0.1.14/PKG-INFO
--rw-rw-rw-   0        0        0     1243 2023-04-20 20:51:26.000000 ds4finance-0.1.14/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 14:09:04.244049 ds4finance-0.1.14/ds4finance/
--rw-rw-rw-   0        0        0      963 2023-04-23 19:09:16.000000 ds4finance-0.1.14/ds4finance/__init__.py
--rw-rw-rw-   0        0        0    31358 2023-05-08 14:07:04.000000 ds4finance-0.1.14/ds4finance/functions.py
-drwxrwxrwx   0        0        0        0 2023-05-08 14:09:04.262679 ds4finance-0.1.14/ds4finance.egg-info/
--rw-rw-rw-   0        0        0     2627 2023-05-08 14:09:04.000000 ds4finance-0.1.14/ds4finance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-05-08 14:09:04.000000 ds4finance-0.1.14/ds4finance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 14:09:04.000000 ds4finance-0.1.14/ds4finance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-08 14:09:04.000000 ds4finance-0.1.14/ds4finance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-08 14:09:04.000000 ds4finance-0.1.14/ds4finance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 14:09:04.264680 ds4finance-0.1.14/setup.cfg
--rw-rw-rw-   0        0        0     1174 2023-05-08 14:05:59.000000 ds4finance-0.1.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 14:17:32.784198 ds4finance-0.1.15/
+-rw-rw-rw-   0        0        0     2627 2023-05-08 14:17:32.783197 ds4finance-0.1.15/PKG-INFO
+-rw-rw-rw-   0        0        0     1243 2023-04-20 20:51:26.000000 ds4finance-0.1.15/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 14:17:32.767194 ds4finance-0.1.15/ds4finance/
+-rw-rw-rw-   0        0        0     1021 2023-05-08 14:17:00.000000 ds4finance-0.1.15/ds4finance/__init__.py
+-rw-rw-rw-   0        0        0    31358 2023-05-08 14:07:04.000000 ds4finance-0.1.15/ds4finance/functions.py
+drwxrwxrwx   0        0        0        0 2023-05-08 14:17:32.781197 ds4finance-0.1.15/ds4finance.egg-info/
+-rw-rw-rw-   0        0        0     2627 2023-05-08 14:17:32.000000 ds4finance-0.1.15/ds4finance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-05-08 14:17:32.000000 ds4finance-0.1.15/ds4finance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 14:17:32.000000 ds4finance-0.1.15/ds4finance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-08 14:17:32.000000 ds4finance-0.1.15/ds4finance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-08 14:17:32.000000 ds4finance-0.1.15/ds4finance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 14:17:32.784198 ds4finance-0.1.15/setup.cfg
+-rw-rw-rw-   0        0        0     1174 2023-05-08 14:17:29.000000 ds4finance-0.1.15/setup.py
```

### Comparing `ds4finance-0.1.14/PKG-INFO` & `ds4finance-0.1.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds4finance
-Version: 0.1.14
+Version: 0.1.15
 Summary: A collection of data science tools for finance
 Home-page: https://github.com/LuisSousaSilva/ds4finance
 Author: Luis Silva
 Author-email: luis_paulo_silva@hotmail.com
 License: MIT
 Description: # ds4finance
```

### Comparing `ds4finance-0.1.14/README.md` & `ds4finance-0.1.15/README.md`

 * *Files identical despite different names*

### Comparing `ds4finance-0.1.14/ds4finance/__init__.py` & `ds4finance-0.1.15/ds4finance/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 from .functions import compute_time_period  # noqa: F401
 from .functions import compute_drawdowns_i  # noqa: F401
 from .functions import compute_drawdowns_periods  # noqa: F401
 from .functions import compute_max_drawdown_in_period  # noqa: F401
 from .functions import compute_drawdowns_min  # noqa: F401
 from .functions import compute_drawdowns_table  # noqa: F401
 from .functions import merge_time_series  # noqa: F401
-from .functions import ichart  # noqa: F401
+from .functions import ichart  # noqa: F401
+from .functions import compute_time_series  # noqa: F401
```

### Comparing `ds4finance-0.1.14/ds4finance/functions.py` & `ds4finance-0.1.15/ds4finance/functions.py`

 * *Files identical despite different names*

### Comparing `ds4finance-0.1.14/ds4finance.egg-info/PKG-INFO` & `ds4finance-0.1.15/ds4finance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds4finance
-Version: 0.1.14
+Version: 0.1.15
 Summary: A collection of data science tools for finance
 Home-page: https://github.com/LuisSousaSilva/ds4finance
 Author: Luis Silva
 Author-email: luis_paulo_silva@hotmail.com
 License: MIT
 Description: # ds4finance
```

### Comparing `ds4finance-0.1.14/setup.py` & `ds4finance-0.1.15/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ds4finance",
-    version="0.1.14",
+    version="0.1.15",
     description="A collection of data science tools for finance",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     author="Luis Silva",
     author_email="luis_paulo_silva@hotmail.com",
     url="https://github.com/LuisSousaSilva/ds4finance",
     packages=find_packages(),
```

