# Comparing `tmp/django-pistoke-0.8rc10.tar.gz` & `tmp/django-pistoke-0.8rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pistoke-0.8rc10.tar", last modified: Fri Mar  3 09:24:57 2023, max compression
+gzip compressed data, was "django-pistoke-0.8rc2.tar", last modified: Mon Jan  2 08:59:06 2023, max compression
```

## Comparing `django-pistoke-0.8rc10.tar` & `django-pistoke-0.8rc2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-03-03 09:24:57.149552 django-pistoke-0.8rc10/
--rw-r--r--   0 aha        (501) staff       (20)       73 2020-04-20 13:45:50.000000 django-pistoke-0.8rc10/MANIFEST.in
--rw-r--r--   0 aha        (501) staff       (20)      304 2023-03-03 09:24:57.149370 django-pistoke-0.8rc10/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)    10647 2022-11-18 12:58:33.000000 django-pistoke-0.8rc10/README.md
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-03-03 09:24:57.145960 django-pistoke-0.8rc10/django_pistoke.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)      304 2023-03-03 09:24:53.000000 django-pistoke-0.8rc10/django_pistoke.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      662 2023-03-03 09:24:57.000000 django-pistoke-0.8rc10/django_pistoke.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2023-03-03 09:24:53.000000 django-pistoke-0.8rc10/django_pistoke.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)       47 2023-03-03 09:24:53.000000 django-pistoke-0.8rc10/django_pistoke.egg-info/entry_points.txt
--rw-r--r--   0 aha        (501) staff       (20)    10304 2023-03-03 09:24:57.000000 django-pistoke-0.8rc10/django_pistoke.egg-info/historia.json
--rw-r--r--   0 aha        (501) staff       (20)        1 2020-04-16 06:40:21.000000 django-pistoke-0.8rc10/django_pistoke.egg-info/not-zip-safe
--rw-r--r--   0 aha        (501) staff       (20)       86 2023-03-03 09:24:53.000000 django-pistoke-0.8rc10/django_pistoke.egg-info/requires.txt
--rw-r--r--   0 aha        (501) staff       (20)        8 2023-03-03 09:24:53.000000 django-pistoke-0.8rc10/django_pistoke.egg-info/top_level.txt
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-03-03 09:24:57.148467 django-pistoke-0.8rc10/pistoke/
--rw-r--r--   0 aha        (501) staff       (20)      227 2022-11-18 12:57:25.000000 django-pistoke-0.8rc10/pistoke/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)      383 2023-03-03 06:56:22.000000 django-pistoke-0.8rc10/pistoke/asetukset.py
--rw-r--r--   0 aha        (501) staff       (20)     5638 2023-03-01 14:03:05.000000 django-pistoke-0.8rc10/pistoke/kasittelija.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-03-03 09:24:57.148739 django-pistoke-0.8rc10/pistoke/management/
--rw-r--r--   0 aha        (501) staff       (20)        0 2020-04-20 13:45:50.000000 django-pistoke-0.8rc10/pistoke/management/__init__.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-03-03 09:24:57.148993 django-pistoke-0.8rc10/pistoke/management/commands/
--rw-r--r--   0 aha        (501) staff       (20)        0 2020-04-20 13:45:50.000000 django-pistoke-0.8rc10/pistoke/management/commands/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)     6906 2023-02-07 12:04:42.000000 django-pistoke-0.8rc10/pistoke/management/commands/runserver.py
--rw-r--r--   0 aha        (501) staff       (20)     1675 2022-11-07 09:32:48.000000 django-pistoke-0.8rc10/pistoke/nakyma.py
--rw-r--r--   0 aha        (501) staff       (20)     6618 2023-03-03 07:00:47.000000 django-pistoke-0.8rc10/pistoke/ohjain.py
--rw-r--r--   0 aha        (501) staff       (20)     1283 2022-11-18 12:57:25.000000 django-pistoke-0.8rc10/pistoke/poistuvat.py
--rw-r--r--   0 aha        (501) staff       (20)     5151 2023-03-01 14:03:32.000000 django-pistoke-0.8rc10/pistoke/protokolla.py
--rw-r--r--   0 aha        (501) staff       (20)     4115 2022-11-18 12:57:25.000000 django-pistoke-0.8rc10/pistoke/pyynto.py
--rw-r--r--   0 aha        (501) staff       (20)    12080 2022-11-18 12:58:33.000000 django-pistoke-0.8rc10/pistoke/testaus.py
--rw-r--r--   0 aha        (501) staff       (20)     2852 2023-02-20 13:30:35.000000 django-pistoke-0.8rc10/pistoke/tyokalut.py
--rw-r--r--   0 aha        (501) staff       (20)       79 2022-11-07 08:02:44.000000 django-pistoke-0.8rc10/pyproject.toml
--rw-r--r--   0 aha        (501) staff       (20)       38 2023-03-03 09:24:57.149597 django-pistoke-0.8rc10/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)      700 2023-03-01 14:03:33.000000 django-pistoke-0.8rc10/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-01-02 08:59:06.176042 django-pistoke-0.8rc2/
+-rw-r--r--   0 aha        (501) staff       (20)       73 2020-04-20 13:45:50.000000 django-pistoke-0.8rc2/MANIFEST.in
+-rw-r--r--   0 aha        (501) staff       (20)      303 2023-01-02 08:59:06.175843 django-pistoke-0.8rc2/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)    10647 2022-11-18 12:58:33.000000 django-pistoke-0.8rc2/README.md
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-01-02 08:59:06.172420 django-pistoke-0.8rc2/django_pistoke.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)      303 2023-01-02 08:59:05.000000 django-pistoke-0.8rc2/django_pistoke.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      662 2023-01-02 08:59:06.000000 django-pistoke-0.8rc2/django_pistoke.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2023-01-02 08:59:05.000000 django-pistoke-0.8rc2/django_pistoke.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)       47 2023-01-02 08:59:06.000000 django-pistoke-0.8rc2/django_pistoke.egg-info/entry_points.txt
+-rw-r--r--   0 aha        (501) staff       (20)     8973 2023-01-02 08:59:05.000000 django-pistoke-0.8rc2/django_pistoke.egg-info/historia.json
+-rw-r--r--   0 aha        (501) staff       (20)        1 2020-04-16 06:40:21.000000 django-pistoke-0.8rc2/django_pistoke.egg-info/not-zip-safe
+-rw-r--r--   0 aha        (501) staff       (20)       72 2023-01-02 08:59:06.000000 django-pistoke-0.8rc2/django_pistoke.egg-info/requires.txt
+-rw-r--r--   0 aha        (501) staff       (20)        8 2023-01-02 08:59:06.000000 django-pistoke-0.8rc2/django_pistoke.egg-info/top_level.txt
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-01-02 08:59:06.174937 django-pistoke-0.8rc2/pistoke/
+-rw-r--r--   0 aha        (501) staff       (20)      227 2022-11-18 12:57:25.000000 django-pistoke-0.8rc2/pistoke/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)      329 2022-11-18 12:56:52.000000 django-pistoke-0.8rc2/pistoke/asetukset.py
+-rw-r--r--   0 aha        (501) staff       (20)     5831 2022-12-14 07:01:59.000000 django-pistoke-0.8rc2/pistoke/kasittelija.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-01-02 08:59:06.175210 django-pistoke-0.8rc2/pistoke/management/
+-rw-r--r--   0 aha        (501) staff       (20)        0 2020-04-20 13:45:50.000000 django-pistoke-0.8rc2/pistoke/management/__init__.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-01-02 08:59:06.175443 django-pistoke-0.8rc2/pistoke/management/commands/
+-rw-r--r--   0 aha        (501) staff       (20)        0 2020-04-20 13:45:50.000000 django-pistoke-0.8rc2/pistoke/management/commands/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)     6617 2022-11-07 09:33:01.000000 django-pistoke-0.8rc2/pistoke/management/commands/runserver.py
+-rw-r--r--   0 aha        (501) staff       (20)     1675 2022-11-07 09:32:48.000000 django-pistoke-0.8rc2/pistoke/nakyma.py
+-rw-r--r--   0 aha        (501) staff       (20)     5674 2022-11-18 12:56:52.000000 django-pistoke-0.8rc2/pistoke/ohjain.py
+-rw-r--r--   0 aha        (501) staff       (20)     1283 2022-11-18 12:57:25.000000 django-pistoke-0.8rc2/pistoke/poistuvat.py
+-rw-r--r--   0 aha        (501) staff       (20)     5272 2022-11-23 08:00:13.000000 django-pistoke-0.8rc2/pistoke/protokolla.py
+-rw-r--r--   0 aha        (501) staff       (20)     4115 2022-11-18 12:57:25.000000 django-pistoke-0.8rc2/pistoke/pyynto.py
+-rw-r--r--   0 aha        (501) staff       (20)    12080 2022-11-18 12:58:33.000000 django-pistoke-0.8rc2/pistoke/testaus.py
+-rw-r--r--   0 aha        (501) staff       (20)     2929 2022-11-18 12:57:25.000000 django-pistoke-0.8rc2/pistoke/tyokalut.py
+-rw-r--r--   0 aha        (501) staff       (20)       79 2022-11-07 08:02:44.000000 django-pistoke-0.8rc2/pyproject.toml
+-rw-r--r--   0 aha        (501) staff       (20)       38 2023-01-02 08:59:06.176087 django-pistoke-0.8rc2/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)      672 2022-11-18 12:58:33.000000 django-pistoke-0.8rc2/setup.py
```

### Comparing `django-pistoke-0.8rc10/README.md` & `django-pistoke-0.8rc2/README.md`

 * *Files identical despite different names*

### Comparing `django-pistoke-0.8rc10/django_pistoke.egg-info/SOURCES.txt` & `django-pistoke-0.8rc2/django_pistoke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pistoke-0.8rc10/django_pistoke.egg-info/historia.json` & `django-pistoke-0.8rc2/django_pistoke.egg-info/historia.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {'delete': '[7, 6, 5, 4, 3, 2, 1, 0]'}*

```diff
@@ -1,49 +1,9 @@
 [
     {
-        "kuvaus": "Lis\u00e4tty testit ohjaimien (middleware) toiminnan varmentamiseksi",
-        "revisio": "f478d112795fea51f3d1180f273520588f042869",
-        "versio": "0.8rc10"
-    },
-    {
-        "kuvaus": "Pudotettu Django 3.1- ja 4.0-tuki",
-        "revisio": "041b66289ee00033cb42243f18e7c3326caa53b9",
-        "versio": "0.8rc9"
-    },
-    {
-        "kuvaus": "Korjattu `OriginPoikkeus`-koriste",
-        "revisio": "b48d4bffa7c081c1255cacaf53edcff8f27b5e1c",
-        "versio": "0.8rc8"
-    },
-    {
-        "kuvaus": "Palautetaan HTTP 403, mik\u00e4li WS-ohjainketju tuottaa HTTP-vastauksen",
-        "revisio": "77f3aaa3f24aad52295ca52a2eecdbbacc5a28a2",
-        "versio": "0.8rc7"
-    },
-    {
-        "kuvaus": "P\u00e4ivitetty WS-ohjaimet: automaattinen periytys",
-        "revisio": "c59b275bacb75ad12e72c1619c11af78bb53fd7f",
-        "versio": "0.8rc6"
-    },
-    {
-        "kuvaus": "Korjattu `setup_requires`",
-        "revisio": "01f0622432ed68928dd475b63af928538939aa22",
-        "versio": "0.8rc5"
-    },
-    {
-        "kuvaus": "Runserver: estetty selaimen v\u00e4limuisti staattisten tiedostojen osalta",
-        "revisio": "75eb751ff84341d93f9b74ed402c9f98807b2873",
-        "versio": "0.8rc4"
-    },
-    {
-        "kuvaus": "Korjattu v\u00e4likkeelt\u00e4 palautuvan HTTP-virhesanoman l\u00e4hetys Websocket-pyynn\u00f6ll\u00e4",
-        "revisio": "6f969452d993cef350d083f78ffbeacca3d73409",
-        "versio": "0.8rc3"
-    },
-    {
         "kuvaus": "Palautetaan HTTP 403, mik\u00e4li WS-n\u00e4kym\u00e4funktio ei tuota alirutiinia",
         "revisio": "a0851ec9895ede11a1e846b0beb895d3256fceb5",
         "versio": "0.8rc2"
     },
     {
         "kuvaus": "Lis\u00e4tty Websocket-testausty\u00f6kalut ja alustavat yksikk\u00f6testit",
         "revisio": "dc6acc99723da3013e7c5e5cfc76980ddd5bb2af",
```

### Comparing `django-pistoke-0.8rc10/pistoke/kasittelija.py` & `django-pistoke-0.8rc2/pistoke/kasittelija.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import django
 from django.conf import settings
 from django.core.handlers.asgi import ASGIHandler
 from django.core import signals
 from django.test.utils import override_settings
 from django.urls import set_script_prefix, set_urlconf
 
+from pistoke.ohjain import WEBSOCKET_MIDDLEWARE
 from pistoke.pyynto import WebsocketPyynto
 
 
 loki = logging.getLogger('django.' + __name__)
 
 
 class WebsocketVirhe(RuntimeError):
@@ -96,16 +97,22 @@
     # async def __call__
 
   def load_middleware(self, is_async=False):
     '''
     Ajetaan vain muunnostaulun mukaiset Websocket-pyynnölle käyttöön
     otettavat ohjaimet.
     '''
-    from pistoke.ohjain import websocket_ohjaimet
-    with override_settings(MIDDLEWARE=websocket_ohjaimet):
+    with override_settings(MIDDLEWARE=list(filter(None, (
+      ws_ohjain if isinstance(ws_ohjain, str)
+      else ohjain if ws_ohjain else None
+      for ohjain, ws_ohjain in (
+        (ohjain, WEBSOCKET_MIDDLEWARE.get(ohjain, False))
+        for ohjain in settings.MIDDLEWARE
+      )
+    )))):
       super().load_middleware(is_async=is_async)
     # def load_middleware
 
   # Synkroniset pyynnöt nostavat poikkeuksen.
   def get_response(self, request):
     raise WebsocketVirhe
   def _get_response(self, request):
@@ -116,29 +123,23 @@
     set_urlconf(settings.ROOT_URLCONF)
     return await self._middleware_chain(request)
     # async def get_response_async
 
   async def _get_response_async(self, request):
     ''' Ohitetaan paluusanoman käsittelyyn liittyvät funktiokutsut. '''
     # pylint: disable=not-callable, protected-access
-    from pistoke.protokolla import WebsocketProtokolla
-    @WebsocketProtokolla
-    async def evatty(*args, **kwargs): pass
-
     callback, callback_args, callback_kwargs = self.resolve_request(request)
     for middleware_method in self._view_middleware:
       vastaus = await middleware_method(
         request, callback, callback_args, callback_kwargs
       )
       if vastaus is not None:
-        loki.debug(
-          'Ohjainketju palautti HTTP-vastauksen %r.',
-          vastaus,
+        return await self.send_response(
+          request, vastaus
         )
-        return evatty
       # for middleware_method in self._view_middleware
 
     # Mikäli `callback` on asynkroninen funktio (tai kääre),
     # palautetaan sen tuottama alirutiini.
     if asyncio.iscoroutinefunction(callback) \
     or asyncio.iscoroutinefunction(
       getattr(callback, '__call__', callback)
@@ -164,14 +165,17 @@
       # kirjautumissivulle.
       # Evätään tällöin Websocket-pyyntö.
       loki.debug(
         'Websocket-näkymä %r palautti alirutiinin sijaan arvon %r.',
         getattr(callback, 'view_class', callback),
         nakyma,
       )
+      from pistoke.protokolla import WebsocketProtokolla
+      @WebsocketProtokolla
+      async def evatty(*args, **kwargs): pass
       return evatty
     else:
       raise ValueError(
         f'Websocket-näkymä {callback!r} ei ole kelvollinen funktio.'
       )
     # async def _get_response_async
```

### Comparing `django-pistoke-0.8rc10/pistoke/management/commands/runserver.py` & `django-pistoke-0.8rc2/pistoke/management/commands/runserver.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,29 +24,21 @@
   #     kyseisessä sovelluksessa periytetystä `runserver`-komennosta ja
   # (2) käytetään erillistä ASGI-käsittelijää
   #     staattisten tiedostojen tarjoilemiseen.
   from django.contrib.staticfiles.management.commands.runserver import (
     Command as _Command
   )
   from django.contrib.staticfiles.handlers import StaticFilesHandlerMixin
-  from django.utils.cache import add_never_cache_headers
   class static_handler(StaticFilesHandlerMixin, ASGIHandler):
     ''' Vrt. staticfiles.handlers.ASGIStaticFilesHandler '''
     def __init__(self):
       # pylint: disable=super-init-not-called
       # Ei kutsuta `ASGIHandler.__init__`-metodia,
       # joka lataa välikkeet (middleware); niitä ei tarvita.
       self.base_url = urlparse(self.get_base_url())
-      # def __init__
-    def serve(self, request):
-      # Kielletään staattisten tiedostojen paikallinen välimuisti.
-      tulos = super().serve(request)
-      add_never_cache_headers(tulos)
-      return tulos
-      # def serve
     # class static_handler
   # if 'django.contrib.staticfiles' in settings.INSTALLED_APPS
 
 else:
   # Muuten periytetään suoraan django.core-versiosta.
   from django.core.management.commands.runserver import (
     Command as _Command
```

### Comparing `django-pistoke-0.8rc10/pistoke/nakyma.py` & `django-pistoke-0.8rc2/pistoke/nakyma.py`

 * *Files identical despite different names*

### Comparing `django-pistoke-0.8rc10/pistoke/ohjain.py` & `django-pistoke-0.8rc2/pistoke/ohjain.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,19 +32,16 @@
 from django.conf import settings
 from django.contrib.sessions.middleware import SessionMiddleware
 from django.core.handlers.asgi import ASGIRequest
 from django.http.request import split_domain_port, validate_host
 from django.http import HttpResponseForbidden
 from django.middleware.csrf import CsrfViewMiddleware
 from django.utils.decorators import sync_and_async_middleware
-from django.utils.module_loading import import_string
 from django.utils.log import log_response
 
-import mmaare
-
 
 logger = logging.getLogger('django.pistoke.origin')
 
 
 @sync_and_async_middleware
 class WebsocketOhjain:
   '''
@@ -76,35 +73,26 @@
     # def __call__
 
   # class WebsocketOhjain
 
 
 @sync_and_async_middleware
 class OriginVaatimus:
-  '''
-  Ohjain, joka tarkistaa mahdollisen Websocket-pyynnöllä annetun
-  Origin-otsakkeen vastaavasti kuin Django-CSRF-ohjain tarkistaa
-  sen POST-pyynnöllä.
-  '''
+
   def __init__(self, get_response):
     self.get_response = get_response
     if asyncio.iscoroutinefunction(self.get_response):
       self._is_coroutine = asyncio.coroutines._is_coroutine
     # def __init__
 
   def __call__(self, request):
     return self.get_response(request)
     # def __call__
 
   def process_view(self, request, callback, callback_args, callback_kwargs):
-    # pylint: disable=unused-argument
-    assert request.method == 'Websocket'
-    #if request.method != 'Websocket':
-    #  return None
-    #elif getattr(callback, 'origin_poikkeus', False):
     if getattr(callback, 'origin_poikkeus', False):
       return None
     elif 'HTTP_ORIGIN' not in request.META:
       return None
     origin = split_domain_port(
       urlparse(request.META['HTTP_ORIGIN']).netloc.lower()
     )[0]
@@ -144,57 +132,32 @@
 
 class IstuntoOhjain(OhitaPaluusanoma, SessionMiddleware):
   pass
 
 
 # Muunnostaulu Websocket-pyyntöihin sovellettavista
 # Middleware-ohjaimista.
-# Muut kuin tässä mainitut ohjaimet periytetään automaattisesti
-# `OhitaPaluusanoma`-saateluokasta.
+# Muiden kuin tässä mainittujen ohjaimien lataus ohitetaan.
 WEBSOCKET_MIDDLEWARE = {
-  # Ohitetaan kokonaan.
+  # Ohitetaan.
   'corsheaders.middleware.CorsMiddleware': False,
   'debug_toolbar.middleware.DebugToolbarMiddleware': False,
   'django.middleware.gzip.GZipMiddleware': False,
+  'django.middleware.security.SecurityMiddleware' : False,
+  'django.middleware.common.CommonMiddleware': False,
   'django.middleware.clickjacking.XFrameOptionsMiddleware': False,
   'django_hosts.middleware.HostsResponseMiddleware': False,
 
-  # Korvataan muunnoksella.
+  # Suoritetaan.
+  'django_hosts.middleware.HostsRequestMiddleware': True,
   'django.middleware.csrf.CsrfViewMiddleware': 'pistoke.ohjain.CsrfOhjain',
   'django.contrib.sessions.middleware.SessionMiddleware': \
     'pistoke.ohjain.IstuntoOhjain',
+  'django.contrib.auth.middleware.AuthenticationMiddleware': True,
+  'django.contrib.messages.middleware.MessageMiddleware': True,
+  'impersonate.middleware.ImpersonateMiddleware': True,
+  'silk.middleware.SilkyMiddleware': True,
 
-  # Suoritetaan sellaisenaan.
+  # Lisätty.
   'pistoke.ohjain.WebsocketOhjain': True,
+  'pistoke.ohjain.OriginVaatimus': True,
 }
-
-
-def sovita_ohjain_websocket_pyynnolle(ohjain):
-  if isinstance(ohjain, str):
-    ohjain = import_string(ohjain)
-  assert isinstance(ohjain, type)
-  return type(
-    ohjain.__name__,
-    (OhitaPaluusanoma, ohjain),
-    {}
-  )
-  # def sovita_ohjain_websocket_pyynnolle
-
-@mmaare
-def __websocket_ohjaimet(moduuli):
-  def _websocket_ohjaimet():
-    for ohjain in settings.MIDDLEWARE:
-      muunnos = WEBSOCKET_MIDDLEWARE.get(ohjain, None)
-      if muunnos is False:
-        continue
-      elif muunnos is True:
-        yield ohjain
-        continue
-      elif muunnos is not None:
-        yield muunnos
-        continue
-      ohjain = sovita_ohjain_websocket_pyynnolle(ohjain)
-      setattr(moduuli, ohjain.__name__, ohjain)
-      yield '.'.join((__name__, ohjain.__name__))
-    yield 'pistoke.ohjain.OriginVaatimus'
-  return list(_websocket_ohjaimet())
-  # def __websocket_ohjaimet
```

### Comparing `django-pistoke-0.8rc10/pistoke/poistuvat.py` & `django-pistoke-0.8rc2/pistoke/poistuvat.py`

 * *Files identical despite different names*

### Comparing `django-pistoke-0.8rc10/pistoke/protokolla.py` & `django-pistoke-0.8rc2/pistoke/protokolla.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,18 @@
     }, 'Avaava kättely epäonnistui: %r' % (
       avaava_kattely
     )
     await request.send({'type': 'websocket.accept'})
     # async def _avaa_yhteys
 
   async def _sulje_yhteys(self, request):
-    await request.send({'type': 'websocket.close'})
+    if getattr(request, '__suljettu__', False):
+      raise RuntimeError
+    request.__suljettu__ = True
+    await asyncio.shield(request.send({'type': 'websocket.close'}))
     # async def _sulje_yhteys
 
   async def _vastaanota_sanoma(self, receive):
     sanoma = await receive()
     if sanoma['type'] == 'websocket.receive':
       return sanoma.get('text', sanoma.get('bytes', None))
     elif sanoma['type'] == 'websocket.disconnect':
```

### Comparing `django-pistoke-0.8rc10/pistoke/pyynto.py` & `django-pistoke-0.8rc2/pistoke/pyynto.py`

 * *Files identical despite different names*

### Comparing `django-pistoke-0.8rc10/pistoke/testaus.py` & `django-pistoke-0.8rc2/pistoke/testaus.py`

 * *Files identical despite different names*

### Comparing `django-pistoke-0.8rc10/pistoke/tyokalut.py` & `django-pistoke-0.8rc2/pistoke/tyokalut.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,17 @@
     # def __call__
 
   # class Koriste
 
 
 class OriginPoikkeus(Koriste):
   ''' Ohita Origin-otsakkeen tarkistus Websocket-pyynnön yhteydessä. '''
-  origin_poikkeus = True
+  def __init__(self, websocket):
+    super().__init__(websocket)
+    websocket.origin_poikkeus = True
   # def origin_poikkeus
 
 
 class JsonLiikenne(Koriste):
 
   def __init__(
     self,
```

### Comparing `django-pistoke-0.8rc10/setup.py` & `django-pistoke-0.8rc2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
-  setup_requires='git-versiointi>=1.6b9',
+  setup_requires='git-versiointi',
   name='django-pistoke',
   description='Django-Websocket-laajennos',
   url='https://github.com/an7oine/django-pistoke.git',
   author='Antti Hautaniemi',
   author_email='antti.hautaniemi@me.com',
   licence='MIT',
   packages=find_packages(exclude=['testit']),
   include_package_data=True,
   python_requires='>=3.6',
   install_requires=[
-    'django>=3.2',
-    'python-mmaare',
+    'django>=3.1',
   ],
   extras_require={
     'runserver': ['uvicorn[standard]'],
     'websocket': ['websockets>=8.0'],
   },
   entry_points={'django.asetukset': [
     'pistoke = pistoke.asetukset',
```

