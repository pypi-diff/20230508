# Comparing `tmp/bmw-lobster-tool-codebeamer-0.9.1.tar.gz` & `tmp/bmw-lobster-tool-codebeamer-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-tool-codebeamer-0.9.1.tar", last modified: Wed May  3 14:22:58 2023, max compression
+gzip compressed data, was "bmw-lobster-tool-codebeamer-0.9.2.tar", last modified: Mon May  8 15:06:39 2023, max compression
```

## Comparing `bmw-lobster-tool-codebeamer-0.9.1.tar` & `bmw-lobster-tool-codebeamer-0.9.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:58.152383 bmw-lobster-tool-codebeamer-0.9.1/
--rw-r--r--   0 florian   (1000) florian   (1000)     1754 2023-05-03 14:22:58.152383 bmw-lobster-tool-codebeamer-0.9.1/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      814 2023-05-03 14:09:11.000000 bmw-lobster-tool-codebeamer-0.9.1/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:58.148383 bmw-lobster-tool-codebeamer-0.9.1/bmw_lobster_tool_codebeamer.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     1754 2023-05-03 14:22:58.000000 bmw-lobster-tool-codebeamer-0.9.1/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      402 2023-05-03 14:22:58.000000 bmw-lobster-tool-codebeamer-0.9.1/bmw_lobster_tool_codebeamer.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-03 14:22:58.000000 bmw-lobster-tool-codebeamer-0.9.1/bmw_lobster_tool_codebeamer.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       80 2023-05-03 14:22:58.000000 bmw-lobster-tool-codebeamer-0.9.1/bmw_lobster_tool_codebeamer.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       39 2023-05-03 14:22:58.000000 bmw-lobster-tool-codebeamer-0.9.1/bmw_lobster_tool_codebeamer.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-05-03 14:22:58.000000 bmw-lobster-tool-codebeamer-0.9.1/bmw_lobster_tool_codebeamer.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:58.148383 bmw-lobster-tool-codebeamer-0.9.1/lobster/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:58.148383 bmw-lobster-tool-codebeamer-0.9.1/lobster/tools/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:58.152383 bmw-lobster-tool-codebeamer-0.9.1/lobster/tools/codebeamer/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-03 14:09:11.000000 bmw-lobster-tool-codebeamer-0.9.1/lobster/tools/codebeamer/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     7865 2023-05-03 14:09:11.000000 bmw-lobster-tool-codebeamer-0.9.1/lobster/tools/codebeamer/codebeamer.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-03 14:22:58.152383 bmw-lobster-tool-codebeamer-0.9.1/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2296 2023-05-03 14:09:11.000000 bmw-lobster-tool-codebeamer-0.9.1/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:39.273490 bmw-lobster-tool-codebeamer-0.9.2/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1754 2023-05-08 15:06:39.273490 bmw-lobster-tool-codebeamer-0.9.2/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      814 2023-05-08 15:03:18.000000 bmw-lobster-tool-codebeamer-0.9.2/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:39.273490 bmw-lobster-tool-codebeamer-0.9.2/bmw_lobster_tool_codebeamer.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1754 2023-05-08 15:06:39.000000 bmw-lobster-tool-codebeamer-0.9.2/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      402 2023-05-08 15:06:39.000000 bmw-lobster-tool-codebeamer-0.9.2/bmw_lobster_tool_codebeamer.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-08 15:06:39.000000 bmw-lobster-tool-codebeamer-0.9.2/bmw_lobster_tool_codebeamer.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       80 2023-05-08 15:06:39.000000 bmw-lobster-tool-codebeamer-0.9.2/bmw_lobster_tool_codebeamer.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       39 2023-05-08 15:06:39.000000 bmw-lobster-tool-codebeamer-0.9.2/bmw_lobster_tool_codebeamer.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-05-08 15:06:39.000000 bmw-lobster-tool-codebeamer-0.9.2/bmw_lobster_tool_codebeamer.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:39.273490 bmw-lobster-tool-codebeamer-0.9.2/lobster/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:39.273490 bmw-lobster-tool-codebeamer-0.9.2/lobster/tools/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:39.273490 bmw-lobster-tool-codebeamer-0.9.2/lobster/tools/codebeamer/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:39.000000 bmw-lobster-tool-codebeamer-0.9.2/lobster/tools/codebeamer/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     7902 2023-05-08 15:06:39.000000 bmw-lobster-tool-codebeamer-0.9.2/lobster/tools/codebeamer/codebeamer.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-08 15:06:39.273490 bmw-lobster-tool-codebeamer-0.9.2/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2296 2023-05-08 15:03:18.000000 bmw-lobster-tool-codebeamer-0.9.2/setup.py
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.1/PKG-INFO` & `bmw-lobster-tool-codebeamer-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-codebeamer
-Version: 0.9.1
+Version: 0.9.2
 Summary: LOBSTER Tool for Codebeamer
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.1/README.md` & `bmw-lobster-tool-codebeamer-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `bmw-lobster-tool-codebeamer-0.9.1/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO` & `bmw-lobster-tool-codebeamer-0.9.2/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-codebeamer
-Version: 0.9.1
+Version: 0.9.2
 Summary: LOBSTER Tool for Codebeamer
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.1/lobster/tools/codebeamer/codebeamer.py` & `bmw-lobster-tool-codebeamer-0.9.2/lobster/tools/codebeamer/codebeamer.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,39 +35,40 @@
 #
 # However you _can_ import all the items referenced from another
 # lobster artefact.
 
 import os
 import sys
 import argparse
-import json
 
 from copy import copy
 
+import requests
+
 from lobster.items import Tracing_Tag, Requirement
 from lobster.location import Codebeamer_Reference
 from lobster.errors import Message_Handler, LOBSTER_Error
 from lobster.io import lobster_read, lobster_write
 
-import requests
-
 
 def query_cb_single(cb_config, url):
     assert isinstance(cb_config, dict)
     assert isinstance(url, str)
 
-    r = requests.get(url, auth=(cb_config["user"],
-                                cb_config["pass"]))
-    if r.status_code != 200:
+    result = requests.get(url,
+                          auth=(cb_config["user"],
+                                cb_config["pass"]),
+                          timeout=10.0)
+    if result.status_code != 200:
         print("Could not fetch %s" % url)
-        print("Status = %u" % r.status_code)
-        print(r.text)
+        print("Status = %u" % result.status_code)
+        print(result.text)
         sys.exit(1)
 
-    return r.json()
+    return result.json()
 
 
 def get_single_item(cb_config, item_id):
     assert isinstance(item_id, int) and item_id > 0
 
     url = "%s/item/%u" % (cb_config["base"],
                           item_id)
@@ -148,16 +149,16 @@
 
             cb_item    = get_single_item(cb_config, target)
             l_item     = to_lobster(cb_config, cb_item)
             tracker_id = l_item.location.tracker
             rv.append(l_item)
 
         else:
-            print("Attempting to fetch %u items from %u" % (len(work_list),
-                                                            tracker_id))
+            print("Attempting to fetch %u items from %s" %
+                  (len(work_list), tracker_id))
             cb_items = get_many_items_maybe(cb_config, tracker_id, work_list)
 
             for cb_item in cb_items:
                 l_item = to_lobster(cb_config, cb_item)
                 assert tracker_id == l_item.location.tracker
                 rv.append(l_item)
                 work_list.remove(l_item.location.item)
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.1/setup.py` & `bmw-lobster-tool-codebeamer-0.9.2/setup.py`

 * *Files identical despite different names*

