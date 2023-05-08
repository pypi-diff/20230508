# Comparing `tmp/psl-2023.5.1.tar.gz` & `tmp/psl-2023.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psl-2023.5.1.tar", last modified: Mon May  1 13:05:00 2023, max compression
+gzip compressed data, was "psl-2023.5.8.tar", last modified: Mon May  8 13:05:37 2023, max compression
```

## Comparing `psl-2023.5.1.tar` & `psl-2023.5.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:05:00.642043 psl-2023.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-05-01 13:04:29.000000 psl-2023.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-01 13:04:29.000000 psl-2023.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-01 13:05:00.642043 psl-2023.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-01 13:04:29.000000 psl-2023.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:05:00.638043 psl-2023.5.1/psl/
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-01 13:04:36.000000 psl-2023.5.1/psl/__init__.py
--rw-------   0 runner    (1001) docker     (123)   108964 2023-05-01 13:04:36.000000 psl-2023.5.1/psl/psl.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 13:04:29.000000 psl-2023.5.1/psl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:05:00.642043 psl-2023.5.1/psl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-01 13:05:00.000000 psl-2023.5.1/psl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-01 13:05:00.000000 psl-2023.5.1/psl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 13:05:00.000000 psl-2023.5.1/psl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 13:04:49.000000 psl-2023.5.1/psl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-01 13:05:00.000000 psl-2023.5.1/psl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 13:05:00.642043 psl-2023.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-01 13:04:29.000000 psl-2023.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:05:37.747381 psl-2023.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-05-08 13:04:54.000000 psl-2023.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-08 13:04:54.000000 psl-2023.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-08 13:05:37.747381 psl-2023.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-08 13:04:54.000000 psl-2023.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:05:37.743381 psl-2023.5.8/psl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-08 13:05:05.000000 psl-2023.5.8/psl/__init__.py
+-rw-------   0 runner    (1001) docker     (123)   109057 2023-05-08 13:05:05.000000 psl-2023.5.8/psl/psl.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:54.000000 psl-2023.5.8/psl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:05:37.747381 psl-2023.5.8/psl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-08 13:05:37.000000 psl-2023.5.8/psl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-08 13:05:37.000000 psl-2023.5.8/psl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:05:37.000000 psl-2023.5.8/psl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:05:22.000000 psl-2023.5.8/psl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-08 13:05:37.000000 psl-2023.5.8/psl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:05:37.747381 psl-2023.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-08 13:04:54.000000 psl-2023.5.8/setup.py
```

### Comparing `psl-2023.5.1/LICENSE` & `psl-2023.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `psl-2023.5.1/PKG-INFO` & `psl-2023.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2023.5.1
+Version: 2023.5.8
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2023.5.1/README.md` & `psl-2023.5.8/README.md`

 * *Files identical despite different names*

### Comparing `psl-2023.5.1/psl/__init__.py` & `psl-2023.5.8/psl/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import pathlib
 import typing
 
-__version__ = "2023.5.1"
-__checksum__ = "88c37e4a48740c9940a7765f98c68ac8cb05706b"
+__version__ = "2023.5.8"
+__checksum__ = "76d72cafbb85dd7412b50757685c721d91c8a356"
 __all__ = ["PUBLIC_SUFFIX_URL", "domain_suffixes", "Suffixes", "domain_can_set_cookie"]
 
 
 PUBLIC_SUFFIX_URL = "https://publicsuffix.org/list/public_suffix_list.dat"
 _PUBLIC_SUFFIX_PATH = pathlib.Path(__file__).parent / "psl.txt"
```

### Comparing `psl-2023.5.1/psl/psl.txt` & `psl-2023.5.8/psl/psl.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4594,60 +4594,68 @@
 targi.pl
 tm.pl
 tourism.pl
 travel.pl
 turystyka.pl
 gov.pl
 ap.gov.pl
+griw.gov.pl
 ic.gov.pl
 is.gov.pl
-us.gov.pl
 kmpsp.gov.pl
+konsulat.gov.pl
 kppsp.gov.pl
-kwpsp.gov.pl
-psp.gov.pl
-wskr.gov.pl
 kwp.gov.pl
+kwpsp.gov.pl
+mup.gov.pl
 mw.gov.pl
-ug.gov.pl
-um.gov.pl
-umig.gov.pl
-ugim.gov.pl
-upow.gov.pl
-uw.gov.pl
-starostwo.gov.pl
+oia.gov.pl
+oirm.gov.pl
+oke.gov.pl
+oow.gov.pl
+oschr.gov.pl
+oum.gov.pl
 pa.gov.pl
+pinb.gov.pl
+piw.gov.pl
 po.gov.pl
+pr.gov.pl
+psp.gov.pl
 psse.gov.pl
 pup.gov.pl
 rzgw.gov.pl
 sa.gov.pl
+sdn.gov.pl
+sko.gov.pl
 so.gov.pl
 sr.gov.pl
-wsa.gov.pl
-sko.gov.pl
+starostwo.gov.pl
+ug.gov.pl
+ugim.gov.pl
+um.gov.pl
+umig.gov.pl
+upow.gov.pl
+uppo.gov.pl
+us.gov.pl
+uw.gov.pl
 uzs.gov.pl
+wif.gov.pl
 wiih.gov.pl
 winb.gov.pl
-pinb.gov.pl
 wios.gov.pl
 witd.gov.pl
-wzmiuw.gov.pl
-piw.gov.pl
 wiw.gov.pl
-griw.gov.pl
-wif.gov.pl
-oum.gov.pl
-sdn.gov.pl
-zp.gov.pl
-uppo.gov.pl
-mup.gov.pl
+wkz.gov.pl
+wsa.gov.pl
+wskr.gov.pl
+wsse.gov.pl
 wuoz.gov.pl
-konsulat.gov.pl
-oirm.gov.pl
+wzmiuw.gov.pl
+zp.gov.pl
+zpisdn.gov.pl
 augustow.pl
 babia-gora.pl
 bedzin.pl
 beskidy.pl
 bialowieza.pl
 bialystok.pl
 bielawa.pl
```

### Comparing `psl-2023.5.1/psl.egg-info/PKG-INFO` & `psl-2023.5.8/psl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2023.5.1
+Version: 2023.5.8
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2023.5.1/setup.py` & `psl-2023.5.8/setup.py`

 * *Files identical despite different names*

