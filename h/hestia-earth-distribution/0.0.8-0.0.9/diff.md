# Comparing `tmp/hestia-earth-distribution-0.0.8.tar.gz` & `tmp/hestia-earth-distribution-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hestia-earth-distribution-0.0.8.tar", last modified: Sat Jan 28 06:28:04 2023, max compression
+gzip compressed data, was "hestia-earth-distribution-0.0.9.tar", last modified: Fri Feb 10 10:27:03 2023, max compression
```

## Comparing `hestia-earth-distribution-0.0.8.tar` & `hestia-earth-distribution-0.0.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 06:28:04.657721 hestia-earth-distribution-0.0.8/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3889 2023-01-28 06:28:04.657721 hestia-earth-distribution-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3402 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 06:28:04.644728 hestia-earth-distribution-0.0.8/hestia_earth/
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/hestia_earth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 06:28:04.647726 hestia-earth-distribution-0.0.8/hestia_earth/distribution/
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/hestia_earth/distribution/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1686 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/hestia_earth/distribution/cycle.py
--rw-rw-rw-   0 root         (0) root         (0)     2522 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/hestia_earth/distribution/likelihood.py
--rw-rw-rw-   0 root         (0) root         (0)     1166 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/hestia_earth/distribution/log.py
--rw-rw-rw-   0 root         (0) root         (0)     2929 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/hestia_earth/distribution/posterior_fert.py
--rw-rw-rw-   0 root         (0) root         (0)     2749 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/hestia_earth/distribution/posterior_yield.py
--rw-rw-rw-   0 root         (0) root         (0)     3677 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/hestia_earth/distribution/prior_fert.py
--rw-rw-rw-   0 root         (0) root         (0)     3606 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/hestia_earth/distribution/prior_yield.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 06:28:04.649725 hestia-earth-distribution-0.0.8/hestia_earth/distribution/utils/
--rw-rw-rw-   0 root         (0) root         (0)      763 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/hestia_earth/distribution/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1757 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/hestia_earth/distribution/utils/cycle.py
--rw-rw-rw-   0 root         (0) root         (0)     6495 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/hestia_earth/distribution/utils/fao.py
--rw-rw-rw-   0 root         (0) root         (0)     5619 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/hestia_earth/distribution/utils/posterior.py
--rw-rw-rw-   0 root         (0) root         (0)     2814 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/hestia_earth/distribution/utils/priors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 06:28:04.651724 hestia-earth-distribution-0.0.8/hestia_earth/distribution/utils/storage/
--rw-rw-rw-   0 root         (0) root         (0)     1469 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/hestia_earth/distribution/utils/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      499 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/hestia_earth/distribution/utils/storage/_azure_client.py
--rw-rw-rw-   0 root         (0) root         (0)      613 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/hestia_earth/distribution/utils/storage/_local_client.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/hestia_earth/distribution/utils/storage/_s3_client.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/hestia_earth/distribution/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 06:28:04.653723 hestia-earth-distribution-0.0.8/hestia_earth_distribution.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3889 2023-01-28 06:28:04.000000 hestia-earth-distribution-0.0.8/hestia_earth_distribution.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1524 2023-01-28 06:28:04.000000 hestia-earth-distribution-0.0.8/hestia_earth_distribution.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-28 06:28:04.000000 hestia-earth-distribution-0.0.8/hestia_earth_distribution.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       96 2023-01-28 06:28:04.000000 hestia-earth-distribution-0.0.8/hestia_earth_distribution.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-01-28 06:28:04.000000 hestia-earth-distribution-0.0.8/hestia_earth_distribution.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-01-28 06:28:04.658720 hestia-earth-distribution-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 06:28:04.641730 hestia-earth-distribution-0.0.8/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 06:28:04.655722 hestia-earth-distribution-0.0.8/tests/distribution/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/tests/distribution/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/tests/distribution/test_cycle.py
--rw-rw-rw-   0 root         (0) root         (0)     1354 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/tests/distribution/test_likelihood.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/tests/distribution/test_posterior_fert.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/tests/distribution/test_posterior_yield.py
--rw-rw-rw-   0 root         (0) root         (0)     1486 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/tests/distribution/test_prior_fert.py
--rw-rw-rw-   0 root         (0) root         (0)     1523 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/tests/distribution/test_prior_yield.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 06:28:04.657721 hestia-earth-distribution-0.0.8/tests/distribution/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/tests/distribution/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/tests/distribution/utils/test_cycle.py
--rw-rw-rw-   0 root         (0) root         (0)     6896 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/tests/distribution/utils/test_posterior.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2023-01-28 06:27:28.000000 hestia-earth-distribution-0.0.8/tests/distribution/utils/test_priors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 10:27:03.636716 hestia-earth-distribution-0.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-02-10 10:27:03.636716 hestia-earth-distribution-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 10:27:03.622714 hestia-earth-distribution-0.0.9/hestia_earth/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/hestia_earth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 10:27:03.626715 hestia-earth-distribution-0.0.9/hestia_earth/distribution/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/hestia_earth/distribution/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/hestia_earth/distribution/cycle.py
+-rw-rw-rw-   0 root         (0) root         (0)     2332 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/hestia_earth/distribution/likelihood.py
+-rw-rw-rw-   0 root         (0) root         (0)     1166 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/hestia_earth/distribution/log.py
+-rw-rw-rw-   0 root         (0) root         (0)     3239 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/hestia_earth/distribution/posterior_fert.py
+-rw-rw-rw-   0 root         (0) root         (0)     2759 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/hestia_earth/distribution/posterior_yield.py
+-rw-rw-rw-   0 root         (0) root         (0)     3618 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/hestia_earth/distribution/prior_fert.py
+-rw-rw-rw-   0 root         (0) root         (0)     3581 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/hestia_earth/distribution/prior_yield.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 10:27:03.628715 hestia-earth-distribution-0.0.9/hestia_earth/distribution/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      763 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/hestia_earth/distribution/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2375 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/hestia_earth/distribution/utils/cycle.py
+-rw-rw-rw-   0 root         (0) root         (0)     5814 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/hestia_earth/distribution/utils/fao.py
+-rw-rw-rw-   0 root         (0) root         (0)     7474 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/hestia_earth/distribution/utils/posterior.py
+-rw-rw-rw-   0 root         (0) root         (0)     2834 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/hestia_earth/distribution/utils/priors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 10:27:03.629715 hestia-earth-distribution-0.0.9/hestia_earth/distribution/utils/storage/
+-rw-rw-rw-   0 root         (0) root         (0)     1469 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/hestia_earth/distribution/utils/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/hestia_earth/distribution/utils/storage/_azure_client.py
+-rw-rw-rw-   0 root         (0) root         (0)      613 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/hestia_earth/distribution/utils/storage/_local_client.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/hestia_earth/distribution/utils/storage/_s3_client.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/hestia_earth/distribution/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 10:27:03.631715 hestia-earth-distribution-0.0.9/hestia_earth_distribution.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-02-10 10:27:03.000000 hestia-earth-distribution-0.0.9/hestia_earth_distribution.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1524 2023-02-10 10:27:03.000000 hestia-earth-distribution-0.0.9/hestia_earth_distribution.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-10 10:27:03.000000 hestia-earth-distribution-0.0.9/hestia_earth_distribution.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-02-10 10:27:03.000000 hestia-earth-distribution-0.0.9/hestia_earth_distribution.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-02-10 10:27:03.000000 hestia-earth-distribution-0.0.9/hestia_earth_distribution.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-02-10 10:27:03.637716 hestia-earth-distribution-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 10:27:03.619714 hestia-earth-distribution-0.0.9/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 10:27:03.634715 hestia-earth-distribution-0.0.9/tests/distribution/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/tests/distribution/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1205 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/tests/distribution/test_cycle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/tests/distribution/test_likelihood.py
+-rw-rw-rw-   0 root         (0) root         (0)      850 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/tests/distribution/test_posterior_fert.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/tests/distribution/test_posterior_yield.py
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/tests/distribution/test_prior_fert.py
+-rw-rw-rw-   0 root         (0) root         (0)     1528 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/tests/distribution/test_prior_yield.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 10:27:03.636716 hestia-earth-distribution-0.0.9/tests/distribution/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/tests/distribution/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/tests/distribution/utils/test_cycle.py
+-rw-rw-rw-   0 root         (0) root         (0)     7507 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/tests/distribution/utils/test_posterior.py
+-rw-rw-rw-   0 root         (0) root         (0)      818 2023-02-10 10:26:22.000000 hestia-earth-distribution-0.0.9/tests/distribution/utils/test_priors.py
```

### Comparing `hestia-earth-distribution-0.0.8/PKG-INFO` & `hestia-earth-distribution-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: hestia-earth-distribution
-Version: 0.0.8
+Version: 0.0.9
 Summary: Hestia's Distribution library
 Home-page: https://gitlab.com/hestia-earth/hestia-distribution
 Author: Hestia Team
 Author-email: guillaume@hestia.earth
-License: GPL-3.0-or-later
+License: MIT
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: stats
 License-File: LICENSE
```

### Comparing `hestia-earth-distribution-0.0.8/README.md` & `hestia-earth-distribution-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hestia-earth-distribution-0.0.8/hestia_earth/distribution/cycle.py` & `hestia-earth-distribution-0.0.9/hestia_earth/distribution/cycle.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from hestia_earth.utils.tools import list_sum, list_average, flatten
 
 INDEX_COLUMN = 'cycle.id'
 YIELD_COLUMN = 'Grain yield (kg/ha)'
 FERTILISER_COLUMNS = [
     'Nitrogen (kg N)',
     'Phosphorus (kg P2O5)',
-    'Potash (kg K2O)',
+    'Potassium (kg K2O)',
     'Magnesium (kg Mg)'
     # 'Sulphur (kg S)'
 ]
 FERTILISER_TERM_TYPES = [
     TermTermType.ORGANICFERTILISER.value,
     TermTermType.INORGANICFERTILISER.value
 ]
@@ -40,14 +40,17 @@
             list_sum(i.get('value', []), 0) > 0
         ])
     ]
     fertilisers_values = reduce(_group_inputs(fertilisers), FERTILISER_COLUMNS, {})
     return {
         INDEX_COLUMN: cycle.get('@id'),
         YIELD_COLUMN: list_average((find_primary_product(cycle) or {}).get('value', []), 0),
-        **fertilisers_values
+        **fertilisers_values,
+        'completeness.fertiliser': cycle.get('completeness', {}).get('fertiliser', False)
     }
 
 
 def cycle_yield_distribution(cycles: list):
     values = list(map(group_cycle_inputs, cycles))
-    return pd.DataFrame.from_records(values, index=[INDEX_COLUMN])
+    # in case there are no values, we should still set the columns
+    columns = group_cycle_inputs({}).keys()
+    return pd.DataFrame.from_records(values, index=[INDEX_COLUMN], columns=columns)
```

### Comparing `hestia-earth-distribution-0.0.8/hestia_earth/distribution/likelihood.py` & `hestia-earth-distribution-0.0.9/hestia_earth/distribution/likelihood.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from io import BytesIO
 import pandas as pd
-from hestia_earth.utils.api import download_hestia
 from hestia_earth.schema import TermTermType
 
 from .utils import df_to_csv_buffer
 from .utils.storage import file_exists, load_from_storage, write_to_storage
 from .utils.cycle import find_cycles
 from .cycle import INDEX_COLUMN, cycle_yield_distribution
 
@@ -14,49 +13,48 @@
     TermTermType.INORGANICFERTILISER.value: 'inputs',
     TermTermType.ORGANICFERTILISER.value: 'inputs'
 }
 
 
 def _read_likl_file(likl_filename: str):
     data = load_from_storage(likl_filename)
-    return pd.read_csv(BytesIO(data)).set_index(INDEX_COLUMN)
+    df = pd.read_csv(BytesIO(data))
+    return df.set_index(INDEX_COLUMN) if not df.empty else df
 
 
-def _generate_likl_file(country_id: str, term_id: str, filepath: str, limit: int):
-    term_type = download_hestia(term_id).get('termType')
-    cycles = find_cycles(country_id, term_id, TERM_TYPE_TO_KEY.get(term_type), limit=limit)
+def _generate_likl_file(country_id: str, product_id: str, filepath: str, limit: int):
+    cycles = find_cycles(country_id, product_id, limit=limit)
     df = cycle_yield_distribution(cycles)
     # skip writing when the file exists and the data will not be updated
     should_write_to_storage = not file_exists(filepath) or len(cycles) > 0
     write_to_storage(filepath, df_to_csv_buffer(df)) if should_write_to_storage else None
     return df
 
 
 def likl_filename(country_id: str, product_id: str): return f'{country_id}_{product_id}_non-aggregated_cycles.csv'
 
 
-def generate_likl_file(country_id: str, term_id: str, limit: int = 10000, overwrite=False):
+def generate_likl_file(country_id: str, product_id: str, limit: int = 10000, overwrite=False):
     """
     Return all likelihood data for a given country and a given product.
     If likelihood file exisits, data will be read in; otherwise, generate likelihood data and store
     into likl_filename path.
 
     Parameters
     ----------
     country_id: str
-        Region `@id` from Hestia glossary, e.g. 'GADM-GBR', or 'region-south-america'.
-    term_id: str
-        Term `@id` from Hestia glossary,  can be any product, fertiliser, or pesticide, etc.
-        e.g. 'wheatGrain' as a crop product ID, or 'ammoniumNitrateKgN' as a fertiliser term ID
+        Country `@id` from Hestia glossary, e.g. 'GADM-GBR' (regions not supported yet).
+    product_id: str
+        Product `@id` from Hestia glossary, e.g. 'wheatGrain' as a crop product ID.
     limit: int
         Max number of Cycles to compute likelihood data. Defaults to `10000`.
     overwrite: bool
         Whether to overwrite existing likelihood file or not. Defaults to `False`.
 
     Returns
     -------
     pd.DataFrame
         A dataframe storing the likelihood data.
     """
-    filepath = f"{FOLDER}/{likl_filename(country_id, term_id)}"
+    filepath = f"{FOLDER}/{likl_filename(country_id, product_id)}"
     read_existing = file_exists(filepath) and not overwrite
-    return _read_likl_file(filepath) if read_existing else _generate_likl_file(country_id, term_id, filepath, limit)
+    return _read_likl_file(filepath) if read_existing else _generate_likl_file(country_id, product_id, filepath, limit)
```

### Comparing `hestia-earth-distribution-0.0.8/hestia_earth/distribution/log.py` & `hestia-earth-distribution-0.0.9/hestia_earth/distribution/log.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-distribution-0.0.8/hestia_earth/distribution/posterior_fert.py` & `hestia-earth-distribution-0.0.9/hestia_earth/distribution/posterior_fert.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 import pandas as pd
 
-from .utils.fao import get_fert_group_id
+from .utils.cycle import get_fert_group_id, get_input_ids
 from .utils.posterior import update_all_post_data, get_post_data, get_post_ensemble_data
 from .prior_fert import generate_prior_fert_file
 
-POSTERIOR_FERT_FILENAME = 'posterior_fert_use.csv'
+POSTERIOR_FERT_FILENAME = 'posterior_crop_fert.csv'
 
 
-def get_post_ensemble(country_id: str, input_id: str, overwrite=False, df_prior: pd.DataFrame = None):
+def get_post_ensemble(country_id: str, product_id: str, input_id: str, overwrite=False, df_prior: pd.DataFrame = None):
     """
-    Return posterior data for a given country and a given product.
+    Return posterior data for a given country, a given product and a given input.
     If posterior file exisits, data will be read in; otherwise, generate posterior data and store
     into a pickle or json file.
 
     Parameters
     ----------
     country_id: str
         Region `@id` from Hestia glossary, e.g. 'GADM-GBR', or 'region-south-america'.
+    product_id: str
+        Product term `@id` from Hestia glossary, e.g. 'wheatGrain'.
     input_id: str
         Fertiliser term `@id` from Hestia glossary, e.g. 'ammoniumNitrateKgN', or
         'inorganicNitrogenFertiliserUnspecifiedKgN'.
     overwrite: bool
         Whether to overwrite existing posterior file or not. Defaults to `False`.
     df_prior: pd.DataFrame
         Optional - if prior file is already loaded, pass it here.
 
     Returns
     -------
     tuple(mu, sd)
         List of float storing the posterior mu and sd ensembles.
     """
     fert_id = get_fert_group_id(input_id)
-    return get_post_ensemble_data(country_id, fert_id,
+    return get_post_ensemble_data(country_id, product_id, fert_id,
                                   overwrite=overwrite, df_prior=df_prior, generate_prior=generate_prior_fert_file)
 
 
 def update_all_post(rows: list = None, cols: list = None, overwrite=True):
     """
     Update crop posterior data for all countries and all products.
     It creates or re-write json files to store posterior data for each country and each product.
@@ -52,30 +54,33 @@
 
     Returns
     -------
     DataFrame
         A DataFrame storing all posterior data.
     """
     df_prior = generate_prior_fert_file()
-    return update_all_post_data(df_prior, POSTERIOR_FERT_FILENAME, rows, cols, overwrite)
+    term_ids = get_input_ids()
+    return update_all_post_data(df_prior, POSTERIOR_FERT_FILENAME, rows, cols, term_ids, overwrite)
 
 
-def get_post(country_id: str, input_id: str):
+def get_post(country_id: str, product_id: str, input_id: str):
     """
     Return posterior data for a given country and a given product.
     Data is read from the file containing all posterior data.
     Cannot use this function to generate new post files.
 
     Parameters
     ----------
     country_id: str
         Region `@id` from Hestia glossary, e.g. 'GADM-GBR', or 'region-south-america'.
+    product_id: str
+        Product term `@id` from Hestia glossary, e.g. 'wheatGrain'.
     input_id: str
         Fertiliser term `@id` from Hestia glossary, e.g. 'ammoniumNitrateKgN'.
 
     Returns
     -------
     tuple(mu, sd)
         Mean values of mu and sd.
     """
     fert_id = get_fert_group_id(input_id)
-    return get_post_data(country_id, fert_id, POSTERIOR_FERT_FILENAME)
+    return get_post_data(country_id, (product_id, fert_id), POSTERIOR_FERT_FILENAME)
```

### Comparing `hestia-earth-distribution-0.0.8/hestia_earth/distribution/posterior_yield.py` & `hestia-earth-distribution-0.0.9/hestia_earth/distribution/posterior_yield.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     Returns
     -------
     DataFrame
         A DataFrame storing all posterior data.
     """
     df_prior = generate_prior_yield_file()
-    return update_all_post_data(df_prior, POSTERIOR_YIELD_FILENAME, rows, cols, overwrite)
+    return update_all_post_data(df_prior, POSTERIOR_YIELD_FILENAME, rows, cols, overwrite=overwrite)
 
 
 def get_post(country_id: str, product_id: str):
     """
     Return posterior data for a given country and a given product.
     Data is read from the file containing all posterior data.
     Cannot use this function to generate new post files.
```

### Comparing `hestia-earth-distribution-0.0.8/hestia_earth/distribution/prior_fert.py` & `hestia-earth-distribution-0.0.9/hestia_earth/distribution/prior_fert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import pandas as pd
 from hestia_earth.utils.lookup import download_lookup
 
 from .log import logger
 from .utils import SIGMA_SCALER, get_stats_from_df
 from .utils.storage import file_exists
-from .utils.fao import (
-    LOOKUP_FERTUSE, FERT_GROUPS, get_fao_fertuse, get_mean_std_per_country_per_product, get_fert_group_id
-)
-from .utils.priors import read_prior_stats, generate_and_save_priors
+from .utils.fao import LOOKUP_FERTUSE, get_fao_fertuse, get_mean_std_per_country_per_product
+from .utils.cycle import get_fert_group_id, get_input_ids
+from .utils.priors import FOLDER, read_prior_stats, generate_and_save_priors
 
-FOLDER = 'prior_files'
 PRIOR_FERT_FILENAME = 'FAO_Fert_prior_per_input_per_country.csv'
 
 
 def get_fao_fert(country_id: str, input_id: str, n_years: int = 10):
     """
     Look up the FAO yield per country per product from the glossary.
 
@@ -47,18 +45,17 @@
     Returns
     -------
     pd.DataFrame
         A dataframe of all prior information (mu, sigma_of_mu, and n_years, sigma).
     """
     fert_lookup = download_lookup(LOOKUP_FERTUSE)
     countries = pd.Series(fert_lookup['termid']).drop_duplicates()
-    df_stats = pd.DataFrame(columns=countries, index=FERT_GROUPS.values())[:n_rows]
+    df_stats = pd.DataFrame(columns=countries, index=get_input_ids())[:n_rows]
 
-    for fert_id in FERT_GROUPS.values():
-        # fert_group = get_fert_group_name(fert_id)
+    for fert_id in get_input_ids():
         logger.info(f'Processing {fert_id}...')
         for gadm_code in fert_lookup['termid']:
             stats = get_mean_std_per_country_per_product(fert_id, gadm_code, get_fao_fertuse)
             if None not in stats:
                 df_stats.loc[fert_id, gadm_code] = stats[0], stats[1]*SIGMA_SCALER, stats[2], stats[1]
 
     df_stats.index.rename('term.id', inplace=True)
```

### Comparing `hestia-earth-distribution-0.0.8/hestia_earth/distribution/prior_yield.py` & `hestia-earth-distribution-0.0.9/hestia_earth/distribution/prior_yield.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 import numpy as np
 from hestia_earth.utils.lookup import download_lookup
 
 from .log import logger
 from .utils import SIGMA_SCALER, get_stats_from_df
 from .utils.storage import file_exists
 from .utils.fao import LOOKUP_YIELD, get_fao_yield, create_df_fao, get_mean_std_per_country_per_product
-from .utils.priors import read_prior_stats, generate_and_save_priors
+from .utils.priors import FOLDER, read_prior_stats, generate_and_save_priors
 
-FOLDER = 'prior_files'
 PRIOR_YIELD_FILENAME = 'FAO_Yield_prior_per_product_per_country.csv'
 
 
 def calculate_worldwide_mean_sigma(product_id: str):
     """
     Calculate the means and sigmas for worldwide means and standard deviations of FAO yield for a specific product.
 
@@ -36,20 +35,20 @@
             world_sigmas.append(stats[1])
     world_means = np.array(world_means)
     world_sigmas = np.array(world_sigmas)
     return [world_means.mean(), world_means.std(), world_sigmas.mean(), world_sigmas.std()]
 
 
 def _get_yield_priors(n_rows=10000):
-    term_lookup = download_lookup('crop.csv')[:n_rows]
+    product_ids = download_lookup('crop.csv')[:n_rows]['termid']
     yield_lookup = download_lookup(LOOKUP_YIELD)
 
-    df = pd.DataFrame(columns=yield_lookup['termid'], index=term_lookup['termid'])
+    df = pd.DataFrame(columns=yield_lookup['termid'], index=product_ids)
 
-    for product_id in term_lookup['termid']:
+    for product_id in product_ids:
         logger.info(f'Processing {product_id}...')
         for gadm_code in yield_lookup['termid']:
             stats = get_mean_std_per_country_per_product(product_id, gadm_code, get_fao_yield)
             if None not in stats:
                 df.loc[product_id, gadm_code] = stats[0], stats[1]*SIGMA_SCALER, stats[2], stats[1]
 
     df.index.rename('term.id', inplace=True)
```

### Comparing `hestia-earth-distribution-0.0.8/hestia_earth/distribution/utils/__init__.py` & `hestia-earth-distribution-0.0.9/hestia_earth/distribution/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-distribution-0.0.8/hestia_earth/distribution/utils/fao.py` & `hestia-earth-distribution-0.0.9/hestia_earth/distribution/utils/fao.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,15 @@
 import pandas as pd
 import numpy as np
 from hestia_earth.utils.lookup import download_lookup, get_table_value, column_name
 
 from . import is_nonempty_str
 
 LOOKUP_YIELD = 'region-crop-cropGroupingFaostatProduction-yield.csv'
-LOOKUP_FERTUSE = 'region-inorganicFertiliser-usePerAreaOfCropland.csv'
-
-FERT_GROUPS = {
-    'N': 'inorganicNitrogenFertiliserUnspecifiedKgN',
-    'P2O5': 'inorganicPhosphorusFertiliserUnspecifiedKgP2O5',
-    'K2O': 'inorganicPotassiumFertiliserUnspecifiedKgK2O'
-}
-
-
-def get_fert_group_name(fert_id: str):
-    """
-    Look up the fertiliser group (N, P2O5, K2O) of a Hestia fertliser term
-
-    Parameters
-    ----------
-    fert_id: str
-        Inorganic or organic fertiliser term ID from Hestia glossary, e.g. 'ammoniumNitrateKgN'.
-
-    Returns
-    -------
-    str
-        fertiliser group, e.g. 'N', 'P2O5' or 'K2O'.
-    """
-    return fert_id.split('Kg')[-1]
-
-
-def get_fert_group_id(term_id: str): return FERT_GROUPS.get(get_fert_group_name(term_id))
+LOOKUP_FERTUSE = 'region-inorganicFertiliser-fertilisersUsage.csv'
 
 
 def create_df_fao():
     """
     Create a DataFrame to store all FAO crop yield data.
     This DataFrame can be used by plotting functions, especially with multiple subplots.
 
@@ -70,24 +44,24 @@
     str
         FAO Crop product term, e.g. 'Wheat'.
     """
     lookup = download_lookup('crop.csv')
     return get_table_value(lookup, 'termid', product_id, column_name('cropGroupingFaostatProduction'))
 
 
-def fao_str_record_to_array(fao_str: str, output_type=np.int32, n_years: int = 10, scaler: int = 1):
+def fao_str_record_to_array(fao_str: str, output_type=np.float32, n_years: int = 10, scaler: int = 1):
     """
     Converts FAO string records to np.array, and rescale if needed.
 
     Parameters
     ----------
     fao_str: str
         A string with time-series data read from FAO lookup file.
     output_type: dtype
-        Output data type, default np.int32.
+        Output data type, default `np.float32`.
     n_years: int
         Only fecth the latest N year of data, it will be restricted to any integer between 0 and 70.
     scaler: int
         Scaler for converting FAO units to Hestia units, defaults to `1`.
         Use `10` for converting from hg/ha to kg/ha, when reading FAO yield strings.
         This scaler will only be applied to the data array, not the year array.
```

### Comparing `hestia-earth-distribution-0.0.8/hestia_earth/distribution/utils/posterior.py` & `hestia-earth-distribution-0.0.9/hestia_earth/distribution/utils/posterior.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,55 @@
 from io import BytesIO
 import json
 import pandas as pd
 import numpy as np
-from hestia_earth.utils.api import download_hestia
+from typing import Union
 from hestia_earth.schema import TermTermType
+from hestia_earth.utils.api import download_hestia
+from hestia_earth.utils.lookup import download_lookup
+from hestia_earth.utils.tools import non_empty_list
 
 from hestia_earth.distribution.log import logger
-from . import df_to_csv_buffer, get_stats_from_df
-from ..cycle import YIELD_COLUMN, FERTILISER_COLUMNS
-from ..likelihood import generate_likl_file
+from hestia_earth.distribution.cycle import YIELD_COLUMN, FERTILISER_COLUMNS
+from hestia_earth.distribution.likelihood import generate_likl_file
 from .storage import file_exists, load_from_storage, write_to_storage
+from . import df_to_csv_buffer, get_stats_from_df
 
 FOLDER = 'posterior_files'
+INDEX_COLUMN = 'term.id'
+MULTI_INDEX_COLUMNS = ['product', 'inputs']
 TERM_TYPE_TO_COLUMN = {
     TermTermType.CROP.value: YIELD_COLUMN,
     TermTermType.INORGANICFERTILISER.value: FERTILISER_COLUMNS,
     TermTermType.ORGANICFERTILISER.value: FERTILISER_COLUMNS
 }
 
 
-def posterior_by_country(df_prior: pd.DataFrame, data, country_id: str, term_id: str, n_sample=1000):
+def _progress(values: list):
+    try:
+        from tqdm import tqdm
+        return tqdm(values)
+    except ModuleNotFoundError:
+        return values
+
+
+def posterior_by_country(df_prior: pd.DataFrame, data, country_id: str, term_id: str, n_sample=500):
+    # input mu_prior doesn't have to depend on product
     mu_country, sigma_country = get_stats_from_df(df_prior, country_id, term_id)
 
     logger.info(f'Prior mu ={mu_country}, std = {sigma_country}; Obs mean ={data.mean()}, std ={data.std()}')
 
     try:
         import pymc as pm
     except ImportError:
         raise ImportError("Run `pip install pymc==4` to use this functionality")
 
     if sigma_country > 0:
         with pm.Model():
-            pm.Normal('mu', mu=mu_country, sigma=sigma_country)
+            pm.TruncatedNormal('mu', mu=mu_country, sigma=sigma_country, lower=0)
             pm.HalfNormal('sd', sigma=sigma_country)
 
             sample = pm.sample(n_sample*2, tune=n_sample, cores=4)
             sample.extend(pm.sample_posterior_predictive(sample))
             # mu, sd = pm.summary(sample)['mean']
             return sample
 
@@ -52,36 +66,38 @@
 
 
 def _read_post(filename: str):
     data = json.loads(load_from_storage(filename))
     return data.get('posterior', {}).get('mu', []), data.get('posterior', {}).get('sd', [])
 
 
-def _write_post(country_id: str, term_id: str, filepath: str, df_prior: pd.DataFrame, generate_prior):
+def _write_post(country_id: str, product_id: str, term_id: str, filepath: str, df_prior: pd.DataFrame, generate_prior):
     data = {
         'posterior': {'mu': [], 'sd': []}
     }
-    df_likl = generate_likl_file(country_id, term_id)
+    df_likl = generate_likl_file(country_id, product_id)
 
-    if len(df_likl) > 0:
+    if not df_likl.empty:
         # make sure we don't load prior file muliple times when generating all posteriors
         _df_prior = generate_prior() if df_prior is None else df_prior
+        term_id = product_id if term_id == '' else term_id
         likl_data = df_likl[_find_matching_column(term_id)]
         posterior_data = posterior_by_country(_df_prior, likl_data, country_id, term_id)
         if posterior_data is not None:
             data['posterior']['mu'] = posterior_data['posterior']['mu'].to_dict()['data']
             data['posterior']['sd'] = posterior_data['posterior']['sd'].to_dict()['data']
 
     # skip writing when the file exists and the data will not be updated
     should_write_to_storage = not file_exists(filepath) or len(df_likl) > 0
     write_to_storage(filepath, json.dumps(data).encode('utf-8')) if should_write_to_storage else None
     return data.get('posterior', {}).get('mu', []), data.get('posterior', {}).get('sd', [])
 
 
-def post_filename(country_id: str, term_id: str): return f'posterior_{country_id}_{term_id}.json'
+def _post_filename(country_id: str, product_id: str, term_id: str = ''):
+    return f"{'_'.join(non_empty_list(['posterior', country_id, product_id, term_id]))}.json"
 
 
 def get_esemble_means(mu_ensemble: list, sd_ensemble: list):
     """
     Return posterior means for an ensembles of mu and an ensembles of sigma (sd).
 
     Parameters
@@ -102,39 +118,60 @@
     ]) else None
 
 
 def get_index_range(values: list, index: list): return values or list(range(len(index)))
 
 
 def get_post_ensemble_data(
-    country_id: str, term_id: str,
+    country_id: str, product_id: str, term_id: str = '',
     overwrite=False, df_prior: pd.DataFrame = None, generate_prior=None
 ):
-    filepath = f"{FOLDER}/{post_filename(country_id, term_id)}"
+    filepath = f"{FOLDER}/{_post_filename(country_id, product_id, term_id)}"
     read_existing = file_exists(filepath) and not overwrite
-    return _read_post(filepath) if read_existing else _write_post(country_id, term_id, filepath,
-                                                                  df_prior, generate_prior)
+    return _read_post(filepath) if read_existing else _write_post(country_id, product_id, term_id,
+                                                                  filepath, df_prior, generate_prior)
+
+
+def _update_by_product_input(df, df_prior, product_id, country_id, input_ids, overwrite):
+    for input_id in input_ids:
+        if not pd.isnull(df_prior.loc[input_id, country_id]):
+            mu_ensemble, sd_ensemble = get_post_ensemble_data(country_id, product_id, input_id,
+                                                              overwrite=overwrite, df_prior=df_prior)
+            df.loc[(product_id, input_id)][country_id] = get_esemble_means(mu_ensemble, sd_ensemble)
+    return df
 
 
-def update_all_post_data(df_prior: pd.DataFrame, filename: str, rows: list = None, cols: list = None, overwrite=True):
+def _update_by_product(df, df_prior, product_id, country_id, overwrite):
+    if not pd.isnull(df_prior.loc[product_id, country_id]):
+        mu_ensemble, sd_ensemble = get_post_ensemble_data(country_id, product_id,
+                                                          overwrite=overwrite, df_prior=df_prior)
+        df.loc[product_id, country_id] = get_esemble_means(mu_ensemble, sd_ensemble)
+    return df
+
+
+def update_all_post_data(df_prior: pd.DataFrame, filename: str, rows: list = None, cols: list = None,
+                         input_ids: list = None, overwrite=True):
     rows = get_index_range(rows, df_prior.index)
-    term_ids = df_prior.index[rows]
+    product_ids = df_prior.index[rows] if input_ids is None else download_lookup('crop.csv')['termid']
     cols = get_index_range(cols, df_prior.columns)
     country_ids = df_prior.columns[cols]
-    df = pd.DataFrame(index=term_ids, columns=country_ids)
-
-    for country_id in country_ids:
-        for term_id in term_ids:
-            if not pd.isnull(df_prior.loc[term_id, country_id]):
-                mu_ensemble, sd_ensemble = get_post_ensemble_data(country_id, term_id,
-                                                                  overwrite=overwrite, df_prior=df_prior)
-                df.loc[term_id, country_id] = get_esemble_means(mu_ensemble, sd_ensemble)
+    index = product_ids if input_ids is None else (
+        pd.MultiIndex.from_product([product_ids, input_ids], names=MULTI_INDEX_COLUMNS)
+    )
+    df = pd.DataFrame(index=index, columns=country_ids)
+
+    for country_id in _progress(country_ids):
+        for product_id in product_ids:
+            df = (
+                _update_by_product_input(df, df_prior, product_id, country_id, input_ids, overwrite) if input_ids
+                else _update_by_product(df, df_prior, product_id, country_id, overwrite)
+            )
 
-    df.index.rename('term.id', inplace=True)
+    df.index.rename(INDEX_COLUMN, inplace=True) if input_ids is None else None
     write_to_storage(f"{FOLDER}/{filename}", df_to_csv_buffer(df))
     return df.dropna(axis=1, how='all').dropna(axis=0, how='all')
 
 
-def get_post_data(country_id: str, term_id: str, filename: str):
+def get_post_data(country_id: str, term_ids: Union[str, tuple], filename: str):
     data = load_from_storage(f"{FOLDER}/{filename}")
-    df = pd.read_csv(BytesIO(data), index_col=0)
-    return get_stats_from_df(df, country_id, term_id)
+    df = pd.read_csv(BytesIO(data)).set_index(INDEX_COLUMN if type(term_ids) == str else MULTI_INDEX_COLUMNS)
+    return get_stats_from_df(df, country_id, term_ids)
```

### Comparing `hestia-earth-distribution-0.0.8/hestia_earth/distribution/utils/priors.py` & `hestia-earth-distribution-0.0.9/hestia_earth/distribution/utils/priors.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 from io import BytesIO
 import pandas as pd
 
 from hestia_earth.distribution.log import logger
 from . import is_nonempty_str
 from .storage import load_from_storage, write_to_storage
 
-
+FOLDER = 'prior_files'
 READ_BY_TYPE = {
     '.pkl': lambda x: pd.read_pickle(x),
     '.csv': lambda x: pd.read_csv(x, na_values='-', index_col=['term.id']),
     None: lambda *args: logger.error('Unsupported file type.')
 }
-
-
 WRITE_BY_TYPE = {
     '.pkl': lambda df, buffer: df.to_pickle(buffer),
     '.csv': lambda df, buffer: df.to_csv(buffer, na_rep='-', index=True, index_label='term.id'),
     None: lambda *args: logger.error('Unsupported file type.')
 }
```

### Comparing `hestia-earth-distribution-0.0.8/hestia_earth/distribution/utils/storage/__init__.py` & `hestia-earth-distribution-0.0.9/hestia_earth/distribution/utils/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-distribution-0.0.8/hestia_earth/distribution/utils/storage/_local_client.py` & `hestia-earth-distribution-0.0.9/hestia_earth/distribution/utils/storage/_local_client.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-distribution-0.0.8/hestia_earth_distribution.egg-info/PKG-INFO` & `hestia-earth-distribution-0.0.9/hestia_earth_distribution.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: hestia-earth-distribution
-Version: 0.0.8
+Version: 0.0.9
 Summary: Hestia's Distribution library
 Home-page: https://gitlab.com/hestia-earth/hestia-distribution
 Author: Hestia Team
 Author-email: guillaume@hestia.earth
-License: GPL-3.0-or-later
+License: MIT
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: stats
 License-File: LICENSE
```

### Comparing `hestia-earth-distribution-0.0.8/hestia_earth_distribution.egg-info/SOURCES.txt` & `hestia-earth-distribution-0.0.9/hestia_earth_distribution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hestia-earth-distribution-0.0.8/setup.py` & `hestia-earth-distribution-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     version=VERSION,
     description="Hestia's Distribution library",
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://gitlab.com/hestia-earth/hestia-distribution',
     author='Hestia Team',
     author_email='guillaume@hestia.earth',
-    license='GPL-3.0-or-later',
+    license='MIT',
     classifiers=[
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3.6',
     ],
     packages=find_packages(exclude=('tests', 'scripts')),
     include_package_data=True,
     install_requires=REQUIRES,
```

### Comparing `hestia-earth-distribution-0.0.8/tests/distribution/test_cycle.py` & `hestia-earth-distribution-0.0.9/tests/distribution/test_cycle.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,9 +24,9 @@
         cycles = json.load(f)
     results = group_cycle_inputs(cycles[0])
     assert results.get('Nitrogen (kg N)') == 192
 
 
 def test_get_input_group():
     assert get_input_group({'term': {'units': 'kg N'}}) == 'Nitrogen (kg N)'
-    assert get_input_group({'term': {'units': 'kg K2O'}}) == 'Potash (kg K2O)'
+    assert get_input_group({'term': {'units': 'kg K2O'}}) == 'Potassium (kg K2O)'
     assert get_input_group({'term': {'units': 'kg CaCO3'}}) is None
```

### Comparing `hestia-earth-distribution-0.0.8/tests/distribution/test_likelihood.py` & `hestia-earth-distribution-0.0.9/tests/distribution/test_likelihood.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,10 +32,9 @@
     product_id = 'wheatGrain'
 
     expected = pd.read_csv(os.path.join(fixtures_folder, 'result.csv'), index_col=0)
     result = generate_likl_file(country_id, product_id)
     round_df_column(result, 'Grain yield (kg/ha)')
     round_df_column(result, 'Nitrogen (kg N)')
     round_df_column(result, 'Phosphorus (kg P2O5)')
-    round_df_column(result, 'Potash (kg K2O)')
-
+    round_df_column(result, 'Potassium (kg K2O)')
     assert result.to_csv() == expected.to_csv()
```

### Comparing `hestia-earth-distribution-0.0.8/tests/distribution/test_posterior_fert.py` & `hestia-earth-distribution-0.0.9/tests/distribution/test_posterior_fert.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 )
 
 class_path = 'hestia_earth.distribution.posterior_fert'
 
 
 @patch(f"{class_path}.get_post_ensemble_data")
 def test_get_post_ensemble(mock_get_post_ensemble_data):
-    get_post_ensemble('GADM-ALB', 'manureSaltsKgK2O')
+    get_post_ensemble('GADM-ALB', 'wheatGrain', 'manureSaltsKgK2O')
     mock_get_post_ensemble_data.assert_called_once()
 
 
 @patch(f"{class_path}.generate_prior_fert_file", return_value={})
 @patch(f"{class_path}.update_all_post_data")
 def test_update_all_post(mock_update_all_post_data, *args):
     update_all_post()
     mock_update_all_post_data.assert_called_once()
 
 
 @patch(f"{class_path}.get_post_data")
 def test_get_post(mock_get_post_data):
-    get_post('GADM-ALB', 'manureSaltsKgK2O')
+    get_post('GADM-ALB', 'wheatGrain', 'manureSaltsKgK2O')
     mock_get_post_data.assert_called_once()
```

### Comparing `hestia-earth-distribution-0.0.8/tests/distribution/test_posterior_yield.py` & `hestia-earth-distribution-0.0.9/tests/distribution/test_posterior_yield.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 )
 
 class_path = 'hestia_earth.distribution.posterior_yield'
 
 
 @patch(f"{class_path}.get_post_ensemble_data")
 def test_get_post_ensemble(mock_get_post_ensemble_data):
-    get_post_ensemble('GADM-CHE', 'genericCropSeed')
+    get_post_ensemble('GADM-CHE', 'bananaFruit')
     mock_get_post_ensemble_data.assert_called_once()
 
 
 @patch(f"{class_path}.generate_prior_yield_file", return_value={})
 @patch(f"{class_path}.update_all_post_data")
 def test_update_all_post(mock_update_all_post_data, *args):
     update_all_post()
     mock_update_all_post_data.assert_called_once()
 
 
 @patch(f"{class_path}.get_post_data")
 def test_get_post(mock_get_post_data):
-    get_post('GADM-CHE', 'genericCropSeed')
+    get_post('GADM-CHE', 'bananaFruit')
     mock_get_post_data.assert_called_once()
```

### Comparing `hestia-earth-distribution-0.0.8/tests/distribution/test_prior_fert.py` & `hestia-earth-distribution-0.0.9/tests/distribution/test_prior_fert.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-distribution-0.0.8/tests/distribution/test_prior_yield.py` & `hestia-earth-distribution-0.0.9/tests/distribution/test_prior_yield.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 )
 
 fixtures_folder = os.path.join(fixtures_path, 'prior_yield')
 
 
 def test_worldwide_mean_sigma():
     stats = calculate_worldwide_mean_sigma('wheatGrain')
-    assert [round(s) for s in stats] == [3197, 1854, 371, 241]
+    assert [round(s) for s in stats] == [3276, 1896, 389, 311]
 
 
 @patch('hestia_earth.distribution.utils.priors.write_to_storage')
 def test_generate_prior_yield_file(*args):
-    result = generate_prior_yield_file(10, overwrite=True)
+    result = generate_prior_yield_file(35, overwrite=True)
     expected = read_prior_stats(os.path.join(fixtures_folder, 'result.csv'))
     assert result.to_csv() == expected.to_csv()
 
 
 def read_prior_file(*args):
     with open(os.path.join(fixtures_folder, 'result.csv'), 'rb') as f:
         return f.read()
 
 
 @patch('hestia_earth.distribution.utils.priors.load_from_storage', side_effect=read_prior_file)
 def test_get_prior(*args):
-    mu, sd = get_prior('GADM-CHE', 'genericCropSeed')
-    assert mu == 2710.3
-    assert sd == 1786.7588024129054
+    mu, sd = get_prior('GADM-ETH', 'abacaPlant')
+    assert mu == 66.06000061035157
+    assert sd == 2.217568562003663
 
 
 @patch('hestia_earth.distribution.utils.priors.load_from_storage', side_effect=read_prior_file)
 def test_get_prior_missing(*args):
     # data is empty
     mu, sd = get_prior('GADM-AFG', 'genericCropSeed')
     assert mu is None
```

### Comparing `hestia-earth-distribution-0.0.8/tests/distribution/utils/test_posterior.py` & `hestia-earth-distribution-0.0.9/tests/distribution/utils/test_posterior.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,79 +2,79 @@
 import os
 import json
 import pandas as pd
 from tests.utils import fixtures_path
 from hestia_earth.distribution.utils.priors import read_prior_stats
 
 from hestia_earth.distribution.utils.posterior import (
-    update_all_post_data, get_post_data, get_post_ensemble_data, post_filename
+    INDEX_COLUMN, MULTI_INDEX_COLUMNS, update_all_post_data, get_post_data, get_post_ensemble_data, _post_filename
 )
 
 
 class_path = 'hestia_earth.distribution.utils.posterior'
 
 
 def fake_generate_prior_file(folder: str):
     def run(*args):
         return read_prior_stats(os.path.join(fixtures_path, folder, 'prior.csv'))
     return run
 
 
 def fake_generate_likl_file(folder: str):
-    def run(country_id, product_id):
+    def run(country_id, product_id, *args):
         likl_file = os.path.join(fixtures_path, folder, 'likelihood', f"{'-'.join([country_id, product_id])}.csv")
-        return pd.read_csv(likl_file) if os.path.exists(likl_file) else []
+        return pd.read_csv(likl_file) if os.path.exists(likl_file) else pd.DataFrame()
     return run
 
 
 def read_posterior_file(folder: str):
     def run(*args):
         with open(os.path.join(fixtures_path, folder, 'result.csv'), 'rb') as f:
             return f.read()
     return run
 
 
 @patch(f"{class_path}.load_from_storage", side_effect=read_posterior_file('posterior_yield'))
 def test_get_post_yield(*args):
-    mu, sd = get_post_data('GADM-CHE', 'genericCropSeed', '')
+    mu, sd = get_post_data('GADM-COL', 'bananaFruit', '')
     assert mu == 2716
     assert sd == 486
 
 
 @patch(f"{class_path}.load_from_storage", side_effect=read_posterior_file('posterior_yield'))
 def test_get_post_yield_missing(*args):
     mu, sd = get_post_data('GADM-FRA', 'wheatGrain', '')
     assert mu is None
     assert sd is None
 
 
 @patch(f"{class_path}.load_from_storage", side_effect=read_posterior_file('posterior_yield'))
 def test_get_post_yield_empty(*args):
-    mu, sd = get_post_data('GADM-AFG', 'wheatGrain', '')
+    mu, sd = get_post_data('GADM-COL', 'wheatGrain', '')
     assert mu is None
     assert sd is None
 
 
 @patch(f"{class_path}.load_from_storage", side_effect=read_posterior_file('posterior_fert'))
 def test_get_post_fert(*args):
-    mu, sd = get_post_data('GADM-ALB', 'inorganicPotassiumFertiliserUnspecifiedKgK2O', '')
-    assert mu == 2.4407828918588113
-    assert sd == 5.792617394824452
+    mu, sd = get_post_data('GADM-ALB', ('wheatGrain', 'inorganicPotassiumFertiliserUnspecifiedKgK2O'), '')
+    assert mu == 2.6290606152464733
+    assert sd == 5.785971787572081
 
 
 @patch(f"{class_path}.load_from_storage", side_effect=read_posterior_file('posterior_fert'))
 def test_get_post_fert_missing(*args):
-    mu, sd = get_post_data('GADM-FRA', 'inorganicPotassiumFertiliserUnspecifiedKgK2O', '')
+    mu, sd = get_post_data('GADM-FRA', ('wheatGrain', 'inorganicPotassiumFertiliserUnspecifiedKgK2O'), '')
     assert mu is None
     assert sd is None
 
 
 @patch(f"{class_path}.load_from_storage", side_effect=read_posterior_file('posterior_fert'))
 def test_get_post_fert_empty(*args):
-    mu, sd = get_post_data('GADM-AUT', 'inorganicPotassiumFertiliserUnspecifiedKgK2O', '')
+    mu, sd = get_post_data('GADM-AUT', ('wheatGrain', 'inorganicPotassiumFertiliserUnspecifiedKgK2O'), '')
     assert mu is None
     assert sd is None
 
 
 def read_posterior_json(folder: str):
     def read_posterior(filename: str):
         file = filename.split('/')[1]
@@ -82,85 +82,90 @@
             return f.read()
     return read_posterior
 
 
 @patch(f"{class_path}.load_from_storage", side_effect=read_posterior_json('posterior_yield'))
 @patch(f"{class_path}.file_exists", return_value=True)
 def test_get_post_ensemble_data_yield(*args):
-    mu_ensemble, sd_ensemble = get_post_ensemble_data('GADM-CHE', 'genericCropSeed')
+    mu_ensemble, sd_ensemble = get_post_ensemble_data('GADM-COL', 'bananaFruit')
     assert len(mu_ensemble) == 4
     assert len(sd_ensemble) == 4
 
 
 @patch(f"{class_path}.generate_likl_file", side_effect=fake_generate_likl_file('posterior_yield'))
 @patch(f"{class_path}.write_to_storage")
 @patch(f"{class_path}.file_exists", return_value=False)
 def test_get_post_ensemble_data_yield_missing(*args):
-    mu_ensemble, sd_ensemble = get_post_ensemble_data('GADM-CHE', 'genericCropSeed',
+    mu_ensemble, sd_ensemble = get_post_ensemble_data('GADM-CHE', 'appleFruit',
                                                       generate_prior=fake_generate_prior_file('posterior_yield'))
-    assert len(mu_ensemble) == 4
-    assert len(sd_ensemble) == 4
+    assert len(mu_ensemble) == 0
+    assert len(sd_ensemble) == 0
 
 
 @patch(f"{class_path}.load_from_storage", side_effect=read_posterior_json('posterior_yield'))
 @patch(f"{class_path}.file_exists", return_value=True)
 def test_get_post_ensemble_data_yield_empty(*args):
     mu_ensemble, sd_ensemble = get_post_ensemble_data('GADM-AFG', 'wheatGrain')
     assert len(mu_ensemble) == 0
     assert len(sd_ensemble) == 0
 
 
 @patch(f"{class_path}.load_from_storage", side_effect=read_posterior_json('posterior_fert'))
 @patch(f"{class_path}.file_exists", return_value=True)
 def test_get_post_ensemble_data_fert(*args):
-    mu_ensemble, sd_ensemble = get_post_ensemble_data('GADM-ALB', 'inorganicPotassiumFertiliserUnspecifiedKgK2O')
-    assert len(mu_ensemble) == 2
-    assert len(sd_ensemble) == 2
+    mu_ensemble, sd_ensemble = get_post_ensemble_data('GADM-ALB', 'wheatGrain',
+                                                      'inorganicPotassiumFertiliserUnspecifiedKgK2O',
+                                                      generate_prior=fake_generate_prior_file('posterior_fert'))
+    assert len(mu_ensemble) == 4
+    assert len(sd_ensemble) == 4
 
 
 @patch(f"{class_path}.generate_likl_file", side_effect=fake_generate_likl_file('posterior_fert'))
 @patch(f"{class_path}.write_to_storage")
 @patch(f"{class_path}.file_exists", return_value=False)
 def test_get_post_ensemble_data_fert_missing(*args):
-    mu_ensemble, sd_ensemble = get_post_ensemble_data('GADM-ALB', 'inorganicPotassiumFertiliserUnspecifiedKgK2O',
+    mu_ensemble, sd_ensemble = get_post_ensemble_data('GADM-ALB', 'wheatGrain',
+                                                      'inorganicPotassiumFertiliserUnspecifiedKgK2O',
                                                       generate_prior=fake_generate_prior_file('posterior_fert'))
     assert len(mu_ensemble) == 4
     assert len(sd_ensemble) == 4
 
 
 @patch(f"{class_path}.load_from_storage", side_effect=read_posterior_json('posterior_fert'))
 @patch(f"{class_path}.file_exists", return_value=True)
 def test_get_post_ensemble_data_fert_empty(*args):
-    mu_ensemble, sd_ensemble = get_post_ensemble_data('GADM-AUT', 'inorganicPotassiumFertiliserUnspecifiedKgK2O')
+    mu_ensemble, sd_ensemble = get_post_ensemble_data('GADM-AUT', 'wheatGrain',
+                                                      'inorganicPotassiumFertiliserUnspecifiedKgK2O',
+                                                      generate_prior=fake_generate_prior_file('posterior_fert'))
     assert len(mu_ensemble) == 0
     assert len(sd_ensemble) == 0
 
 
 def fake_get_post_ensemble(folder: str):
-    def run(country_id, product_id, **kwargs):
-        filepath = os.path.join(fixtures_path, folder, post_filename(country_id, product_id))
+    def run(country_id, product_id, term_id='', **kwargs):
+        filepath = os.path.join(fixtures_path, folder, _post_filename(country_id, product_id, term_id))
         data = {}
         if os.path.exists(filepath):
             with open(filepath, 'r') as f:
                 data = json.load(f)
         return data.get('posterior', {}).get('mu', []), data.get('posterior', {}).get('sd', [])
     return run
 
 
 @patch(f"{class_path}.get_post_ensemble_data", side_effect=fake_get_post_ensemble('posterior_yield'))
 @patch(f"{class_path}.write_to_storage")
 def test_update_all_post_data_yield(*args):
     df_prior = read_prior_stats(os.path.join(fixtures_path, 'posterior_yield', 'prior.csv'))
     result = update_all_post_data(df_prior, '')
     expected_file = os.path.join(fixtures_path, 'posterior_yield', 'result.csv')
-    expected = pd.read_csv(expected_file, na_values='-', index_col=['term.id'])
+    expected = pd.read_csv(expected_file, na_values='-', index_col=INDEX_COLUMN)
     assert (result.columns == expected.columns).all() and (result.index == expected.index).all()
 
 
 @patch(f"{class_path}.get_post_ensemble_data", side_effect=fake_get_post_ensemble('posterior_fert'))
 @patch(f"{class_path}.write_to_storage")
 def test_update_all_post_data_fert(*args):
     df_prior = read_prior_stats(os.path.join(fixtures_path, 'posterior_fert', 'prior.csv'))
-    result = update_all_post_data(df_prior, '')
+    result = update_all_post_data(df_prior, '', input_ids=['inorganicPotassiumFertiliserUnspecifiedKgK2O'])
     expected_file = os.path.join(fixtures_path, 'posterior_fert', 'result.csv')
-    expected = pd.read_csv(expected_file, na_values='-', index_col=['term.id'])
+    expected = pd.read_csv(expected_file, na_values='-', index_col=MULTI_INDEX_COLUMNS)
     assert (result.columns == expected.columns).all() and (result.index == expected.index).all()
```

### Comparing `hestia-earth-distribution-0.0.8/tests/distribution/utils/test_priors.py` & `hestia-earth-distribution-0.0.9/tests/distribution/utils/test_priors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 from tests.utils import fixtures_path
 
 from hestia_earth.distribution.utils.priors import get_prior_by_country_by_product
 
 
 def test_get_prior_by_country_by_product_yield():
-    country_id = 'GADM-AUT'
-    product_id = 'genericCropSeed'
+    country_id = 'GADM-CRI'
+    product_id = 'abacaLeafStalk'
     prior_filename = os.path.join(fixtures_path, 'prior_yield', 'result.csv')
     vals = get_prior_by_country_by_product(prior_filename, country_id, product_id)
-    assert [round(v) for v in vals] == [3673, 1514, 10, 505]
+    assert [round(v) for v in vals] == [1157, 18, 10, 6]
 
 
 def test_get_prior_by_country_by_product_fert():
     country_id = 'GADM-AFG'
     product_id = 'inorganicNitrogenFertiliserUnspecifiedKgN'
     prior_filename = os.path.join(fixtures_path, 'prior_fert', 'result.csv')
     vals = get_prior_by_country_by_product(prior_filename, country_id, product_id)
```

