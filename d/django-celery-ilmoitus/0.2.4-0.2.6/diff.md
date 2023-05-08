# Comparing `tmp/django-celery-ilmoitus-0.2.4.tar.gz` & `tmp/django-celery-ilmoitus-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/aha/git/django-celery-ilmoitus/dist/tmpyk5zy7m7/django-celery-ilmoitus-0.2.4.tar", last modified: Wed May 18 10:33:41 2022, max compression
+gzip compressed data, was "django-celery-ilmoitus-0.2.6.tar", last modified: Mon May  8 14:01:40 2023, max compression
```

## Comparing `django-celery-ilmoitus-0.2.4.tar` & `django-celery-ilmoitus-0.2.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-05-18 10:33:41.446276 django-celery-ilmoitus-0.2.4/
--rw-r--r--   0 aha        (501) staff       (20)       39 2021-02-12 12:19:21.000000 django-celery-ilmoitus-0.2.4/MANIFEST.in
--rw-r--r--   0 aha        (501) staff       (20)      278 2022-05-18 10:33:41.445910 django-celery-ilmoitus-0.2.4/PKG-INFO
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-05-18 10:33:41.441759 django-celery-ilmoitus-0.2.4/django_celery_ilmoitus.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)      278 2022-05-18 10:33:40.000000 django-celery-ilmoitus-0.2.4/django_celery_ilmoitus.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      543 2022-05-18 10:33:41.000000 django-celery-ilmoitus-0.2.4/django_celery_ilmoitus.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2022-05-18 10:33:40.000000 django-celery-ilmoitus-0.2.4/django_celery_ilmoitus.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)      103 2022-05-18 10:33:41.000000 django-celery-ilmoitus-0.2.4/django_celery_ilmoitus.egg-info/entry_points.txt
--rw-r--r--   0 aha        (501) staff       (20)     2254 2022-05-18 10:33:40.000000 django-celery-ilmoitus-0.2.4/django_celery_ilmoitus.egg-info/historia.json
--rw-r--r--   0 aha        (501) staff       (20)        1 2021-02-23 10:09:09.000000 django-celery-ilmoitus-0.2.4/django_celery_ilmoitus.egg-info/not-zip-safe
--rw-r--r--   0 aha        (501) staff       (20)       42 2022-05-18 10:33:41.000000 django-celery-ilmoitus-0.2.4/django_celery_ilmoitus.egg-info/requires.txt
--rw-r--r--   0 aha        (501) staff       (20)        9 2022-05-18 10:33:41.000000 django-celery-ilmoitus-0.2.4/django_celery_ilmoitus.egg-info/top_level.txt
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-05-18 10:33:41.444530 django-celery-ilmoitus-0.2.4/ilmoitus/
--rw-r--r--   0 aha        (501) staff       (20)        0 2021-02-12 12:05:10.000000 django-celery-ilmoitus-0.2.4/ilmoitus/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)      173 2021-02-12 12:13:02.000000 django-celery-ilmoitus-0.2.4/ilmoitus/celery.py
--rw-r--r--   0 aha        (501) staff       (20)     3199 2021-09-10 06:22:55.000000 django-celery-ilmoitus-0.2.4/ilmoitus/nakyma.py
--rw-r--r--   0 aha        (501) staff       (20)      565 2021-02-12 12:10:06.000000 django-celery-ilmoitus-0.2.4/ilmoitus/sovellus.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-05-18 10:33:41.438730 django-celery-ilmoitus-0.2.4/ilmoitus/templates/
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-05-18 10:33:41.445424 django-celery-ilmoitus-0.2.4/ilmoitus/templates/ilmoitus/
--rw-r--r--   0 aha        (501) staff       (20)     2409 2021-09-10 06:21:03.000000 django-celery-ilmoitus-0.2.4/ilmoitus/templates/ilmoitus/ilmoitus.html
--rw-r--r--   0 aha        (501) staff       (20)     1558 2021-02-12 12:41:21.000000 django-celery-ilmoitus-0.2.4/ilmoitus/uusi.py
--rw-r--r--   0 aha        (501) staff       (20)       72 2021-03-18 13:07:55.000000 django-celery-ilmoitus-0.2.4/pyproject.toml
--rw-r--r--   0 aha        (501) staff       (20)       38 2022-05-18 10:33:41.446378 django-celery-ilmoitus-0.2.4/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)      664 2021-02-12 12:16:25.000000 django-celery-ilmoitus-0.2.4/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-08 14:01:40.117506 django-celery-ilmoitus-0.2.6/
+-rw-r--r--   0 aha        (501) staff       (20)       39 2021-02-12 12:19:21.000000 django-celery-ilmoitus-0.2.6/MANIFEST.in
+-rw-r--r--   0 aha        (501) staff       (20)      278 2023-05-08 14:01:40.117359 django-celery-ilmoitus-0.2.6/PKG-INFO
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-08 14:01:40.115066 django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)      278 2023-05-08 14:01:40.000000 django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      543 2023-05-08 14:01:40.000000 django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2023-05-08 14:01:40.000000 django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)      103 2023-05-08 14:01:40.000000 django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/entry_points.txt
+-rw-r--r--   0 aha        (501) staff       (20)     1913 2023-05-08 14:01:40.000000 django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/historia.json
+-rw-r--r--   0 aha        (501) staff       (20)        1 2021-02-23 10:09:09.000000 django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/not-zip-safe
+-rw-r--r--   0 aha        (501) staff       (20)       42 2023-05-08 14:01:40.000000 django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/requires.txt
+-rw-r--r--   0 aha        (501) staff       (20)        9 2023-05-08 14:01:40.000000 django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/top_level.txt
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-08 14:01:40.116907 django-celery-ilmoitus-0.2.6/ilmoitus/
+-rw-r--r--   0 aha        (501) staff       (20)        0 2021-02-12 12:05:10.000000 django-celery-ilmoitus-0.2.6/ilmoitus/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)      173 2021-02-12 12:13:02.000000 django-celery-ilmoitus-0.2.6/ilmoitus/celery.py
+-rw-r--r--   0 aha        (501) staff       (20)     3724 2023-05-02 09:42:25.000000 django-celery-ilmoitus-0.2.6/ilmoitus/nakyma.py
+-rw-r--r--   0 aha        (501) staff       (20)      565 2021-02-12 12:10:06.000000 django-celery-ilmoitus-0.2.6/ilmoitus/sovellus.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-08 14:01:40.113583 django-celery-ilmoitus-0.2.6/ilmoitus/templates/
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-08 14:01:40.117063 django-celery-ilmoitus-0.2.6/ilmoitus/templates/ilmoitus/
+-rw-r--r--   0 aha        (501) staff       (20)     2409 2023-01-25 12:51:55.000000 django-celery-ilmoitus-0.2.6/ilmoitus/templates/ilmoitus/ilmoitus.html
+-rw-r--r--   0 aha        (501) staff       (20)     1558 2021-02-12 12:41:21.000000 django-celery-ilmoitus-0.2.6/ilmoitus/uusi.py
+-rw-r--r--   0 aha        (501) staff       (20)       79 2023-05-08 14:01:33.000000 django-celery-ilmoitus-0.2.6/pyproject.toml
+-rw-r--r--   0 aha        (501) staff       (20)       38 2023-05-08 14:01:40.117541 django-celery-ilmoitus-0.2.6/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)      664 2021-02-12 12:16:25.000000 django-celery-ilmoitus-0.2.6/setup.py
```

### Comparing `django-celery-ilmoitus-0.2.4/django_celery_ilmoitus.egg-info/SOURCES.txt` & `django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-celery-ilmoitus-0.2.4/ilmoitus/nakyma.py` & `django-celery-ilmoitus-0.2.6/ilmoitus/nakyma.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,20 +7,30 @@
 from asgiref.sync import async_to_sync, sync_to_async
 
 from django.contrib.auth.mixins import LoginRequiredMixin
 from django.contrib.messages import get_messages
 from django.contrib.messages.storage import default_storage
 from django.http import JsonResponse
 from django.urls import path
-from django.views import generic
+from django.utils.decorators import method_decorator
+
+# Mikäli pistoke-paketti ei ole käytössä, käytetään Djangon vakio-
+# näkymäluokkaa. Tällöin metodi `async def websocket` ei ole ongelma,
+# sillä sitä ei tunnisteta HTTP-verbin toteutukseksi.
+try:
+  from pistoke.nakyma import WebsocketNakyma
+  from pistoke import WebsocketProtokolla
+except ImportError:
+  # pylint: disable=ungrouped-imports
+  from django.views.generic import View as WebsocketNakyma
 
 from .celery import celery_app, celery_viestikanava
 
 
-class Ilmoitukset(LoginRequiredMixin, generic.View):
+class Ilmoitukset(LoginRequiredMixin, WebsocketNakyma):
 
   bootstrap_luokat = {
     'debug': 'alert-info',
     'info': 'alert-info',
     'success': 'alert-success',
     'warning': 'alert-warning',
     'error': 'alert-danger',
@@ -44,17 +54,20 @@
     storage = get_messages(request)
     return JsonResponse([
       self._ilmoitus(ilmoitus)
       for ilmoitus in storage
     ], safe=False)
     # def get
 
+  @method_decorator(WebsocketProtokolla)
   async def websocket(self, request):
     '''
     Websocket-toteutus. Palauta ilmoituksia sitä mukaa, kun niitä tallennetaan.
+
+    Vaatii django-pistoke-paketin asennuksen.
     '''
     async def laheta_ilmoitukset(signaali=None):
       ''' Lähetä kaikki olemassaolevat ilmoitukset selaimelle. '''
       # pylint: disable=unused-argument
       def hae_ilmoitukset():
         # pylint: disable=protected-access
         request.session._session_cache = request.session.load()
```

### Comparing `django-celery-ilmoitus-0.2.4/ilmoitus/sovellus.py` & `django-celery-ilmoitus-0.2.6/ilmoitus/sovellus.py`

 * *Files identical despite different names*

### Comparing `django-celery-ilmoitus-0.2.4/ilmoitus/templates/ilmoitus/ilmoitus.html` & `django-celery-ilmoitus-0.2.6/ilmoitus/templates/ilmoitus/ilmoitus.html`

 * *Files identical despite different names*

### Comparing `django-celery-ilmoitus-0.2.4/ilmoitus/uusi.py` & `django-celery-ilmoitus-0.2.6/ilmoitus/uusi.py`

 * *Files identical despite different names*

### Comparing `django-celery-ilmoitus-0.2.4/setup.py` & `django-celery-ilmoitus-0.2.6/setup.py`

 * *Files identical despite different names*

