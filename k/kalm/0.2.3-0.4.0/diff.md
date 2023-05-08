# Comparing `tmp/kalm-0.2.3.tar.gz` & `tmp/kalm-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.2.3.tar", max compression
+gzip compressed data, was "kalm-0.4.0.tar", max compression
```

## Comparing `kalm-0.2.3.tar` & `kalm-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1081 2023-05-08 11:54:16.776225 kalm-0.2.3/LICENSE.txt
--rw-r--r--   0        0        0     1817 2023-05-08 12:31:22.493176 kalm-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    10616 2023-05-08 12:31:22.493176 kalm-0.2.3/src/kalm/__init__.py
--rw-r--r--   0        0        0    32858 2023-05-08 12:31:22.493176 kalm-0.2.3/src/kalm/kalm.py
--rw-r--r--   0        0        0     6484 2023-05-08 11:54:16.776225 kalm-0.2.3/src/kalm/kalm_api.py
--rw-r--r--   0        0        0     1296 2023-05-08 11:54:16.776225 kalm-0.2.3/src/kalm/netbox.py
--rw-r--r--   0        0        0        9 2023-05-08 11:54:16.776225 kalm-0.2.3/src/kalm/package_data.dat
--rw-r--r--   0        0        0      312 2023-05-08 11:54:16.776225 kalm-0.2.3/src/kalm/toolbox.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-05 20:49:24.880279 kalm-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     1832 2023-05-08 13:16:21.377102 kalm-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    10421 2023-05-05 20:49:24.884279 kalm-0.4.0/src/kalm/__init__.py
+-rw-r--r--   0        0        0    32306 2023-05-06 18:34:39.159664 kalm-0.4.0/src/kalm/kalm.py
+-rw-r--r--   0        0        0     6484 2023-05-05 20:49:24.884279 kalm-0.4.0/src/kalm/kalm_api.py
+-rw-r--r--   0        0        0     1296 2023-05-05 20:49:24.884279 kalm-0.4.0/src/kalm/netbox.py
+-rw-r--r--   0        0        0        9 2023-05-05 20:49:24.884279 kalm-0.4.0/src/kalm/package_data.dat
+-rw-r--r--   0        0        0      312 2023-05-05 20:49:24.884279 kalm-0.4.0/src/kalm/toolbox.py
+-rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 kalm-0.4.0/PKG-INFO
```

### Comparing `kalm-0.2.3/LICENSE.txt` & `kalm-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.2.3/pyproject.toml` & `kalm-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "kalm"
-version = "0.2.3"
+version = "0.4.0"
 description = "Knowit Automation lifecycle management"
 authors = ["Jakob Holst <jakob.holst@knowit.dk>"]
 license = "MIT"
 homepage = "https://kalm.openknowit.com"
 repository = "https://github.com/miracle-as/openknowit_kalm.git"
 
+[tool.poetry.scripts]
+kalm = "kalm:main"
+
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.25"
 pytest = "^6.2"
 mypy = "^0.910"
 redis = "^4.5.3"
 pynetbox = "^6.6.2"
 wheel = "^0.34.2"
 hvac = "^1.1.0"
 netbox = "^0.0.2"
-python-jenkins = "^1.7.0"
-
 
 
 [project]
 name = "kalm"  
 version = "0.2.0-Development" 
 description = "Knowit automation lifecycle management"
 readme = "README.md" # Optional
```

### Comparing `kalm-0.2.3/src/kalm/__init__.py` & `kalm-0.4.0/src/kalm/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from kalm import kalm
-
 import os
 import sys
 import redis
 import time
 import subprocess
 import json
 import argparse
@@ -151,28 +150,27 @@
     else:
         return True
 
 
 def main():
     parser = argparse.ArgumentParser(description="Keep kalm and automate", usage="kalm <action> \n\n \
                \
-               version : 0.2.2 BETA \n                                              \
+               version : 0.1.2 BETA \n                                              \
                actions:\n                                                      \
                core           Run kalm using the core/initial process to ensure the core environment is intact (/etc/kalm/kalm.json)\n  \
                seeder         Run kalm using the config files in (/etc/kalm.d)\n  \
                seed           Run kalm using the config specific configuration\n  \
                check          check access to core services defined\n  \
                setup          setup access to core services defined\n  \
                netbox         Run kalm to update netbox configured in /etc/kalm/netbox.json \n  \
                service        Run kalm from systemd service \n  \
                initservice    setup kalm systemd service \n  \
                stopservice    disable and cleanup kalm systemd service \n  \
                startservice   setup and enable kalm systemd service \n  \
                deploy         deploy an ansible tower, awx, awxrpm \n  \
-               jenkins        Control a jenkins instance \n  \
                \
                2023 Knowit Miracle\
                ")
     parser.add_argument('action', metavar='<action>', type=str, nargs='+', help='setup netbox')
     args = parser.parse_args()
     ready = False
     print("check if we are ready to go")
@@ -260,19 +258,13 @@
 
     if ready and ( args.action[0] == "reset" or args.action[0] == "init"):
         r = redis.Redis()
         r.flushdb()
         ansibletoken = os.getenv("ANSIBLE_TOKEN")
         kalm.kalm(ansibletoken, r)
 
-    if  ( args.action[0] == "jenkins"):
-        r = redis.Redis()
-        r.flushdb()
-        kalm.kalm_jenkins(ansibletoken, r)
-
-
```

### Comparing `kalm-0.2.3/src/kalm/kalm.py` & `kalm-0.4.0/src/kalm/kalm.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import datetime
 
 def prettyllog(function, action, item, organization, statuscode, text):
   d_date = datetime.datetime.now()
   reg_format_date = d_date.strftime("%Y-%m-%d %I:%M:%S %p")
   print("%-20s: %-12s %20s %-50s %-20s %-4s %-50s " %( reg_format_date, function,action,item,organization,statuscode, text))
 
-def dummy():
+def dummy:
     print("dummy")
 
 #def prettyllog(function, action, item, organization, statuscode, text):
  # d_date = datetime.datetime.now()
  # reg_format_date = d_date.strftime("%Y-%m-%d %I:%M:%S %p")
  # print("%-20s: %-12s %20s %-50s %-20s %-4s %-50s " %( reg_format_date, function,action,item,organization,statuscode, text))
 
@@ -611,29 +611,14 @@
 # function: Refresh AWX data
 ######################################
 def refresh_awx_data(mytoken,r ):
   items = {"organizations", "projects", "credentials", "hosts", "inventories", "credential_types", "labels" , "instance_groups", "job_templates"}    
   for item in items:
     getawxdata(item, mytoken, r)
 
-import jenkins
-
-def kalm_jenkins(mytoken, r):
-  prettyllog("init", "runtime", "config", "init", "001", "initiating jenkins")
-  jenkinsusername = os.getenv('JENKINS_USERNAME')
-  jenkinspassword = os.getenv('JENKINS_PASSWORD')
-  server = jenkins.Jenkins('https://jenkins.openknowit.com', username=jenkinsusername, password=jenkinspassword)
-  prettyllog("init", "runtime", "config", "init", "001", "jenkins initiated")
-  user = server.get_whoami()
-  version = server.get_version()
-  print('Hello %s from Jenkins %s' % (user['fullName'], version))
-  
-
-
-
 
 ########################################################################################################################
 # Main:  start
 ########################################################################################################################
 
 def kalm(mytoken, r):
```

### Comparing `kalm-0.2.3/src/kalm/kalm_api.py` & `kalm-0.4.0/src/kalm/kalm_api.py`

 * *Files identical despite different names*

### Comparing `kalm-0.2.3/src/kalm/netbox.py` & `kalm-0.4.0/src/kalm/netbox.py`

 * *Files identical despite different names*

### Comparing `kalm-0.2.3/PKG-INFO` & `kalm-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.2.3
+Version: 0.4.0
 Summary: Knowit Automation lifecycle management
 Home-page: https://kalm.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,12 +14,11 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: hvac (>=1.1.0,<2.0.0)
 Requires-Dist: mypy (>=0.910,<0.911)
 Requires-Dist: netbox (>=0.0.2,<0.0.3)
 Requires-Dist: pynetbox (>=6.6.2,<7.0.0)
 Requires-Dist: pytest (>=6.2,<7.0)
-Requires-Dist: python-jenkins (>=1.7.0,<2.0.0)
 Requires-Dist: redis (>=4.5.3,<5.0.0)
 Requires-Dist: requests (>=2.25,<3.0)
 Requires-Dist: wheel (>=0.34.2,<0.35.0)
 Project-URL: Repository, https://github.com/miracle-as/openknowit_kalm.git
```

