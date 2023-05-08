# Comparing `tmp/nbsite-0.8.0rc8.tar.gz` & `tmp/nbsite-0.8.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nbsite-0.8.0rc8.tar", last modified: Tue Feb 28 11:08:03 2023, max compression
+gzip compressed data, was "dist/nbsite-0.8.0rc9.tar", last modified: Thu Mar  9 16:55:32 2023, max compression
```

## Comparing `nbsite-0.8.0rc8.tar` & `nbsite-0.8.0rc9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/nbsite/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/nbsite/.version
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/nbsite/_shared_static/
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/_shared_static/holoviz-icon-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/_shared_static/mystnb.css
--rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/_shared_static/nbsite.css
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/_shared_static/nbsite.js
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/_shared_static/require.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/nbsite/_shared_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/_shared_templates/copyright-last-updated.html
--rw-r--r--   0 runner    (1001) docker     (123)    12930 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/nbsite/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/gallery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23623 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/gallery/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/gallery/thumbnailer.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/ipystartup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18035 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/nbbuild.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/paramdoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/nbsite/pyodide/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/pyodide/ServiceHandler.js
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/pyodide/ServiceWorker.js
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/pyodide/WebWorker.js
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/pyodide/WorkerHandler.js
--rw-r--r--   0 runner    (1001) docker     (123)    13951 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/pyodide/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/nbsite/pyodide/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/pyodide/_static/run_cell.js
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/pyodide/_static/runbutton.css
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/pyodide/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/shared_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/nbsite/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/nbsite/templates/basic/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/templates/basic/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/templates/basic/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/templates/basic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/nbsite/templates/holoviz/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/templates/holoviz/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/templates/holoviz/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/templates/holoviz/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/templates/holoviz/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/nbsite/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18588 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/tests/test_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/nbsite/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/nbsite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/nbsite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/nbsite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/nbsite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/nbsite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/nbsite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/nbsite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/scripts/nbsite_cleandisthtml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5851 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/scripts/nbsite_fix_links.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/scripts/nbsite_from_tmplate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11127 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/scripts/nbsite_generate_modules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/scripts/nbsite_nbpagebuild.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-28 11:08:03.000000 nbsite-0.8.0rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-02-28 11:07:09.000000 nbsite-0.8.0rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/.version
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/_shared_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/_shared_static/holoviz-icon-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/_shared_static/mystnb.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/_shared_static/nbsite.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/_shared_static/nbsite.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/_shared_static/require.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/_shared_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/_shared_templates/copyright-last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12930 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/gallery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23623 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/gallery/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/gallery/thumbnailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/ipystartup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18035 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/nbbuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/paramdoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/pyodide/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/pyodide/ServiceHandler.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/pyodide/ServiceWorker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/pyodide/WebWorker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/pyodide/WorkerHandler.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14119 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/pyodide/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/pyodide/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/pyodide/_static/run_cell.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/pyodide/_static/runbutton.css
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/pyodide/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/shared_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/templates/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/templates/basic/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/templates/basic/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/templates/basic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/templates/holoviz/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/templates/holoviz/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/templates/holoviz/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/templates/holoviz/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/templates/holoviz/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18588 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/tests/test_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/nbsite/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/nbsite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/scripts/nbsite_cleandisthtml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5851 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/scripts/nbsite_fix_links.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/scripts/nbsite_from_tmplate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11127 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/scripts/nbsite_generate_modules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/scripts/nbsite_nbpagebuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-09 16:55:32.000000 nbsite-0.8.0rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-03-09 16:54:37.000000 nbsite-0.8.0rc9/setup.py
```

### Comparing `nbsite-0.8.0rc8/LICENSE.txt` & `nbsite-0.8.0rc9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/PKG-INFO` & `nbsite-0.8.0rc9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbsite
-Version: 0.8.0rc8
+Version: 0.8.0rc9
 Summary: Build a tested, sphinx-based website from notebooks.
 Home-page: https://nbsite.pyviz.org/
 Author: PyViz developers
 Author-email: developers@pyviz.org
 Maintainer: PyViz developers
 Maintainer-email: developers@pyviz.org
 License: BSD-3
```

### Comparing `nbsite-0.8.0rc8/README.md` & `nbsite-0.8.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/__main__.py` & `nbsite-0.8.0rc9/nbsite/__main__.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/_shared_static/holoviz-icon-white.svg` & `nbsite-0.8.0rc9/nbsite/_shared_static/holoviz-icon-white.svg`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/_shared_static/mystnb.css` & `nbsite-0.8.0rc9/nbsite/_shared_static/mystnb.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/_shared_static/nbsite.css` & `nbsite-0.8.0rc9/nbsite/_shared_static/nbsite.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/_shared_static/nbsite.js` & `nbsite-0.8.0rc9/nbsite/_shared_static/nbsite.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/_shared_static/require.js` & `nbsite-0.8.0rc9/nbsite/_shared_static/require.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/_shared_templates/copyright-last-updated.html` & `nbsite-0.8.0rc9/nbsite/_shared_templates/copyright-last-updated.html`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/cmd.py` & `nbsite-0.8.0rc9/nbsite/cmd.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/gallery/gen.py` & `nbsite-0.8.0rc9/nbsite/gallery/gen.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/gallery/thumbnailer.py` & `nbsite-0.8.0rc9/nbsite/gallery/thumbnailer.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/nbbuild.py` & `nbsite-0.8.0rc9/nbsite/nbbuild.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/paramdoc.py` & `nbsite-0.8.0rc9/nbsite/paramdoc.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/pyodide/ServiceWorker.js` & `nbsite-0.8.0rc9/nbsite/pyodide/ServiceWorker.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/pyodide/WebWorker.js` & `nbsite-0.8.0rc9/nbsite/pyodide/WebWorker.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/pyodide/WorkerHandler.js` & `nbsite-0.8.0rc9/nbsite/pyodide/WorkerHandler.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/pyodide/__init__.py` & `nbsite-0.8.0rc9/nbsite/pyodide/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,24 +39,30 @@
 
 WEB_WORKER_TEMPLATE = _env.get_template('WebWorker.js')
 WORKER_HANDLER_TEMPLATE = _env.get_template('WorkerHandler.js')
 SERVICE_WORKER_TEMPLATE = _env.get_template('ServiceWorker.js')
 SERVICE_HANDLER_TEMPLATE = _env.get_template('ServiceHandler.js')
 WEB_MANIFEST_TEMPLATE = _env.get_template('site.webmanifest')
 
+bokeh_version = Version(BOKEH_VERSION)
+if bokeh_version.is_devrelease or bokeh_version.is_prerelease:
+    bk_prefix = 'dev'
+else:
+    bk_prefix = 'release'
+
 DEFAULT_PYODIDE_CONF = {
     'PYODIDE_URL': 'https://cdn.jsdelivr.net/pyodide/v0.21.3/full/pyodide.js',
     'autodetect_deps': True,
     'enable_pwa': True,
     'requirements': ['panel', 'pandas'],
     'precache': [],
     'scripts': [
-        f'https://cdn.bokeh.org/bokeh/release/bokeh-{BOKEH_VERSION}.min.js',
-        f'https://cdn.bokeh.org/bokeh/release/bokeh-widgets-{BOKEH_VERSION}.min.js',
-        f'https://cdn.bokeh.org/bokeh/release/bokeh-tables-{BOKEH_VERSION}.min.js',
+        f'https://cdn.bokeh.org/bokeh/{bk_prefix}/bokeh-{BOKEH_VERSION}.min.js',
+        f'https://cdn.bokeh.org/bokeh/{bk_prefix}/bokeh-widgets-{BOKEH_VERSION}.min.js',
+        f'https://cdn.bokeh.org/bokeh/{bk_prefix}/bokeh-tables-{BOKEH_VERSION}.min.js',
         f'{CDN_DIST}panel.min.js'
     ],
     'extra_css': [],
     'cache_patterns': [
         CDN_DIST,
         'https://cdn.bokeh.org/bokeh/',
         'https://cdn.jsdelivr.net/pyodide/',
@@ -154,15 +160,14 @@
     _client = None
     _listener = None
     _conn = None
     _send_address = ('localhost', 33355)
     _rcv_address = ('localhost', 33356)
     _password = b'pyodide'
 
-
     @classmethod
     def _execution_process(cls, pipe):
         """
         Process execution loop to run in separate process that is used
         to evaluate code.
         """
         while True:
```

### Comparing `nbsite-0.8.0rc8/nbsite/pyodide/_static/run_cell.js` & `nbsite-0.8.0rc9/nbsite/pyodide/_static/run_cell.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/pyodide/_static/runbutton.css` & `nbsite-0.8.0rc9/nbsite/pyodide/_static/runbutton.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/pyodide/site.webmanifest` & `nbsite-0.8.0rc9/nbsite/pyodide/site.webmanifest`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/shared_conf.py` & `nbsite-0.8.0rc9/nbsite/shared_conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/templates/basic/conf.py` & `nbsite-0.8.0rc9/nbsite/templates/basic/conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/templates/holoviz/conf.py` & `nbsite-0.8.0rc9/nbsite/templates/holoviz/conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/tests/test_cmd.py` & `nbsite-0.8.0rc9/nbsite/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/tests/test_util.py` & `nbsite-0.8.0rc9/nbsite/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite/util.py` & `nbsite-0.8.0rc9/nbsite/util.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/nbsite.egg-info/PKG-INFO` & `nbsite-0.8.0rc9/nbsite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbsite
-Version: 0.8.0rc8
+Version: 0.8.0rc9
 Summary: Build a tested, sphinx-based website from notebooks.
 Home-page: https://nbsite.pyviz.org/
 Author: PyViz developers
 Author-email: developers@pyviz.org
 Maintainer: PyViz developers
 Maintainer-email: developers@pyviz.org
 License: BSD-3
```

### Comparing `nbsite-0.8.0rc8/nbsite.egg-info/SOURCES.txt` & `nbsite-0.8.0rc9/nbsite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/scripts/nbsite_cleandisthtml.py` & `nbsite-0.8.0rc9/scripts/nbsite_cleandisthtml.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/scripts/nbsite_fix_links.py` & `nbsite-0.8.0rc9/scripts/nbsite_fix_links.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/scripts/nbsite_generate_modules.py` & `nbsite-0.8.0rc9/scripts/nbsite_generate_modules.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/scripts/nbsite_nbpagebuild.py` & `nbsite-0.8.0rc9/scripts/nbsite_nbpagebuild.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.0rc8/setup.py` & `nbsite-0.8.0rc9/setup.py`

 * *Files identical despite different names*

