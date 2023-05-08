# Comparing `tmp/openstg-1.12.0.tar.gz` & `tmp/openstg-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openstg-1.12.0.tar", last modified: Mon May  8 13:26:11 2023, max compression
+gzip compressed data, was "dist/openstg-1.2.0.tar", last modified: Thu Feb 27 08:51:19 2020, max compression
```

## Comparing `openstg-1.12.0.tar` & `openstg-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,24 @@
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2023-05-08 13:26:11.000000 openstg-1.12.0/
--rw-rw-r--   0 afita     (1000) afita     (1000)      291 2023-05-08 13:26:11.000000 openstg-1.12.0/PKG-INFO
--rw-rw-r--   0 afita     (1000) afita     (1000)       38 2023-05-08 13:26:11.000000 openstg-1.12.0/setup.cfg
--rw-rw-r--   0 afita     (1000) afita     (1000)      648 2023-05-08 13:25:02.000000 openstg-1.12.0/setup.py
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2023-05-08 13:26:11.000000 openstg-1.12.0/openstg/
--rw-r--r--   0 afita     (1000) afita     (1000)      210 2020-07-07 08:22:35.000000 openstg-1.12.0/openstg/app.py
--rw-r--r--   0 afita     (1000) afita     (1000)     1102 2020-02-27 08:49:02.000000 openstg-1.12.0/openstg/SqliteCounter.py
--rw-rw-r--   0 afita     (1000) afita     (1000)     6205 2022-03-17 15:08:50.000000 openstg-1.12.0/openstg/ws_stg.py
--rw-r--r--   0 afita     (1000) afita     (1000)      218 2020-07-07 08:22:35.000000 openstg-1.12.0/openstg/stgapp.py
--rw-r--r--   0 afita     (1000) afita     (1000)     1381 2020-02-27 08:49:02.000000 openstg-1.12.0/openstg/utils.py
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2023-05-08 13:26:11.000000 openstg-1.12.0/openstg/api/
--rw-rw-r--   0 afita     (1000) afita     (1000)    33775 2023-05-08 13:24:43.000000 openstg-1.12.0/openstg/api/__init__.py
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2023-05-08 13:26:11.000000 openstg-1.12.0/openstg/serializers/
--rw-rw-r--   0 afita     (1000) afita     (1000)      855 2023-05-08 13:24:43.000000 openstg-1.12.0/openstg/serializers/__init__.py
--rw-r--r--   0 afita     (1000) afita     (1000)       14 2020-02-27 08:49:02.000000 openstg-1.12.0/openstg/__init__.py
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2023-05-08 13:26:11.000000 openstg-1.12.0/openstg/models/
--rw-rw-r--   0 afita     (1000) afita     (1000)     1862 2023-05-08 13:24:43.000000 openstg-1.12.0/openstg/models/__init__.py
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2023-05-08 13:26:11.000000 openstg-1.12.0/openstg/stg/
--rw-r--r--   0 afita     (1000) afita     (1000)     4943 2020-07-07 08:22:35.000000 openstg-1.12.0/openstg/stg/__init__.py
--rw-rw-r--   0 afita     (1000) afita     (1000)     2114 2023-05-08 13:22:28.000000 openstg-1.12.0/openstg/config.py
--rw-rw-r--   0 afita     (1000) afita     (1000)     4170 2022-10-25 18:11:13.000000 openstg-1.12.0/openstg/erpapi.py
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2023-05-08 13:26:11.000000 openstg-1.12.0/openstg.egg-info/
--rw-r--r--   0 afita     (1000) afita     (1000)        8 2023-05-08 13:26:11.000000 openstg-1.12.0/openstg.egg-info/top_level.txt
--rw-r--r--   0 afita     (1000) afita     (1000)      428 2023-05-08 13:26:11.000000 openstg-1.12.0/openstg.egg-info/SOURCES.txt
--rw-r--r--   0 afita     (1000) afita     (1000)      291 2023-05-08 13:26:11.000000 openstg-1.12.0/openstg.egg-info/PKG-INFO
--rw-r--r--   0 afita     (1000) afita     (1000)        1 2023-05-08 13:26:11.000000 openstg-1.12.0/openstg.egg-info/dependency_links.txt
--rw-r--r--   0 afita     (1000) afita     (1000)      154 2023-05-08 13:26:11.000000 openstg-1.12.0/openstg.egg-info/requires.txt
--rw-r--r--   0 afita     (1000) afita     (1000)      380 2020-07-07 08:22:35.000000 openstg-1.12.0/README.md
+drwxr-xr-x   0 afita     (1000) afita     (1000)        0 2020-02-27 08:51:19.000000 openstg-1.2.0/
+-rw-r--r--   0 afita     (1000) afita     (1000)      290 2020-02-27 08:51:19.000000 openstg-1.2.0/PKG-INFO
+-rw-r--r--   0 afita     (1000) afita     (1000)       38 2020-02-27 08:51:19.000000 openstg-1.2.0/setup.cfg
+-rw-r--r--   0 afita     (1000) afita     (1000)      653 2020-02-27 08:49:24.000000 openstg-1.2.0/setup.py
+drwxr-xr-x   0 afita     (1000) afita     (1000)        0 2020-02-27 08:51:19.000000 openstg-1.2.0/openstg/
+-rw-r--r--   0 afita     (1000) afita     (1000)      163 2020-02-27 08:49:02.000000 openstg-1.2.0/openstg/app.py
+-rw-r--r--   0 afita     (1000) afita     (1000)     4672 2020-02-27 08:49:02.000000 openstg-1.2.0/openstg/server.py
+-rw-r--r--   0 afita     (1000) afita     (1000)     1102 2020-02-27 08:49:02.000000 openstg-1.2.0/openstg/SqliteCounter.py
+-rw-r--r--   0 afita     (1000) afita     (1000)     1381 2020-02-27 08:49:02.000000 openstg-1.2.0/openstg/utils.py
+drwxr-xr-x   0 afita     (1000) afita     (1000)        0 2020-02-27 08:51:19.000000 openstg-1.2.0/openstg/api/
+-rw-r--r--   0 afita     (1000) afita     (1000)    19729 2020-02-27 08:49:02.000000 openstg-1.2.0/openstg/api/__init__.py
+drwxr-xr-x   0 afita     (1000) afita     (1000)        0 2020-02-27 08:51:19.000000 openstg-1.2.0/openstg/serializers/
+-rw-r--r--   0 afita     (1000) afita     (1000)      687 2020-02-27 08:49:02.000000 openstg-1.2.0/openstg/serializers/__init__.py
+-rw-r--r--   0 afita     (1000) afita     (1000)       14 2020-02-27 08:49:02.000000 openstg-1.2.0/openstg/__init__.py
+drwxr-xr-x   0 afita     (1000) afita     (1000)        0 2020-02-27 08:51:19.000000 openstg-1.2.0/openstg/models/
+-rw-r--r--   0 afita     (1000) afita     (1000)     1771 2020-02-27 08:49:02.000000 openstg-1.2.0/openstg/models/__init__.py
+-rw-r--r--   0 afita     (1000) afita     (1000)     1568 2020-02-27 08:49:02.000000 openstg-1.2.0/openstg/config.py
+drwxr-xr-x   0 afita     (1000) afita     (1000)        0 2020-02-27 08:51:19.000000 openstg-1.2.0/openstg.egg-info/
+-rw-r--r--   0 afita     (1000) afita     (1000)        8 2020-02-27 08:51:19.000000 openstg-1.2.0/openstg.egg-info/top_level.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)      368 2020-02-27 08:51:19.000000 openstg-1.2.0/openstg.egg-info/SOURCES.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)      290 2020-02-27 08:51:19.000000 openstg-1.2.0/openstg.egg-info/PKG-INFO
+-rw-r--r--   0 afita     (1000) afita     (1000)        1 2020-02-27 08:51:19.000000 openstg-1.2.0/openstg.egg-info/dependency_links.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)      160 2020-02-27 08:51:19.000000 openstg-1.2.0/openstg.egg-info/requires.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)       98 2020-02-27 08:49:02.000000 openstg-1.2.0/README.md
```

### Comparing `openstg-1.12.0/setup.py` & `openstg-1.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='openstg',
-    version='1.12.0',
+    version='1.2.0',
     packages=find_packages(),
     url='https://github.com/gisce/openstg',
     license='GNU Affero General Public License v3',
     author='GISCE-TI, S.L.',
     author_email='devel@gisce.net',
     install_requires=[
-        'ERPpeek',
+        'ERPpeek==1.6.3',
         'Flask==0.12.2',
         'Flask-Cors==3.0.2',
         'Flask-Login==0.2.11',
         'Flask-RESTful==0.3.5',
         'flask-restplus==0.10.1',
-        'primestg>=1.32.0',
+        'primestg>=1.3.0',
         'marshmallow<3',
         'osconf==0.1.3',
         'pytz',
     ],
     description='API for STG-Protocol-DC Interface Specification'
 )
```

### Comparing `openstg-1.12.0/openstg/SqliteCounter.py` & `openstg-1.2.0/openstg/SqliteCounter.py`

 * *Files identical despite different names*

### Comparing `openstg-1.12.0/openstg/utils.py` & `openstg-1.2.0/openstg/utils.py`

 * *Files identical despite different names*

### Comparing `openstg-1.12.0/openstg/serializers/__init__.py` & `openstg-1.2.0/openstg/serializers/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,17 +7,14 @@
     name = fields.Str(attribute="name")
     ip_address = fields.Str(attribute="ip_address")
     model = fields.Str(attribute="model")
     type = fields.Str(attribute="type")
     dc_address = fields.Str(attribute="dc_ws_address")
     ws_ip = fields.Str(attribute="stg_ws_ip_address")
     ws_pass = fields.Str(attribute="stg_ws_password")
-    ws_version = fields.Str(attribute="dc_ws_stg_version")
-    admin_pass = fields.Str(attribute="w_password")
-    web_address = fields.Str(attribute="dc_web_address")
 
 
 class RegisterSchema(Schema):
     id = fields.Int()
     number = fields.Str()
     name = fields.Str(attribute="name")
     tg_name = fields.Str(attribute="name")
```

### Comparing `openstg-1.12.0/openstg/models/__init__.py` & `openstg-1.2.0/openstg/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,29 +42,26 @@
         'type',
         'w_password',
         'r_password',
         'fw_version',
         'fw_comm_version',
         'protocol',
         'communication',
-        'dc_web_address',
         'dc_ws_address',
         'stg_ws_ip_address',
         'stg_ws_password',
         'modem_user',
         'modem_password',
-        'dc_ws_stg_version',
     ])
     serializer = ConcentratorSchema()
 
 
 class RegisterModel(Model):
     model = 'giscedata.registrador'
     schema = unflatdot([
         'name',
         'cnc_id.id',
         'cnc_id.name',
         'cnc_id.ip_address',
         'cnc_id.dc_ws_address',
-        'cnc_id.dc_ws_stg_version',
     ])
     serializer = RegisterSchema()
```

### Comparing `openstg-1.12.0/openstg/stg/__init__.py` & `openstg-1.2.0/openstg/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# coding: utf-8
 from flask import Flask, request
-from flask_restplus import Api, Resource
 import xml.dom.minidom as xmlmd
 import time
 import os
-
+app = Flask(__name__)
 
 dc_status = {
         '0': "SUCCESS: The request with ID {} for the concentrator {} have "
              "finished successfully. {}",
         '1': "WORKING: The request with ID {} for the concentrator {} is "
              "still in progress. {}",
         '2': "ERROR: The request with ID {} for the concentrator {} has "
@@ -41,41 +39,31 @@
              "ID {}. But any report after it is missing",
         '3': "ERROR: The meter {} couldn't finish serving the request with "
              "ID {}. Order partially applied (part of the data sent in the "
              "order were not correctly applied in the meter)."
     }
 
 
-class Stg(Api):
-    def _register_doc(self, app_or_blueprint):
-        #We have to
-        pass
-
-
 def getText(nodelist):
     rc = []
     for node in nodelist:
         if node.nodeType == node.TEXT_NODE:
             rc.append(node.data)
     return ''.join(rc)
 
 
-class WSStgResource(Resource):
-
-    def post(self):
-        f_name = '/tmp/post-{}'.format(time.time())
-        if isinstance(request.data, bytes):
-            # Python3 backwards compatibility
-            request.data = request.data.decode()
-        with open(f_name, 'w') as f:
-            f.write(request.data)
-        out_msg = manage_request()
-        os.remove(f_name)
-        print(out_msg)
-        return "Ok", 200
+@app.route('/', methods=['POST'])
+def allrequests():
+    f_name = 'post-{}'.format(time.time())
+    with open(f_name, 'w') as f:
+        f.write(request.data)
+    out_msg = manage_request()
+    os.remove(f_name)
+    print out_msg
+    return "Ok", 200
 
 
 def manage_request_status(info):
     if 'Reference' not in info:
         info['Reference'] = ''
     default = "ERROR: The request with ID {} for the concentrator {}. has " \
               "suffered an UNKNOWN error {}".format(info['IdPet'],
@@ -124,10 +112,9 @@
         dc_status.get(info['ReqStatus'], default).format(info['IdPet'],
                                                          info['IdDC'],
                                                          info['Reference']))
 
     # TODO: Connect to ERP to read the S15 report received
 
 
-resources = [
-    (WSStgResource, '/ws')
-]
+if __name__ == '__main__':
+    app.run(host='0.0.0.0', port=5656, debug=True)
```

