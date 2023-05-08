# Comparing `tmp/htag-0.9.8.tar.gz` & `tmp/htag-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htag-0.9.8.tar", max compression
+gzip compressed data, was "htag-0.9.9.tar", max compression
```

## Comparing `htag-0.9.8.tar` & `htag-0.9.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1065 2022-10-30 17:12:38.795551 htag-0.9.8/LICENSE
--rw-r--r--   0        0        0     3794 2022-10-30 17:12:38.795551 htag-0.9.8/README.md
--rw-r--r--   0        0        0      402 2022-10-30 17:12:39.155562 htag-0.9.8/htag/__init__.py
--rw-r--r--   0        0        0     1559 2022-10-30 17:12:38.803551 htag-0.9.8/htag/__main__.py
--rw-r--r--   0        0        0     3358 2022-10-30 17:12:38.803551 htag-0.9.8/htag/attrs.py
--rw-r--r--   0        0        0    15093 2022-10-30 17:12:38.803551 htag-0.9.8/htag/render.py
--rw-r--r--   0        0        0     2085 2022-10-30 17:12:38.803551 htag-0.9.8/htag/runners/__init__.py
--rw-r--r--   0        0        0     5305 2022-10-30 17:12:38.803551 htag-0.9.8/htag/runners/androidapp.py
--rw-r--r--   0        0        0     4057 2022-10-30 17:12:38.803551 htag-0.9.8/htag/runners/browserhttp.py
--rw-r--r--   0        0        0     2156 2022-10-30 17:12:38.803551 htag-0.9.8/htag/runners/browserstarlettehttp.py
--rw-r--r--   0        0        0     2298 2022-10-30 17:12:38.803551 htag-0.9.8/htag/runners/browserstarlettews.py
--rw-r--r--   0        0        0     2251 2022-10-30 17:12:38.803551 htag-0.9.8/htag/runners/browsertornadohttp.py
--rw-r--r--   0        0        0     7930 2022-10-30 17:12:38.803551 htag-0.9.8/htag/runners/chromeapp.py
--rw-r--r--   0        0        0      747 2022-10-30 17:12:38.803551 htag-0.9.8/htag/runners/common.py
--rw-r--r--   0        0        0     6318 2022-10-30 17:12:38.803551 htag-0.9.8/htag/runners/devapp.py
--rw-r--r--   0        0        0     1764 2022-10-30 17:12:38.803551 htag-0.9.8/htag/runners/pyscript.py
--rw-r--r--   0        0        0     1639 2022-10-30 17:12:38.803551 htag-0.9.8/htag/runners/pywebview.py
--rw-r--r--   0        0        0     5509 2022-10-30 17:12:38.803551 htag-0.9.8/htag/runners/webhttp.py
--rw-r--r--   0        0        0     3035 2022-10-30 17:12:38.803551 htag-0.9.8/htag/runners/winapp.py
--rw-r--r--   0        0        0    18358 2022-10-30 17:12:38.803551 htag-0.9.8/htag/tag.py
--rw-r--r--   0        0        0     1195 2022-10-30 17:12:39.155562 htag-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     4533 1970-01-01 00:00:00.000000 htag-0.9.8/setup.py
--rw-r--r--   0        0        0     5008 1970-01-01 00:00:00.000000 htag-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-11-01 09:35:25.618879 htag-0.9.9/LICENSE
+-rw-r--r--   0        0        0     3794 2022-11-01 09:35:25.618879 htag-0.9.9/README.md
+-rw-r--r--   0        0        0      402 2022-11-01 09:35:25.906884 htag-0.9.9/htag/__init__.py
+-rw-r--r--   0        0        0     1559 2022-11-01 09:35:25.618879 htag-0.9.9/htag/__main__.py
+-rw-r--r--   0        0        0     3358 2022-11-01 09:35:25.618879 htag-0.9.9/htag/attrs.py
+-rw-r--r--   0        0        0    15093 2022-11-01 09:35:25.622879 htag-0.9.9/htag/render.py
+-rw-r--r--   0        0        0     2085 2022-11-01 09:35:25.622879 htag-0.9.9/htag/runners/__init__.py
+-rw-r--r--   0        0        0     5305 2022-11-01 09:35:25.622879 htag-0.9.9/htag/runners/androidapp.py
+-rw-r--r--   0        0        0     4057 2022-11-01 09:35:25.622879 htag-0.9.9/htag/runners/browserhttp.py
+-rw-r--r--   0        0        0     2156 2022-11-01 09:35:25.622879 htag-0.9.9/htag/runners/browserstarlettehttp.py
+-rw-r--r--   0        0        0     2298 2022-11-01 09:35:25.622879 htag-0.9.9/htag/runners/browserstarlettews.py
+-rw-r--r--   0        0        0     2251 2022-11-01 09:35:25.622879 htag-0.9.9/htag/runners/browsertornadohttp.py
+-rw-r--r--   0        0        0     7930 2022-11-01 09:35:25.622879 htag-0.9.9/htag/runners/chromeapp.py
+-rw-r--r--   0        0        0     3070 2022-11-01 09:35:25.622879 htag-0.9.9/htag/runners/common.py
+-rw-r--r--   0        0        0     6318 2022-11-01 09:35:25.622879 htag-0.9.9/htag/runners/devapp.py
+-rw-r--r--   0        0        0     1764 2022-11-01 09:35:25.622879 htag-0.9.9/htag/runners/pyscript.py
+-rw-r--r--   0        0        0     1639 2022-11-01 09:35:25.622879 htag-0.9.9/htag/runners/pywebview.py
+-rw-r--r--   0        0        0     5140 2022-11-01 09:35:25.622879 htag-0.9.9/htag/runners/webhttp.py
+-rw-r--r--   0        0        0     3035 2022-11-01 09:35:25.622879 htag-0.9.9/htag/runners/winapp.py
+-rw-r--r--   0        0        0    18358 2022-11-01 09:35:25.622879 htag-0.9.9/htag/tag.py
+-rw-r--r--   0        0        0     1195 2022-11-01 09:35:25.906884 htag-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     4533 1970-01-01 00:00:00.000000 htag-0.9.9/setup.py
+-rw-r--r--   0        0        0     5008 1970-01-01 00:00:00.000000 htag-0.9.9/PKG-INFO
```

### Comparing `htag-0.9.8/LICENSE` & `htag-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `htag-0.9.8/README.md` & `htag-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `htag-0.9.8/htag/__main__.py` & `htag-0.9.9/htag/__main__.py`

 * *Files identical despite different names*

### Comparing `htag-0.9.8/htag/attrs.py` & `htag-0.9.9/htag/attrs.py`

 * *Files identical despite different names*

### Comparing `htag-0.9.8/htag/render.py` & `htag-0.9.9/htag/render.py`

 * *Files identical despite different names*

### Comparing `htag-0.9.8/htag/runners/__init__.py` & `htag-0.9.9/htag/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `htag-0.9.8/htag/runners/androidapp.py` & `htag-0.9.9/htag/runners/androidapp.py`

 * *Files identical despite different names*

### Comparing `htag-0.9.8/htag/runners/browserhttp.py` & `htag-0.9.9/htag/runners/browserhttp.py`

 * *Files identical despite different names*

### Comparing `htag-0.9.8/htag/runners/browserstarlettehttp.py` & `htag-0.9.9/htag/runners/browserstarlettehttp.py`

 * *Files identical despite different names*

### Comparing `htag-0.9.8/htag/runners/browserstarlettews.py` & `htag-0.9.9/htag/runners/browserstarlettews.py`

 * *Files identical despite different names*

### Comparing `htag-0.9.8/htag/runners/browsertornadohttp.py` & `htag-0.9.9/htag/runners/browsertornadohttp.py`

 * *Files identical despite different names*

### Comparing `htag-0.9.8/htag/runners/chromeapp.py` & `htag-0.9.9/htag/runners/chromeapp.py`

 * *Files identical despite different names*

### Comparing `htag-0.9.8/htag/runners/devapp.py` & `htag-0.9.9/htag/runners/devapp.py`

 * *Files identical despite different names*

### Comparing `htag-0.9.8/htag/runners/pyscript.py` & `htag-0.9.9/htag/runners/pyscript.py`

 * *Files identical despite different names*

### Comparing `htag-0.9.8/htag/runners/pywebview.py` & `htag-0.9.9/htag/runners/pywebview.py`

 * *Files identical despite different names*

### Comparing `htag-0.9.8/htag/runners/webhttp.py` & `htag-0.9.9/htag/runners/webhttp.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,34 +39,29 @@
     """ Simple ASync Web Server (with starlette) with HTTP interactions with htag.
         can handle multiple instances & multiples Tag
 
         The instance is an ASGI htag app
     """
     def __init__(self,tagClass:type=None, timeout=5*60):
         if tagClass: assert issubclass(tagClass,Tag)
-        self.sessions={} # nb htag instances (htag x user)
+        self.sessions=common.Sessions()
         self.tagClass=tagClass
         self.timeout=timeout
 
         routes=[ Route('/{sesid}',   self.POST,  methods=["POST"]) ]
         if tagClass:
             routes.append( Route("/",   self.GET,   methods=["GET"]) )
 
         Starlette.__init__(self,debug=True, routes=routes, on_startup=[self._purgeSessions])
 
     async def _purgeSessions(self):
 
         async def purge():
             while True:
-                now=time.time()
-                for ses_id,ses_info in list(self.sessions.items()):
-                    if now - ses_info["lastaccess"] > self.timeout:
-                        logger.info("PURGE SESSION: %s (sessions:%s)", ses_id, len(self.sessions))
-                        del self.sessions[ses_id]
-
+                self.sessions.purge( self.timeout )
                 await asyncio.sleep(60) # check every 60s
 
         asyncio.ensure_future( purge() )
 
     async def GET(self,request) -> HTMLResponse:
         return self.serve(request, self.tagClass )
 
@@ -85,66 +80,63 @@
             init = common.url2ak( str(request.url) )
         else:
             assert type(init)==tuple
             assert type(init[0])==tuple
             assert type(init[1])==dict
 
         hr = self.instanciate(htuid, klass, init , renew)
-
+        
         r = HTMLResponse( str(hr) )
         r.set_cookie("htuid",htuid,path="/")
         return r
 
     def instanciate(self, htuid, klass, init, renew) -> HRenderer:
         """ get|create an instance of `klass` for user session `htuid`
         (get|save it into self.sessions)
         """
         sesid = f"{QN(klass)}|{htuid}"   # there can be only one instance of klass, at a time !
 
         logger.info("intanciate : renew=%s",renew)
-        if renew==False and (sesid in self.sessions) and self.sessions[sesid]["renderer"].init == init:
+        hr=self.sessions.get_hr( sesid )
+        if renew==False and hr and hr.init == init:
             # same url (same klass/params), same htuid -> same instance
             logger.info("intanciate : Reuse Renderer %s for %s",QN(klass),sesid)
-            hr=self.sessions[sesid]["renderer"]
         else:
             # url has changed ... recreate an instance
             logger.info("intanciate : Create Renderer %s for %s",QN(klass),sesid)
             js = """
                 async function interact( o ) {
                     action( await (await window.fetch("/%s",{method:"POST", body:JSON.stringify(o)})).text() )
                 }
 
                 window.addEventListener('DOMContentLoaded', start );
             """ % sesid
+            
+            # create a session property on the future main tag instance
+            klass.session = self.sessions.get_ses(htuid)["session"]
+            
             hr=HRenderer(klass, js, init=init ) # NO EXIT !!
 
+
         # update session info
-        self.sessions[ sesid ] = dict(
-            lastaccess=time.time(),
-            renderer=hr,
-        )
+        self.sessions.set_hr( sesid, hr)
 
         return hr
 
 
     async def POST(self,request) -> Response:
         sesid=request.path_params.get('sesid',None)
 
-        if sesid in self.sessions:
-            hr = self.sessions[ sesid ]["renderer"]
-
-            self.sessions[ sesid ]["lastaccess"]=time.time()
-
-            logger.info("INTERACT WITH SESSION %s (sessions:%s)",sesid,len(self.sessions))
+        hr=self.sessions.get_hr(sesid)
+        if hr:
+            logger.info("INTERACT WITH SESSION %s",sesid)
             data=await request.json()
             actions = await hr.interact(data["id"],data["method"],data["args"],data["kargs"],data["event"])
             return JSONResponse(actions)
-
         else:
             # session expired or bad call
             return HTMLResponse( "400 BAD REQUEST" , status_code=400 )
 
 
-
     def run(self, host="0.0.0.0", port=8000):   # wide, by default !!
         import uvicorn
         uvicorn.run(self, host=host, port=port)
```

### Comparing `htag-0.9.8/htag/runners/winapp.py` & `htag-0.9.9/htag/runners/winapp.py`

 * *Files identical despite different names*

### Comparing `htag-0.9.8/htag/tag.py` & `htag-0.9.9/htag/tag.py`

 * *Files identical despite different names*

### Comparing `htag-0.9.8/pyproject.toml` & `htag-0.9.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htag"
-version = "0.9.8" # auto-updated
+version = "0.9.9" # auto-updated
 description = "GUI toolkit for building GUI toolkits (and create beautiful applications for mobile, web, and desktop from a single python3 codebase)"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['gui', 'electron', "cef", "pywebview", "starlette", "uvicorn", "tornado", "asyncio", "desktop", "web", "mobile", "http", "websocket", "html", "pyscript", "android", "kivy", "apk"]
 homepage = "https://github.com/manatlan/htag"
 repository = "https://github.com/manatlan/htag"
```

### Comparing `htag-0.9.8/setup.py` & `htag-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['htag', 'htag.runners']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'htag',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': 'GUI toolkit for building GUI toolkits (and create beautiful applications for mobile, web, and desktop from a single python3 codebase)',
     'long_description': '# HTag : "H(tml)Tag"\n\n<img src="https://manatlan.github.io/htag/htag.png" width="100" height="100">\n\n[![Test](https://github.com/manatlan/htag/actions/workflows/on_commit_do_all_unittests.yml/badge.svg)](https://github.com/manatlan/htag/actions/workflows/on_commit_do_all_unittests.yml)\n\n<a href="https://pypi.org/project/htag/">\n    <img src="https://badge.fury.io/py/htag.svg?x" alt="Package version">\n</a>\n\n\nA new python library to create UI (or UI toolkit), which render nativly in anything which can render **html/js/css**.\nThoses can be a browser, a pywebview, an android/apk, or anything based on cef, depending on an [htag runner](https://manatlan.github.io/htag/runners/)\xa0!\nAs it\'s based on html/js rendering: you can easily mix powerful JS libs with powerful PY3 libs : and make powerful python apps !\n\n * For a **desktop app** : You can use the [PyWebView runner](https://manatlan.github.io/htag/runners/#pywebwiew), which will run the UI in a pywebview container (or "ChromeApp runner", in a local chrome app mode).\xa0\n * For a **web app** : You can use the [WebHTTP runner](https://manatlan.github.io/htag/runners/#webhttp), which will run the UI in a web server, and serve the UI on client side, in a browser.\xa0\n * For a **android app** : You can use the [AndroidApp runner](https://manatlan.github.io/htag/runners/#androidapp), which will run the UI in a kiwi webview thru tornado webserver, and can be embedded in an apk ([recipes](https://github.com/manatlan/htagapk))\n * For a **pyscript app** : you can use the [PyScript runner](https://manatlan.github.io/htag/runners/#pyscript), which will run completly in client side\n\nBut yes … the promise is here : **it\'s a GUI toolkit for building "beautiful" applications for mobile, web, and desktop from a single codebase**.\n\n[DOCUMENTATION](https://manatlan.github.io/htag/)\n\n[DEMO/TUTORIAL](https://htag.glitch.me/)\n\n[Changelog](https://github.com/manatlan/htag/releases)\n\n[Available on pypi.org](https://pypi.org/project/htag/)\n\n[Announcement on reddit (22/07/14)](https://www.reddit.com/r/Python/comments/vysnci/htag_a_new_gui_tookit_for_webdesktopandroid_from/)\n\n## To have a look\n\nTODO: need to find a super demo ;-)\n\n## ROADMAP to 1.0.0\n\n * rock solid (need more tests)\n * setup minimal docs ;-)\n * ~~top level api could change (Tag() -> create a Tag, Tag.mytag() -> create a TagBase ... can be a little bit ambiguous)~~\n * ~~manage "query params" from url to initialize Tags/routes~~\n * ~~I don\'t really like the current way to generate js in interaction : need to found something more solid.~~\n * ~~the current way to initiate the statics is odd (only on real (embedded) Tag\'s) : should find a better way (static like gtag ?!)~~\n\nand more technicals :\n- ~~better js try/catch to sort js/py error~~ + try/catch on http com error (for thoses which kill session webhttp/pye)\n- ~~getStateImage is non sense coz it\'s str\'ing (why not returning the str ?!)~~\n- mix the Tag.__init__ with the old system (like this: it\'s unmaintable)\n- ~~introduce a virtual tag/placeholder~~\n- ...\n\n## History\n\nAt the beginning, there was [guy](https://github.com/manatlan/guy), which was/is the same concept as [python-eel](https://github.com/ChrisKnott/Eel), but more advanced.\nOne day, I\'ve discovered [remi](https://github.com/rawpython/remi), and asked my self, if it could be done in a *guy way*. The POC was very good, so I released\na version of it, named [gtag](https://github.com/manatlan/gtag). It worked well despite some drawbacks, but was too difficult to maintain. So I decided to rewrite all\nfrom scratch, while staying away from *guy* (to separate, *rendering* and *runners*)... and [htag](https://github.com/manatlan/htag) was born. The codebase is very short, concepts are better implemented, and it\'s very easy to maintain.\n\n\n',
     'author': 'manatlan',
     'author_email': 'manatlan@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/manatlan/htag',
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['htag',
 'htag.runners'] package_data = \ {'': ['*']} setup_kwargs = { 'name': 'htag',
-'version': '0.9.8', 'description': 'GUI toolkit for building GUI toolkits (and
+'version': '0.9.9', 'description': 'GUI toolkit for building GUI toolkits (and
 create beautiful applications for mobile, web, and desktop from a single
 python3 codebase)', 'long_description': '# HTag : "H(tml)Tag"\n\n[https://
 manatlan.github.io/htag/htag.png]\n\n[![Test](https://github.com/manatlan/htag/
 actions/workflows/on_commit_do_all_unittests.yml/badge.svg)](https://
 github.com/manatlan/htag/actions/workflows/
 on_commit_do_all_unittests.yml)\n\n\n_[Package_version]\n\n\n\nA new python
 library to create UI (or UI toolkit), which render nativly in anything which
```

### Comparing `htag-0.9.8/PKG-INFO` & `htag-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htag
-Version: 0.9.8
+Version: 0.9.9
 Summary: GUI toolkit for building GUI toolkits (and create beautiful applications for mobile, web, and desktop from a single python3 codebase)
 Home-page: https://github.com/manatlan/htag
 License: MIT
 Keywords: gui,electron,cef,pywebview,starlette,uvicorn,tornado,asyncio,desktop,web,mobile,http,websocket,html,pyscript,android,kivy,apk
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: htag Version: 0.9.8 Summary: GUI toolkit for
+Metadata-Version: 2.1 Name: htag Version: 0.9.9 Summary: GUI toolkit for
 building GUI toolkits (and create beautiful applications for mobile, web, and
 desktop from a single python3 codebase) Home-page: https://github.com/manatlan/
 htag License: MIT Keywords:
 gui,electron,cef,pywebview,starlette,uvicorn,tornado,asyncio,desktop,web,mobile,http,websocket,html,pyscript,android,kivy,apk
 Author: manatlan Author-email: manatlan@gmail.com Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

