# Comparing `tmp/kalm-0.4.3.tar.gz` & `tmp/kalm-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.4.3.tar", max compression
+gzip compressed data, was "kalm-0.4.4.tar", max compression
```

## Comparing `kalm-0.4.3.tar` & `kalm-0.4.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1081 2023-05-05 20:49:24.880279 kalm-0.4.3/LICENSE.txt
--rw-r--r--   0        0        0     1832 2023-05-08 13:32:39.302817 kalm-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    10663 2023-05-08 13:32:39.302817 kalm-0.4.3/src/kalm/__init__.py
--rw-r--r--   0        0        0    32308 2023-05-08 13:21:45.550993 kalm-0.4.3/src/kalm/kalm.py
--rw-r--r--   0        0        0     6484 2023-05-05 20:49:24.884279 kalm-0.4.3/src/kalm/kalm_api.py
--rw-r--r--   0        0        0     1296 2023-05-05 20:49:24.884279 kalm-0.4.3/src/kalm/netbox.py
--rw-r--r--   0        0        0        9 2023-05-05 20:49:24.884279 kalm-0.4.3/src/kalm/package_data.dat
--rw-r--r--   0        0        0      312 2023-05-05 20:49:24.884279 kalm-0.4.3/src/kalm/toolbox.py
--rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 kalm-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-05 20:49:24.880279 kalm-0.4.4/LICENSE.txt
+-rw-r--r--   0        0        0     1832 2023-05-08 13:35:45.619909 kalm-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0    10663 2023-05-08 13:34:59.939641 kalm-0.4.4/src/kalm/__init__.py
+-rw-r--r--   0        0        0    32308 2023-05-08 13:21:45.550993 kalm-0.4.4/src/kalm/kalm.py
+-rw-r--r--   0        0        0     6484 2023-05-05 20:49:24.884279 kalm-0.4.4/src/kalm/kalm_api.py
+-rw-r--r--   0        0        0     1296 2023-05-05 20:49:24.884279 kalm-0.4.4/src/kalm/netbox.py
+-rw-r--r--   0        0        0        9 2023-05-05 20:49:24.884279 kalm-0.4.4/src/kalm/package_data.dat
+-rw-r--r--   0        0        0      312 2023-05-05 20:49:24.884279 kalm-0.4.4/src/kalm/toolbox.py
+-rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 kalm-0.4.4/PKG-INFO
```

### Comparing `kalm-0.4.3/LICENSE.txt` & `kalm-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.4.3/pyproject.toml` & `kalm-0.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kalm"
-version = "0.4.3"
+version = "0.4.4"
 description = "Knowit Automation lifecycle management"
 authors = ["Jakob Holst <jakob.holst@knowit.dk>"]
 license = "MIT"
 homepage = "https://kalm.openknowit.com"
 repository = "https://github.com/miracle-as/openknowit_kalm.git"
 
 [tool.poetry.scripts]
```

### Comparing `kalm-0.4.3/src/kalm/__init__.py` & `kalm-0.4.4/src/kalm/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,14 @@
                \
                2023 Knowit Miracle\
                ")
     parser.add_argument('action', metavar='<action>', type=str, nargs='+', help='setup netbox')
     args = parser.parse_args()
     ready = False
     print("check if we are ready to go")
-    ready  = connectiontest()
 
     if args.action[0] == "jenkins":
         if ready:
             print("Jenkins adminitrator")
             kalm.jenkins()
 
             exit(0)
@@ -215,14 +214,15 @@
             kalm.kalm(token, r)
             print("Daemon sleeping")
             time.sleep(60)
             
 
             
 
+    ready  = connectiontest()
 
     if ready and args.action[0] == "initservice":
         print("Init service")
         r = redis.Redis()
         r.flushdb()
         result = runme("/usr/local/bin/awx --conf.color False tokens create |jq '{'id': .id, 'token': .token }")
         parsed_json = json.loads(result["stdout"])
```

### Comparing `kalm-0.4.3/src/kalm/kalm.py` & `kalm-0.4.4/src/kalm/kalm.py`

 * *Files identical despite different names*

### Comparing `kalm-0.4.3/src/kalm/kalm_api.py` & `kalm-0.4.4/src/kalm/kalm_api.py`

 * *Files identical despite different names*

### Comparing `kalm-0.4.3/src/kalm/netbox.py` & `kalm-0.4.4/src/kalm/netbox.py`

 * *Files identical despite different names*

### Comparing `kalm-0.4.3/PKG-INFO` & `kalm-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.4.3
+Version: 0.4.4
 Summary: Knowit Automation lifecycle management
 Home-page: https://kalm.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

