# Comparing `tmp/madblog-0.2.8.tar.gz` & `tmp/madblog-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madblog-0.2.8.tar", last modified: Thu Aug  4 01:43:55 2022, max compression
+gzip compressed data, was "madblog-0.2.9.tar", last modified: Wed Aug 10 14:37:46 2022, max compression
```

## Comparing `madblog-0.2.8.tar` & `madblog-0.2.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 blacklight  (1001) blacklight  (1000)        0 2022-08-04 01:43:55.108545 madblog-0.2.8/
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)     1081 2022-01-10 18:12:11.000000 madblog-0.2.8/LICENSE.txt
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)      157 2022-01-10 23:39:04.000000 madblog-0.2.8/MANIFEST.in
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)     3834 2022-08-04 01:43:55.108545 madblog-0.2.8/PKG-INFO
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)     3334 2022-06-13 22:32:06.000000 madblog-0.2.8/README.md
-drwxr-xr-x   0 blacklight  (1001) blacklight  (1000)        0 2022-08-04 01:43:55.101878 madblog-0.2.8/madblog/
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)       22 2022-08-03 21:42:57.000000 madblog-0.2.8/madblog/__init__.py
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)       59 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/__main__.py
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)     1394 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/_sorters.py
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)     6074 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/app.py
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)     1504 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/cli.py
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)     1449 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/config.py
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)     7348 2022-08-03 21:42:29.000000 madblog-0.2.8/madblog/latex.py
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)     4162 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/routes.py
-drwxr-xr-x   0 blacklight  (1001) blacklight  (1000)        0 2022-08-04 01:43:55.098545 madblog-0.2.8/madblog/static/
-drwxr-xr-x   0 blacklight  (1001) blacklight  (1000)        0 2022-08-04 01:43:55.105211 madblog-0.2.8/madblog/static/css/
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)     1008 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/static/css/blog.css
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)     4880 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/static/css/code.css
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)     2072 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/static/css/common.css
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)     1831 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/static/css/home.css
-drwxr-xr-x   0 blacklight  (1001) blacklight  (1000)        0 2022-08-04 01:43:55.108545 madblog-0.2.8/madblog/static/fonts/
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)   154584 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/static/fonts/Poppins.ttf
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)   287372 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/static/fonts/fira-sans-200.ttf
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)   288852 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/static/fonts/fira-sans-300.ttf
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)      318 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/static/fonts/fira-sans.css
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)      151 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/static/fonts/poppins.css
-drwxr-xr-x   0 blacklight  (1001) blacklight  (1000)        0 2022-08-04 01:43:55.108545 madblog-0.2.8/madblog/static/img/
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)     2238 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/static/img/favicon.ico
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)     5937 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/static/img/icon.png
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)     1772 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/static/img/rss.png
-drwxr-xr-x   0 blacklight  (1001) blacklight  (1000)        0 2022-08-04 01:43:55.108545 madblog-0.2.8/madblog/templates/
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)     1398 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/templates/article.html
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)     1381 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/templates/common-head.html
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)       16 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/templates/common-tail.html
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)      110 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/templates/footer.html
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)     1791 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/templates/index.html
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)      427 2022-08-02 23:13:09.000000 madblog-0.2.8/madblog/uwsgi.py
-drwxr-xr-x   0 blacklight  (1001) blacklight  (1000)        0 2022-08-04 01:43:55.101878 madblog-0.2.8/madblog.egg-info/
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)     3834 2022-08-04 01:43:54.000000 madblog-0.2.8/madblog.egg-info/PKG-INFO
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)      939 2022-08-04 01:43:55.000000 madblog-0.2.8/madblog.egg-info/SOURCES.txt
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)        1 2022-08-04 01:43:54.000000 madblog-0.2.8/madblog.egg-info/dependency_links.txt
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)       44 2022-08-04 01:43:54.000000 madblog-0.2.8/madblog.egg-info/entry_points.txt
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)       31 2022-08-04 01:43:54.000000 madblog-0.2.8/madblog.egg-info/requires.txt
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)        8 2022-08-04 01:43:54.000000 madblog-0.2.8/madblog.egg-info/top_level.txt
--rw-r--r--   0 blacklight  (1001) blacklight  (1000)      143 2022-08-04 01:43:55.111878 madblog-0.2.8/setup.cfg
--rwxr-xr-x   0 blacklight  (1001) blacklight  (1000)     1015 2022-08-03 21:42:57.000000 madblog-0.2.8/setup.py
+drwxr-xr-x   0 blacklight  (1000) blacklight  (1000)        0 2022-08-10 14:37:46.572317 madblog-0.2.9/
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)     1081 2022-08-03 22:40:58.000000 madblog-0.2.9/LICENSE.txt
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)      157 2022-08-03 22:40:58.000000 madblog-0.2.9/MANIFEST.in
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)     3834 2022-08-10 14:37:46.572317 madblog-0.2.9/PKG-INFO
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)     3334 2022-08-03 22:40:58.000000 madblog-0.2.9/README.md
+drwxr-xr-x   0 blacklight  (1000) blacklight  (1000)        0 2022-08-10 14:37:46.568983 madblog-0.2.9/madblog/
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)       22 2022-08-10 14:36:11.000000 madblog-0.2.9/madblog/__init__.py
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)       59 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/__main__.py
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)     1394 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/_sorters.py
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)     6074 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/app.py
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)     1504 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/cli.py
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)     1449 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/config.py
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)     7348 2022-08-04 00:27:12.000000 madblog-0.2.9/madblog/latex.py
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)     4162 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/routes.py
+drwxr-xr-x   0 blacklight  (1000) blacklight  (1000)        0 2022-08-10 14:37:46.568983 madblog-0.2.9/madblog/static/
+drwxr-xr-x   0 blacklight  (1000) blacklight  (1000)        0 2022-08-10 14:37:46.568983 madblog-0.2.9/madblog/static/css/
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)      915 2022-08-10 14:09:01.000000 madblog-0.2.9/madblog/static/css/blog.css
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)     4880 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/static/css/code.css
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)     2093 2022-08-10 14:09:30.000000 madblog-0.2.9/madblog/static/css/common.css
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)     1831 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/static/css/home.css
+drwxr-xr-x   0 blacklight  (1000) blacklight  (1000)        0 2022-08-10 14:37:46.572317 madblog-0.2.9/madblog/static/fonts/
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)   154584 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/static/fonts/Poppins.ttf
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)   287372 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/static/fonts/fira-sans-200.ttf
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)   288852 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/static/fonts/fira-sans-300.ttf
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)      318 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/static/fonts/fira-sans.css
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)      151 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/static/fonts/poppins.css
+drwxr-xr-x   0 blacklight  (1000) blacklight  (1000)        0 2022-08-10 14:37:46.572317 madblog-0.2.9/madblog/static/img/
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)     2238 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/static/img/favicon.ico
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)     5937 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/static/img/icon.png
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)     1772 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/static/img/rss.png
+drwxr-xr-x   0 blacklight  (1000) blacklight  (1000)        0 2022-08-10 14:37:46.572317 madblog-0.2.9/madblog/templates/
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)     1398 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/templates/article.html
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)     1381 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/templates/common-head.html
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)       16 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/templates/common-tail.html
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)      110 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/templates/footer.html
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)     1791 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/templates/index.html
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)      427 2022-08-03 22:40:58.000000 madblog-0.2.9/madblog/uwsgi.py
+drwxr-xr-x   0 blacklight  (1000) blacklight  (1000)        0 2022-08-10 14:37:46.568983 madblog-0.2.9/madblog.egg-info/
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)     3834 2022-08-10 14:37:46.000000 madblog-0.2.9/madblog.egg-info/PKG-INFO
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)      939 2022-08-10 14:37:46.000000 madblog-0.2.9/madblog.egg-info/SOURCES.txt
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)        1 2022-08-10 14:37:46.000000 madblog-0.2.9/madblog.egg-info/dependency_links.txt
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)       44 2022-08-10 14:37:46.000000 madblog-0.2.9/madblog.egg-info/entry_points.txt
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)       31 2022-08-10 14:37:46.000000 madblog-0.2.9/madblog.egg-info/requires.txt
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)        8 2022-08-10 14:37:46.000000 madblog-0.2.9/madblog.egg-info/top_level.txt
+-rw-r--r--   0 blacklight  (1000) blacklight  (1000)      143 2022-08-10 14:37:46.572317 madblog-0.2.9/setup.cfg
+-rwxr-xr-x   0 blacklight  (1000) blacklight  (1000)     1015 2022-08-10 14:36:11.000000 madblog-0.2.9/setup.py
```

### Comparing `madblog-0.2.8/LICENSE.txt` & `madblog-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `madblog-0.2.8/PKG-INFO` & `madblog-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: madblog
-Version: 0.2.8
+Version: 0.2.9
 Summary: A minimal platform for Markdown-based blogs
 Home-page: https://git.platypush.tech/blacklight/madblog
 Author: Fabio Manganiello
 Author-email: info@fabiomanganiello.com
 License: MIT
 Keywords: blog markdown
 Platform: UNKNOWN
```

### Comparing `madblog-0.2.8/README.md` & `madblog-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `madblog-0.2.8/madblog/_sorters.py` & `madblog-0.2.9/madblog/_sorters.py`

 * *Files identical despite different names*

### Comparing `madblog-0.2.8/madblog/app.py` & `madblog-0.2.9/madblog/app.py`

 * *Files identical despite different names*

### Comparing `madblog-0.2.8/madblog/cli.py` & `madblog-0.2.9/madblog/cli.py`

 * *Files identical despite different names*

### Comparing `madblog-0.2.8/madblog/config.py` & `madblog-0.2.9/madblog/config.py`

 * *Files identical despite different names*

### Comparing `madblog-0.2.8/madblog/latex.py` & `madblog-0.2.9/madblog/latex.py`

 * *Files identical despite different names*

### Comparing `madblog-0.2.8/madblog/routes.py` & `madblog-0.2.9/madblog/routes.py`

 * *Files identical despite different names*

### Comparing `madblog-0.2.8/madblog/static/css/blog.css` & `madblog-0.2.9/madblog/static/css/blog.css`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,14 @@
   display: flex;
   flex-direction: column;
   line-height: 1.5em;
 }
 
 main .content p,
 main .content ul {
-  font-family: Avenir, Palatino, charter, Georgia, Cambria, "Times New Roman", Times, serif;
   text-align: justify;
   overflow-wrap: break-word;
   word-break: break-word;
 }
 
 main .content code, .codehilite {
   font-size: .85em;
```

### Comparing `madblog-0.2.8/madblog/static/css/code.css` & `madblog-0.2.9/madblog/static/css/code.css`

 * *Files identical despite different names*

### Comparing `madblog-0.2.8/madblog/static/css/common.css` & `madblog-0.2.9/madblog/static/css/common.css`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 html {
   height: -webkit-fill-available;
   height: -moz-available;
   font-size: 20px;
-  font-family: BlinkMacSystemFont, -apple-system, Segoe UI, Roboto, Oxygen, Ubuntu, Cantarell, Fira Sans, Droid Sans, Helvetica Neue, Helvetica, Arial, sans-serif;
+  font-family: BlinkMacSystemFont, -apple-system, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Open Sans", "Droid Sans", "Helvetica Neue", Helvetica, Arial, sans-serif;
   font-weight: 400;
   text-rendering: optimizeLegibility;
 }
 
 body {
   margin: 0;
   height: 100vh;
```

### Comparing `madblog-0.2.8/madblog/static/css/home.css` & `madblog-0.2.9/madblog/static/css/home.css`

 * *Files identical despite different names*

### Comparing `madblog-0.2.8/madblog/static/fonts/Poppins.ttf` & `madblog-0.2.9/madblog/static/fonts/Poppins.ttf`

 * *Files identical despite different names*

### Comparing `madblog-0.2.8/madblog/static/fonts/fira-sans-200.ttf` & `madblog-0.2.9/madblog/static/fonts/fira-sans-200.ttf`

 * *Files identical despite different names*

### Comparing `madblog-0.2.8/madblog/static/fonts/fira-sans-300.ttf` & `madblog-0.2.9/madblog/static/fonts/fira-sans-300.ttf`

 * *Files identical despite different names*

### Comparing `madblog-0.2.8/madblog/static/img/favicon.ico` & `madblog-0.2.9/madblog/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `madblog-0.2.8/madblog/static/img/icon.png` & `madblog-0.2.9/madblog/static/img/icon.png`

 * *Files identical despite different names*

### Comparing `madblog-0.2.8/madblog/static/img/rss.png` & `madblog-0.2.9/madblog/static/img/rss.png`

 * *Files identical despite different names*

### Comparing `madblog-0.2.8/madblog/templates/article.html` & `madblog-0.2.9/madblog/templates/article.html`

 * *Files identical despite different names*

### Comparing `madblog-0.2.8/madblog/templates/common-head.html` & `madblog-0.2.9/madblog/templates/common-head.html`

 * *Files identical despite different names*

### Comparing `madblog-0.2.8/madblog/templates/index.html` & `madblog-0.2.9/madblog/templates/index.html`

 * *Files identical despite different names*

### Comparing `madblog-0.2.8/madblog.egg-info/PKG-INFO` & `madblog-0.2.9/madblog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: madblog
-Version: 0.2.8
+Version: 0.2.9
 Summary: A minimal platform for Markdown-based blogs
 Home-page: https://git.platypush.tech/blacklight/madblog
 Author: Fabio Manganiello
 Author-email: info@fabiomanganiello.com
 License: MIT
 Keywords: blog markdown
 Platform: UNKNOWN
```

### Comparing `madblog-0.2.8/madblog.egg-info/SOURCES.txt` & `madblog-0.2.9/madblog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `madblog-0.2.8/setup.py` & `madblog-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def readfile(file):
     with open(file, 'r') as f:
         return f.read()
 
 
 setup(
     name='madblog',
-    version='0.2.8',
+    version='0.2.9',
     author='Fabio Manganiello',
     author_email='info@fabiomanganiello.com',
     description='A minimal platform for Markdown-based blogs',
     license='MIT',
     python_requires='>= 3.8',
     keywords='blog markdown',
     url='https://git.platypush.tech/blacklight/madblog',
```

