# Comparing `tmp/klym-telemetry-0.1.7.tar.gz` & `tmp/klym-telemetry-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klym-telemetry-0.1.7.tar", last modified: Mon May  8 16:59:46 2023, max compression
+gzip compressed data, was "klym-telemetry-0.1.8.tar", last modified: Mon May  8 17:26:51 2023, max compression
```

## Comparing `klym-telemetry-0.1.7.tar` & `klym-telemetry-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 16:59:46.856473 klym-telemetry-0.1.7/
--rw-rw-rw-   0        0        0     4076 2023-05-08 16:59:46.853473 klym-telemetry-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3148 2023-05-01 21:12:52.000000 klym-telemetry-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 16:59:46.809332 klym-telemetry-0.1.7/klym_telemetry/
--rw-rw-rw-   0        0        0        0 2023-04-22 00:00:44.000000 klym-telemetry-0.1.7/klym_telemetry/__init__.py
--rw-rw-rw-   0        0        0     2612 2023-04-23 22:09:56.000000 klym-telemetry-0.1.7/klym_telemetry/helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-08 16:59:46.849952 klym-telemetry-0.1.7/klym_telemetry/instrumenters/
--rw-rw-rw-   0        0        0     1175 2023-05-08 16:52:38.000000 klym-telemetry-0.1.7/klym_telemetry/instrumenters/__init__.py
--rw-rw-rw-   0        0        0      878 2023-05-08 16:59:10.000000 klym-telemetry-0.1.7/klym_telemetry/instrumenters/airflow.py
--rw-rw-rw-   0        0        0     2131 2023-04-25 19:42:07.000000 klym-telemetry-0.1.7/klym_telemetry/instrumenters/base.py
--rw-rw-rw-   0        0        0      507 2023-05-03 15:19:21.000000 klym-telemetry-0.1.7/klym_telemetry/instrumenters/celery.py
--rw-rw-rw-   0        0        0      507 2023-05-03 15:18:48.000000 klym-telemetry-0.1.7/klym_telemetry/instrumenters/django.py
--rw-rw-rw-   0        0        0      874 2023-05-08 13:47:20.000000 klym-telemetry-0.1.7/klym_telemetry/instrumenters/fastapi.py
--rw-rw-rw-   0        0        0      636 2023-05-08 16:52:38.000000 klym-telemetry-0.1.7/klym_telemetry/instrumenters/module_import.py
--rw-rw-rw-   0        0        0      515 2023-05-01 21:09:25.000000 klym-telemetry-0.1.7/klym_telemetry/instrumenters/postgres.py
--rw-rw-rw-   0        0        0      515 2023-05-03 15:19:21.000000 klym-telemetry-0.1.7/klym_telemetry/instrumenters/requests.py
--rw-rw-rw-   0        0        0     5693 2023-04-23 22:09:56.000000 klym-telemetry-0.1.7/klym_telemetry/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 16:59:46.825617 klym-telemetry-0.1.7/klym_telemetry.egg-info/
--rw-rw-rw-   0        0        0     4076 2023-05-08 16:59:46.000000 klym-telemetry-0.1.7/klym_telemetry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      648 2023-05-08 16:59:46.000000 klym-telemetry-0.1.7/klym_telemetry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 16:59:46.000000 klym-telemetry-0.1.7/klym_telemetry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      406 2023-05-08 16:59:46.000000 klym-telemetry-0.1.7/klym_telemetry.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-08 16:59:46.000000 klym-telemetry-0.1.7/klym_telemetry.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 16:59:46.857472 klym-telemetry-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1795 2023-05-08 16:59:39.000000 klym-telemetry-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:26:51.531158 klym-telemetry-0.1.8/
+-rw-rw-rw-   0        0        0     4076 2023-05-08 17:26:51.530103 klym-telemetry-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3148 2023-05-01 21:12:52.000000 klym-telemetry-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 17:26:51.494086 klym-telemetry-0.1.8/klym_telemetry/
+-rw-rw-rw-   0        0        0        0 2023-04-22 00:00:44.000000 klym-telemetry-0.1.8/klym_telemetry/__init__.py
+-rw-rw-rw-   0        0        0     2612 2023-04-23 22:09:56.000000 klym-telemetry-0.1.8/klym_telemetry/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:26:51.527063 klym-telemetry-0.1.8/klym_telemetry/instrumenters/
+-rw-rw-rw-   0        0        0     1175 2023-05-08 16:52:38.000000 klym-telemetry-0.1.8/klym_telemetry/instrumenters/__init__.py
+-rw-rw-rw-   0        0        0      878 2023-05-08 16:59:10.000000 klym-telemetry-0.1.8/klym_telemetry/instrumenters/airflow.py
+-rw-rw-rw-   0        0        0     2131 2023-04-25 19:42:07.000000 klym-telemetry-0.1.8/klym_telemetry/instrumenters/base.py
+-rw-rw-rw-   0        0        0      507 2023-05-03 15:19:21.000000 klym-telemetry-0.1.8/klym_telemetry/instrumenters/celery.py
+-rw-rw-rw-   0        0        0      507 2023-05-03 15:18:48.000000 klym-telemetry-0.1.8/klym_telemetry/instrumenters/django.py
+-rw-rw-rw-   0        0        0      874 2023-05-08 13:47:20.000000 klym-telemetry-0.1.8/klym_telemetry/instrumenters/fastapi.py
+-rw-rw-rw-   0        0        0      636 2023-05-08 16:52:38.000000 klym-telemetry-0.1.8/klym_telemetry/instrumenters/module_import.py
+-rw-rw-rw-   0        0        0      515 2023-05-01 21:09:25.000000 klym-telemetry-0.1.8/klym_telemetry/instrumenters/psycopg2.py
+-rw-rw-rw-   0        0        0      515 2023-05-03 15:19:21.000000 klym-telemetry-0.1.8/klym_telemetry/instrumenters/requests.py
+-rw-rw-rw-   0        0        0     5693 2023-04-23 22:09:56.000000 klym-telemetry-0.1.8/klym_telemetry/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:26:51.503060 klym-telemetry-0.1.8/klym_telemetry.egg-info/
+-rw-rw-rw-   0        0        0     4076 2023-05-08 17:26:51.000000 klym-telemetry-0.1.8/klym_telemetry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      648 2023-05-08 17:26:51.000000 klym-telemetry-0.1.8/klym_telemetry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 17:26:51.000000 klym-telemetry-0.1.8/klym_telemetry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      406 2023-05-08 17:26:51.000000 klym-telemetry-0.1.8/klym_telemetry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-08 17:26:51.000000 klym-telemetry-0.1.8/klym_telemetry.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 17:26:51.531158 klym-telemetry-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1795 2023-05-08 17:20:26.000000 klym-telemetry-0.1.8/setup.py
```

### Comparing `klym-telemetry-0.1.7/PKG-INFO` & `klym-telemetry-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klym-telemetry
-Version: 0.1.7
+Version: 0.1.8
 Summary: Scaffold library
 Home-page: https://dummy.readthedocs.io/
 Author: Klym Telemetry
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `klym-telemetry-0.1.7/README.md` & `klym-telemetry-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.7/klym_telemetry/helpers.py` & `klym-telemetry-0.1.8/klym_telemetry/helpers.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.7/klym_telemetry/instrumenters/__init__.py` & `klym-telemetry-0.1.8/klym_telemetry/instrumenters/__init__.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.7/klym_telemetry/instrumenters/airflow.py` & `klym-telemetry-0.1.8/klym_telemetry/instrumenters/airflow.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.7/klym_telemetry/instrumenters/base.py` & `klym-telemetry-0.1.8/klym_telemetry/instrumenters/base.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.7/klym_telemetry/instrumenters/fastapi.py` & `klym-telemetry-0.1.8/klym_telemetry/instrumenters/fastapi.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.7/klym_telemetry/instrumenters/module_import.py` & `klym-telemetry-0.1.8/klym_telemetry/instrumenters/module_import.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.7/klym_telemetry/instrumenters/postgres.py` & `klym-telemetry-0.1.8/klym_telemetry/instrumenters/psycopg2.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.7/klym_telemetry/instrumenters/requests.py` & `klym-telemetry-0.1.8/klym_telemetry/instrumenters/requests.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.7/klym_telemetry/utils.py` & `klym-telemetry-0.1.8/klym_telemetry/utils.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.7/klym_telemetry.egg-info/PKG-INFO` & `klym-telemetry-0.1.8/klym_telemetry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klym-telemetry
-Version: 0.1.7
+Version: 0.1.8
 Summary: Scaffold library
 Home-page: https://dummy.readthedocs.io/
 Author: Klym Telemetry
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `klym-telemetry-0.1.7/klym_telemetry.egg-info/SOURCES.txt` & `klym-telemetry-0.1.8/klym_telemetry.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 klym_telemetry/instrumenters/__init__.py
 klym_telemetry/instrumenters/airflow.py
 klym_telemetry/instrumenters/base.py
 klym_telemetry/instrumenters/celery.py
 klym_telemetry/instrumenters/django.py
 klym_telemetry/instrumenters/fastapi.py
 klym_telemetry/instrumenters/module_import.py
-klym_telemetry/instrumenters/postgres.py
+klym_telemetry/instrumenters/psycopg2.py
 klym_telemetry/instrumenters/requests.py
```

### Comparing `klym-telemetry-0.1.7/setup.py` & `klym-telemetry-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="klym-telemetry",
-    version="0.1.7",
+    version="0.1.8",
     description="Scaffold library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://dummy.readthedocs.io/",
     author="Klym Telemetry",
     author_email="example@email.com",
     license="MIT",
```

