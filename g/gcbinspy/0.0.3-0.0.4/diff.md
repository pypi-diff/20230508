# Comparing `tmp/gcbinspy-0.0.3.tar.gz` & `tmp/gcbinspy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcbinspy-0.0.3.tar", last modified: Tue Feb  7 11:20:04 2023, max compression
+gzip compressed data, was "gcbinspy-0.0.4.tar", last modified: Mon May  8 09:14:17 2023, max compression
```

## Comparing `gcbinspy-0.0.3.tar` & `gcbinspy-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:20:04.521564 gcbinspy-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-07 11:19:55.000000 gcbinspy-0.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-02-07 11:20:04.521564 gcbinspy-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-02-07 11:19:55.000000 gcbinspy-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:20:04.521564 gcbinspy-0.0.3/gcbinspy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 11:19:55.000000 gcbinspy-0.0.3/gcbinspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-02-07 11:19:55.000000 gcbinspy-0.0.3/gcbinspy/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-02-07 11:19:55.000000 gcbinspy-0.0.3/gcbinspy/gcbinspy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:20:04.521564 gcbinspy-0.0.3/gcbinspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-02-07 11:20:04.000000 gcbinspy-0.0.3/gcbinspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-07 11:20:04.000000 gcbinspy-0.0.3/gcbinspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 11:20:04.000000 gcbinspy-0.0.3/gcbinspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-07 11:20:04.000000 gcbinspy-0.0.3/gcbinspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-07 11:20:04.000000 gcbinspy-0.0.3/gcbinspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-07 11:19:55.000000 gcbinspy-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 11:20:04.525564 gcbinspy-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-07 11:19:55.000000 gcbinspy-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:14:17.671961 gcbinspy-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-08 09:14:08.000000 gcbinspy-0.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-08 09:14:17.671961 gcbinspy-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-08 09:14:08.000000 gcbinspy-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:14:17.671961 gcbinspy-0.0.4/gcbinspy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:14:08.000000 gcbinspy-0.0.4/gcbinspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-08 09:14:08.000000 gcbinspy-0.0.4/gcbinspy/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-08 09:14:08.000000 gcbinspy-0.0.4/gcbinspy/gcbinspy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:14:17.671961 gcbinspy-0.0.4/gcbinspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-08 09:14:17.000000 gcbinspy-0.0.4/gcbinspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-08 09:14:17.000000 gcbinspy-0.0.4/gcbinspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:14:17.000000 gcbinspy-0.0.4/gcbinspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 09:14:17.000000 gcbinspy-0.0.4/gcbinspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 09:14:17.000000 gcbinspy-0.0.4/gcbinspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-08 09:14:08.000000 gcbinspy-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 09:14:17.671961 gcbinspy-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-08 09:14:08.000000 gcbinspy-0.0.4/setup.py
```

### Comparing `gcbinspy-0.0.3/LICENSE.md` & `gcbinspy-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gcbinspy-0.0.3/PKG-INFO` & `gcbinspy-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcbinspy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Gold Coast bin days
 Author-email: poroping <poroping@github.com>
 Project-URL: Homepage, https://github.com/poroping/gcbinspy
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
@@ -17,14 +17,14 @@
 Example:
 
 ```
 import gcbinspy
 
 address = "26 Eleventh Ave, Palm Beach QLD 4221"
 
-client = bins.GoldCoastBins(address)
+client = gcbinspy.GoldCoastBins(address)
 client.property_id()
 client.update_next_bin_days()
 print(client.next_landfill().isoformat())
 print(client.is_recycling_day())
 print(client.is_organics_day_tomorrow())
 ```
```

### Comparing `gcbinspy-0.0.3/README.md` & `gcbinspy-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 Example:
 
 ```
 import gcbinspy
 
 address = "26 Eleventh Ave, Palm Beach QLD 4221"
 
-client = bins.GoldCoastBins(address)
+client = gcbinspy.GoldCoastBins(address)
 client.property_id()
 client.update_next_bin_days()
 print(client.next_landfill().isoformat())
 print(client.is_recycling_day())
 print(client.is_organics_day_tomorrow())
 ```
```

### Comparing `gcbinspy-0.0.3/gcbinspy/gcbinspy.py` & `gcbinspy-0.0.4/gcbinspy/gcbinspy.py`

 * *Files identical despite different names*

### Comparing `gcbinspy-0.0.3/gcbinspy.egg-info/PKG-INFO` & `gcbinspy-0.0.4/gcbinspy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcbinspy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Gold Coast bin days
 Author-email: poroping <poroping@github.com>
 Project-URL: Homepage, https://github.com/poroping/gcbinspy
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
@@ -17,14 +17,14 @@
 Example:
 
 ```
 import gcbinspy
 
 address = "26 Eleventh Ave, Palm Beach QLD 4221"
 
-client = bins.GoldCoastBins(address)
+client = gcbinspy.GoldCoastBins(address)
 client.property_id()
 client.update_next_bin_days()
 print(client.next_landfill().isoformat())
 print(client.is_recycling_day())
 print(client.is_organics_day_tomorrow())
 ```
```

