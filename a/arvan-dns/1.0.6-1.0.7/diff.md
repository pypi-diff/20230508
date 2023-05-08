# Comparing `tmp/arvan_dns-1.0.6.tar.gz` & `tmp/arvan_dns-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arvan_dns-1.0.6.tar", last modified: Mon May  8 10:35:27 2023, max compression
+gzip compressed data, was "arvan_dns-1.0.7.tar", last modified: Mon May  8 10:37:46 2023, max compression
```

## Comparing `arvan_dns-1.0.6.tar` & `arvan_dns-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 seyed      (501) staff       (20)        0 2023-05-08 10:35:27.839925 arvan_dns-1.0.6/
--rw-r--r--   0 seyed      (501) staff       (20)       56 2023-05-08 03:35:00.000000 arvan_dns-1.0.6/.gitignore
--rw-r--r--   0 seyed      (501) staff       (20)      841 2023-05-08 10:35:27.839752 arvan_dns-1.0.6/PKG-INFO
--rw-r--r--   0 seyed      (501) staff       (20)      588 2023-05-07 13:06:38.000000 arvan_dns-1.0.6/README.md
--rw-r--r--   0 seyed      (501) staff       (20)        0 2023-05-06 19:41:19.000000 arvan_dns-1.0.6/__init__.py
-drwxr-xr-x   0 seyed      (501) staff       (20)        0 2023-05-08 10:35:27.839537 arvan_dns-1.0.6/arvan_dns.egg-info/
--rw-r--r--   0 seyed      (501) staff       (20)      841 2023-05-08 10:35:27.000000 arvan_dns-1.0.6/arvan_dns.egg-info/PKG-INFO
--rw-r--r--   0 seyed      (501) staff       (20)      254 2023-05-08 10:35:27.000000 arvan_dns-1.0.6/arvan_dns.egg-info/SOURCES.txt
--rw-r--r--   0 seyed      (501) staff       (20)        1 2023-05-08 10:35:27.000000 arvan_dns-1.0.6/arvan_dns.egg-info/dependency_links.txt
--rw-r--r--   0 seyed      (501) staff       (20)       45 2023-05-08 10:35:27.000000 arvan_dns-1.0.6/arvan_dns.egg-info/entry_points.txt
--rw-r--r--   0 seyed      (501) staff       (20)       18 2023-05-08 10:35:27.000000 arvan_dns-1.0.6/arvan_dns.egg-info/requires.txt
--rw-r--r--   0 seyed      (501) staff       (20)       10 2023-05-08 10:35:27.000000 arvan_dns-1.0.6/arvan_dns.egg-info/top_level.txt
--rw-r--r--   0 seyed      (501) staff       (20)     5070 2023-05-08 10:33:54.000000 arvan_dns-1.0.6/arvan_dns.py
--rw-r--r--   0 seyed      (501) staff       (20)       38 2023-05-08 10:35:27.839968 arvan_dns-1.0.6/setup.cfg
--rw-r--r--   0 seyed      (501) staff       (20)      533 2023-05-08 10:34:58.000000 arvan_dns-1.0.6/setup.py
+drwxr-xr-x   0 seyed      (501) staff       (20)        0 2023-05-08 10:37:46.375067 arvan_dns-1.0.7/
+-rw-r--r--   0 seyed      (501) staff       (20)       56 2023-05-08 03:35:00.000000 arvan_dns-1.0.7/.gitignore
+-rw-r--r--   0 seyed      (501) staff       (20)      853 2023-05-08 10:37:46.374883 arvan_dns-1.0.7/PKG-INFO
+-rw-r--r--   0 seyed      (501) staff       (20)      600 2023-05-08 10:36:52.000000 arvan_dns-1.0.7/README.md
+-rw-r--r--   0 seyed      (501) staff       (20)        0 2023-05-06 19:41:19.000000 arvan_dns-1.0.7/__init__.py
+drwxr-xr-x   0 seyed      (501) staff       (20)        0 2023-05-08 10:37:46.374631 arvan_dns-1.0.7/arvan_dns.egg-info/
+-rw-r--r--   0 seyed      (501) staff       (20)      853 2023-05-08 10:37:46.000000 arvan_dns-1.0.7/arvan_dns.egg-info/PKG-INFO
+-rw-r--r--   0 seyed      (501) staff       (20)      254 2023-05-08 10:37:46.000000 arvan_dns-1.0.7/arvan_dns.egg-info/SOURCES.txt
+-rw-r--r--   0 seyed      (501) staff       (20)        1 2023-05-08 10:37:46.000000 arvan_dns-1.0.7/arvan_dns.egg-info/dependency_links.txt
+-rw-r--r--   0 seyed      (501) staff       (20)       45 2023-05-08 10:37:46.000000 arvan_dns-1.0.7/arvan_dns.egg-info/entry_points.txt
+-rw-r--r--   0 seyed      (501) staff       (20)       18 2023-05-08 10:37:46.000000 arvan_dns-1.0.7/arvan_dns.egg-info/requires.txt
+-rw-r--r--   0 seyed      (501) staff       (20)       10 2023-05-08 10:37:46.000000 arvan_dns-1.0.7/arvan_dns.egg-info/top_level.txt
+-rw-r--r--   0 seyed      (501) staff       (20)     5070 2023-05-08 10:33:54.000000 arvan_dns-1.0.7/arvan_dns.py
+-rw-r--r--   0 seyed      (501) staff       (20)       38 2023-05-08 10:37:46.375123 arvan_dns-1.0.7/setup.cfg
+-rw-r--r--   0 seyed      (501) staff       (20)      533 2023-05-08 10:36:58.000000 arvan_dns-1.0.7/setup.py
```

### Comparing `arvan_dns-1.0.6/PKG-INFO` & `arvan_dns-1.0.7/arvan_dns.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: arvan_dns
-Version: 1.0.6
+Name: arvan-dns
+Version: 1.0.7
 Summary: Arvan DNS updater
 Home-page: https://github.com/seyed-dev/arvan-dns
 Author: SeYeD.DeV
 Author-email: me@seyed.dev
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -28,15 +28,15 @@
 example.ir
 example.net
 ```
 
 ### run the command
 
 ```bash
-arvan-dns --bearer_token=<your bearer_token> --old_ip=<your old ip> --new_ip=<your new ip> --port=<your new port> --domains_file=<your domains file>
+arvan-dns --email=<your email> --password=your password> --old_ip=<your old ip> --new_ip=<your new ip> --port=<your new port> --domains_file=<your domains file>
 ```
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `arvan_dns-1.0.6/README.md` & `arvan_dns-1.0.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: arvan_dns
+Version: 1.0.7
+Summary: Arvan DNS updater
+Home-page: https://github.com/seyed-dev/arvan-dns
+Author: SeYeD.DeV
+Author-email: me@seyed.dev
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
 # DNS Manager For ArvanCloud
 
 This is a simple python script to change the ip of your domains in ArvanCloud DNS Manager.
 
 ## Installation
 
 ```bash
@@ -17,13 +28,15 @@
 example.ir
 example.net
 ```
 
 ### run the command
 
 ```bash
-arvan-dns --bearer_token=<your bearer_token> --old_ip=<your old ip> --new_ip=<your new ip> --port=<your new port> --domains_file=<your domains file>
+arvan-dns --email=<your email> --password=your password> --old_ip=<your old ip> --new_ip=<your new ip> --port=<your new port> --domains_file=<your domains file>
 ```
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+
```

### Comparing `arvan_dns-1.0.6/arvan_dns.py` & `arvan_dns-1.0.7/arvan_dns.py`

 * *Files identical despite different names*

### Comparing `arvan_dns-1.0.6/setup.py` & `arvan_dns-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='arvan_dns',
-    version='1.0.6',
+    version='1.0.7',
     description='Arvan DNS updater',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     py_modules=['arvan_dns'],
     install_requires=[
         'requests',
         'argparse'
```

