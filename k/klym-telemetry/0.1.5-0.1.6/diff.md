# Comparing `tmp/klym-telemetry-0.1.5.tar.gz` & `tmp/klym-telemetry-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klym-telemetry-0.1.5.tar", last modified: Mon May  8 13:51:23 2023, max compression
+gzip compressed data, was "klym-telemetry-0.1.6.tar", last modified: Mon May  8 16:52:48 2023, max compression
```

## Comparing `klym-telemetry-0.1.5.tar` & `klym-telemetry-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 13:51:23.097485 klym-telemetry-0.1.5/
--rw-rw-rw-   0        0        0     4076 2023-05-08 13:51:23.094497 klym-telemetry-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3148 2023-05-01 21:12:52.000000 klym-telemetry-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 13:51:23.042485 klym-telemetry-0.1.5/klym_telemetry/
--rw-rw-rw-   0        0        0        0 2023-04-22 00:00:44.000000 klym-telemetry-0.1.5/klym_telemetry/__init__.py
--rw-rw-rw-   0        0        0     2612 2023-04-23 22:09:56.000000 klym-telemetry-0.1.5/klym_telemetry/helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-08 13:51:23.090745 klym-telemetry-0.1.5/klym_telemetry/instrumenters/
--rw-rw-rw-   0        0        0     1040 2023-05-08 13:47:20.000000 klym-telemetry-0.1.5/klym_telemetry/instrumenters/__init__.py
--rw-rw-rw-   0        0        0     2131 2023-04-25 19:42:07.000000 klym-telemetry-0.1.5/klym_telemetry/instrumenters/base.py
--rw-rw-rw-   0        0        0      507 2023-05-03 15:19:21.000000 klym-telemetry-0.1.5/klym_telemetry/instrumenters/celery.py
--rw-rw-rw-   0        0        0      507 2023-05-03 15:18:48.000000 klym-telemetry-0.1.5/klym_telemetry/instrumenters/django.py
--rw-rw-rw-   0        0        0      874 2023-05-08 13:47:20.000000 klym-telemetry-0.1.5/klym_telemetry/instrumenters/fastapi.py
--rw-rw-rw-   0        0        0      633 2023-05-08 13:47:20.000000 klym-telemetry-0.1.5/klym_telemetry/instrumenters/module_import.py
--rw-rw-rw-   0        0        0      515 2023-05-01 21:09:25.000000 klym-telemetry-0.1.5/klym_telemetry/instrumenters/postgres.py
--rw-rw-rw-   0        0        0      515 2023-05-03 15:19:21.000000 klym-telemetry-0.1.5/klym_telemetry/instrumenters/requests.py
--rw-rw-rw-   0        0        0     5693 2023-04-23 22:09:56.000000 klym-telemetry-0.1.5/klym_telemetry/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 13:51:23.058486 klym-telemetry-0.1.5/klym_telemetry.egg-info/
--rw-rw-rw-   0        0        0     4076 2023-05-08 13:51:22.000000 klym-telemetry-0.1.5/klym_telemetry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      608 2023-05-08 13:51:22.000000 klym-telemetry-0.1.5/klym_telemetry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 13:51:22.000000 klym-telemetry-0.1.5/klym_telemetry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      406 2023-05-08 13:51:22.000000 klym-telemetry-0.1.5/klym_telemetry.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-08 13:51:22.000000 klym-telemetry-0.1.5/klym_telemetry.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 13:51:23.098486 klym-telemetry-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1795 2023-05-08 13:50:55.000000 klym-telemetry-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:52:48.062551 klym-telemetry-0.1.6/
+-rw-rw-rw-   0        0        0     4076 2023-05-08 16:52:48.062247 klym-telemetry-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3148 2023-05-01 21:12:52.000000 klym-telemetry-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 16:52:48.035184 klym-telemetry-0.1.6/klym_telemetry/
+-rw-rw-rw-   0        0        0        0 2023-04-22 00:00:44.000000 klym-telemetry-0.1.6/klym_telemetry/__init__.py
+-rw-rw-rw-   0        0        0     2612 2023-04-23 22:09:56.000000 klym-telemetry-0.1.6/klym_telemetry/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:52:48.059549 klym-telemetry-0.1.6/klym_telemetry/instrumenters/
+-rw-rw-rw-   0        0        0     1175 2023-05-08 16:52:38.000000 klym-telemetry-0.1.6/klym_telemetry/instrumenters/__init__.py
+-rw-rw-rw-   0        0        0      880 2023-05-08 16:51:21.000000 klym-telemetry-0.1.6/klym_telemetry/instrumenters/airflow.py
+-rw-rw-rw-   0        0        0     2131 2023-04-25 19:42:07.000000 klym-telemetry-0.1.6/klym_telemetry/instrumenters/base.py
+-rw-rw-rw-   0        0        0      507 2023-05-03 15:19:21.000000 klym-telemetry-0.1.6/klym_telemetry/instrumenters/celery.py
+-rw-rw-rw-   0        0        0      507 2023-05-03 15:18:48.000000 klym-telemetry-0.1.6/klym_telemetry/instrumenters/django.py
+-rw-rw-rw-   0        0        0      874 2023-05-08 13:47:20.000000 klym-telemetry-0.1.6/klym_telemetry/instrumenters/fastapi.py
+-rw-rw-rw-   0        0        0      636 2023-05-08 16:52:38.000000 klym-telemetry-0.1.6/klym_telemetry/instrumenters/module_import.py
+-rw-rw-rw-   0        0        0      515 2023-05-01 21:09:25.000000 klym-telemetry-0.1.6/klym_telemetry/instrumenters/postgres.py
+-rw-rw-rw-   0        0        0      515 2023-05-03 15:19:21.000000 klym-telemetry-0.1.6/klym_telemetry/instrumenters/requests.py
+-rw-rw-rw-   0        0        0     5693 2023-04-23 22:09:56.000000 klym-telemetry-0.1.6/klym_telemetry/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:52:48.042552 klym-telemetry-0.1.6/klym_telemetry.egg-info/
+-rw-rw-rw-   0        0        0     4076 2023-05-08 16:52:47.000000 klym-telemetry-0.1.6/klym_telemetry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      648 2023-05-08 16:52:47.000000 klym-telemetry-0.1.6/klym_telemetry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 16:52:47.000000 klym-telemetry-0.1.6/klym_telemetry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      406 2023-05-08 16:52:47.000000 klym-telemetry-0.1.6/klym_telemetry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-08 16:52:47.000000 klym-telemetry-0.1.6/klym_telemetry.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 16:52:48.062551 klym-telemetry-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1795 2023-05-08 16:48:25.000000 klym-telemetry-0.1.6/setup.py
```

### Comparing `klym-telemetry-0.1.5/PKG-INFO` & `klym-telemetry-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klym-telemetry
-Version: 0.1.5
+Version: 0.1.6
 Summary: Scaffold library
 Home-page: https://dummy.readthedocs.io/
 Author: Klym Telemetry
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `klym-telemetry-0.1.5/README.md` & `klym-telemetry-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.5/klym_telemetry/helpers.py` & `klym-telemetry-0.1.6/klym_telemetry/helpers.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.5/klym_telemetry/instrumenters/__init__.py` & `klym-telemetry-0.1.6/klym_telemetry/instrumenters/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+import traceback
 from enum import Enum
 import klym_telemetry.instrumenters.module_import as importer
 
 class SupportedInstrumenters(Enum):
 
     INSTRUMENTERS = {
         "fastapi": ("klym_telemetry.instrumenters.fastapi", "_FastAPIInstrumentor"),
+        "airflow": ("klym_telemetry.instrumenters.airflow", "_AirflowInstrumentor"),
         "django": ("klym_telemetry.instrumenters.django", "_DjangoInstrumentor"),
         "celery": ("klym_telemetry.instrumenters.celery", "_CeleryInstrumentor"),
         "psycopg2": ("klym_telemetry.instrumenters.psycopg2", "_Psycopg2Instrumentor"),
         "requests": ("klym_telemetry.instrumenters.requests", "_RequestsInstrumentor"),
     }
 
 def instrument_app(app_type: str, **kwargs):
     try:
         package = SupportedInstrumenters.INSTRUMENTERS.value.get(app_type)[0]
         classname = SupportedInstrumenters.INSTRUMENTERS.value.get(app_type)[1]
         return importer.import_module(package, classname)(**kwargs).instrument()
     except Exception as e:
+        traceback.print_exc()
         print(f"Dependency error. You need to import the instrumenter for {app_type} if you want to use it")
         raise
```

### Comparing `klym-telemetry-0.1.5/klym_telemetry/instrumenters/base.py` & `klym-telemetry-0.1.6/klym_telemetry/instrumenters/base.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.5/klym_telemetry/instrumenters/fastapi.py` & `klym-telemetry-0.1.6/klym_telemetry/instrumenters/fastapi.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.5/klym_telemetry/instrumenters/module_import.py` & `klym-telemetry-0.1.6/klym_telemetry/instrumenters/module_import.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 def import_module(package: str, classname: str):
     try:
         print(f"Importing module: {package}.{classname}")
         module = __get_optional_module(package)
         print(module)
         if module:
             return getattr(module, classname)
-    except Exception:
+    except Exception as e:
         # Do something additional with the exception
-        return None
+        raise e
 
 
 def __get_optional_module(module_path: str) -> Any:
     try:
         return importlib.import_module(module_path)
     except Exception as e:
         print(f"Error importing module {module_path}. Exception: {e}")
-        raise
+        raise e
```

### Comparing `klym-telemetry-0.1.5/klym_telemetry/instrumenters/postgres.py` & `klym-telemetry-0.1.6/klym_telemetry/instrumenters/postgres.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.5/klym_telemetry/instrumenters/requests.py` & `klym-telemetry-0.1.6/klym_telemetry/instrumenters/requests.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.5/klym_telemetry/utils.py` & `klym-telemetry-0.1.6/klym_telemetry/utils.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.5/klym_telemetry.egg-info/PKG-INFO` & `klym-telemetry-0.1.6/klym_telemetry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klym-telemetry
-Version: 0.1.5
+Version: 0.1.6
 Summary: Scaffold library
 Home-page: https://dummy.readthedocs.io/
 Author: Klym Telemetry
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `klym-telemetry-0.1.5/klym_telemetry.egg-info/SOURCES.txt` & `klym-telemetry-0.1.6/klym_telemetry.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 klym_telemetry/utils.py
 klym_telemetry.egg-info/PKG-INFO
 klym_telemetry.egg-info/SOURCES.txt
 klym_telemetry.egg-info/dependency_links.txt
 klym_telemetry.egg-info/requires.txt
 klym_telemetry.egg-info/top_level.txt
 klym_telemetry/instrumenters/__init__.py
+klym_telemetry/instrumenters/airflow.py
 klym_telemetry/instrumenters/base.py
 klym_telemetry/instrumenters/celery.py
 klym_telemetry/instrumenters/django.py
 klym_telemetry/instrumenters/fastapi.py
 klym_telemetry/instrumenters/module_import.py
 klym_telemetry/instrumenters/postgres.py
 klym_telemetry/instrumenters/requests.py
```

### Comparing `klym-telemetry-0.1.5/setup.py` & `klym-telemetry-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="klym-telemetry",
-    version="0.1.5",
+    version="0.1.6",
     description="Scaffold library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://dummy.readthedocs.io/",
     author="Klym Telemetry",
     author_email="example@email.com",
     license="MIT",
```

