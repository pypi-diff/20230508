# Comparing `tmp/pytigon-batteries-0.230402.tar.gz` & `tmp/pytigon-batteries-0.230508.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytigon-batteries-0.230402.tar", last modified: Sun Apr  2 17:40:20 2023, max compression
+gzip compressed data, was "pytigon-batteries-0.230508.tar", last modified: Mon May  8 20:09:45 2023, max compression
```

## Comparing `pytigon-batteries-0.230402.tar` & `pytigon-batteries-0.230508.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:40:20.283025 pytigon-batteries-0.230402/
--rw-rw-r--   0 sch       (1000) sch       (1000)     7652 2023-04-02 17:20:54.000000 pytigon-batteries-0.230402/LICENSE
--rw-rw-r--   0 sch       (1000) sch       (1000)     1122 2023-04-02 17:40:20.283025 pytigon-batteries-0.230402/PKG-INFO
--rw-rw-r--   0 sch       (1000) sch       (1000)       53 2023-04-02 17:20:54.000000 pytigon-batteries-0.230402/README.md
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:40:20.283025 pytigon-batteries-0.230402/pytigon_batteries.egg-info/
--rw-rw-r--   0 sch       (1000) sch       (1000)     1122 2023-04-02 17:40:20.000000 pytigon-batteries-0.230402/pytigon_batteries.egg-info/PKG-INFO
--rw-rw-r--   0 sch       (1000) sch       (1000)      230 2023-04-02 17:40:20.000000 pytigon-batteries-0.230402/pytigon_batteries.egg-info/SOURCES.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)        1 2023-04-02 17:40:20.000000 pytigon-batteries-0.230402/pytigon_batteries.egg-info/dependency_links.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)      656 2023-04-02 17:40:20.000000 pytigon-batteries-0.230402/pytigon_batteries.egg-info/requires.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)        1 2023-04-02 17:40:20.000000 pytigon-batteries-0.230402/pytigon_batteries.egg-info/top_level.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)       38 2023-04-02 17:40:20.283025 pytigon-batteries-0.230402/setup.cfg
--rw-rw-r--   0 sch       (1000) sch       (1000)     1703 2023-04-02 17:20:54.000000 pytigon-batteries-0.230402/setup.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:09:45.454252 pytigon-batteries-0.230508/
+-rw-rw-r--   0 sch       (1000) sch       (1000)     7652 2023-05-08 20:06:50.000000 pytigon-batteries-0.230508/LICENSE
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1173 2023-05-08 20:09:45.454252 pytigon-batteries-0.230508/PKG-INFO
+-rw-rw-r--   0 sch       (1000) sch       (1000)       53 2023-05-08 20:06:50.000000 pytigon-batteries-0.230508/README.md
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:09:45.454252 pytigon-batteries-0.230508/pytigon_batteries.egg-info/
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1173 2023-05-08 20:09:45.000000 pytigon-batteries-0.230508/pytigon_batteries.egg-info/PKG-INFO
+-rw-rw-r--   0 sch       (1000) sch       (1000)      230 2023-05-08 20:09:45.000000 pytigon-batteries-0.230508/pytigon_batteries.egg-info/SOURCES.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)        1 2023-05-08 20:09:45.000000 pytigon-batteries-0.230508/pytigon_batteries.egg-info/dependency_links.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)      669 2023-05-08 20:09:45.000000 pytigon-batteries-0.230508/pytigon_batteries.egg-info/requires.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)        1 2023-05-08 20:09:45.000000 pytigon-batteries-0.230508/pytigon_batteries.egg-info/top_level.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)       38 2023-05-08 20:09:45.454252 pytigon-batteries-0.230508/setup.cfg
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1753 2023-05-08 20:06:50.000000 pytigon-batteries-0.230508/setup.py
```

### Comparing `pytigon-batteries-0.230402/LICENSE` & `pytigon-batteries-0.230508/LICENSE`

 * *Files identical despite different names*

### Comparing `pytigon-batteries-0.230402/PKG-INFO` & `pytigon-batteries-0.230508/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytigon-batteries
-Version: 0.230402
+Version: 0.230508
 Summary: Pytigon library
 Home-page: UNKNOWN
 Author: Sławomir Chołaj
 Author-email: slawomir.cholaj@gmail.com
 License: LGPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3
 License-File: LICENSE
```

### Comparing `pytigon-batteries-0.230402/pytigon_batteries.egg-info/PKG-INFO` & `pytigon-batteries-0.230508/pytigon_batteries.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytigon-batteries
-Version: 0.230402
+Version: 0.230508
 Summary: Pytigon library
 Home-page: UNKNOWN
 Author: Sławomir Chołaj
 Author-email: slawomir.cholaj@gmail.com
 License: LGPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3
 License-File: LICENSE
```

### Comparing `pytigon-batteries-0.230402/pytigon_batteries.egg-info/requires.txt` & `pytigon-batteries-0.230508/pytigon_batteries.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 PyYAML
 Twisted[http2,tls]
 autobahn
 cffi
 channels
+channels-redis
 croniter
 daphne
 django-allauth
 django-filer
 django-filter
 django-graphql-jwt
 django-guardian
@@ -40,16 +41,16 @@
 pandas
 plotly
 psutil
 pygments
 pyopenssl
 pypdf
 pytigon
+redis
 reportlab
-seaborn
 svglib
 uritemplate
 uvicorn[standard]
 waitress
 wasmer
 wasmer_compiler_cranelift
 xonsh
```

### Comparing `pytigon-batteries-0.230402/setup.py` & `pytigon-batteries-0.230508/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 with open("requirements.txt") as f:
     tmp = f.read().strip().split("\n")
     install_requires = [pos for pos in tmp]
 
 setup(
     name="pytigon-batteries",
-    version="0.230402",
+    version="0.230508",
     description="Pytigon library",
     author="Sławomir Chołaj",
     author_email="slawomir.cholaj@gmail.com",
     license="LGPLv3",
     packages=find_packages(),
     package_data={"": extra_files},
     install_requires=install_requires,
@@ -34,14 +34,15 @@
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     python_requires=">=3",
```

