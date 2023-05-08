# Comparing `tmp/catwalk_client-0.0.8.tar.gz` & `tmp/catwalk_client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catwalk_client-0.0.8.tar", last modified: Wed Mar  8 14:23:20 2023, max compression
+gzip compressed data, was "catwalk_client-0.0.9.tar", last modified: Fri Mar 10 13:28:36 2023, max compression
```

## Comparing `catwalk_client-0.0.8.tar` & `catwalk_client-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-03-08 14:23:20.172915 catwalk_client-0.0.8/
--rw-rw-r--   0 marek     (1000) marek     (1000)     5104 2023-03-08 14:23:20.172915 catwalk_client-0.0.8/PKG-INFO
--rw-rw-r--   0 marek     (1000) marek     (1000)     4750 2023-03-08 14:22:54.000000 catwalk_client-0.0.8/README.md
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-03-08 14:23:20.168915 catwalk_client-0.0.8/catwalk_client/
--rw-rw-r--   0 marek     (1000) marek     (1000)       34 2023-03-06 09:49:52.000000 catwalk_client-0.0.8/catwalk_client/__init__.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     2913 2023-03-08 14:22:54.000000 catwalk_client-0.0.8/catwalk_client/client.py
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-03-08 14:23:20.172915 catwalk_client-0.0.8/catwalk_client/common/
--rw-rw-r--   0 marek     (1000) marek     (1000)       51 2023-03-08 14:22:54.000000 catwalk_client-0.0.8/catwalk_client/common/__init__.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     2853 2023-03-08 14:22:54.000000 catwalk_client-0.0.8/catwalk_client/common/_http_client.py
--rw-rw-r--   0 marek     (1000) marek     (1000)      825 2023-03-08 14:22:54.000000 catwalk_client-0.0.8/catwalk_client/common/catwalk_http_client.py
--rw-rw-r--   0 marek     (1000) marek     (1000)      216 2023-03-08 14:22:54.000000 catwalk_client-0.0.8/catwalk_client/common/constants.py
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-03-08 14:23:20.172915 catwalk_client-0.0.8/catwalk_client/tools/
--rw-rw-r--   0 marek     (1000) marek     (1000)       80 2023-03-08 14:22:54.000000 catwalk_client-0.0.8/catwalk_client/tools/__init__.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     1638 2023-03-08 14:22:54.000000 catwalk_client-0.0.8/catwalk_client/tools/_case_builder.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     2745 2023-03-08 14:22:54.000000 catwalk_client-0.0.8/catwalk_client/tools/_case_exporter.py
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-03-08 14:23:20.172915 catwalk_client-0.0.8/catwalk_client.egg-info/
--rw-rw-r--   0 marek     (1000) marek     (1000)     5104 2023-03-08 14:23:20.000000 catwalk_client-0.0.8/catwalk_client.egg-info/PKG-INFO
--rw-rw-r--   0 marek     (1000) marek     (1000)      527 2023-03-08 14:23:20.000000 catwalk_client-0.0.8/catwalk_client.egg-info/SOURCES.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)        1 2023-03-08 14:23:20.000000 catwalk_client-0.0.8/catwalk_client.egg-info/dependency_links.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)       22 2023-03-08 14:23:20.000000 catwalk_client-0.0.8/catwalk_client.egg-info/requires.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)       15 2023-03-08 14:23:20.000000 catwalk_client-0.0.8/catwalk_client.egg-info/top_level.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)      442 2023-03-08 14:22:54.000000 catwalk_client-0.0.8/pyproject.toml
--rw-rw-r--   0 marek     (1000) marek     (1000)       38 2023-03-08 14:23:20.172915 catwalk_client-0.0.8/setup.cfg
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-03-10 13:28:36.351777 catwalk_client-0.0.9/
+-rw-rw-r--   0 marek     (1000) marek     (1000)     5104 2023-03-10 13:28:36.351777 catwalk_client-0.0.9/PKG-INFO
+-rw-rw-r--   0 marek     (1000) marek     (1000)     4750 2023-03-09 15:11:53.000000 catwalk_client-0.0.9/README.md
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-03-10 13:28:36.347777 catwalk_client-0.0.9/catwalk_client/
+-rw-rw-r--   0 marek     (1000) marek     (1000)       34 2023-03-06 09:49:52.000000 catwalk_client-0.0.9/catwalk_client/__init__.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)     2866 2023-03-10 11:43:39.000000 catwalk_client-0.0.9/catwalk_client/client.py
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-03-10 13:28:36.351777 catwalk_client-0.0.9/catwalk_client/common/
+-rw-rw-r--   0 marek     (1000) marek     (1000)       51 2023-03-09 15:11:53.000000 catwalk_client-0.0.9/catwalk_client/common/__init__.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)     2853 2023-03-09 15:11:53.000000 catwalk_client-0.0.9/catwalk_client/common/_http_client.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)      825 2023-03-09 15:11:53.000000 catwalk_client-0.0.9/catwalk_client/common/catwalk_http_client.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)      216 2023-03-09 15:11:53.000000 catwalk_client-0.0.9/catwalk_client/common/constants.py
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-03-10 13:28:36.351777 catwalk_client-0.0.9/catwalk_client/tools/
+-rw-rw-r--   0 marek     (1000) marek     (1000)       80 2023-03-09 15:11:53.000000 catwalk_client-0.0.9/catwalk_client/tools/__init__.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)     1638 2023-03-09 15:11:53.000000 catwalk_client-0.0.9/catwalk_client/tools/_case_builder.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)     2745 2023-03-09 15:11:53.000000 catwalk_client-0.0.9/catwalk_client/tools/_case_exporter.py
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-03-10 13:28:36.351777 catwalk_client-0.0.9/catwalk_client.egg-info/
+-rw-rw-r--   0 marek     (1000) marek     (1000)     5104 2023-03-10 13:28:36.000000 catwalk_client-0.0.9/catwalk_client.egg-info/PKG-INFO
+-rw-rw-r--   0 marek     (1000) marek     (1000)      527 2023-03-10 13:28:36.000000 catwalk_client-0.0.9/catwalk_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)        1 2023-03-10 13:28:36.000000 catwalk_client-0.0.9/catwalk_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)       22 2023-03-10 13:28:36.000000 catwalk_client-0.0.9/catwalk_client.egg-info/requires.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)       15 2023-03-10 13:28:36.000000 catwalk_client-0.0.9/catwalk_client.egg-info/top_level.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)      442 2023-03-10 11:46:11.000000 catwalk_client-0.0.9/pyproject.toml
+-rw-rw-r--   0 marek     (1000) marek     (1000)       38 2023-03-10 13:28:36.351777 catwalk_client-0.0.9/setup.cfg
```

### Comparing `catwalk_client-0.0.8/PKG-INFO` & `catwalk_client-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catwalk_client
-Version: 0.0.8
+Version: 0.0.9
 Summary: Client for Catwalk
 Author-email: Marek Połom <marek.polom@deepsense.ai>, Mateusz Hordyński <mateusz.hordynski@deepsense.ai>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `catwalk_client-0.0.8/README.md` & `catwalk_client-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `catwalk_client-0.0.8/catwalk_client/client.py` & `catwalk_client-0.0.9/catwalk_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,22 +44,21 @@
 
     def set_insecure(self, insecure: bool):
         self.http_client.insecure = insecure
 
     def new_case(self) -> CaseBuilder:
         return CaseBuilder(client=self)
 
-    def send(self, case_id: str, case: dict):
+    def send(self, case: dict):
         try:
             case = CommonCaseFormat(
                 submitter={
                     "name": self.submitter_name,
                     "version": self.submitter_version,
                 },
-                case_id=case_id,
                 **case,
             )
 
             response, success = self.http_client.post("/api/cases/collect", case.json())
 
             if success:
                 case_id = loads(response)["id"]
```

### Comparing `catwalk_client-0.0.8/catwalk_client/common/_http_client.py` & `catwalk_client-0.0.9/catwalk_client/common/_http_client.py`

 * *Files identical despite different names*

### Comparing `catwalk_client-0.0.8/catwalk_client/common/catwalk_http_client.py` & `catwalk_client-0.0.9/catwalk_client/common/catwalk_http_client.py`

 * *Files identical despite different names*

### Comparing `catwalk_client-0.0.8/catwalk_client/tools/_case_builder.py` & `catwalk_client-0.0.9/catwalk_client/tools/_case_builder.py`

 * *Files identical despite different names*

### Comparing `catwalk_client-0.0.8/catwalk_client/tools/_case_exporter.py` & `catwalk_client-0.0.9/catwalk_client/tools/_case_exporter.py`

 * *Files identical despite different names*

### Comparing `catwalk_client-0.0.8/catwalk_client.egg-info/PKG-INFO` & `catwalk_client-0.0.9/catwalk_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catwalk-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: Client for Catwalk
 Author-email: Marek Połom <marek.polom@deepsense.ai>, Mateusz Hordyński <mateusz.hordynski@deepsense.ai>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `catwalk_client-0.0.8/catwalk_client.egg-info/SOURCES.txt` & `catwalk_client-0.0.9/catwalk_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

