# Comparing `tmp/catwalk_common-0.0.3.tar.gz` & `tmp/catwalk_common-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catwalk_common-0.0.3.tar", last modified: Wed Mar  8 14:23:42 2023, max compression
+gzip compressed data, was "catwalk_common-0.0.4.tar", last modified: Mon May  8 14:18:18 2023, max compression
```

## Comparing `catwalk_common-0.0.3.tar` & `catwalk_common-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-03-08 14:23:42.893158 catwalk_common-0.0.3/
--rw-rw-r--   0 marek     (1000) marek     (1000)      578 2023-03-08 14:23:42.893158 catwalk_common-0.0.3/PKG-INFO
--rw-rw-r--   0 marek     (1000) marek     (1000)       49 2023-03-08 14:22:54.000000 catwalk_common-0.0.3/README.md
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-03-08 14:23:42.893158 catwalk_common-0.0.3/catwalk_common/
--rw-rw-r--   0 marek     (1000) marek     (1000)       86 2023-03-08 14:21:41.000000 catwalk_common-0.0.3/catwalk_common/__init__.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     1542 2023-03-08 14:21:41.000000 catwalk_common-0.0.3/catwalk_common/_common_case_format.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     2225 2023-03-08 14:21:41.000000 catwalk_common-0.0.3/catwalk_common/plugins.py
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-03-08 14:23:42.893158 catwalk_common-0.0.3/catwalk_common.egg-info/
--rw-rw-r--   0 marek     (1000) marek     (1000)      578 2023-03-08 14:23:42.000000 catwalk_common-0.0.3/catwalk_common.egg-info/PKG-INFO
--rw-rw-r--   0 marek     (1000) marek     (1000)      304 2023-03-08 14:23:42.000000 catwalk_common-0.0.3/catwalk_common.egg-info/SOURCES.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)        1 2023-03-08 14:23:42.000000 catwalk_common-0.0.3/catwalk_common.egg-info/dependency_links.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)       16 2023-03-08 14:23:42.000000 catwalk_common-0.0.3/catwalk_common.egg-info/requires.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)       15 2023-03-08 14:23:42.000000 catwalk_common-0.0.3/catwalk_common.egg-info/top_level.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)      603 2023-03-08 14:22:54.000000 catwalk_common-0.0.3/pyproject.toml
--rw-rw-r--   0 marek     (1000) marek     (1000)       38 2023-03-08 14:23:42.893158 catwalk_common-0.0.3/setup.cfg
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-05-08 14:18:18.983118 catwalk_common-0.0.4/
+-rw-rw-r--   0 marek     (1000) marek     (1000)      578 2023-05-08 14:18:18.983118 catwalk_common-0.0.4/PKG-INFO
+-rw-rw-r--   0 marek     (1000) marek     (1000)       49 2023-05-08 13:58:38.000000 catwalk_common-0.0.4/README.md
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-05-08 14:18:18.983118 catwalk_common-0.0.4/catwalk_common/
+-rw-rw-r--   0 marek     (1000) marek     (1000)       86 2023-05-08 13:58:38.000000 catwalk_common-0.0.4/catwalk_common/__init__.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)     1616 2023-05-08 13:58:38.000000 catwalk_common-0.0.4/catwalk_common/_common_case_format.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)     2225 2023-03-08 14:21:41.000000 catwalk_common-0.0.4/catwalk_common/plugins.py
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-05-08 14:18:18.983118 catwalk_common-0.0.4/catwalk_common.egg-info/
+-rw-rw-r--   0 marek     (1000) marek     (1000)      578 2023-05-08 14:18:18.000000 catwalk_common-0.0.4/catwalk_common.egg-info/PKG-INFO
+-rw-rw-r--   0 marek     (1000) marek     (1000)      304 2023-05-08 14:18:18.000000 catwalk_common-0.0.4/catwalk_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)        1 2023-05-08 14:18:18.000000 catwalk_common-0.0.4/catwalk_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)       16 2023-05-08 14:18:18.000000 catwalk_common-0.0.4/catwalk_common.egg-info/requires.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)       15 2023-05-08 14:18:18.000000 catwalk_common-0.0.4/catwalk_common.egg-info/top_level.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)      603 2023-05-08 13:58:38.000000 catwalk_common-0.0.4/pyproject.toml
+-rw-rw-r--   0 marek     (1000) marek     (1000)       38 2023-05-08 14:18:18.983118 catwalk_common-0.0.4/setup.cfg
```

### Comparing `catwalk_common-0.0.3/PKG-INFO` & `catwalk_common-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catwalk_common
-Version: 0.0.3
+Version: 0.0.4
 Author-email: Mateusz Hordyński <mateusz.hordynski@deepsense.ai>, Marek Połom <marek.polom@deepsense.ai>
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

### Comparing `catwalk_common-0.0.3/catwalk_common/_common_case_format.py` & `catwalk_common-0.0.4/catwalk_common/_common_case_format.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,7 +63,9 @@
         ..., description="Additional metadata that will be saved with the case"
     )
 
 
 class OpenCase(CommonCaseFormat):
     id: str
     created_at: str
+    is_archived: Optional[bool] = None
+    is_open: Optional[bool] = None
```

### Comparing `catwalk_common-0.0.3/catwalk_common/plugins.py` & `catwalk_common-0.0.4/catwalk_common/plugins.py`

 * *Files identical despite different names*

### Comparing `catwalk_common-0.0.3/catwalk_common.egg-info/PKG-INFO` & `catwalk_common-0.0.4/catwalk_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catwalk-common
-Version: 0.0.3
+Version: 0.0.4
 Author-email: Mateusz Hordyński <mateusz.hordynski@deepsense.ai>, Marek Połom <marek.polom@deepsense.ai>
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

### Comparing `catwalk_common-0.0.3/pyproject.toml` & `catwalk_common-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "catwalk_common"
-version = "0.0.3"
+version = "0.0.4"
 license = { text = "GPLv3+" }
 authors = [
     { name = "Mateusz Hordyński", email = "mateusz.hordynski@deepsense.ai" },
     { name = "Marek Połom", email = "marek.polom@deepsense.ai" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

