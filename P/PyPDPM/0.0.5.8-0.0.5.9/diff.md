# Comparing `tmp/PyPDPM-0.0.5.8.tar.gz` & `tmp/PyPDPM-0.0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPDPM-0.0.5.8.tar", last modified: Wed May  3 03:49:41 2023, max compression
+gzip compressed data, was "PyPDPM-0.0.5.9.tar", last modified: Wed May  3 03:56:51 2023, max compression
```

## Comparing `PyPDPM-0.0.5.8.tar` & `PyPDPM-0.0.5.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 03:49:41.789608 PyPDPM-0.0.5.8/
--rw-rw-rw-   0        0        0     1091 2023-04-17 07:06:47.000000 PyPDPM-0.0.5.8/LICENSE.txt
--rw-rw-rw-   0        0        0     4928 2023-05-03 03:49:41.790607 PyPDPM-0.0.5.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 03:49:41.769609 PyPDPM-0.0.5.8/PyPDPM/
--rw-rw-rw-   0        0        0    26092 2023-05-03 03:48:38.000000 PyPDPM-0.0.5.8/PyPDPM/HIPPS.py
--rw-rw-rw-   0        0        0        0 2023-05-03 03:44:42.000000 PyPDPM-0.0.5.8/PyPDPM/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 03:49:41.788630 PyPDPM-0.0.5.8/PyPDPM.egg-info/
--rw-rw-rw-   0        0        0     4928 2023-05-03 03:49:41.000000 PyPDPM-0.0.5.8/PyPDPM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-05-03 03:49:41.000000 PyPDPM-0.0.5.8/PyPDPM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 03:49:41.000000 PyPDPM-0.0.5.8/PyPDPM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-03 03:49:41.000000 PyPDPM-0.0.5.8/PyPDPM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4596 2023-05-03 03:05:29.000000 PyPDPM-0.0.5.8/README.rst
--rw-rw-rw-   0        0        0       87 2023-05-03 03:49:41.792609 PyPDPM-0.0.5.8/setup.cfg
--rw-rw-rw-   0        0        0      641 2023-05-03 03:49:33.000000 PyPDPM-0.0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:56:51.092650 PyPDPM-0.0.5.9/
+-rw-rw-rw-   0        0        0     1091 2023-04-17 07:06:47.000000 PyPDPM-0.0.5.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     4928 2023-05-03 03:56:51.093650 PyPDPM-0.0.5.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 03:56:51.082650 PyPDPM-0.0.5.9/PyPDPM/
+-rw-rw-rw-   0        0        0  3067232 2023-05-03 03:56:03.000000 PyPDPM-0.0.5.9/PyPDPM/HIPPS.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 03:44:42.000000 PyPDPM-0.0.5.9/PyPDPM/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:56:51.091649 PyPDPM-0.0.5.9/PyPDPM.egg-info/
+-rw-rw-rw-   0        0        0     4928 2023-05-03 03:56:51.000000 PyPDPM-0.0.5.9/PyPDPM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-05-03 03:56:51.000000 PyPDPM-0.0.5.9/PyPDPM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 03:56:51.000000 PyPDPM-0.0.5.9/PyPDPM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-03 03:56:51.000000 PyPDPM-0.0.5.9/PyPDPM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4596 2023-05-03 03:05:29.000000 PyPDPM-0.0.5.9/README.rst
+-rw-rw-rw-   0        0        0       87 2023-05-03 03:56:51.094649 PyPDPM-0.0.5.9/setup.cfg
+-rw-rw-rw-   0        0        0      641 2023-05-03 03:56:34.000000 PyPDPM-0.0.5.9/setup.py
```

### Comparing `PyPDPM-0.0.5.8/LICENSE.txt` & `PyPDPM-0.0.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyPDPM-0.0.5.8/PKG-INFO` & `PyPDPM-0.0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPDPM
-Version: 0.0.5.8
+Version: 0.0.5.9
 Summary: A Python library for dealing with PDPM HIPP codes
 Home-page: https://github.com/Scorks/PyPDPM
 Author: Caro Strickland
 Author-email: carostrickland321@gmail.com
 License: MIT
 Keywords: PDPM,HIPPS,ICD-10-CM Codes
 Platform: UNKNOWN
```

### Comparing `PyPDPM-0.0.5.8/PyPDPM.egg-info/PKG-INFO` & `PyPDPM-0.0.5.9/PyPDPM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPDPM
-Version: 0.0.5.8
+Version: 0.0.5.9
 Summary: A Python library for dealing with PDPM HIPP codes
 Home-page: https://github.com/Scorks/PyPDPM
 Author: Caro Strickland
 Author-email: carostrickland321@gmail.com
 License: MIT
 Keywords: PDPM,HIPPS,ICD-10-CM Codes
 Platform: UNKNOWN
```

### Comparing `PyPDPM-0.0.5.8/README.rst` & `PyPDPM-0.0.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `PyPDPM-0.0.5.8/setup.py` & `PyPDPM-0.0.5.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.rst', 'r') as f:
     readme = f.read()
 
 setup(
     name='PyPDPM',
     packages=find_packages(include=['PyPDPM']),
-    version='0.0.5.8',
+    version='0.0.5.9',
     description='A Python library for dealing with PDPM HIPP codes',
     author='Caro Strickland',
     author_email='carostrickland321@gmail.com',
     url = 'https://github.com/Scorks/PyPDPM',
     long_description=readme,
     keywords = ['PDPM', 'HIPPS', 'ICD-10-CM Codes'],
     license='MIT',
```

