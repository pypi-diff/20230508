# Comparing `tmp/rayserverdl-1.0.5.tar.gz` & `tmp/rayserverdl-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rayserverdl-1.0.5.tar", last modified: Sat May  6 19:37:52 2023, max compression
+gzip compressed data, was "rayserverdl-2.0.1.tar", last modified: Mon May  8 23:51:01 2023, max compression
```

## Comparing `rayserverdl-1.0.5.tar` & `rayserverdl-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 19:37:52.783396 rayserverdl-1.0.5/
--rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 rayserverdl-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     1026 2023-05-06 19:37:52.774396 rayserverdl-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      143 2023-05-06 04:21:57.000000 rayserverdl-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 19:37:52.648388 rayserverdl-1.0.5/rayserverdl/
--rw-rw-rw-   0        0        0     3721 2023-05-06 19:36:56.000000 rayserverdl-1.0.5/rayserverdl/__init__.py
--rw-rw-rw-   0        0        0       75 2023-05-06 19:33:02.000000 rayserverdl-1.0.5/rayserverdl/version.py
-drwxrwxrwx   0        0        0        0 2023-05-06 19:37:52.756394 rayserverdl-1.0.5/rayserverdl.egg-info/
--rw-rw-rw-   0        0        0     1026 2023-05-06 19:37:48.000000 rayserverdl-1.0.5/rayserverdl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-05-06 19:37:50.000000 rayserverdl-1.0.5/rayserverdl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 19:37:48.000000 rayserverdl-1.0.5/rayserverdl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-06 19:37:48.000000 rayserverdl-1.0.5/rayserverdl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-06 19:37:48.000000 rayserverdl-1.0.5/rayserverdl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 19:37:48.000000 rayserverdl-1.0.5/rayserverdl.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-05-06 19:37:52.788396 rayserverdl-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1653 2023-05-06 04:28:01.000000 rayserverdl-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:51:01.676877 rayserverdl-2.0.1/
+-rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 rayserverdl-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1026 2023-05-08 23:51:01.671877 rayserverdl-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      143 2023-05-06 04:21:57.000000 rayserverdl-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 23:51:01.598873 rayserverdl-2.0.1/rayserverdl/
+-rw-rw-rw-   0        0        0     3688 2023-05-08 23:50:04.000000 rayserverdl-2.0.1/rayserverdl/__init__.py
+-rw-rw-rw-   0        0        0       75 2023-05-08 23:44:20.000000 rayserverdl-2.0.1/rayserverdl/version.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:51:01.663877 rayserverdl-2.0.1/rayserverdl.egg-info/
+-rw-rw-rw-   0        0        0     1026 2023-05-08 23:50:58.000000 rayserverdl-2.0.1/rayserverdl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-05-08 23:50:59.000000 rayserverdl-2.0.1/rayserverdl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 23:50:58.000000 rayserverdl-2.0.1/rayserverdl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-08 23:50:58.000000 rayserverdl-2.0.1/rayserverdl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-08 23:50:58.000000 rayserverdl-2.0.1/rayserverdl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-08 23:50:58.000000 rayserverdl-2.0.1/rayserverdl.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-05-08 23:51:01.678877 rayserverdl-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1653 2023-05-06 04:28:01.000000 rayserverdl-2.0.1/setup.py
```

### Comparing `rayserverdl-1.0.5/LICENSE` & `rayserverdl-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rayserverdl-1.0.5/PKG-INFO` & `rayserverdl-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayserverdl
-Version: 1.0.5
+Version: 2.0.1
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/rayserverdl
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,downloader,stream,files
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rayserverdl-1.0.5/rayserverdl/__init__.py` & `rayserverdl-2.0.1/rayserverdl/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,99 @@
-import aiohttp
-import asyncio
+from requests_html import HTMLSession
 import os
+import urllib3
+urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 import pyshortext
 from bs4 import BeautifulSoup
 import sys
 import time
 import platform
 from colorama import init, Fore, Style
 init()
 
+_SESSION = None
+
 def sizeof_fmt(num, suffix='B'):
     for unit in ['','Ki','Mi','Gi','Ti','Pi','Ei','Zi']:
         if abs(num) < 1024.0:
             return "%3.1f%s%s" % (num, unit, suffix)
         num /= 1024.0
     return "%.1f%s%s" % (num, 'Yi', suffix)
 
 def convert_speed(speed):
     if speed >= 1024 * 1024:
         return f"{speed / (1024 * 1024):.2f} MB/s"
     else:
         return f"{speed / 1024:.2f} KB/s"
 
-async def make_file(url):
+def make_file(url):
+    global _SESSION
     print(Style.BRIGHT + Fore.BLUE + "Procesando ." + Style.RESET_ALL)
     values = str(url).split('https://rayserver.downloader/')[1].split('/')
     filesize = int(values[0])
     filename = values[3]
     parts = str(pyshortext.unshort(values[2])).split('|')
     ids = str(parts[1]).split(' ')
     data = str(parts[0]).split(' ')
     host = data[0]
     user = data[1]
     passw = data[2]
     up_id = data[3]
     #login
-    async with aiohttp.ClientSession(connector=aiohttp.TCPConnector(ssl=False)) as session:
-        async with session.get(host + "login") as resp:
-            html = await resp.text()
-        soup = BeautifulSoup(html, 'html.parser')
-        csrfToken = soup.find("input", attrs={"name": "csrfToken"})['value']
-        #print(csrfToken)
+    session = HTMLSession()
+    resp = session.get(host + "login",verify=False)
+    soup = BeautifulSoup(resp.text, 'html.parser')
+    csrfToken = soup.find("input", attrs={"name": "csrfToken"})['value']
+    os.system('cls' if os.name=='nt' else 'clear')
+    print(Style.BRIGHT + Fore.BLUE + "Procesando .." + Style.RESET_ALL)
+    if _SESSION:
+        session = _SESSION
         os.system('cls' if os.name=='nt' else 'clear')
-        print(Style.BRIGHT + Fore.BLUE + "Procesando .." + Style.RESET_ALL)
+        print(Style.BRIGHT + Fore.BLUE + "Procesado" + Style.RESET_ALL)
+    else:
         url_post = host + 'login/signIn'
         payload = {}
         payload["csrfToken"] = csrfToken
         payload["source"] = ""
         payload["username"] = user
         payload["password"] = passw
         payload["remember"] = "1"
-        async with session.post(url_post, data=payload) as resp:
-            os.system('cls' if os.name=='nt' else 'clear')
-            print(Style.BRIGHT + Fore.BLUE + "Procesado" + Style.RESET_ALL)
-            await download_file(host,filename,filesize,ids,up_id,session)
+        resp = session.post(url_post, data=payload,verify=False)
+        os.system('cls' if os.name=='nt' else 'clear')
+        print(Style.BRIGHT + Fore.BLUE + "Procesado" + Style.RESET_ALL)
+        _SESSION = session
+    download_file(host,filename,filesize,ids,up_id,session)
 
-async def download_file(host,filename,filesize,ids,up_id,session):
+def download_file(host,filename,filesize,ids,up_id,session):
     os.system('cls' if os.name=='nt' else 'clear')
-    try:
-        print(Style.BRIGHT + Fore.RED + f"{filename}\n" + Style.RESET_ALL)
-        chunks = 0
-        start_time = time.time()
-        f = open("/storage/emulated/0/Download/"+filename, 'wb')
-        for id in ids:
+    print(Style.BRIGHT + Fore.RED + f"{filename}\n" + Style.RESET_ALL)
+    chunks = 0
+    start_time = time.time()
+    f = open('/storage/emulated/0/Download/'+filename, 'wb')
+    for id in ids:
+        try:
             url = f"{host}$$$call$$$/api/file/file-api/download-file?submissionFileId={id}&submissionId={up_id}&stageId=1"
-            async with session.get(url,ssl=False,timeout=999999999999) as resp:
-                async for chunk in resp.content.iter_chunked(2048):
-                    f.write(chunk)
-                    chunks+=len(chunk)
-                    current_time = time.time()
-                    download_speed = chunks / (current_time - start_time)
-                    text = f"\r[{convert_speed(download_speed)}] {sizeof_fmt(chunks)} de {sizeof_fmt(filesize)}"
-                    print(text, end="|")
-        f.close()
-    except Exception as ex:
-        print(str(ex))
+            resp = session.get(url,verify=False)
+            for chunk in resp.iter_content(2048):
+                f.write(chunk)
+                chunks+=len(chunk)
+                current_time = time.time()
+                download_speed = chunks / (current_time - start_time)
+                text = f"\r[{convert_speed(download_speed)}] {sizeof_fmt(chunks)} de {sizeof_fmt(filesize)}"
+                print(text, end="")
+        except:
+            pass
 
-async def main():
+def main():
     print(Style.BRIGHT + Fore.YELLOW + "Welcome to RayServer.CLi\n" + Style.RESET_ALL)
     url = input("Introduce la URL del archivo que deseas descargar:\n\n> ")
     os.system('cls' if os.name=='nt' else 'clear')
-    await make_file(url)
-    v = input("Desea realizar otra operación? (y/n):\n> ")
+    make_file(url)
+    v = input("\nDesea realizar otra operación? (y/n):\n> ")
     if v=="y":
         os.system('cls' if os.name=='nt' else 'clear')
-        await main()
+        main()
     else:
         print(Style.BRIGHT + Fore.YELLOW + "Gracias por usar RayServer.Cli" + Style.RESET_ALL)
         sys.exit()
 
-loop = asyncio.get_event_loop()
-loop.run_until_complete(main())
+main()
```

### Comparing `rayserverdl-1.0.5/rayserverdl.egg-info/PKG-INFO` & `rayserverdl-2.0.1/rayserverdl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayserverdl
-Version: 1.0.5
+Version: 2.0.1
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/rayserverdl
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,downloader,stream,files
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rayserverdl-1.0.5/setup.py` & `rayserverdl-2.0.1/setup.py`

 * *Files identical despite different names*

