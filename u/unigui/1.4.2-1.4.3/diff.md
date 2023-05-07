# Comparing `tmp/unigui-1.4.2.tar.gz` & `tmp/unigui-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.4.2.tar", last modified: Sun May  7 00:26:14 2023, max compression
+gzip compressed data, was "dist/unigui-1.4.3.tar", last modified: Sun May  7 23:44:05 2023, max compression
```

## Comparing `unigui-1.4.2.tar` & `unigui-1.4.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:26:14.000000 unigui-1.4.2/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui/
--rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.4.2/unigui/manager.py
--rw-rw-r--   0 george    (1000) george    (1000)     7695 2023-05-03 16:32:01.000000 unigui-1.4.2/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.4.2/unigui/userset.py
--rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:39.000000 unigui-1.4.2/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:49.000000 unigui-1.4.2/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.4.2/unigui/utils.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/css/365.b8547d97.css
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/css/vendor.49a52e8f.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)   847622 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/js/vendor.c0de6c67.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/js/193.b4cc3ffe.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/js/430.4be6e8a8.js
--rw-rw-r--   0 george    (1000) george    (1000)     5867 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/js/app.bfd9bd6e.js
--rw-rw-r--   0 george    (1000) george    (1000)    39843 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/js/365.3c494fbf.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.4.2/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      585 2023-05-07 00:26:03.000000 unigui-1.4.2/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    19428 2023-05-07 00:26:14.000000 unigui-1.4.2/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-05-07 00:26:14.000000 unigui-1.4.2/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    19138 2023-05-03 16:32:01.000000 unigui-1.4.2/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.4.2/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       30 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    19428 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.4.2/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1223 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 23:44:05.000000 unigui-1.4.3/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui/
+-rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.4.3/unigui/manager.py
+-rw-rw-r--   0 george    (1000) george    (1000)     7695 2023-05-03 16:32:01.000000 unigui-1.4.3/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.4.3/unigui/userset.py
+-rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:39.000000 unigui-1.4.3/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:49.000000 unigui-1.4.3/unigui/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.4.3/unigui/utils.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/css/748.d94da9c0.css
+-rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/css/vendor.49a52e8f.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)   847622 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/js/vendor.c0de6c67.js
+-rw-rw-r--   0 george    (1000) george    (1000)    39996 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/js/748.67c1fce8.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/js/193.b4cc3ffe.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/js/430.4be6e8a8.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/js/app.73e4276f.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.4.3/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      585 2023-05-07 23:43:23.000000 unigui-1.4.3/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    19428 2023-05-07 23:44:05.000000 unigui-1.4.3/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-05-07 23:44:05.000000 unigui-1.4.3/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    19138 2023-05-03 16:32:01.000000 unigui-1.4.3/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.4.3/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       30 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    19428 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.4.3/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1223 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.4.2/unigui/manager.py` & `unigui-1.4.3/unigui/manager.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/guielements.py` & `unigui-1.4.3/unigui/guielements.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/server.py` & `unigui-1.4.3/unigui/server.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/utils.py` & `unigui-1.4.3/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/web/favicon.ico` & `unigui-1.4.3/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/web/css/365.b8547d97.css` & `unigui-1.4.3/unigui/web/css/748.d94da9c0.css`

 * *Files 12% similar despite different names*

```diff
@@ -1 +1 @@
-thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-7cd4ac4c]{display:flex;justify-content:center}.custom-caption[data-v-7cd4ac4c]{padding:5px!important}.web-camera-container[data-v-7cd4ac4c]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-7cd4ac4c]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-7cd4ac4c]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-7cd4ac4c]{opacity:1}.web-camera-container .camera-shoot[data-v-7cd4ac4c]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-7cd4ac4c]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-7cd4ac4c]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-7cd4ac4c]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-7cd4ac4c]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-7cd4ac4c]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-7cd4ac4c]{animation:preload-7cd4ac4c 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-7cd4ac4c]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-7cd4ac4c]:nth-child(3){animation-delay:.4s}@keyframes preload-7cd4ac4c{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-7cd4ac4c]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
+thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-9805fac6]{display:flex;justify-content:center}.custom-caption[data-v-9805fac6]{padding:5px!important}.web-camera-container[data-v-9805fac6]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-9805fac6]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-9805fac6]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-9805fac6]{opacity:1}.web-camera-container .camera-shoot[data-v-9805fac6]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-9805fac6]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-9805fac6]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-9805fac6]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-9805fac6]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-9805fac6]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-9805fac6]{animation:preload-9805fac6 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-9805fac6]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-9805fac6]:nth-child(3){animation-delay:.4s}@keyframes preload-9805fac6{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-9805fac6]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
```

### Comparing `unigui-1.4.2/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.4.3/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/web/icons/favicon-96x96.png` & `unigui-1.4.3/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/web/icons/favicon-16x16.png` & `unigui-1.4.3/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/web/icons/favicon-32x32.png` & `unigui-1.4.3/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/web/icons/favicon-128x128.png` & `unigui-1.4.3/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.4.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.4.3/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.4.3/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.4.3/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.4.3/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.4.3/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.4.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.4.3/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/web/js/vendor.c0de6c67.js` & `unigui-1.4.3/unigui/web/js/vendor.c0de6c67.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/web/js/193.b4cc3ffe.js` & `unigui-1.4.3/unigui/web/js/193.b4cc3ffe.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/web/js/430.4be6e8a8.js` & `unigui-1.4.3/unigui/web/js/430.4be6e8a8.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui/web/js/app.bfd9bd6e.js` & `unigui-1.4.3/unigui/web/js/app.73e4276f.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(365)]).then(r.bind(r, 365)),
+                        component: () => Promise.all([r.e(736), r.e(748)]).then(r.bind(r, 9748)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -44,30 +44,30 @@
                                     top: 0
                                 }),
                                 routes: v,
                                 history: e("")
                             });
                         return t
                     }));
-                async function b(e, t) {
+                async function g(e, t) {
                     const r = "function" === typeof m ? await m({}) : m,
                         n = e(d);
                     return n.use(o.Z, t), {
                         app: n,
                         router: r
                     }
                 }
-                var g = r(6417),
+                var b = r(6417),
                     y = r(5597);
                 const w = {
                         config: {
                             notify: {}
                         },
                         plugins: {
-                            Notify: g.Z,
+                            Notify: b.Z,
                             Dialog: y.Z
                         }
                     },
                     O = "";
                 async function k({
                     app: e,
                     router: t
@@ -94,15 +94,15 @@
                             urlPath: i,
                             publicPath: O
                         })
                     } catch (l) {
                         return l && l.url ? void a(l.url) : void console.error("[Quasar] boot error:", l)
                     }!0 !== n && (e.use(t), e.mount("#q-app"))
                 }
-                b(n.ri, w).then((e => Promise.all([Promise.resolve().then(r.bind(r, 2390))]).then((t => {
+                g(n.ri, w).then((e => Promise.all([Promise.resolve().then(r.bind(r, 2390))]).then((t => {
                     const r = t.map((e => e.default)).filter((e => "function" === typeof e));
                     k(e, r)
                 }))))
             },
             2390: (e, t, r) => {
                 r.r(t), r.d(t, {
                     default: () => o
@@ -159,25 +159,25 @@
             })
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, n) => (r.f[n](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "b4cc3ffe",
-            365: "3c494fbf",
-            430: "4be6e8a8"
+            430: "4be6e8a8",
+            748: "67c1fce8"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
-            365: "b8547d97",
-            736: "49a52e8f"
+            736: "49a52e8f",
+            748: "d94da9c0"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
             } catch (e) {
@@ -260,15 +260,15 @@
                 e(n, l, o, a)
             })),
             o = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                365: 1
+                748: 1
             };
             o[e] ? t.push(o[e]) : 0 !== o[e] && r[e] && t.push(o[e] = n(e).then((() => {
                 o[e] = 0
             }), (t => {
                 throw delete o[e], t
             })))
         }
```

### Comparing `unigui-1.4.2/unigui/web/js/365.3c494fbf.js` & `unigui-1.4.3/unigui/web/js/748.67c1fce8.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [365], {
-        365: (e, t, a) => {
+    [748], {
+        9748: (e, t, a) => {
             a.r(t), a.d(t, {
-                default: () => Wt
+                default: () => Qt
             });
             var l = a(3673),
                 s = a(2323);
             const i = (0, l._)("div", {
                 class: "q-pa-lg"
             }, null, -1);
 
@@ -104,149 +104,157 @@
                 c = a(8603),
                 h = a.n(c);
             let u = null,
                 p = {},
                 g = !0;
             const m = 136,
                 f = 400,
-                w = `height: ${m}px; width: ${f}px`,
-                y = {},
-                b = {},
-                k = ["error", "progress", "warning", "info"];
+                w = `height: ${m}px; width: ${f}px`;
 
-            function v(e) {
+            function y(e) {
+                let t = e.minheight ? e.minheight : m,
+                    a = e.minwidth ? e.minwidth : f;
+                return `height: ${t}px; width: ${a}px`
+            }
+            const b = {},
+                k = {},
+                v = ["error", "progress", "warning", "info"];
+
+            function C(e) {
                 d = new WebSocket("ws://localhost:8000/ws"), d.onopen = () => e.statusConnect = !0, d.onmessage = t => {
                     g && console.log("socket message", t.data), e.processMessage(JSON.parse(t.data))
                 }, d.onerror = t => e.error(t), d.onclose = t => {
                     t.wasClean ? e.info("Connection closed and was clean.") : e.error("Connection suddenly closed!"), e.statusConnect = !1, g && console.info("close code : " + t.code + " reason: " + t.reason)
                 }, u = e
             }
 
-            function C(e) {
+            function q(e) {
                 console.log("sended", e), d.send(JSON.stringify(e))
             }
-            let q, _ = 0;
+            let _, j = 0;
 
-            function j(e) {
+            function S(e) {
                 for (var t in e) e.hasOwnProperty(t) && delete e[t]
             }
 
-            function S(e, t, a, l = "?") {
-                let s = ++_,
+            function A(e, t, a, l = "?") {
+                let s = ++j,
                     i = [e.pdata.name, e.data.name, l, t, s];
-                C(i), p[s] = a
+                q(i), p[s] = a
             }
 
-            function A() {
-                j(y), j(b)
+            function Z() {
+                S(b), S(k)
             }
 
-            function Z(e, t) {
+            function M(e, t) {
                 Object.assign(e.data, t), e.updated = t.value, e.value = t.value
             }
 
-            function M(e) {
+            function $(e) {
                 if (e.multi)
                     for (let [t, a] of e.update.entries())
                         if (a.length > 1) {
                             a.reverse();
                             let l = a.join("@"),
-                                s = b[l];
-                            Z(s, e.data[t])
+                                s = k[l];
+                            M(s, e.data[t])
                         } else {
-                            let l = y[a[0]];
+                            let l = b[a[0]];
                             Object.assign(l.data, e.data[t])
                         }
                 else {
                     let t, a = e.update;
                     if (a.length > 1) {
                         a.reverse();
                         let e = a.join("@");
-                        t = b[e]
-                    } else t = y[a[0]];
-                    Z(t, e.data), 1 == a.length && h().delay(W, 200, t)
+                        t = k[e]
+                    } else t = b[a[0]];
+                    M(t, e.data), 1 == a.length && h().delay(W, 200, t)
                 }
             }
 
-            function $(e) {
+            function z(e) {
                 typeof e.answer == String ? u.showError() : p[e.id](e.answer), delete p[e.id]
             }
 
-            function z(e) {
+            function D(e) {
                 let t = [];
                 for (let l of e) l instanceof Array ? t.push(l) : t.push([l]);
                 let a = t.shift();
                 return t.reduce(((e, t) => e.flatMap((e => t.map((t => e instanceof Array ? [...e, t] : [e, t]))))), a)
             }
-            let D = h().debounce(W, 200);
-            const O = {
-                childList: !0,
-                subtree: !0,
-                attributes: !0
-            };
 
-            function Q() {
-                q && (q.disconnect(), q = null), q = new MutationObserver(D), q.observe(u.$el, O)
+            function O() {
+                for (let [e, t] of Object.entries(k)) t.expanding && (t.styleSize = y(t.data));
+                (0, l.Y3)((() => {
+                    requestAnimationFrame((() => {
+                        requestAnimationFrame((() => {
+                            W()
+                        }))
+                    }))
+                }))
             }
+            let Q = h().debounce(O, 200);
 
             function W(e) {
-                Array.isArray(e) && (e = null), q && (q.disconnect(), q = null), g && console.log("------------------recalc design");
+                Array.isArray(e) && (e = null), _ && (_.disconnect(), _ = null), g && console.log("------------------recalc design");
                 const t = V(e),
                     a = E(e);
                 for (let [l, s] of Object.entries(t)) {
-                    let e = b[l];
+                    let e = k[l];
                     const [t, i] = a[l];
                     let o, n = e.geom().el,
                         d = e.pdata ? e.pdata.name : e.name,
-                        r = y[d];
+                        r = b[d];
                     for (let a of r.data.childs)
                         if (Array.isArray(a)) {
                             if (a.find((t => t.name == e.data.name))) {
                                 let e = a[a.length - 1],
                                     t = `${e.name}@${d}`;
-                                o = b[t];
+                                o = k[t];
                                 break
                             }
                         } else if (a.name == e.data.name) {
                         o = e;
                         break
                     }
                     let c = r.data.width ? r.data.width - n.clientWidth - t : r.$el.getBoundingClientRect().right - (o ? o.geom().right : e.geom().right);
                     c /= i;
                     let h = l.startsWith("_scroll@") ? e.geom().inner.clientHeight : n.clientHeight;
-                    e.styleSize = `height: ${h+Math.floor(s)}px; width: ${n.clientWidth+c+t}px;`
+                    e.styleSize = `height: ${h+s}px; width: ${n.clientWidth+c+t}px;`
                 }
             }
 
             function V(e) {
                 const t = u.screen.blocks;
                 let a = window.innerHeight;
                 a -= 2;
                 let l = {},
                     s = new Map,
                     i = {};
-                for (let [d, r] of Object.entries(y)) i[r.name] = r.$el.getBoundingClientRect().height;
+                for (let [d, r] of Object.entries(b)) i[r.name] = r.$el.getBoundingClientRect().height;
                 let o = [];
                 for (let d of t) {
                     const e = [];
                     let t = d instanceof Array,
-                        n = t ? z(d) : [
+                        n = t ? D(d) : [
                             [d]
                         ];
                     for (let a of n) {
                         let e = 0;
                         for (let t of a) e += i[t.name] + 8;
                         o.push([e, a])
                     }
                     o.sort(((e, t) => e[0] > t[0] ? -1 : e[0] == t[0] ? 0 : 1));
                     for (let l of o) {
                         let t = l[1];
                         (0, r.hu)(Array.isArray(t));
                         const i = [];
-                        for (let [e, a] of Object.entries(b))
+                        for (let [e, a] of Object.entries(k))
                             if (a.expanding_height) {
                                 let [l, o] = e.split("@");
                                 if (t.find((e => e.name == o))) {
                                     let e = !0;
                                     const t = a.geom();
                                     for (let [l, o] of i.entries()) {
                                         let n = o.geom();
@@ -258,16 +266,27 @@
                                     e && i.push(a)
                                 }
                             } i.length && e.push([a - l[0] - 64, i])
                     }
                     for (let [a, s] of e) {
                         s.sort(((e, t) => e.geom().scrollHeight < t.geom().scrollHeight));
                         let e = s.length;
-                        for (let t of s) t.fullname in l && (e--, a -= l[t.fullname]);
-                        for (let t of s) t.fullname in l || ("docviewer" == t.type ? l[t.fullname] = a / e + 4 : l[t.fullname] = a / e)
+                        for (let i of s) i.fullname in l && (e--, a -= l[i.fullname]);
+                        let t = 0;
+                        for (let i of s)
+                            if (!(i.fullname in l)) {
+                                let s, o = a / e;
+                                if (1 == e) s = o;
+                                else if (s = Math.floor(o), o - s) {
+                                    t += o - s;
+                                    let e = Math.round(t) - t;
+                                    e < .001 && e > -.001 && (s += Math.round(t), t = 0)
+                                }
+                                "docviewer" == i.type ? l[i.fullname] = s + 4 : l[i.fullname] = s
+                            }
                     }
                 }
                 let n = Array.from(s.entries());
                 n.sort(((e, t) => e[0] in l || e[1] in l ? -1 : 1));
                 for (let [d, r] of n) r in l ? l[d] = l[r] : l[r] = l[d];
                 return l
             }
@@ -295,20 +314,20 @@
                     l = e
                 }
                 l.sort(((e, t) => e.length > t.length ? -1 : e.length == t.length ? 0 : 1));
                 const i = [];
                 let o = new Map;
                 for (let n of l) {
                     let e = Array.isArray(n) ? n[n.length - 1] : n,
-                        t = y[e.name].$el.getBoundingClientRect().right;
+                        t = b[e.name].$el.getBoundingClientRect().right;
                     e = Array.isArray(n) ? n[0] : n;
-                    let l = y[e.name].$el.getBoundingClientRect().left,
+                    let l = b[e.name].$el.getBoundingClientRect().left,
                         s = a - t + l - 10;
                     const d = [];
-                    for (let [a, i] of Object.entries(b))
+                    for (let [a, i] of Object.entries(k))
                         if (i.expanding_width) {
                             let e = a.split("@")[1];
                             if (n.find((t => t.name == e))) {
                                 let e = !0,
                                     t = i.geom().left;
                                 for (let [a, l] of d.entries())
                                     if (l !== i && l.geom().left == t) {
@@ -339,15 +358,15 @@
                 for (let [n, d] of o.entries()) d in s ? s[n] = s[d] : s[d] = s[n];
                 return s
             }
             const H = (0, l.aZ)({
                 name: "menubar",
                 methods: {
                     send() {
-                        C(["root", this.name])
+                        q(["root", this.name])
                     }
                 },
                 props: {
                     name: {
                         type: String,
                         required: !0
                     },
@@ -477,15 +496,15 @@
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"]))], 8, le)))), 256))])),
                     _: 1
                 })
             }
             var oe = a(8880);
-            const ne = e => ((0, l.dD)("data-v-7cd4ac4c"), e = e(), (0, l.Cn)(), e),
+            const ne = e => ((0, l.dD)("data-v-9805fac6"), e = e(), (0, l.Cn)(), e),
                 de = ["width", "height"],
                 re = ["src"],
                 ce = {
                     key: 15,
                     class: "web-camera-container"
                 },
                 he = {
@@ -510,35 +529,35 @@
                     key: 1,
                     class: "camera-shoot"
                 },
                 ke = ne((() => (0, l._)("img", {
                     src: "https://img.icons8.com/material-outlined/50/000000/camera--v2.png"
                 }, null, -1))),
                 ve = [ke],
-                Ce = {
+                xe = {
                     key: 2,
                     class: "camera-download"
                 };
 
-            function xe(e, t, a, i, o, n) {
+            function Ce(e, t, a, i, o, n) {
                 const d = (0, l.up)("q-icon"),
                     r = (0, l.up)("q-img"),
                     c = (0, l.up)("q-badge"),
                     h = (0, l.up)("q-select"),
                     u = (0, l.up)("q-checkbox"),
                     p = (0, l.up)("q-toggle"),
                     g = (0, l.up)("q-btn-toggle"),
                     m = (0, l.up)("utable"),
                     f = (0, l.up)("q-input"),
                     w = (0, l.up)("q-tree"),
                     y = (0, l.up)("q-scroll-area"),
                     b = (0, l.up)("q-separator"),
                     k = (0, l.up)("q-uploader"),
                     v = (0, l.up)("cgraph"),
-                    C = (0, l.up)("q-btn");
+                    x = (0, l.up)("q-btn");
                 return "image" == e.type ? ((0, l.wg)(), (0, l.j4)(r, {
                     key: 0,
                     src: e.data.name,
                     "spinner-color": "blue",
                     onClick: (0, oe.iM)(e.switchValue, ["stop"]),
                     fit: "cover",
                     style: (0, s.j5)(e.elemSize)
@@ -742,24 +761,24 @@
                     [oe.F8, e.isPhotoTaken]
                 ])], 2)), [
                     [oe.F8, !e.isLoading]
                 ]) : (0, l.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, l.wg)(), (0, l.iD)("div", be, [(0, l._)("button", {
                     class: "button",
                     type: "button",
                     onClick: t[11] || (t[11] = (...t) => e.takePhoto && e.takePhoto(...t))
-                }, ve)])) : (0, l.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("div", Ce, [(0, l.Wm)(C, {
+                }, ve)])) : (0, l.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("div", xe, [(0, l.Wm)(x, {
                     onClick: e.downloadImage,
                     label: "Send"
-                }, null, 8, ["onClick"])])) : (0, l.kq)("", !0)])) : "" != e.showname ? ((0, l.wg)(), (0, l.j4)(C, {
+                }, null, 8, ["onClick"])])) : (0, l.kq)("", !0)])) : "" != e.showname ? ((0, l.wg)(), (0, l.j4)(x, {
                     key: 16,
                     "no-caps": "",
                     label: e.name,
                     icon: e.data.icon,
                     onClick: e.sendValue
-                }, null, 8, ["label", "icon", "onClick"])) : ((0, l.wg)(), (0, l.j4)(C, {
+                }, null, 8, ["label", "icon", "onClick"])) : ((0, l.wg)(), (0, l.j4)(x, {
                     key: 17,
                     "no-caps": "",
                     dense: "",
                     icon: e.data.icon,
                     onClick: e.sendValue
                 }, null, 8, ["icon", "onClick"]))
             }
@@ -1009,15 +1028,15 @@
                             return a
                         },
                         o = i(),
                         n = (0, Ae.iH)(o),
                         d = (0, Ae.iH)(o),
                         r = (0, Ae.iH)(!Array.isArray(t.value.value)),
                         c = (e, l) => {
-                            C([a.value.name, t.value.name, e, l])
+                            q([a.value.name, t.value.name, e, l])
                         },
                         h = (0, l.Fl)((() => r.value ? d.value.length > 0 ? d.value[0].iiid : null : d.value.map((e => e.iiid)))),
                         u = (0, l.Fl)((() => t.value.value));
                     return (0, l.YP)(s, ((e, t) => {
                         d.value = i(), n.value = d.value
                     })), (0, l.YP)(t, ((e, a) => {
                         g && console.log("data update", a.name), d.value = i(), n.value = d.value, r.value = !Array.isArray(t.value.value)
@@ -1103,23 +1122,23 @@
                                         t = typeof this.data.rows[e][this.cedit];
                                     "string" != t && "number" != t || (this.selected = [this.rows[e]])
                                 }
                                 break
                         }
                     },
                     complete(e, t, a) {
-                        S(this, [e, [this.redit, this.cedit]], (e => t((() => {
+                        A(this, [e, [this.redit, this.cedit]], (e => t((() => {
                             this.options = e
                         }))))
                     },
                     append() {
                         let e = this.data.rows,
                             t = e.length,
                             a = this;
-                        S(this, [t, this.search], (function(l) {
+                        A(this, [t, this.search], (function(l) {
                             if (!Array.isArray(l)) return u.error(l);
                             g && console.log("added row", l), a.search = "", e.push(l), setTimeout((() => {
                                 let e = a.rows;
                                 a.select(e[t], 0), a.showSelected()
                             }), 100)
                         }), "+")
                     },
@@ -1329,15 +1348,15 @@
                         },
                         value() {
                             return this.data.value
                         }
                     },
                     methods: {
                         sendMessage(e, t) {
-                            C([this.pdata["name"], this.data["name"], e, t])
+                            q([this.pdata["name"], this.data["name"], e, t])
                         },
                         showClusterNode(e) {
                             const t = e.data("cluster"),
                                 a = this.cy.nodes(`[cluster='${t}']`),
                                 l = this.cy.nodes(`#${t}`);
                             l.data("isClusterNode", !0), l.animate({
                                 position: {
@@ -1427,61 +1446,55 @@
                 }),
                 Ye = (0, U.Z)(Fe, [
                     ["render", Te]
                 ]),
                 Xe = Ye;
 
             function Je(e) {
-                let t = e.minheight ? e.minheight : m,
-                    a = e.minwidth ? e.minwidth : f;
-                return `height: ${t}px; width: ${a}px`
-            }
-
-            function Ge(e) {
                 let t = new FormData;
                 t.append("image", e);
                 let a = new XMLHttpRequest;
                 a.open("POST", "http://localhost:8000", !0), a.onload = function() {
                     200 === this.status ? console.log(this.response) : console.error(a)
                 }, a.send(t)
             }
-            const et = (0, l.aZ)({
+            const Ge = (0, l.aZ)({
                 name: "element",
                 components: {
                     utable: Ke,
                     cgraph: Xe
                 },
                 methods: {
                     log(e) {
                         console.log(e)
                     },
                     onAdded(e) {
                         0 !== e.length && (0 !== this.fileArr.length ? (this.$refs.uploaderRef.removeFile(this.fileArr[0]), this.fileArr.splice(0, 1, e[0])) : this.fileArr.push(e[0]))
                     },
                     sendMessage(e, t) {
-                        C([this.pdata["name"], this.data["name"], e, t])
+                        q([this.pdata["name"], this.data["name"], e, t])
                     },
                     pressedEnter() {
                         "update" in this.data && this.sendMessage("->", this.value)
                     },
                     updateDom(e) {
                         let t = e.files.length;
-                        t && (this.sendMessage("=", e.files[t - 1].name), D())
+                        t && (this.sendMessage("=", e.files[t - 1].name), Q())
                     },
                     sendValue() {
                         this.sendMessage("=", this.value)
                     },
                     switchValue() {
                         this.value = !this.value
                     },
                     setValue(e) {
                         console.log(e), this.value = e
                     },
                     complete(e, t, a) {
-                        this.value = e, S(this, e, (e => t((() => {
+                        this.value = e, A(this, e, (e => t((() => {
                             this.options = e
                         }))))
                     },
                     lens() {
                         u.lens(this.data)
                     },
                     toggleCamera() {
@@ -1514,15 +1527,15 @@
                             }), e)
                         }
                         this.isPhotoTaken = !this.isPhotoTaken;
                         const e = this.$refs.canvas.getContext("2d");
                         e.drawImage(this.$refs.camera, 0, 0, 450, 337.5)
                     },
                     downloadImage() {
-                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(Ge, "image/jpeg")
+                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(Je, "image/jpeg")
                     },
                     geom() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
                         e || (e = this.$el.previousElementSibling, e = "clientHeight" in e ? e : e.nextElementSibling);
                         let t = this.type;
                         const a = "docviewer" == t || "graph" == t ? e : e.querySelector("table" == t ? ".scroll" : ".q-tree"),
                             l = e.getBoundingClientRect();
@@ -1534,20 +1547,20 @@
                             top: l.top,
                             scrollHeight: a.scrollHeight,
                             scrollWidth: a.scrollWidth
                         }
                     }
                 },
                 mounted() {
-                    b[this.fullname] = this, g && console.log("mounted", this.fullname)
+                    k[this.fullname] = this, g && console.log("mounted", this.fullname)
                 },
                 data() {
                     return {
                         value: this.data.value,
-                        styleSize: Je(this.data),
+                        styleSize: y(this.data),
                         options: [],
                         expandedKeys: [],
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
                             backgroundColor: "#027be3",
                             width: "4px",
@@ -1653,50 +1666,50 @@
                         g && console.log("selection changed", e, this.$refs.inputRef), Array.isArray(e) || (e = [0, 0]);
                         let t = this.$refs.inputRef.$el;
                         t.focus();
                         let a = t.getElementsByTagName("textarea");
                         0 == a.length && (a = t.getElementsByTagName("input")), a[0].setSelectionRange(e[0], e[1])
                     },
                     data(e, t) {
-                        g && console.log("data update", this.fullname, t.name), this.expanding && (this.styleSize || (this.styleSize = Je(this.data), console.log(`${this.name} size changed`))), this.value = this.data.value, this.updated = this.value, b[this.fullname] = this
+                        g && console.log("data update", this.fullname, t.name), this.expanding && (this.styleSize || (this.styleSize = y(this.data), console.log(`${this.name} size changed`))), this.value = this.data.value, this.updated = this.value, k[this.fullname] = this
                     }
                 }
             });
-            var tt = a(4027),
-                at = a(9721),
-                lt = a(8886),
-                st = a(8761),
-                it = a(1232),
-                ot = a(5551),
-                nt = a(5869),
-                dt = a(1745);
-            const rt = (0, U.Z)(et, [
-                    ["render", xe],
-                    ["__scopeId", "data-v-7cd4ac4c"]
+            var et = a(4027),
+                tt = a(9721),
+                at = a(8886),
+                lt = a(8761),
+                st = a(1232),
+                it = a(5551),
+                ot = a(5869),
+                nt = a(1745);
+            const dt = (0, U.Z)(Ge, [
+                    ["render", Ce],
+                    ["__scopeId", "data-v-9805fac6"]
                 ]),
-                ct = rt;
-            R()(et, "components", {
-                QImg: tt.Z,
+                rt = dt;
+            R()(Ge, "components", {
+                QImg: et.Z,
                 QIcon: T.Z,
                 QSelect: He.Z,
-                QBadge: at.Z,
+                QBadge: tt.Z,
                 QCheckbox: Ee.Z,
-                QToggle: lt.Z,
-                QBtnToggle: st.Z,
+                QToggle: at.Z,
+                QBtnToggle: lt.Z,
                 QInput: ze.Z,
-                QScrollArea: it.Z,
-                QTree: ot.Z,
-                QSeparator: nt.Z,
-                QUploader: dt.Z,
+                QScrollArea: st.Z,
+                QTree: it.Z,
+                QSeparator: ot.Z,
+                QUploader: nt.Z,
                 QBtn: De.Z
             });
-            const ht = (0, l.aZ)({
+            const ct = (0, l.aZ)({
                 name: "block",
                 components: {
-                    element: ct
+                    element: rt
                 },
                 data() {
                     return {
                         styleSize: w,
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
@@ -1711,15 +1724,15 @@
                             width: "8px",
                             opacity: .2
                         }
                     }
                 },
                 methods: {
                     log() {
-                        console.log(Object.keys(y).length, this.name, this.$el.getBoundingClientRect())
+                        console.log(Object.keys(b).length, this.name, this.$el.getBoundingClientRect())
                     },
                     geom() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
                         const t = e.querySelector(".q-scrollarea"),
                             a = e.getBoundingClientRect();
                         return {
                             el: e,
@@ -1729,15 +1742,15 @@
                             top: a.top,
                             scrollHeight: window.innerHeight,
                             scrollWidth: window.innerWidth
                         }
                     }
                 },
                 mounted() {
-                    y[this.name] = this, this.expanding && (b[this.fullname] = this)
+                    b[this.name] = this, this.expanding && (k[this.fullname] = this)
                 },
                 computed: {
                     name() {
                         return this.data.name
                     },
                     fullname() {
                         return `_scroll@${this.name}`
@@ -1759,55 +1772,55 @@
                     data: {
                         type: Object,
                         required: !0
                     }
                 },
                 watch: {
                     data(e) {
-                        g && console.log("data update", this.name), this.styleSize = w, y[this.name] = this, this.expanding && (b[this.fullname] = this)
+                        g && console.log("data update", this.name), this.styleSize = w, b[this.name] = this, this.expanding && (k[this.fullname] = this)
                     }
                 }
             });
-            var ut = a(151);
-            const pt = (0, U.Z)(ht, [
+            var ht = a(151);
+            const ut = (0, U.Z)(ct, [
                     ["render", ie]
                 ]),
-                gt = pt;
-            R()(ht, "components", {
-                QCard: ut.Z,
+                pt = ut;
+            R()(ct, "components", {
+                QCard: ht.Z,
                 QIcon: T.Z,
-                QScrollArea: it.Z
+                QScrollArea: st.Z
             });
-            const mt = (0, l.aZ)({
+            const gt = (0, l.aZ)({
                     name: "zone",
                     components: {
-                        block: gt
+                        block: pt
                     },
                     props: {
                         data: Object
                     },
                     updated(e) {
                         (0, l.Y3)((() => {
                             requestAnimationFrame((() => {
                                 requestAnimationFrame((() => {
                                     W()
                                 }))
                             }))
                         }))
                     }
                 }),
-                ft = (0, U.Z)(mt, [
+                mt = (0, U.Z)(gt, [
                     ["render", J]
                 ]),
-                wt = ft,
-                yt = {
+                ft = mt,
+                wt = {
                     class: "row q-gutter-sm row-md"
                 };
 
-            function bt(e, t, a, i, o, n) {
+            function yt(e, t, a, i, o, n) {
                 const d = (0, l.up)("block"),
                     r = (0, l.up)("q-item-label"),
                     c = (0, l.up)("q-space"),
                     h = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-card"),
                     p = (0, l.up)("q-dialog");
                 return (0, l.wg)(), (0, l.j4)(p, {
@@ -1823,40 +1836,40 @@
                             key: 0,
                             data: a.data
                         }, null, 8, ["data"])) : (0, l.kq)("", !0), (0, l.Wm)(r, {
                             class: "text-h6"
                         }, {
                             default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(a.data.text ? a.data.text : ""), 1)])),
                             _: 1
-                        }), (0, l._)("div", yt, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
+                        }), (0, l._)("div", wt, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
                             class: "col-md-3",
                             label: e,
                             color: a.buttons[0] == e ? "primary" : "secondary",
                             onClick: t => n.sendMessage(e)
                         }, null, 8, ["label", "color", "onClick"])))), 256))])])),
                         _: 1
                     }, 8, ["style"])])),
                     _: 1
                 }, 8, ["onHide"])
             }
-            const kt = {
+            const bt = {
                 props: {
                     data: Object,
                     buttons: Array
                 },
                 components: {
-                    block: gt
+                    block: pt
                 },
                 emits: ["ok", "hide"],
                 methods: {
                     show() {
                         this.$refs.dialog.show()
                     },
                     sendMessage(e) {
-                        this.data.internal || C([this.data["name"], e]), this.hide()
+                        this.data.internal || q([this.data["name"], e]), this.hide()
                     },
                     hide() {
                         this.$refs.dialog.hide()
                     },
                     onDialogHide() {
                         this.$emit("hide")
                     },
@@ -1864,30 +1877,30 @@
                         this.$emit("ok"), this.hide()
                     },
                     onCancelClick() {
                         this.hide()
                     }
                 }
             };
-            var vt = a(5926),
-                Ct = a(2025);
-            const xt = (0, U.Z)(kt, [
-                    ["render", bt]
+            var kt = a(5926),
+                vt = a(2025);
+            const xt = (0, U.Z)(bt, [
+                    ["render", yt]
                 ]),
-                qt = xt;
-            R()(kt, "components", {
-                QDialog: vt.Z,
-                QCard: ut.Z,
+                Ct = xt;
+            R()(bt, "components", {
+                QDialog: kt.Z,
+                QCard: ht.Z,
                 QItemLabel: N.Z,
-                QSpace: Ct.Z,
+                QSpace: vt.Z,
                 QBtn: De.Z
             });
-            var _t = !0;
-            let jt = null;
-            const St = (0, l.aZ)({
+            var qt = !0;
+            let _t = null;
+            const jt = (0, l.aZ)({
                 name: "MainLayout",
                 data() {
                     return {
                         leftDrawerOpen: !1,
                         menu: [],
                         tab: "",
                         localServer: !0,
@@ -1895,39 +1908,39 @@
                         screen: {
                             blocks: []
                         }
                     }
                 },
                 components: {
                     menubar: B,
-                    zone: wt
+                    zone: ft
                 },
                 created() {
-                    v(this)
+                    C(this)
                 },
                 unmounted() {
                     window.removeEventListener("resize", this.onResize)
                 },
                 methods: {
                     toggleLeftDrawer() {
                         this.leftDrawerOpen = !this.leftDrawerOpen
                     },
                     tabclick(e) {
-                        C(["root", e])
+                        q(["root", e])
                     },
                     onResize(e) {
-                        g && console.log("window has been resized", window.innerHeight, window.innerWidth), D()
+                        g && console.log("window has been resized", window.innerHeight, window.innerWidth), Q()
                     },
                     lens(e) {
                         let t = {
                                 title: "Photo lens",
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0,
-                                component: qt
+                                component: Ct
                             },
                             {
                                 height: a,
                                 ...l
                             } = e;
                         l.width = 750;
                         let s = {
@@ -1945,82 +1958,82 @@
                         let a = t,
                             l = {
                                 message: e,
                                 type: t,
                                 position: "top",
                                 icon: a
                             };
-                        "progress" == t ? null == jt ? (l = {
+                        "progress" == t ? null == _t ? (l = {
                             group: !1,
                             timeout: 0,
                             spinner: !0,
                             type: "info",
                             message: e || "Progress..",
                             position: "top",
                             color: "secondary"
-                        }, jt = this.$q.notify(l)) : null == e ? (jt(), jt = null) : (l = {
+                        }, _t = this.$q.notify(l)) : null == e ? (_t(), _t = null) : (l = {
                             caption: e
-                        }, jt(l)) : ("error" == t && l.type, this.$q.notify(l))
+                        }, _t(l)) : ("error" == t && l.type, this.$q.notify(l))
                     },
                     error(e) {
                         this.notify(e, "error")
                     },
                     info(e) {
                         this.notify(e, "info")
                     },
                     processMessage(e) {
-                        if (_t) _t = !1, this.menu = e[0].map((e => ({
+                        if (qt) qt = !1, this.menu = e[0].map((e => ({
                             name: e[0],
                             icon: e[1],
                             order: e[2]
-                        }))), Q(), this.screen = e[1], this.tab = this.screen.name, g && console.log("init loading..");
-                        else if ("screen" == e.type) A(), this.screen = e;
+                        }))), this.screen = e[1], this.tab = this.screen.name, g && console.log("init loading..");
+                        else if ("screen" == e.type) Z(), this.screen = e;
                         else if ("dialog" == e.type) {
                             let t = {
                                 title: e.name,
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0
                             };
-                            t.component = qt, t.componentProps = {
+                            t.component = Ct, t.componentProps = {
                                 data: e.content ? e.content : e,
                                 buttons: e.buttons
                             }, this.$q.dialog(t)
-                        } else if (e.hasOwnProperty("answer")) $(e);
+                        } else if (e.hasOwnProperty("answer")) z(e);
                         else {
-                            e.update && M(e);
+                            e.update && $(e);
                             let t = !1;
-                            for (let a of k) a in e && (this.notify(e[a], a), t = !0);
+                            for (let a of v) a in e && (this.notify(e[a], a), t = !0);
                             t || e.update || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
                         }
-                        jt && !e.progress && this.notify(null, "progress")
+                        _t && !e.progress && this.notify(null, "progress")
                     }
                 },
                 mounted() {
                     window.addEventListener("resize", this.onResize)
                 }
             });
-            var At = a(9214),
-                Zt = a(3812),
-                Mt = a(9570),
-                $t = a(7547),
-                zt = a(3269),
-                Dt = a(2652),
-                Ot = a(4379);
-            const Qt = (0, U.Z)(St, [
+            var St = a(9214),
+                At = a(3812),
+                Zt = a(9570),
+                Mt = a(7547),
+                $t = a(3269),
+                zt = a(2652),
+                Dt = a(4379);
+            const Ot = (0, U.Z)(jt, [
                     ["render", o]
                 ]),
-                Wt = Qt;
-            R()(St, "components", {
-                QLayout: At.Z,
-                QHeader: Zt.Z,
-                QToolbar: Mt.Z,
+                Qt = Ot;
+            R()(jt, "components", {
+                QLayout: St.Z,
+                QHeader: At.Z,
+                QToolbar: Zt.Z,
                 QBtn: De.Z,
                 QItemLabel: N.Z,
-                QTabs: $t.Z,
-                QTab: zt.Z,
-                QPageContainer: Dt.Z,
-                QPage: Ot.Z
+                QTabs: Mt.Z,
+                QTab: $t.Z,
+                QPageContainer: zt.Z,
+                QPage: Dt.Z
             })
         }
     }
 ]);
```

### Comparing `unigui-1.4.2/unigui/web/index.html` & `unigui-1.4.3/unigui/web/index.html`

 * *Files 12% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.c0de6c67.js></script><script defer src=js/app.bfd9bd6e.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.c0de6c67.js></script><script defer src=js/app.73e4276f.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.4.2/LICENSE` & `unigui-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/setup.py` & `unigui-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.4.2',      
+      version='1.4.3',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal app browser',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.4.2/PKG-INFO` & `unigui-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.4.2
+Version: 1.4.3
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.4.2/README.md` & `unigui-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `unigui-1.4.2/unigui.egg-info/PKG-INFO` & `unigui-1.4.3/unigui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.4.2
+Version: 1.4.3
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.4.2/unigui.egg-info/SOURCES.txt` & `unigui-1.4.3/unigui.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/365.b8547d97.css
+unigui/web/css/748.d94da9c0.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.49a52e8f.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -28,11 +28,11 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.b4cc3ffe.js
-unigui/web/js/365.3c494fbf.js
 unigui/web/js/430.4be6e8a8.js
-unigui/web/js/app.bfd9bd6e.js
+unigui/web/js/748.67c1fce8.js
+unigui/web/js/app.73e4276f.js
 unigui/web/js/vendor.c0de6c67.js
```

