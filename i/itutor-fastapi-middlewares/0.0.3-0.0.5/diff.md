# Comparing `tmp/itutor_fastapi_middlewares-0.0.3.tar.gz` & `tmp/itutor_fastapi_middlewares-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itutor_fastapi_middlewares-0.0.3.tar", last modified: Wed Apr  5 20:58:50 2023, max compression
+gzip compressed data, was "itutor_fastapi_middlewares-0.0.5.tar", last modified: Mon May  8 15:36:26 2023, max compression
```

## Comparing `itutor_fastapi_middlewares-0.0.3.tar` & `itutor_fastapi_middlewares-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:58:50.650741 itutor_fastapi_middlewares-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-05 20:58:38.000000 itutor_fastapi_middlewares-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-05 20:58:50.650741 itutor_fastapi_middlewares-0.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:58:50.646741 itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 20:58:38.000000 itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-05 20:58:38.000000 itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:58:50.646741 itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/itutor_google_sso/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-05 20:58:38.000000 itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/itutor_google_sso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-04-05 20:58:38.000000 itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/itutor_google_sso/itutor_google_sso.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:58:50.646741 itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/itutor_google_sso/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-05 20:58:38.000000 itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/itutor_google_sso/templates/login.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:58:50.642741 itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/statics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:58:50.642741 itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/statics/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:58:50.646741 itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/statics/dist/css/
--rw-r--r--   0 runner    (1001) docker     (123)   197782 2023-04-05 20:58:38.000000 itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/statics/dist/css/index.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:58:50.646741 itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/statics/dist/js/
--rw-r--r--   0 runner    (1001) docker     (123)  1187141 2023-04-05 20:58:38.000000 itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/statics/dist/js/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-05 20:58:38.000000 itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/statics/dist/js/index.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:58:50.646741 itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/statics/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:58:50.646741 itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/statics/src/images/
--rw-r--r--   0 runner    (1001) docker     (123)    26141 2023-04-05 20:58:38.000000 itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/statics/src/images/itutor-signature-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:58:50.646741 itutor_fastapi_middlewares-0.0.3/itutor_fastapi_middlewares.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-05 20:58:50.000000 itutor_fastapi_middlewares-0.0.3/itutor_fastapi_middlewares.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-05 20:58:50.000000 itutor_fastapi_middlewares-0.0.3/itutor_fastapi_middlewares.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 20:58:50.000000 itutor_fastapi_middlewares-0.0.3/itutor_fastapi_middlewares.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-05 20:58:50.000000 itutor_fastapi_middlewares-0.0.3/itutor_fastapi_middlewares.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-05 20:58:50.000000 itutor_fastapi_middlewares-0.0.3/itutor_fastapi_middlewares.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 20:58:50.650741 itutor_fastapi_middlewares-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-05 20:58:38.000000 itutor_fastapi_middlewares-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:26.594095 itutor_fastapi_middlewares-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 15:36:13.000000 itutor_fastapi_middlewares-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-08 15:36:26.594095 itutor_fastapi_middlewares-0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:26.586094 itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:13.000000 itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-08 15:36:13.000000 itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:26.590095 itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/itutor_google_sso/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-08 15:36:13.000000 itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/itutor_google_sso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-08 15:36:13.000000 itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/itutor_google_sso/itutor_google_sso.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:26.590095 itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/itutor_google_sso/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-08 15:36:13.000000 itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/itutor_google_sso/templates/login.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:26.586094 itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/statics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:26.586094 itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/statics/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:26.590095 itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/statics/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   197782 2023-05-08 15:36:13.000000 itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/statics/dist/css/index.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:26.590095 itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/statics/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (123)  1187141 2023-05-08 15:36:13.000000 itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/statics/dist/js/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-08 15:36:13.000000 itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/statics/dist/js/index.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:26.586094 itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/statics/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:26.590095 itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/statics/src/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    26141 2023-05-08 15:36:13.000000 itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/statics/src/images/itutor-signature-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:26.594095 itutor_fastapi_middlewares-0.0.5/itutor_fastapi_middlewares.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-08 15:36:26.000000 itutor_fastapi_middlewares-0.0.5/itutor_fastapi_middlewares.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-08 15:36:26.000000 itutor_fastapi_middlewares-0.0.5/itutor_fastapi_middlewares.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:36:26.000000 itutor_fastapi_middlewares-0.0.5/itutor_fastapi_middlewares.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 15:36:26.000000 itutor_fastapi_middlewares-0.0.5/itutor_fastapi_middlewares.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-08 15:36:26.000000 itutor_fastapi_middlewares-0.0.5/itutor_fastapi_middlewares.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:36:26.594095 itutor_fastapi_middlewares-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-08 15:36:13.000000 itutor_fastapi_middlewares-0.0.5/setup.py
```

### Comparing `itutor_fastapi_middlewares-0.0.3/PKG-INFO` & `itutor_fastapi_middlewares-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itutor_fastapi_middlewares
-Version: 0.0.3
+Version: 0.0.5
 Summary: Package for google sso login in FastAPI
 Home-page: https://github.com/bcpitutor/fastapi_middlewares
 Author: Nicolas Acosta
 Author-email: nicolas.acosta@itutor.com
 Keywords: google-sso,fastapi
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/examples.py` & `itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/examples.py`

 * *Files identical despite different names*

### Comparing `itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/itutor_google_sso/itutor_google_sso.py` & `itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/itutor_google_sso/itutor_google_sso.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,16 +60,16 @@
                     "redirect_to": path
                     })
                 response = RedirectResponse(f"{self.login_url}?{params}")
                 await response(scope, receive, send)
                 return 
             email: str = user.get("email")
             _, provider = email.split("@")
-            if provider != "itutor.com":
-               message = "Sorry, only @itutor.com email addresses are allowed."
+            if provider not in ["itutor.com", "fullmindlearning.com"]:
+               message = "Sorry, only @itutor.com and @fullmindlearning.com email addresses are allowed."
                response = RedirectResponse(f"{self.login_url}?error_message={str(message)}")
                await response(scope, receive, send)
                return 
             if self.allowed_users and email not in self.allowed_users:
                 message = f"Sorry {user.get('name')}, you are not allowed to access this page. Please contact your administrator to get access."
                 response = RedirectResponse(f"{self.login_url}?error_message={str(message)}")
                 await response(scope, receive, send)
```

### Comparing `itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/itutor_google_sso/templates/login.html` & `itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/itutor_google_sso/templates/login.html`

 * *Files identical despite different names*

### Comparing `itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/statics/dist/css/index.css` & `itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/statics/dist/css/index.css`

 * *Files identical despite different names*

### Comparing `itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/statics/dist/js/index.js` & `itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/statics/dist/js/index.js`

 * *Files identical despite different names*

### Comparing `itutor_fastapi_middlewares-0.0.3/fastapi_middlewares/statics/src/images/itutor-signature-logo.png` & `itutor_fastapi_middlewares-0.0.5/fastapi_middlewares/statics/src/images/itutor-signature-logo.png`

 * *Files identical despite different names*

### Comparing `itutor_fastapi_middlewares-0.0.3/itutor_fastapi_middlewares.egg-info/PKG-INFO` & `itutor_fastapi_middlewares-0.0.5/itutor_fastapi_middlewares.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itutor-fastapi-middlewares
-Version: 0.0.3
+Version: 0.0.5
 Summary: Package for google sso login in FastAPI
 Home-page: https://github.com/bcpitutor/fastapi_middlewares
 Author: Nicolas Acosta
 Author-email: nicolas.acosta@itutor.com
 Keywords: google-sso,fastapi
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `itutor_fastapi_middlewares-0.0.3/itutor_fastapi_middlewares.egg-info/SOURCES.txt` & `itutor_fastapi_middlewares-0.0.5/itutor_fastapi_middlewares.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `itutor_fastapi_middlewares-0.0.3/setup.py` & `itutor_fastapi_middlewares-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3' 
+VERSION = '0.0.5' 
 DESCRIPTION = 'Package for google sso login in FastAPI'
 LONG_DESCRIPTION = 'Package for google sso login in FastAPI'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="itutor_fastapi_middlewares",
```

