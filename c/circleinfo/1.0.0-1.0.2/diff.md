# Comparing `tmp/circleinfo-1.0.0.tar.gz` & `tmp/circleinfo-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circleinfo-1.0.0.tar", last modified: Sun May  7 18:54:01 2023, max compression
+gzip compressed data, was "circleinfo-1.0.2.tar", last modified: Mon May  8 01:26:14 2023, max compression
```

## Comparing `circleinfo-1.0.0.tar` & `circleinfo-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-07 18:54:01.250993 circleinfo-1.0.0/
--rw-rw----   0 root         (0) everybody  (9997)     2351 2023-05-07 18:54:01.250993 circleinfo-1.0.0/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     1574 2023-05-07 18:53:25.000000 circleinfo-1.0.0/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-07 18:54:01.120993 circleinfo-1.0.0/circleinfo/
--rw-rw----   0 root         (0) everybody  (9997)        0 2022-11-24 10:35:57.000000 circleinfo-1.0.0/circleinfo/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)   236004 2023-05-05 09:58:08.000000 circleinfo-1.0.0/circleinfo/circleinfo.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-07 18:54:01.240993 circleinfo-1.0.0/circleinfo.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     2351 2023-05-07 18:54:00.000000 circleinfo-1.0.0/circleinfo.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      249 2023-05-07 18:54:00.000000 circleinfo-1.0.0/circleinfo.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-07 18:54:00.000000 circleinfo-1.0.0/circleinfo.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       64 2023-05-07 18:54:00.000000 circleinfo-1.0.0/circleinfo.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       11 2023-05-07 18:54:00.000000 circleinfo-1.0.0/circleinfo.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)      495 2023-05-07 18:54:01.260993 circleinfo-1.0.0/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1245 2023-05-07 18:52:29.000000 circleinfo-1.0.0/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-08 01:26:14.460984 circleinfo-1.0.2/
+-rw-rw----   0 root         (0) everybody  (9997)     2351 2023-05-08 01:26:14.460984 circleinfo-1.0.2/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     1574 2023-05-07 18:53:25.000000 circleinfo-1.0.2/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-08 01:26:14.290984 circleinfo-1.0.2/circleinfo/
+-rw-rw----   0 root         (0) everybody  (9997)        0 2022-11-24 10:35:57.000000 circleinfo-1.0.2/circleinfo/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)   680380 2023-05-08 01:25:09.000000 circleinfo-1.0.2/circleinfo/circleinfo.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-08 01:26:14.440984 circleinfo-1.0.2/circleinfo.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     2351 2023-05-08 01:26:13.000000 circleinfo-1.0.2/circleinfo.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      249 2023-05-08 01:26:14.000000 circleinfo-1.0.2/circleinfo.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-08 01:26:14.000000 circleinfo-1.0.2/circleinfo.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       64 2023-05-08 01:26:14.000000 circleinfo-1.0.2/circleinfo.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       11 2023-05-08 01:26:14.000000 circleinfo-1.0.2/circleinfo.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)      495 2023-05-08 01:26:14.460984 circleinfo-1.0.2/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1245 2023-05-08 01:19:03.000000 circleinfo-1.0.2/setup.py
```

### Comparing `circleinfo-1.0.0/PKG-INFO` & `circleinfo-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circleinfo
-Version: 1.0.0
+Version: 1.0.2
 Summary: Bangladeshi Robi/Airtel Circle Information Tools!
 Home-page: https://github.com/ShTasrif
 Author: CyberSH
 Author-email: cybershbd@gmail.com
 License: MIT
 Keywords: cybershbd,cyber sh,circleinfo,circle info,circle number to info,circle username to information,circle nickname to information,robi Airtel circle
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: circleinfo Version: 1.0.0 Summary: Bangladeshi
+Metadata-Version: 2.1 Name: circleinfo Version: 1.0.2 Summary: Bangladeshi
 Robi/Airtel Circle Information Tools! Home-page: https://github.com/ShTasrif
 Author: CyberSH Author-email: cybershbd@gmail.com License: MIT Keywords:
 cybershbd,cyber sh,circleinfo,circle info,circle number to info,circle username
 to information,circle nickname to information,robi Airtel circle Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
```

### Comparing `circleinfo-1.0.0/README.md` & `circleinfo-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `circleinfo-1.0.0/circleinfo.egg-info/PKG-INFO` & `circleinfo-1.0.2/circleinfo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circleinfo
-Version: 1.0.0
+Version: 1.0.2
 Summary: Bangladeshi Robi/Airtel Circle Information Tools!
 Home-page: https://github.com/ShTasrif
 Author: CyberSH
 Author-email: cybershbd@gmail.com
 License: MIT
 Keywords: cybershbd,cyber sh,circleinfo,circle info,circle number to info,circle username to information,circle nickname to information,robi Airtel circle
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: circleinfo Version: 1.0.0 Summary: Bangladeshi
+Metadata-Version: 2.1 Name: circleinfo Version: 1.0.2 Summary: Bangladeshi
 Robi/Airtel Circle Information Tools! Home-page: https://github.com/ShTasrif
 Author: CyberSH Author-email: cybershbd@gmail.com License: MIT Keywords:
 cybershbd,cyber sh,circleinfo,circle info,circle number to info,circle username
 to information,circle nickname to information,robi Airtel circle Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
```

### Comparing `circleinfo-1.0.0/setup.py` & `circleinfo-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='circleinfo',
     packages=find_packages(),
     include_package_data=True,
-    version="1.0.0",
+    version="1.0.2",
     description='Bangladeshi Robi/Airtel Circle Information Tools!',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='CyberSH',
     author_email='cybershbd@gmail.com',
     #install_requires=[],
```

