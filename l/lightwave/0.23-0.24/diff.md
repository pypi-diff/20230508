# Comparing `tmp/lightwave-0.23.tar.gz` & `tmp/lightwave-0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightwave-0.23.tar", last modified: Mon May  8 10:22:55 2023, max compression
+gzip compressed data, was "lightwave-0.24.tar", last modified: Mon May  8 10:41:48 2023, max compression
```

## Comparing `lightwave-0.23.tar` & `lightwave-0.24.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2023-05-08 10:22:55.957760 lightwave-0.23/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1068 2023-01-04 14:14:06.000000 lightwave-0.23/LICENSE
--rw-rw-r--   0 colin     (1000) colin     (1000)     3619 2023-05-08 10:22:55.957760 lightwave-0.23/PKG-INFO
--rw-rw-r--   0 colin     (1000) colin     (1000)     3211 2023-05-08 10:07:39.000000 lightwave-0.23/README.md
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2023-05-08 10:22:55.957760 lightwave-0.23/lightwave/
--rw-rw-r--   0 colin     (1000) colin     (1000)        0 2023-01-04 14:14:06.000000 lightwave-0.23/lightwave/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     9030 2023-05-08 10:20:33.000000 lightwave-0.23/lightwave/lightwave.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2023-05-08 10:22:55.957760 lightwave-0.23/lightwave.egg-info/
--rw-rw-r--   0 colin     (1000) colin     (1000)     3619 2023-05-08 10:22:55.000000 lightwave-0.23/lightwave.egg-info/PKG-INFO
--rw-rw-r--   0 colin     (1000) colin     (1000)      265 2023-05-08 10:22:55.000000 lightwave-0.23/lightwave.egg-info/SOURCES.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)        1 2023-05-08 10:22:55.000000 lightwave-0.23/lightwave.egg-info/dependency_links.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)        1 2023-01-07 13:37:53.000000 lightwave-0.23/lightwave.egg-info/not-zip-safe
--rw-rw-r--   0 colin     (1000) colin     (1000)       10 2023-05-08 10:22:55.000000 lightwave-0.23/lightwave.egg-info/top_level.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)       38 2023-05-08 10:22:55.957760 lightwave-0.23/setup.cfg
--rw-rw-r--   0 colin     (1000) colin     (1000)      652 2023-05-08 10:22:08.000000 lightwave-0.23/setup.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2023-05-08 10:22:55.957760 lightwave-0.23/test/
--rw-rw-r--   0 colin     (1000) colin     (1000)      630 2023-01-04 14:14:06.000000 lightwave-0.23/test/test.py
--rw-rw-r--   0 colin     (1000) colin     (1000)      328 2023-01-04 14:14:06.000000 lightwave-0.23/test/test_trv.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2023-05-08 10:41:48.724088 lightwave-0.24/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1068 2023-01-04 14:14:06.000000 lightwave-0.24/LICENSE
+-rw-rw-r--   0 colin     (1000) colin     (1000)     3619 2023-05-08 10:41:48.724088 lightwave-0.24/PKG-INFO
+-rw-rw-r--   0 colin     (1000) colin     (1000)     3211 2023-05-08 10:07:39.000000 lightwave-0.24/README.md
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2023-05-08 10:41:48.724088 lightwave-0.24/lightwave/
+-rw-rw-r--   0 colin     (1000) colin     (1000)        0 2023-01-04 14:14:06.000000 lightwave-0.24/lightwave/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     9087 2023-05-08 10:40:00.000000 lightwave-0.24/lightwave/lightwave.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2023-05-08 10:41:48.724088 lightwave-0.24/lightwave.egg-info/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     3619 2023-05-08 10:41:48.000000 lightwave-0.24/lightwave.egg-info/PKG-INFO
+-rw-rw-r--   0 colin     (1000) colin     (1000)      265 2023-05-08 10:41:48.000000 lightwave-0.24/lightwave.egg-info/SOURCES.txt
+-rw-rw-r--   0 colin     (1000) colin     (1000)        1 2023-05-08 10:41:48.000000 lightwave-0.24/lightwave.egg-info/dependency_links.txt
+-rw-rw-r--   0 colin     (1000) colin     (1000)        1 2023-01-07 13:37:53.000000 lightwave-0.24/lightwave.egg-info/not-zip-safe
+-rw-rw-r--   0 colin     (1000) colin     (1000)       10 2023-05-08 10:41:48.000000 lightwave-0.24/lightwave.egg-info/top_level.txt
+-rw-rw-r--   0 colin     (1000) colin     (1000)       38 2023-05-08 10:41:48.724088 lightwave-0.24/setup.cfg
+-rw-rw-r--   0 colin     (1000) colin     (1000)      652 2023-05-08 10:41:08.000000 lightwave-0.24/setup.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2023-05-08 10:41:48.724088 lightwave-0.24/test/
+-rw-rw-r--   0 colin     (1000) colin     (1000)      630 2023-01-04 14:14:06.000000 lightwave-0.24/test/test.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)      328 2023-01-04 14:14:06.000000 lightwave-0.24/test/test_trv.py
```

### Comparing `lightwave-0.23/LICENSE` & `lightwave-0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `lightwave-0.23/PKG-INFO` & `lightwave-0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightwave
-Version: 0.23
+Version: 0.24
 Summary: Python library to provide a reliable communication link with LightWaveRF lights, switches and TRVs.
 Home-page: https://github.com/GeoffAtHome/lightwave
 Author: Geoff Soord
 Author-email: geoff@soord.org.uk
 License: MIT
 Keywords: Lightwave,LightwaveRF,Lightwave WiFiLink,Lightwave Link
 Description-Content-Type: text/markdown
```

### Comparing `lightwave-0.23/README.md` & `lightwave-0.24/README.md`

 * *Files identical despite different names*

### Comparing `lightwave-0.23/lightwave/lightwave.py` & `lightwave-0.24/lightwave/lightwave.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,16 @@
             self.register()
             return True
 
         if response.startswith("%d,OK" % trans_id):
             _LOGGER.debug("got OK")
             return True
 
-        _LOGGER.error("error %s", response)
+        if response.startswith("%d,ERR" % trans_id):
+            _LOGGER.error("error %s", response)
 
         return False
 
     def _send_reliable_message(self, msg):
         """Send msg to LightwaveRF hub."""
         result = False
         max_retries = 15
```

### Comparing `lightwave-0.23/lightwave.egg-info/PKG-INFO` & `lightwave-0.24/lightwave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightwave
-Version: 0.23
+Version: 0.24
 Summary: Python library to provide a reliable communication link with LightWaveRF lights, switches and TRVs.
 Home-page: https://github.com/GeoffAtHome/lightwave
 Author: Geoff Soord
 Author-email: geoff@soord.org.uk
 License: MIT
 Keywords: Lightwave,LightwaveRF,Lightwave WiFiLink,Lightwave Link
 Description-Content-Type: text/markdown
```

### Comparing `lightwave-0.23/setup.py` & `lightwave-0.24/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='lightwave',
-    version='0.23',
+    version='0.24',
     description='Python library to provide a reliable communication link with LightWaveRF lights, switches and TRVs.',
     url='https://github.com/GeoffAtHome/lightwave',
     author='Geoff Soord',
     author_email='geoff@soord.org.uk',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

### Comparing `lightwave-0.23/test/test.py` & `lightwave-0.24/test/test.py`

 * *Files identical despite different names*

