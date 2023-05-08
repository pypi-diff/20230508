# Comparing `tmp/toast_auth-0.1.1.tar.gz` & `tmp/toast_auth-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toast_auth-0.1.1.tar", last modified: Fri May  5 19:51:35 2023, max compression
+gzip compressed data, was "toast_auth-0.1.2.tar", last modified: Mon May  8 18:24:12 2023, max compression
```

## Comparing `toast_auth-0.1.1.tar` & `toast_auth-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 turner    (1000) turner    (1000)        0 2023-05-05 19:51:35.107593 toast_auth-0.1.1/
--rw-rw-r--   0 turner    (1000) turner    (1000)      247 2023-05-05 19:51:35.107593 toast_auth-0.1.1/PKG-INFO
--rw-rw-r--   0 turner    (1000) turner    (1000)     1093 2023-05-05 16:23:48.000000 toast_auth-0.1.1/README.md
--rw-rw-r--   0 turner    (1000) turner    (1000)      107 2023-05-05 19:51:35.111593 toast_auth-0.1.1/setup.cfg
--rw-rw-r--   0 turner    (1000) turner    (1000)      638 2023-05-05 19:51:27.000000 toast_auth-0.1.1/setup.py
-drwxrwxr-x   0 turner    (1000) turner    (1000)        0 2023-05-05 19:51:35.107593 toast_auth-0.1.1/src/
-drwxrwxr-x   0 turner    (1000) turner    (1000)        0 2023-05-05 19:51:35.107593 toast_auth-0.1.1/src/storage/
--rw-rw-r--   0 turner    (1000) turner    (1000)        0 2023-05-05 14:42:59.000000 toast_auth-0.1.1/src/storage/__init__.py
--rw-rw-r--   0 turner    (1000) turner    (1000)     1250 2023-05-05 16:21:15.000000 toast_auth-0.1.1/src/storage/get_token.py
-drwxrwxr-x   0 turner    (1000) turner    (1000)        0 2023-05-05 19:51:35.107593 toast_auth-0.1.1/src/toast_auth/
--rw-rw-r--   0 turner    (1000) turner    (1000)       35 2023-05-05 16:10:31.000000 toast_auth-0.1.1/src/toast_auth/__init__.py
--rw-rw-r--   0 turner    (1000) turner    (1000)     3221 2023-05-05 16:29:33.000000 toast_auth-0.1.1/src/toast_auth/toast_token.py
-drwxrwxr-x   0 turner    (1000) turner    (1000)        0 2023-05-05 19:51:35.107593 toast_auth-0.1.1/src/toast_auth.egg-info/
--rw-rw-r--   0 turner    (1000) turner    (1000)      247 2023-05-05 19:51:35.000000 toast_auth-0.1.1/src/toast_auth.egg-info/PKG-INFO
--rw-rw-r--   0 turner    (1000) turner    (1000)      323 2023-05-05 19:51:35.000000 toast_auth-0.1.1/src/toast_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 turner    (1000) turner    (1000)        1 2023-05-05 19:51:35.000000 toast_auth-0.1.1/src/toast_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 turner    (1000) turner    (1000)      104 2023-05-05 19:51:35.000000 toast_auth-0.1.1/src/toast_auth.egg-info/requires.txt
--rw-rw-r--   0 turner    (1000) turner    (1000)       19 2023-05-05 19:51:35.000000 toast_auth-0.1.1/src/toast_auth.egg-info/top_level.txt
+drwxrwxr-x   0 turner    (1000) turner    (1000)        0 2023-05-08 18:24:12.632770 toast_auth-0.1.2/
+-rw-rw-r--   0 turner    (1000) turner    (1000)      247 2023-05-08 18:24:12.632770 toast_auth-0.1.2/PKG-INFO
+-rw-rw-r--   0 turner    (1000) turner    (1000)     1093 2023-05-05 16:23:48.000000 toast_auth-0.1.2/README.md
+-rw-rw-r--   0 turner    (1000) turner    (1000)      107 2023-05-08 18:24:12.632770 toast_auth-0.1.2/setup.cfg
+-rw-rw-r--   0 turner    (1000) turner    (1000)      638 2023-05-08 18:20:17.000000 toast_auth-0.1.2/setup.py
+drwxrwxr-x   0 turner    (1000) turner    (1000)        0 2023-05-08 18:24:12.632770 toast_auth-0.1.2/src/
+drwxrwxr-x   0 turner    (1000) turner    (1000)        0 2023-05-08 18:24:12.632770 toast_auth-0.1.2/src/storage/
+-rw-rw-r--   0 turner    (1000) turner    (1000)        0 2023-05-05 14:42:59.000000 toast_auth-0.1.2/src/storage/__init__.py
+-rw-rw-r--   0 turner    (1000) turner    (1000)     1250 2023-05-05 16:21:15.000000 toast_auth-0.1.2/src/storage/get_token.py
+drwxrwxr-x   0 turner    (1000) turner    (1000)        0 2023-05-08 18:24:12.632770 toast_auth-0.1.2/src/toast_auth/
+-rw-rw-r--   0 turner    (1000) turner    (1000)       35 2023-05-05 16:10:31.000000 toast_auth-0.1.2/src/toast_auth/__init__.py
+-rw-rw-r--   0 turner    (1000) turner    (1000)     3323 2023-05-08 17:15:29.000000 toast_auth-0.1.2/src/toast_auth/toast_token.py
+drwxrwxr-x   0 turner    (1000) turner    (1000)        0 2023-05-08 18:24:12.632770 toast_auth-0.1.2/src/toast_auth.egg-info/
+-rw-rw-r--   0 turner    (1000) turner    (1000)      247 2023-05-08 18:24:12.000000 toast_auth-0.1.2/src/toast_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 turner    (1000) turner    (1000)      323 2023-05-08 18:24:12.000000 toast_auth-0.1.2/src/toast_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 turner    (1000) turner    (1000)        1 2023-05-08 18:24:12.000000 toast_auth-0.1.2/src/toast_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 turner    (1000) turner    (1000)      104 2023-05-08 18:24:12.000000 toast_auth-0.1.2/src/toast_auth.egg-info/requires.txt
+-rw-rw-r--   0 turner    (1000) turner    (1000)       19 2023-05-08 18:24:12.000000 toast_auth-0.1.2/src/toast_auth.egg-info/top_level.txt
```

### Comparing `toast_auth-0.1.1/README.md` & `toast_auth-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `toast_auth-0.1.1/setup.py` & `toast_auth-0.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='toast_auth',
-    version='0.1.1',
+    version='0.1.2',
     license='MIT',
     description='Class object to help facilitate authentication with Toast API.',
     url='https://github.com/turnerluke/toast_auth',
     author='Turner Luke',
     author_email='turnermluke@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
```

### Comparing `toast_auth-0.1.1/src/storage/get_token.py` & `toast_auth-0.1.2/src/storage/get_token.py`

 * *Files identical despite different names*

### Comparing `toast_auth-0.1.1/src/toast_auth/toast_token.py` & `toast_auth-0.1.2/src/toast_auth/toast_token.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,18 +71,21 @@
             url = f'{os.environ.get("TOAST_API_SERVER")}/authentication/v1/authentication/login'
 
             payload = {
                 "clientId": os.environ.get('TOAST_CLIENT_ID'),
                 "clientSecret": os.environ.get('TOAST_CLIENT_SECRET'),
                 "userAccessType": "TOAST_MACHINE_CLIENT"
             }
+
             headers = {"Content-Type": "application/json"}
             response = requests.post(url, json=payload, headers=headers)
 
             data = response.json()
+            if data['status'] == 401:
+                raise ValueError("Invalid Toast credentials.")
             token = data['token']['accessToken']
 
             expires = dt.datetime.now() + dt.timedelta(seconds=data['token']['expiresIn'])
             self.write_token_json(token, expires)
             return f"Bearer {token}", expires
 
     @property
```

