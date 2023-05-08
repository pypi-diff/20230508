# Comparing `tmp/cidc_api_modules-0.9.4.tar.gz` & `tmp/cidc_api_modules-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cidc_api_modules-0.9.4.tar", last modified: Wed Nov 13 15:15:20 2019, max compression
+gzip compressed data, was "dist/cidc_api_modules-0.9.5.tar", last modified: Fri Nov 15 16:44:42 2019, max compression
```

## Comparing `cidc_api_modules-0.9.4.tar` & `cidc_api_modules-0.9.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-13 15:15:20.000000 cidc_api_modules-0.9.4/
--rw-rw-r--   0 travis    (2000) travis    (2000)      156 2019-11-13 15:13:27.000000 cidc_api_modules-0.9.4/requirements.modules.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       32 2019-11-13 15:13:27.000000 cidc_api_modules-0.9.4/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      274 2019-11-13 15:15:20.000000 cidc_api_modules-0.9.4/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     8164 2019-11-13 15:13:27.000000 cidc_api_modules-0.9.4/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-11-13 15:15:20.000000 cidc_api_modules-0.9.4/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-13 15:15:20.000000 cidc_api_modules-0.9.4/cidc_api_modules.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      274 2019-11-13 15:15:20.000000 cidc_api_modules-0.9.4/cidc_api_modules.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-13 15:15:20.000000 cidc_api_modules-0.9.4/cidc_api_modules.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2019-11-13 15:15:20.000000 cidc_api_modules-0.9.4/cidc_api_modules.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-13 15:15:20.000000 cidc_api_modules-0.9.4/cidc_api_modules.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      462 2019-11-13 15:15:20.000000 cidc_api_modules-0.9.4/cidc_api_modules.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      156 2019-11-13 15:15:20.000000 cidc_api_modules-0.9.4/cidc_api_modules.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      606 2019-11-13 15:13:27.000000 cidc_api_modules-0.9.4/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-13 15:15:20.000000 cidc_api_modules-0.9.4/cidc_api/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7115 2019-11-13 15:13:27.000000 cidc_api_modules-0.9.4/cidc_api/gcloud_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2738 2019-11-13 15:13:27.000000 cidc_api_modules-0.9.4/cidc_api/emails.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26866 2019-11-13 15:13:27.000000 cidc_api_modules-0.9.4/cidc_api/models.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-13 15:15:20.000000 cidc_api_modules-0.9.4/cidc_api/config/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1857 2019-11-13 15:13:27.000000 cidc_api_modules-0.9.4/cidc_api/config/secrets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1443 2019-11-13 15:13:27.000000 cidc_api_modules-0.9.4/cidc_api/config/db.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      188 2019-11-13 15:13:27.000000 cidc_api_modules-0.9.4/cidc_api/config/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2274 2019-11-13 15:13:27.000000 cidc_api_modules-0.9.4/cidc_api/config/settings.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-15 16:44:42.000000 cidc_api_modules-0.9.5/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      195 2019-11-15 16:42:38.000000 cidc_api_modules-0.9.5/requirements.modules.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       32 2019-11-15 16:42:38.000000 cidc_api_modules-0.9.5/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      274 2019-11-15 16:44:42.000000 cidc_api_modules-0.9.5/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8164 2019-11-15 16:42:38.000000 cidc_api_modules-0.9.5/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-11-15 16:44:42.000000 cidc_api_modules-0.9.5/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-15 16:44:42.000000 cidc_api_modules-0.9.5/cidc_api_modules.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      274 2019-11-15 16:44:42.000000 cidc_api_modules-0.9.5/cidc_api_modules.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-15 16:44:42.000000 cidc_api_modules-0.9.5/cidc_api_modules.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2019-11-15 16:44:42.000000 cidc_api_modules-0.9.5/cidc_api_modules.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-15 16:44:42.000000 cidc_api_modules-0.9.5/cidc_api_modules.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      462 2019-11-15 16:44:42.000000 cidc_api_modules-0.9.5/cidc_api_modules.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      195 2019-11-15 16:44:42.000000 cidc_api_modules-0.9.5/cidc_api_modules.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      606 2019-11-15 16:42:38.000000 cidc_api_modules-0.9.5/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-15 16:44:42.000000 cidc_api_modules-0.9.5/cidc_api/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7115 2019-11-15 16:42:38.000000 cidc_api_modules-0.9.5/cidc_api/gcloud_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2738 2019-11-15 16:42:38.000000 cidc_api_modules-0.9.5/cidc_api/emails.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26866 2019-11-15 16:42:38.000000 cidc_api_modules-0.9.5/cidc_api/models.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-15 16:44:42.000000 cidc_api_modules-0.9.5/cidc_api/config/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1857 2019-11-15 16:42:38.000000 cidc_api_modules-0.9.5/cidc_api/config/secrets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1443 2019-11-15 16:42:38.000000 cidc_api_modules-0.9.5/cidc_api/config/db.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      188 2019-11-15 16:42:38.000000 cidc_api_modules-0.9.5/cidc_api/config/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2274 2019-11-15 16:42:38.000000 cidc_api_modules-0.9.5/cidc_api/config/settings.py
```

### Comparing `cidc_api_modules-0.9.4/README.md` & `cidc_api_modules-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `cidc_api_modules-0.9.4/setup.py` & `cidc_api_modules-0.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,10 +10,10 @@
     description="SQLAlchemy data models and configuration tools used in the CIDC API",
     python_requires=">=3.6",
     install_requires=requirements,
     license="MIT license",
     packages=["cidc_api.config"],
     py_modules=["cidc_api.models", "cidc_api.gcloud_client", "cidc_api.emails"],
     url="https://github.com/CIMAC-CIDC/cidc_api-gae",
-    version="0.9.4",
+    version="0.9.5",
     zip_safe=False,
 )
```

### Comparing `cidc_api_modules-0.9.4/cidc_api/gcloud_client.py` & `cidc_api_modules-0.9.5/cidc_api/gcloud_client.py`

 * *Files identical despite different names*

### Comparing `cidc_api_modules-0.9.4/cidc_api/emails.py` & `cidc_api_modules-0.9.5/cidc_api/emails.py`

 * *Files identical despite different names*

### Comparing `cidc_api_modules-0.9.4/cidc_api/models.py` & `cidc_api_modules-0.9.5/cidc_api/models.py`

 * *Files identical despite different names*

### Comparing `cidc_api_modules-0.9.4/cidc_api/config/secrets.py` & `cidc_api_modules-0.9.5/cidc_api/config/secrets.py`

 * *Files identical despite different names*

### Comparing `cidc_api_modules-0.9.4/cidc_api/config/db.py` & `cidc_api_modules-0.9.5/cidc_api/config/db.py`

 * *Files identical despite different names*

### Comparing `cidc_api_modules-0.9.4/cidc_api/config/settings.py` & `cidc_api_modules-0.9.5/cidc_api/config/settings.py`

 * *Files identical despite different names*

