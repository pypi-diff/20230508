# Comparing `tmp/klym-telemetry-0.1.4.tar.gz` & `tmp/klym-telemetry-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klym-telemetry-0.1.4.tar", last modified: Wed May  3 15:22:14 2023, max compression
+gzip compressed data, was "klym-telemetry-0.1.5.tar", last modified: Mon May  8 13:51:23 2023, max compression
```

## Comparing `klym-telemetry-0.1.4.tar` & `klym-telemetry-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 15:22:14.656577 klym-telemetry-0.1.4/
--rw-rw-rw-   0        0        0     4076 2023-05-03 15:22:14.655755 klym-telemetry-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3148 2023-05-01 21:12:52.000000 klym-telemetry-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 15:22:14.616328 klym-telemetry-0.1.4/klym_telemetry/
--rw-rw-rw-   0        0        0        0 2023-04-22 00:00:44.000000 klym-telemetry-0.1.4/klym_telemetry/__init__.py
--rw-rw-rw-   0        0        0     2612 2023-04-23 22:09:56.000000 klym-telemetry-0.1.4/klym_telemetry/helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-03 15:22:14.651578 klym-telemetry-0.1.4/klym_telemetry/instrumenters/
--rw-rw-rw-   0        0        0      760 2023-05-03 15:20:06.000000 klym-telemetry-0.1.4/klym_telemetry/instrumenters/__init__.py
--rw-rw-rw-   0        0        0     2131 2023-04-25 19:42:07.000000 klym-telemetry-0.1.4/klym_telemetry/instrumenters/base.py
--rw-rw-rw-   0        0        0      507 2023-05-03 15:19:21.000000 klym-telemetry-0.1.4/klym_telemetry/instrumenters/celery.py
--rw-rw-rw-   0        0        0      507 2023-05-03 15:18:48.000000 klym-telemetry-0.1.4/klym_telemetry/instrumenters/django.py
--rw-rw-rw-   0        0        0      947 2023-05-03 15:17:41.000000 klym-telemetry-0.1.4/klym_telemetry/instrumenters/fastapi.py
--rw-rw-rw-   0        0        0      515 2023-05-01 21:09:25.000000 klym-telemetry-0.1.4/klym_telemetry/instrumenters/postgres.py
--rw-rw-rw-   0        0        0      515 2023-05-03 15:19:21.000000 klym-telemetry-0.1.4/klym_telemetry/instrumenters/requests.py
--rw-rw-rw-   0        0        0     5693 2023-04-23 22:09:56.000000 klym-telemetry-0.1.4/klym_telemetry/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-03 15:22:14.631353 klym-telemetry-0.1.4/klym_telemetry.egg-info/
--rw-rw-rw-   0        0        0     4076 2023-05-03 15:22:14.000000 klym-telemetry-0.1.4/klym_telemetry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      562 2023-05-03 15:22:14.000000 klym-telemetry-0.1.4/klym_telemetry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 15:22:14.000000 klym-telemetry-0.1.4/klym_telemetry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      406 2023-05-03 15:22:14.000000 klym-telemetry-0.1.4/klym_telemetry.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-03 15:22:14.000000 klym-telemetry-0.1.4/klym_telemetry.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 15:22:14.657598 klym-telemetry-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1795 2023-05-03 15:21:54.000000 klym-telemetry-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:51:23.097485 klym-telemetry-0.1.5/
+-rw-rw-rw-   0        0        0     4076 2023-05-08 13:51:23.094497 klym-telemetry-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3148 2023-05-01 21:12:52.000000 klym-telemetry-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 13:51:23.042485 klym-telemetry-0.1.5/klym_telemetry/
+-rw-rw-rw-   0        0        0        0 2023-04-22 00:00:44.000000 klym-telemetry-0.1.5/klym_telemetry/__init__.py
+-rw-rw-rw-   0        0        0     2612 2023-04-23 22:09:56.000000 klym-telemetry-0.1.5/klym_telemetry/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:51:23.090745 klym-telemetry-0.1.5/klym_telemetry/instrumenters/
+-rw-rw-rw-   0        0        0     1040 2023-05-08 13:47:20.000000 klym-telemetry-0.1.5/klym_telemetry/instrumenters/__init__.py
+-rw-rw-rw-   0        0        0     2131 2023-04-25 19:42:07.000000 klym-telemetry-0.1.5/klym_telemetry/instrumenters/base.py
+-rw-rw-rw-   0        0        0      507 2023-05-03 15:19:21.000000 klym-telemetry-0.1.5/klym_telemetry/instrumenters/celery.py
+-rw-rw-rw-   0        0        0      507 2023-05-03 15:18:48.000000 klym-telemetry-0.1.5/klym_telemetry/instrumenters/django.py
+-rw-rw-rw-   0        0        0      874 2023-05-08 13:47:20.000000 klym-telemetry-0.1.5/klym_telemetry/instrumenters/fastapi.py
+-rw-rw-rw-   0        0        0      633 2023-05-08 13:47:20.000000 klym-telemetry-0.1.5/klym_telemetry/instrumenters/module_import.py
+-rw-rw-rw-   0        0        0      515 2023-05-01 21:09:25.000000 klym-telemetry-0.1.5/klym_telemetry/instrumenters/postgres.py
+-rw-rw-rw-   0        0        0      515 2023-05-03 15:19:21.000000 klym-telemetry-0.1.5/klym_telemetry/instrumenters/requests.py
+-rw-rw-rw-   0        0        0     5693 2023-04-23 22:09:56.000000 klym-telemetry-0.1.5/klym_telemetry/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:51:23.058486 klym-telemetry-0.1.5/klym_telemetry.egg-info/
+-rw-rw-rw-   0        0        0     4076 2023-05-08 13:51:22.000000 klym-telemetry-0.1.5/klym_telemetry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      608 2023-05-08 13:51:22.000000 klym-telemetry-0.1.5/klym_telemetry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 13:51:22.000000 klym-telemetry-0.1.5/klym_telemetry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      406 2023-05-08 13:51:22.000000 klym-telemetry-0.1.5/klym_telemetry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-08 13:51:22.000000 klym-telemetry-0.1.5/klym_telemetry.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 13:51:23.098486 klym-telemetry-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1795 2023-05-08 13:50:55.000000 klym-telemetry-0.1.5/setup.py
```

### Comparing `klym-telemetry-0.1.4/PKG-INFO` & `klym-telemetry-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klym-telemetry
-Version: 0.1.4
+Version: 0.1.5
 Summary: Scaffold library
 Home-page: https://dummy.readthedocs.io/
 Author: Klym Telemetry
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `klym-telemetry-0.1.4/README.md` & `klym-telemetry-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.4/klym_telemetry/helpers.py` & `klym-telemetry-0.1.5/klym_telemetry/helpers.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.4/klym_telemetry/instrumenters/base.py` & `klym-telemetry-0.1.5/klym_telemetry/instrumenters/base.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.4/klym_telemetry/instrumenters/fastapi.py` & `klym-telemetry-0.1.5/klym_telemetry/instrumenters/fastapi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from opentelemetry.instrumentation.fastapi import FastAPIInstrumentor
-from opentelemetry.instrumentation.requests import RequestsInstrumentor
 
 from klym_telemetry.instrumenters.base import KLYMInstrumentor
 
 
 class _FastAPIInstrumentor(KLYMInstrumentor):
 
     def __init__(self, service_name: str, endpoint: str, **kwargs) -> None:
```

### Comparing `klym-telemetry-0.1.4/klym_telemetry/instrumenters/postgres.py` & `klym-telemetry-0.1.5/klym_telemetry/instrumenters/postgres.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.4/klym_telemetry/instrumenters/requests.py` & `klym-telemetry-0.1.5/klym_telemetry/instrumenters/requests.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.4/klym_telemetry/utils.py` & `klym-telemetry-0.1.5/klym_telemetry/utils.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.4/klym_telemetry.egg-info/PKG-INFO` & `klym-telemetry-0.1.5/klym_telemetry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klym-telemetry
-Version: 0.1.4
+Version: 0.1.5
 Summary: Scaffold library
 Home-page: https://dummy.readthedocs.io/
 Author: Klym Telemetry
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `klym-telemetry-0.1.4/klym_telemetry.egg-info/SOURCES.txt` & `klym-telemetry-0.1.5/klym_telemetry.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,9 +9,10 @@
 klym_telemetry.egg-info/requires.txt
 klym_telemetry.egg-info/top_level.txt
 klym_telemetry/instrumenters/__init__.py
 klym_telemetry/instrumenters/base.py
 klym_telemetry/instrumenters/celery.py
 klym_telemetry/instrumenters/django.py
 klym_telemetry/instrumenters/fastapi.py
+klym_telemetry/instrumenters/module_import.py
 klym_telemetry/instrumenters/postgres.py
 klym_telemetry/instrumenters/requests.py
```

### Comparing `klym-telemetry-0.1.4/setup.py` & `klym-telemetry-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="klym-telemetry",
-    version="0.1.4",
+    version="0.1.5",
     description="Scaffold library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://dummy.readthedocs.io/",
     author="Klym Telemetry",
     author_email="example@email.com",
     license="MIT",
```

