# Comparing `tmp/ajenti-panel-2.2.4.tar.gz` & `tmp/ajenti-panel-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ajenti-panel-2.2.4.tar", last modified: Mon Feb 13 11:54:55 2023, max compression
+gzip compressed data, was "ajenti-panel-2.2.5.tar", last modified: Mon May  8 04:10:16 2023, max compression
```

## Comparing `ajenti-panel-2.2.4.tar` & `ajenti-panel-2.2.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-02-13 11:54:55.610257 ajenti-panel-2.2.4/
--rw-r--r--   0 eugene     (501) staff       (20)      190 2023-02-13 11:54:55.610332 ajenti-panel-2.2.4/PKG-INFO
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-02-13 11:54:55.604886 ajenti-panel-2.2.4/aj/
--rw-r--r--   0 eugene     (501) staff       (20)     4243 2023-02-13 11:54:42.000000 ajenti-panel-2.2.4/aj/__init__.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-02-13 11:54:55.605492 ajenti-panel-2.2.4/aj/api/
--rw-r--r--   0 eugene     (501) staff       (20)      188 2020-04-13 10:52:48.000000 ajenti-panel-2.2.4/aj/api/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)     3940 2023-02-13 11:54:42.000000 ajenti-panel-2.2.4/aj/api/endpoint.py
--rw-r--r--   0 eugene     (501) staff       (20)     7176 2023-02-13 11:54:42.000000 ajenti-panel-2.2.4/aj/api/http.py
--rw-r--r--   0 eugene     (501) staff       (20)     4994 2022-02-17 09:04:54.000000 ajenti-panel-2.2.4/aj/api/mail.py
--rw-r--r--   0 eugene     (501) staff       (20)     8389 2022-06-28 14:12:43.000000 ajenti-panel-2.2.4/aj/auth.py
--rw-r--r--   0 eugene     (501) staff       (20)     2161 2022-06-28 14:12:43.000000 ajenti-panel-2.2.4/aj/compat.py
--rw-r--r--   0 eugene     (501) staff       (20)    12255 2023-02-13 11:54:42.000000 ajenti-panel-2.2.4/aj/config.py
--rw-r--r--   0 eugene     (501) staff       (20)    10353 2023-01-06 10:26:21.000000 ajenti-panel-2.2.4/aj/core.py
--rw-r--r--   0 eugene     (501) staff       (20)     1958 2022-02-17 09:04:54.000000 ajenti-panel-2.2.4/aj/entry.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-02-13 11:54:55.606496 ajenti-panel-2.2.4/aj/gate/
--rw-r--r--   0 eugene     (501) staff       (20)        0 2020-04-13 10:52:48.000000 ajenti-panel-2.2.4/aj/gate/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)     6351 2023-01-06 10:26:21.000000 ajenti-panel-2.2.4/aj/gate/gate.py
--rw-r--r--   0 eugene     (501) staff       (20)     9770 2023-02-13 11:54:42.000000 ajenti-panel-2.2.4/aj/gate/middleware.py
--rw-r--r--   0 eugene     (501) staff       (20)     2134 2023-02-13 11:54:42.000000 ajenti-panel-2.2.4/aj/gate/session.py
--rw-r--r--   0 eugene     (501) staff       (20)     3899 2022-02-17 09:04:54.000000 ajenti-panel-2.2.4/aj/gate/stream.py
--rw-r--r--   0 eugene     (501) staff       (20)     7857 2023-01-06 10:26:21.000000 ajenti-panel-2.2.4/aj/gate/worker.py
--rw-r--r--   0 eugene     (501) staff       (20)    13431 2023-02-13 11:54:42.000000 ajenti-panel-2.2.4/aj/http.py
--rw-r--r--   0 eugene     (501) staff       (20)      856 2022-06-28 14:12:43.000000 ajenti-panel-2.2.4/aj/https_redirect.py
--rw-r--r--   0 eugene     (501) staff       (20)     4095 2022-06-28 14:12:43.000000 ajenti-panel-2.2.4/aj/log.py
--rw-r--r--   0 eugene     (501) staff       (20)    10728 2023-02-13 11:54:42.000000 ajenti-panel-2.2.4/aj/plugins.py
--rw-r--r--   0 eugene     (501) staff       (20)     4533 2023-01-06 10:26:21.000000 ajenti-panel-2.2.4/aj/routing.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-02-13 11:54:55.607229 ajenti-panel-2.2.4/aj/security/
--rw-r--r--   0 eugene     (501) staff       (20)        0 2020-04-13 10:52:48.000000 ajenti-panel-2.2.4/aj/security/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)     4395 2022-02-17 09:04:54.000000 ajenti-panel-2.2.4/aj/security/pwreset.py
--rw-r--r--   0 eugene     (501) staff       (20)      786 2023-01-06 10:26:21.000000 ajenti-panel-2.2.4/aj/security/totp.py
--rw-r--r--   0 eugene     (501) staff       (20)      802 2022-06-28 14:12:43.000000 ajenti-panel-2.2.4/aj/security/verifier.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-02-13 11:54:55.601192 ajenti-panel-2.2.4/aj/static/
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-02-13 11:54:55.607437 ajenti-panel-2.2.4/aj/static/emails/
--rw-r--r--   0 eugene     (501) staff       (20)     1680 2022-02-17 09:04:54.000000 ajenti-panel-2.2.4/aj/static/emails/reset_email.html
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-02-13 11:54:55.607975 ajenti-panel-2.2.4/aj/static/images/
--rw-r--r--   0 eugene     (501) staff       (20)    19273 2022-02-17 09:04:54.000000 ajenti-panel-2.2.4/aj/static/images/Logo.png
--rw-r--r--   0 eugene     (501) staff       (20)     3612 2020-04-13 10:52:48.000000 ajenti-panel-2.2.4/aj/static/images/error.jpeg
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-02-13 11:54:55.609268 ajenti-panel-2.2.4/aj/util/
--rw-r--r--   0 eugene     (501) staff       (20)      340 2020-04-13 10:52:48.000000 ajenti-panel-2.2.4/aj/util/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)      402 2020-05-02 13:26:29.000000 ajenti-panel-2.2.4/aj/util/broadcast_queue.py
--rw-r--r--   0 eugene     (501) staff       (20)      708 2022-02-17 09:04:54.000000 ajenti-panel-2.2.4/aj/util/lazy.py
--rw-r--r--   0 eugene     (501) staff       (20)     1577 2022-02-17 09:04:54.000000 ajenti-panel-2.2.4/aj/util/misc.py
--rw-r--r--   0 eugene     (501) staff       (20)     1074 2020-05-02 13:26:29.000000 ajenti-panel-2.2.4/aj/util/pidfile.py
--rw-r--r--   0 eugene     (501) staff       (20)      527 2020-04-13 10:52:48.000000 ajenti-panel-2.2.4/aj/util/public.py
--rw-r--r--   0 eugene     (501) staff       (20)      373 2022-06-28 14:12:43.000000 ajenti-panel-2.2.4/aj/util/strings.py
--rw-r--r--   0 eugene     (501) staff       (20)     2424 2022-06-28 14:12:43.000000 ajenti-panel-2.2.4/aj/wsgi.py
--rwxr-xr-x   0 eugene     (501) staff       (20)     1858 2022-06-28 14:12:43.000000 ajenti-panel-2.2.4/ajenti-client-ssl-gen
--rwxr-xr-x   0 eugene     (501) staff       (20)     4261 2023-01-06 10:26:21.000000 ajenti-panel-2.2.4/ajenti-panel
--rwxr-xr-x   0 eugene     (501) staff       (20)     1340 2022-06-28 14:12:43.000000 ajenti-panel-2.2.4/ajenti-ssl-gen
--rwxr-xr-x   0 eugene     (501) staff       (20)     1477 2022-02-17 09:04:54.000000 ajenti-panel-2.2.4/ajenti-upgrade
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-02-13 11:54:55.610106 ajenti-panel-2.2.4/ajenti_panel.egg-info/
--rw-r--r--   0 eugene     (501) staff       (20)      190 2023-02-13 11:54:55.000000 ajenti-panel-2.2.4/ajenti_panel.egg-info/PKG-INFO
--rw-r--r--   0 eugene     (501) staff       (20)      913 2023-02-13 11:54:55.000000 ajenti-panel-2.2.4/ajenti_panel.egg-info/SOURCES.txt
--rw-r--r--   0 eugene     (501) staff       (20)        1 2023-02-13 11:54:55.000000 ajenti-panel-2.2.4/ajenti_panel.egg-info/dependency_links.txt
--rw-r--r--   0 eugene     (501) staff       (20)       26 2023-02-13 11:54:55.000000 ajenti-panel-2.2.4/ajenti_panel.egg-info/requires.txt
--rw-r--r--   0 eugene     (501) staff       (20)        3 2023-02-13 11:54:55.000000 ajenti-panel-2.2.4/ajenti_panel.egg-info/top_level.txt
--rw-r--r--   0 eugene     (501) staff       (20)       67 2023-02-13 11:54:55.610565 ajenti-panel-2.2.4/setup.cfg
--rwxr-xr-x   0 eugene     (501) staff       (20)     1924 2023-02-13 11:54:42.000000 ajenti-panel-2.2.4/setup.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:16.653646 ajenti-panel-2.2.5/
+-rw-r--r--   0 eugene     (501) staff       (20)      190 2023-05-08 04:10:16.653733 ajenti-panel-2.2.5/PKG-INFO
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:16.649271 ajenti-panel-2.2.5/aj/
+-rw-r--r--   0 eugene     (501) staff       (20)     4243 2023-05-08 04:08:59.000000 ajenti-panel-2.2.5/aj/__init__.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:16.649768 ajenti-panel-2.2.5/aj/api/
+-rw-r--r--   0 eugene     (501) staff       (20)      188 2020-04-13 10:52:48.000000 ajenti-panel-2.2.5/aj/api/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)     3940 2023-02-13 11:54:42.000000 ajenti-panel-2.2.5/aj/api/endpoint.py
+-rw-r--r--   0 eugene     (501) staff       (20)     7176 2023-02-13 11:54:42.000000 ajenti-panel-2.2.5/aj/api/http.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4994 2022-02-17 09:04:54.000000 ajenti-panel-2.2.5/aj/api/mail.py
+-rw-r--r--   0 eugene     (501) staff       (20)     8389 2022-06-28 14:12:43.000000 ajenti-panel-2.2.5/aj/auth.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2161 2022-06-28 14:12:43.000000 ajenti-panel-2.2.5/aj/compat.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12255 2023-02-13 11:54:42.000000 ajenti-panel-2.2.5/aj/config.py
+-rw-r--r--   0 eugene     (501) staff       (20)    10353 2023-01-06 10:26:21.000000 ajenti-panel-2.2.5/aj/core.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1958 2022-02-17 09:04:54.000000 ajenti-panel-2.2.5/aj/entry.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:16.650577 ajenti-panel-2.2.5/aj/gate/
+-rw-r--r--   0 eugene     (501) staff       (20)        0 2020-04-13 10:52:48.000000 ajenti-panel-2.2.5/aj/gate/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)     6351 2023-01-06 10:26:21.000000 ajenti-panel-2.2.5/aj/gate/gate.py
+-rw-r--r--   0 eugene     (501) staff       (20)     9770 2023-02-13 11:54:42.000000 ajenti-panel-2.2.5/aj/gate/middleware.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2134 2023-02-13 11:54:42.000000 ajenti-panel-2.2.5/aj/gate/session.py
+-rw-r--r--   0 eugene     (501) staff       (20)     3899 2022-02-17 09:04:54.000000 ajenti-panel-2.2.5/aj/gate/stream.py
+-rw-r--r--   0 eugene     (501) staff       (20)     7857 2023-01-06 10:26:21.000000 ajenti-panel-2.2.5/aj/gate/worker.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13431 2023-02-13 11:54:42.000000 ajenti-panel-2.2.5/aj/http.py
+-rw-r--r--   0 eugene     (501) staff       (20)      856 2022-06-28 14:12:43.000000 ajenti-panel-2.2.5/aj/https_redirect.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4095 2022-06-28 14:12:43.000000 ajenti-panel-2.2.5/aj/log.py
+-rw-r--r--   0 eugene     (501) staff       (20)    10728 2023-02-13 11:54:42.000000 ajenti-panel-2.2.5/aj/plugins.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4533 2023-01-06 10:26:21.000000 ajenti-panel-2.2.5/aj/routing.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:16.651201 ajenti-panel-2.2.5/aj/security/
+-rw-r--r--   0 eugene     (501) staff       (20)        0 2020-04-13 10:52:48.000000 ajenti-panel-2.2.5/aj/security/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4395 2022-02-17 09:04:54.000000 ajenti-panel-2.2.5/aj/security/pwreset.py
+-rw-r--r--   0 eugene     (501) staff       (20)      786 2023-01-06 10:26:21.000000 ajenti-panel-2.2.5/aj/security/totp.py
+-rw-r--r--   0 eugene     (501) staff       (20)      802 2022-06-28 14:12:43.000000 ajenti-panel-2.2.5/aj/security/verifier.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:16.646004 ajenti-panel-2.2.5/aj/static/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:16.651355 ajenti-panel-2.2.5/aj/static/emails/
+-rw-r--r--   0 eugene     (501) staff       (20)     1680 2022-02-17 09:04:54.000000 ajenti-panel-2.2.5/aj/static/emails/reset_email.html
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:16.651753 ajenti-panel-2.2.5/aj/static/images/
+-rw-r--r--   0 eugene     (501) staff       (20)    19273 2022-02-17 09:04:54.000000 ajenti-panel-2.2.5/aj/static/images/Logo.png
+-rw-r--r--   0 eugene     (501) staff       (20)     3612 2020-04-13 10:52:48.000000 ajenti-panel-2.2.5/aj/static/images/error.jpeg
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:16.652873 ajenti-panel-2.2.5/aj/util/
+-rw-r--r--   0 eugene     (501) staff       (20)      340 2020-04-13 10:52:48.000000 ajenti-panel-2.2.5/aj/util/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)      402 2020-05-02 13:26:29.000000 ajenti-panel-2.2.5/aj/util/broadcast_queue.py
+-rw-r--r--   0 eugene     (501) staff       (20)      708 2022-02-17 09:04:54.000000 ajenti-panel-2.2.5/aj/util/lazy.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1577 2022-02-17 09:04:54.000000 ajenti-panel-2.2.5/aj/util/misc.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1074 2020-05-02 13:26:29.000000 ajenti-panel-2.2.5/aj/util/pidfile.py
+-rw-r--r--   0 eugene     (501) staff       (20)      527 2020-04-13 10:52:48.000000 ajenti-panel-2.2.5/aj/util/public.py
+-rw-r--r--   0 eugene     (501) staff       (20)      373 2022-06-28 14:12:43.000000 ajenti-panel-2.2.5/aj/util/strings.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2424 2022-06-28 14:12:43.000000 ajenti-panel-2.2.5/aj/wsgi.py
+-rwxr-xr-x   0 eugene     (501) staff       (20)     1858 2022-06-28 14:12:43.000000 ajenti-panel-2.2.5/ajenti-client-ssl-gen
+-rwxr-xr-x   0 eugene     (501) staff       (20)     4261 2023-01-06 10:26:21.000000 ajenti-panel-2.2.5/ajenti-panel
+-rwxr-xr-x   0 eugene     (501) staff       (20)     1340 2022-06-28 14:12:43.000000 ajenti-panel-2.2.5/ajenti-ssl-gen
+-rwxr-xr-x   0 eugene     (501) staff       (20)     1477 2022-02-17 09:04:54.000000 ajenti-panel-2.2.5/ajenti-upgrade
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:16.653525 ajenti-panel-2.2.5/ajenti_panel.egg-info/
+-rw-r--r--   0 eugene     (501) staff       (20)      190 2023-05-08 04:10:16.000000 ajenti-panel-2.2.5/ajenti_panel.egg-info/PKG-INFO
+-rw-r--r--   0 eugene     (501) staff       (20)      913 2023-05-08 04:10:16.000000 ajenti-panel-2.2.5/ajenti_panel.egg-info/SOURCES.txt
+-rw-r--r--   0 eugene     (501) staff       (20)        1 2023-05-08 04:10:16.000000 ajenti-panel-2.2.5/ajenti_panel.egg-info/dependency_links.txt
+-rw-r--r--   0 eugene     (501) staff       (20)       26 2023-05-08 04:10:16.000000 ajenti-panel-2.2.5/ajenti_panel.egg-info/requires.txt
+-rw-r--r--   0 eugene     (501) staff       (20)        3 2023-05-08 04:10:16.000000 ajenti-panel-2.2.5/ajenti_panel.egg-info/top_level.txt
+-rw-r--r--   0 eugene     (501) staff       (20)       67 2023-05-08 04:10:16.653968 ajenti-panel-2.2.5/setup.cfg
+-rwxr-xr-x   0 eugene     (501) staff       (20)     1924 2023-05-08 04:08:59.000000 ajenti-panel-2.2.5/setup.py
```

### Comparing `ajenti-panel-2.2.4/aj/__init__.py` & `ajenti-panel-2.2.5/aj/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 import platform as pyplatform
 import signal
 import subprocess
 
-__version__ = '2.2.4'
+__version__ = '2.2.5'
 
 # Global state
 
 product = None
 """ Custom product name """
 
 config = None
```

### Comparing `ajenti-panel-2.2.4/aj/api/endpoint.py` & `ajenti-panel-2.2.5/aj/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/api/http.py` & `ajenti-panel-2.2.5/aj/api/http.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/api/mail.py` & `ajenti-panel-2.2.5/aj/api/mail.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/auth.py` & `ajenti-panel-2.2.5/aj/auth.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/compat.py` & `ajenti-panel-2.2.5/aj/compat.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/config.py` & `ajenti-panel-2.2.5/aj/config.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/core.py` & `ajenti-panel-2.2.5/aj/core.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/entry.py` & `ajenti-panel-2.2.5/aj/entry.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/gate/gate.py` & `ajenti-panel-2.2.5/aj/gate/gate.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/gate/middleware.py` & `ajenti-panel-2.2.5/aj/gate/middleware.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/gate/session.py` & `ajenti-panel-2.2.5/aj/gate/session.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/gate/stream.py` & `ajenti-panel-2.2.5/aj/gate/stream.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/gate/worker.py` & `ajenti-panel-2.2.5/aj/gate/worker.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/http.py` & `ajenti-panel-2.2.5/aj/http.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/https_redirect.py` & `ajenti-panel-2.2.5/aj/https_redirect.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/log.py` & `ajenti-panel-2.2.5/aj/log.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/plugins.py` & `ajenti-panel-2.2.5/aj/plugins.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/routing.py` & `ajenti-panel-2.2.5/aj/routing.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/security/pwreset.py` & `ajenti-panel-2.2.5/aj/security/pwreset.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/security/totp.py` & `ajenti-panel-2.2.5/aj/security/totp.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/security/verifier.py` & `ajenti-panel-2.2.5/aj/security/verifier.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/static/emails/reset_email.html` & `ajenti-panel-2.2.5/aj/static/emails/reset_email.html`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/static/images/Logo.png` & `ajenti-panel-2.2.5/aj/static/images/Logo.png`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/static/images/error.jpeg` & `ajenti-panel-2.2.5/aj/static/images/error.jpeg`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/util/lazy.py` & `ajenti-panel-2.2.5/aj/util/lazy.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/util/misc.py` & `ajenti-panel-2.2.5/aj/util/misc.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/util/pidfile.py` & `ajenti-panel-2.2.5/aj/util/pidfile.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/util/public.py` & `ajenti-panel-2.2.5/aj/util/public.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/aj/wsgi.py` & `ajenti-panel-2.2.5/aj/wsgi.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/ajenti-client-ssl-gen` & `ajenti-panel-2.2.5/ajenti-client-ssl-gen`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/ajenti-panel` & `ajenti-panel-2.2.5/ajenti-panel`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/ajenti-ssl-gen` & `ajenti-panel-2.2.5/ajenti-ssl-gen`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/ajenti-upgrade` & `ajenti-panel-2.2.5/ajenti-upgrade`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/ajenti_panel.egg-info/SOURCES.txt` & `ajenti-panel-2.2.5/ajenti_panel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.4/setup.py` & `ajenti-panel-2.2.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,18 +54,18 @@
     def run(self):
         _install.run(self)
         self.execute(_post_install, [self.install_scripts], msg='Running post install script')
 
 
 setup(
     name='ajenti-panel',
-    version='2.2.4',
+    version='2.2.5',
     python_requires='>=3',
     install_requires=[
-        'aj==2.2.4',
+        'aj==2.2.5',
         'pyyaml',
         'requests',
     ],
     description='Ajenti core based panel',
     author='Eugene Pankov',
     author_email='e@ajenti.org',
     url='https://ajenti.org/',
```

