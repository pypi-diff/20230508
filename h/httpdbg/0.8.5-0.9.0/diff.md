# Comparing `tmp/httpdbg-0.8.5.tar.gz` & `tmp/httpdbg-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpdbg-0.8.5.tar", last modified: Wed Apr  5 21:05:34 2023, max compression
+gzip compressed data, was "httpdbg-0.9.0.tar", last modified: Mon Apr 10 17:48:31 2023, max compression
```

## Comparing `httpdbg-0.8.5.tar` & `httpdbg-0.9.0.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 21:05:34.041606 httpdbg-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-05 21:05:22.000000 httpdbg-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-05 21:05:34.041606 httpdbg-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-05 21:05:22.000000 httpdbg-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 21:05:34.033606 httpdbg-0.8.5/httpdbg/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 21:05:34.033606 httpdbg-0.8.5/httpdbg/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/hooks/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/hooks/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/hooks/httpx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/hooks/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    14223 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/hooks/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/hooks/urllib3.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/hooks/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/initiator.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/mode_console.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/mode_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/mode_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 21:05:34.037606 httpdbg-0.8.5/httpdbg/webapp/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/preview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 21:05:34.037606 httpdbg-0.8.5/httpdbg/webapp/static/
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/api.js
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/column.css
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/configuration.js
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/detail.css
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/filter.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 21:05:34.041606 httpdbg-0.8.5/httpdbg/webapp/static/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/icons/download-install-line-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/icons/engine-gears-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/icons/files-papers-outline-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/icons/filter-outline-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/icons/information-mark-circle-outline-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/icons/math-multiplication-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/icons/push-pin-green-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/icons/recycle-bin-line-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/icons/wait-sandclock-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/index.htm
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/main.js
--rw-r--r--   0 runner    (1001) docker     (123)    11186 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/mustache.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/render.js
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/style.css
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-05 21:05:22.000000 httpdbg-0.8.5/httpdbg/webapp/static/table.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 21:05:34.033606 httpdbg-0.8.5/httpdbg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-05 21:05:34.000000 httpdbg-0.8.5/httpdbg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-05 21:05:34.000000 httpdbg-0.8.5/httpdbg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 21:05:34.000000 httpdbg-0.8.5/httpdbg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-05 21:05:34.000000 httpdbg-0.8.5/httpdbg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-05 21:05:34.000000 httpdbg-0.8.5/httpdbg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-05 21:05:22.000000 httpdbg-0.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-05 21:05:34.045606 httpdbg-0.8.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 21:05:34.041606 httpdbg-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-04-05 21:05:22.000000 httpdbg-0.8.5/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-05 21:05:22.000000 httpdbg-0.8.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-05 21:05:22.000000 httpdbg-0.8.5/tests/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-04-05 21:05:22.000000 httpdbg-0.8.5/tests/test_hook_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14552 2023-04-05 21:05:22.000000 httpdbg-0.8.5/tests/test_hook_httpx.py
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-04-05 21:05:22.000000 httpdbg-0.8.5/tests/test_hook_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-05 21:05:22.000000 httpdbg-0.8.5/tests/test_hook_urllib3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-05 21:05:22.000000 httpdbg-0.8.5/tests/test_mode_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-05 21:05:22.000000 httpdbg-0.8.5/tests/test_mode_module_pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-04-05 21:05:22.000000 httpdbg-0.8.5/tests/test_mode_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-05 21:05:22.000000 httpdbg-0.8.5/tests/test_preview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:48:31.853106 httpdbg-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-10 17:48:20.000000 httpdbg-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-10 17:48:31.853106 httpdbg-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-10 17:48:20.000000 httpdbg-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:48:31.841105 httpdbg-0.9.0/httpdbg/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:48:31.845105 httpdbg-0.9.0/httpdbg/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/hooks/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/hooks/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/hooks/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/hooks/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/hooks/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/hooks/urllib3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/hooks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/initiator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/mode_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/mode_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/mode_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:48:31.845105 httpdbg-0.9.0/httpdbg/webapp/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/preview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:48:31.849105 httpdbg-0.9.0/httpdbg/webapp/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/column.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/configuration.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/detail.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/filter.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:48:31.849105 httpdbg-0.9.0/httpdbg/webapp/static/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/icons/download-install-line-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/icons/engine-gears-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/icons/files-papers-outline-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/icons/filter-outline-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/icons/information-mark-circle-outline-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/icons/math-multiplication-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/icons/push-pin-green-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/icons/recycle-bin-line-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/icons/wait-sandclock-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17153 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/index.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11186 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/mustache.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/render.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-10 17:48:20.000000 httpdbg-0.9.0/httpdbg/webapp/static/table.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:48:31.841105 httpdbg-0.9.0/httpdbg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-10 17:48:31.000000 httpdbg-0.9.0/httpdbg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-10 17:48:31.000000 httpdbg-0.9.0/httpdbg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:48:31.000000 httpdbg-0.9.0/httpdbg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-10 17:48:31.000000 httpdbg-0.9.0/httpdbg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 17:48:31.000000 httpdbg-0.9.0/httpdbg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-10 17:48:20.000000 httpdbg-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-10 17:48:31.853106 httpdbg-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:48:31.853106 httpdbg-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-04-10 17:48:20.000000 httpdbg-0.9.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-10 17:48:20.000000 httpdbg-0.9.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-10 17:48:20.000000 httpdbg-0.9.0/tests/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-04-10 17:48:20.000000 httpdbg-0.9.0/tests/test_hook_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14691 2023-04-10 17:48:20.000000 httpdbg-0.9.0/tests/test_hook_httpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8158 2023-04-10 17:48:20.000000 httpdbg-0.9.0/tests/test_hook_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-04-10 17:48:20.000000 httpdbg-0.9.0/tests/test_hook_urllib3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-10 17:48:20.000000 httpdbg-0.9.0/tests/test_initiator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-10 17:48:20.000000 httpdbg-0.9.0/tests/test_mode_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-10 17:48:20.000000 httpdbg-0.9.0/tests/test_mode_module_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-10 17:48:20.000000 httpdbg-0.9.0/tests/test_mode_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-10 17:48:20.000000 httpdbg-0.9.0/tests/test_preview.py
```

### Comparing `httpdbg-0.8.5/LICENSE` & `httpdbg-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/PKG-INFO` & `httpdbg-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpdbg
-Version: 0.8.5
+Version: 0.9.0
 Summary: A very simple tool to debug HTTP(S) client requests
 Author-email: cle-b <cle@tictac.pm>
 License: Apache-2.0
 Project-URL: repository, https://github.com/cle-b/httpdbg
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `httpdbg-0.8.5/README.md` & `httpdbg-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/__main__.py` & `httpdbg-0.9.0/httpdbg/__main__.py`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/args.py` & `httpdbg-0.9.0/httpdbg/args.py`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/hooks/all.py` & `httpdbg-0.9.0/httpdbg/hooks/all.py`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/hooks/socket.py` & `httpdbg-0.9.0/httpdbg/hooks/socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from contextlib import contextmanager
 import socket
 import ssl
 
 from httpdbg.hooks.utils import getcallargs
 from httpdbg.hooks.utils import decorate
 from httpdbg.hooks.utils import undecorate
-from httpdbg.initiator import get_initiator
 from httpdbg.records import HTTPRecord
 from httpdbg.utils import logger
 
 
 def set_hook_for_socket_init(records, method):
     def hook(self, *args, **kwargs):
         records.del_socket_data(self)
@@ -32,15 +31,15 @@
         try:
             r = method(self, address)
         except Exception as ex:
             if not isinstance(
                 ex, (BlockingIOError, OSError)
             ):  # BlockingIOError for async, OSError for ipv6
                 record = HTTPRecord()
-                record.initiator = get_initiator(records._initiators)
+                record.initiator = records.get_initiator()
 
                 record.exception = ex
 
                 records.requests[record.id] = record
 
             raise
 
@@ -52,15 +51,15 @@
 def set_hook_for_ssl_wrap_socket(records, method):
     def hook(sock, *args, **kwargs):
         try:
             sslsocket = method(sock, *args, **kwargs)
         except Exception as ex:
             record = HTTPRecord()
 
-            record.initiator = get_initiator(records._initiators)
+            record.initiator = records.get_initiator()
             record.exception = ex
 
             records.requests[record.id] = record
 
             raise
 
         logger.info(
@@ -79,15 +78,15 @@
 def set_hook_for_sslcontext_wrap_socket(records, method):
     def hook(self, sock, *args, **kwargs):
         try:
             sslsocket = method(self, sock, *args, **kwargs)
         except Exception as ex:
             record = HTTPRecord()
 
-            record.initiator = get_initiator(records._initiators)
+            record.initiator = records.get_initiator()
             record.exception = ex
 
             records.requests[record.id] = record
 
             raise
 
         logger.info(
@@ -105,15 +104,15 @@
 
 def set_hook_for_socket_wrap_bio(records, method):
     def hook(self, *args, **kwargs):
         try:
             sslobject = method(self, *args, **kwargs)
         except Exception as ex:
             record = HTTPRecord()
-            record.initiator = get_initiator(records._initiators)
+            record.initiator = records.get_initiator()
 
             record.exception = ex
 
             records.requests[record.id] = record
 
             raise
 
@@ -190,15 +189,15 @@
                 socketdata.record.request.rawdata += bytes
             else:
                 socketdata.rawdata += bytes
                 http_detected = socketdata.http_detected()
                 if http_detected:
                     logger.info("SENDALL - http detected")
                     socketdata.record = HTTPRecord()
-                    socketdata.record.initiator = get_initiator(records._initiators)
+                    socketdata.record.initiator = records.get_initiator()
                     socketdata.record.address = socketdata.address
                     socketdata.record.ssl = socketdata.ssl
                     socketdata.record.request.rawdata = socketdata.rawdata
                     records.requests[socketdata.record.id] = socketdata.record
                 elif http_detected is False:  # if None, there is nothing to do
                     records._sockets[id(self)] = None
 
@@ -231,15 +230,15 @@
             if socketdata.record:
                 socketdata.record.request.rawdata += bytes[:size]
             else:
                 socketdata.rawdata += bytes[:size]
                 http_detected = socketdata.http_detected()
                 if http_detected:
                     socketdata.record = HTTPRecord()
-                    socketdata.record.initiator = get_initiator(records._initiators)
+                    socketdata.record.initiator = records.get_initiator()
                     socketdata.record.address = socketdata.address
                     socketdata.record.ssl = socketdata.ssl
                     socketdata.record.request.rawdata = socketdata.rawdata
                     records.requests[socketdata.record.id] = socketdata.record
                 elif http_detected is False:  # if None, there is nothing to do
                     records._sockets[id(self)] = None
         return size
@@ -288,15 +287,15 @@
             if socketdata.record:
                 socketdata.record.request.rawdata += bytes(buf[:size])
             else:
                 socketdata.rawdata += bytes(buf[:size])
                 http_detected = socketdata.http_detected()
                 if http_detected:
                     socketdata.record = HTTPRecord()
-                    socketdata.record.initiator = get_initiator(records._initiators)
+                    socketdata.record.initiator = records.get_initiator()
                     socketdata.record.address = socketdata.address
                     socketdata.record.ssl = socketdata.ssl
                     socketdata.record.request.rawdata = socketdata.rawdata
                     records.requests[socketdata.record.id] = socketdata.record
                 elif http_detected is False:  # if None, there is nothing to do
                     records.sockets[id(self)] = None
         return size
```

### Comparing `httpdbg-0.8.5/httpdbg/hooks/urllib3.py` & `httpdbg-0.9.0/httpdbg/hooks/urllib3.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 # -*- coding: utf-8 -*-
 from contextlib import contextmanager
+import traceback
 
 from httpdbg.hooks.utils import getcallargs
 from httpdbg.hooks.utils import decorate
 from httpdbg.hooks.utils import undecorate
-from httpdbg.initiator import get_initiator
+from httpdbg.initiator import httpdbg_initiator
 from httpdbg.records import HTTPRecord
 
 
-def set_hook_for_urrlib3(records, method):
+def set_hook_for_urllib3(records, method):
     def hook(*args, **kwargs):
+        initiator = None
         try:
-            return method(*args, **kwargs)
+            with httpdbg_initiator(
+                records, traceback.extract_stack(), method, *args, **kwargs
+            ) as initiator:
+                ret = method(*args, **kwargs)
+            return ret
         except Exception as ex:
             callargs = getcallargs(method, *args, **kwargs)
-            url = callargs.get("url")
 
-            if url:
-                record = HTTPRecord()
+            if "url" in callargs:
+                if initiator:
+                    record = HTTPRecord()
+
+                    record.initiator = initiator
+                    record.url = str(callargs["url"])
+                    record.exception = ex
 
-                record.initiator = get_initiator(records._initiators)
-                record.url = url
-                record.exception = ex
-
-                records.requests[record.id] = record
+                    records.requests[record.id] = record
             raise
 
     return hook
 
 
 @contextmanager
 def hook_urllib3(records):
     hooks = False
     try:
         import urllib3
 
         urllib3.PoolManager.request = decorate(
-            records, urllib3.PoolManager.request, set_hook_for_urrlib3
+            records, urllib3.PoolManager.request, set_hook_for_urllib3
+        )
+        urllib3.HTTPConnectionPool.request = decorate(
+            records, urllib3.HTTPConnectionPool.request, set_hook_for_urllib3
         )
 
         hooks = True
     except ImportError:
         pass
 
     yield
```

### Comparing `httpdbg-0.8.5/httpdbg/mode_console.py` & `httpdbg-0.9.0/httpdbg/mode_console.py`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/mode_script.py` & `httpdbg-0.9.0/httpdbg/mode_script.py`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/records.py` & `httpdbg-0.9.0/httpdbg/records.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # -*- coding: utf-8 -*-
+import os
 import socket
 import ssl
 import time
+import traceback
 from urllib.parse import urlparse
 from typing import Dict, List, Tuple, Union
 
 from httpdbg.utils import HTTPDBGCookie
 from httpdbg.utils import HTTPDBGHeader
+from httpdbg.initiator import in_lib
+from httpdbg.initiator import compatible_path
 from httpdbg.initiator import Initiator
 from httpdbg.utils import get_new_uuid
 from httpdbg.utils import chunked_to_bytes
 from httpdbg.utils import list_cookies_headers_request_simple_cookies
 from httpdbg.utils import list_cookies_headers_response_simple_cookies
 from httpdbg.utils import logger
 
@@ -184,15 +188,15 @@
 
 
 class HTTPRecord:
     def __init__(self) -> None:
         self.id = get_new_uuid()
         self.address: Tuple[str, int] = ("", 0)
         self._url: Union[str, None] = None
-        self.initiator: Initiator = Initiator("", "", "", "")
+        self.initiator: Initiator = Initiator("", "", None, "", [])
         self.exception = None
         self.request = HTTPRecordRequest()
         self.response = HTTPRecordResponse()
         self.ssl = None
 
     @property
     def url(self) -> str:
@@ -274,14 +278,50 @@
 
     def __getitem__(self, item: int) -> HTTPRecord:
         return list(self.requests.values())[item]
 
     def __len__(self) -> int:
         return len(self.requests)
 
+    def get_initiator(self) -> Initiator:
+        envname = f"HTTPDBG_CURRENT_INITIATOR_{self.id}"
+
+        if envname in os.environ:
+            initiator = self._initiators[os.environ[envname]]
+        else:
+            fullstack = traceback.format_stack()
+            if compatible_path("httpdbg/mode_script.py") in "".join(
+                fullstack
+            ):  # TODO: find another way the detect the mode
+                stack: List[str] = []
+                for line in fullstack[6:]:
+                    if in_lib(line):
+                        break
+                    stack.append(line)
+                long_label = stack[-1]
+                short_label = long_label.split("\n")[1]
+                initiator = Initiator(
+                    get_new_uuid(), short_label, None, long_label, stack
+                )
+            else:
+                initiator = Initiator("console", "console", None, "", [])
+
+        if "PYTEST_CURRENT_TEST" in os.environ:
+            long_label = " ".join(os.environ["PYTEST_CURRENT_TEST"].split(" ")[:-1])
+            short_label = long_label.split("::")[-1]
+            initiator = Initiator(
+                long_label,
+                short_label,
+                long_label,
+                initiator.short_stack,
+                initiator.stack,
+            )
+
+        return initiator
+
     def get_socket_data(self, obj, extra_sock=None, force_new=False, request=None):
         socketdata = None
 
         if force_new:
             self.del_socket_data(obj)
 
         if id(obj) in self._sockets:
```

### Comparing `httpdbg-0.8.5/httpdbg/server.py` & `httpdbg-0.9.0/httpdbg/server.py`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/utils.py` & `httpdbg-0.9.0/httpdbg/utils.py`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/webapp/api.py` & `httpdbg-0.9.0/httpdbg/webapp/api.py`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/webapp/app.py` & `httpdbg-0.9.0/httpdbg/webapp/app.py`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/webapp/preview.py` & `httpdbg-0.9.0/httpdbg/webapp/preview.py`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/webapp/static/api.js` & `httpdbg-0.9.0/httpdbg/webapp/static/api.js`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/webapp/static/configuration.js` & `httpdbg-0.9.0/httpdbg/webapp/static/configuration.js`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/webapp/static/detail.css` & `httpdbg-0.9.0/httpdbg/webapp/static/detail.css`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/webapp/static/favicon.ico` & `httpdbg-0.9.0/httpdbg/webapp/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/webapp/static/icons/download-install-line-icon.svg` & `httpdbg-0.9.0/httpdbg/webapp/static/icons/download-install-line-icon.svg`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/webapp/static/icons/engine-gears-icon.svg` & `httpdbg-0.9.0/httpdbg/webapp/static/icons/engine-gears-icon.svg`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/webapp/static/icons/files-papers-outline-icon.svg` & `httpdbg-0.9.0/httpdbg/webapp/static/icons/files-papers-outline-icon.svg`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/webapp/static/icons/filter-outline-icon.svg` & `httpdbg-0.9.0/httpdbg/webapp/static/icons/filter-outline-icon.svg`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/webapp/static/icons/information-mark-circle-outline-icon.svg` & `httpdbg-0.9.0/httpdbg/webapp/static/icons/information-mark-circle-outline-icon.svg`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/webapp/static/icons/math-multiplication-icon.svg` & `httpdbg-0.9.0/httpdbg/webapp/static/icons/math-multiplication-icon.svg`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/webapp/static/icons/push-pin-green-icon.svg` & `httpdbg-0.9.0/httpdbg/webapp/static/icons/push-pin-green-icon.svg`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/webapp/static/icons/recycle-bin-line-icon.svg` & `httpdbg-0.9.0/httpdbg/webapp/static/icons/recycle-bin-line-icon.svg`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/webapp/static/icons/wait-sandclock-icon.svg` & `httpdbg-0.9.0/httpdbg/webapp/static/icons/wait-sandclock-icon.svg`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/webapp/static/index.htm` & `httpdbg-0.9.0/httpdbg/webapp/static/index.htm`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                         data-qa-request="{{id}}">
                         <td class="pin" onclick="event.stopPropagation();">
                             <input class="pin-checkbox" type="checkbox" id="pin{{id}}" onclick="pin_request('{{id}}',this.checked)" {{pin}}>
                             <label class="pin-icon" for="pin{{id}}"><img class="icon" src="static/icons/push-pin-green-icon.svg-+-$**HTTPDBG_VERSION**$"/></label>
                         </td>
                         <td class="status"><span title="{{reason}}" data-qa-request-status>{{{status_code_view}}}</span></td>
                         <td class="method"><span title="{{verb}}" data-qa-request-method>{{verb}}</span></td>
-                        <td class="url" title="ctrl+click to compare to"><span title="{{url}}" data-qa-request-url><span class="netloc">{{netloc}}</span><span>{{urlext}}</span></span></td>
+                        <td class="url" title="{{title}}"><span data-qa-request-url><span class="netloc">{{netloc}}</span><span>{{urlext}}</span></span></td>
                     </tr>
                 </script>
 
             </table>
 
         </div>
 
@@ -287,15 +287,15 @@
                             <div id="tabStack" class="tabcontent">
                                 <div id="stack" class="content">
                                     <div class="colcontent" name="request">select a request to view details</div>
                                     <div class="colcontent comparison" name="compareto"></div>
                                 </div>
                                 <script id="template_stack" type="x-tmpl-mustache">
                                     {{#initiator}}
-                                        <pre>{{initiator.stack}}</pre>
+                                        <pre class="previewcode">{{initiator.stack}}</pre>
                                     {{/initiator}}
                                 </script>
                             </div>
 
                         </td>
                     </tr>
                 </tbody>
```

### Comparing `httpdbg-0.8.5/httpdbg/webapp/static/mustache.min.js` & `httpdbg-0.9.0/httpdbg/webapp/static/mustache.min.js`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/webapp/static/render.js` & `httpdbg-0.9.0/httpdbg/webapp/static/render.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -11,18 +11,24 @@
         clean();
     };
     k7_id = global.k7;
 
     for (const [request_id, request] of Object.entries(global.requests)) {
         if (request.to_refresh) {
             var elt = document.getElementById("request-" + request.id);
+            request.title = request.url;
+            if (request.initiator.short_stack) {
+                request.title += "\n\n" + request.initiator.short_stack;
+            }
+            request.title += "\n\nclick to select -/- ctrl+click to compare to";
             var rendered = Mustache.render(template_request, request);
             if (!elt) {
                 var elt_initiator = document.getElementById("initiator-" + request.initiator.id);
                 if (!elt_initiator) {
+                    request.initiator.long_label = request.initiator.long_label || request.initiator.short_stack;
                     var rendered_initiator = Mustache.render(template_initiator, request);
                     table.insertAdjacentHTML("beforeend", rendered_initiator);
                     elt_initiator = document.getElementById("initiator-" + request.initiator.id);
                 };
                 elt_initiator.insertAdjacentHTML("beforeend", rendered);
             } else {
                 elt.innerHTML = rendered;
@@ -90,15 +96,14 @@
 
 function fill_content(request_id, name) {
 
     var data = global.requests[request_id].data;
 
     update_with_template("template_title", document.querySelector("#title > div[name='" + name + "']"), data);
 
-
     update_with_template("template_headers", document.querySelector("#headers > div[name='" + name + "']"), data);
 
     update_with_template("template_cookies", document.querySelector("#cookies > div[name='" + name + "']"), data);
 
     var request = data.request ? data.request : {
         "body": null
     };
```

### Comparing `httpdbg-0.8.5/httpdbg/webapp/static/style.css` & `httpdbg-0.9.0/httpdbg/webapp/static/style.css`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg/webapp/static/table.css` & `httpdbg-0.9.0/httpdbg/webapp/static/table.css`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/httpdbg.egg-info/PKG-INFO` & `httpdbg-0.9.0/httpdbg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpdbg
-Version: 0.8.5
+Version: 0.9.0
 Summary: A very simple tool to debug HTTP(S) client requests
 Author-email: cle-b <cle@tictac.pm>
 License: Apache-2.0
 Project-URL: repository, https://github.com/cle-b/httpdbg
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `httpdbg-0.8.5/httpdbg.egg-info/SOURCES.txt` & `httpdbg-0.9.0/httpdbg.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -53,11 +53,12 @@
 tests/test_api.py
 tests/test_cli.py
 tests/test_context_manager.py
 tests/test_hook_aiohttp.py
 tests/test_hook_httpx.py
 tests/test_hook_requests.py
 tests/test_hook_urllib3.py
+tests/test_initiator.py
 tests/test_mode_console.py
 tests/test_mode_module_pytest.py
 tests/test_mode_script.py
 tests/test_preview.py
```

### Comparing `httpdbg-0.8.5/pyproject.toml` & `httpdbg-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/tests/test_api.py` & `httpdbg-0.9.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/tests/test_context_manager.py` & `httpdbg-0.9.0/tests/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/tests/test_hook_aiohttp.py` & `httpdbg-0.9.0/tests/test_hook_aiohttp.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,34 +34,36 @@
 
     assert http_record.url == f"{httpbin_both.url}/get"
     assert http_record.method.upper() == "GET"
     assert http_record.status_code == 200
     assert http_record.reason.upper() == "OK"
 
 
+@pytest.mark.initiator
 @pytest.mark.aiohttp
 @pytest.mark.asyncio
 @pytest.mark.xfail(
     platform.system().lower() == "windows",
     reason="Async HTTP requests not intercepted on Windows",
 )
-async def test_aiohttp_initiator(httpbin):
-    with httpdbg() as records:
-        async with aiohttp.ClientSession() as session:
-            await session.get(f"{httpbin.url}/get")
+async def test_aiohttp_initiator(httpbin, monkeypatch):
+    with monkeypatch.context() as m:
+        m.delenv("PYTEST_CURRENT_TEST")
+        with httpdbg() as records:
+            async with aiohttp.ClientSession() as session:
+                await session.get(f"{httpbin.url}/get")
 
     assert len(records) == 1
     http_record = records[0]
 
-    assert http_record.initiator.short_label == "test_aiohttp_initiator"
     assert (
-        http_record.initiator.long_label
-        == "tests/test_hook_aiohttp.py::test_aiohttp_initiator"
+        http_record.initiator.short_label == 'await session.get(f"{httpbin.url}/get")'
     )
-    assert 'await session.get(f"{httpbin.url}/get")' in "".join(
+    assert http_record.initiator.long_label is None
+    assert 'await session.get(f"{httpbin.url}/get") <====' in "".join(
         http_record.initiator.stack
     )
 
 
 @pytest.mark.aiohttp
 @pytest.mark.asyncio
 @pytest.mark.xfail(
```

### Comparing `httpdbg-0.8.5/tests/test_hook_httpx.py` & `httpdbg-0.9.0/tests/test_hook_httpx.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,28 +26,30 @@
 
     assert http_record.url == f"{httpbin_both.url}/get"
     assert http_record.method.upper() == "GET"
     assert http_record.status_code == 200
     assert http_record.reason.upper() == "OK"
 
 
+@pytest.mark.initiator
 @pytest.mark.httpx
-def test_httpx_initiator(httpbin):
-    with httpdbg() as records:
-        httpx.get(f"{httpbin.url}/get")
+def test_httpx_initiator(httpbin, monkeypatch):
+    with monkeypatch.context() as m:
+        m.delenv("PYTEST_CURRENT_TEST")
+        with httpdbg() as records:
+            httpx.get(f"{httpbin.url}/get")
 
     assert len(records) == 1
     http_record = records[0]
 
-    assert http_record.initiator.short_label == "test_httpx_initiator"
-    assert (
-        http_record.initiator.long_label
-        == "tests/test_hook_httpx.py::test_httpx_initiator"
+    assert http_record.initiator.short_label == 'httpx.get(f"{httpbin.url}/get")'
+    assert http_record.initiator.long_label is None
+    assert 'httpx.get(f"{httpbin.url}/get") <===' in "".join(
+        http_record.initiator.stack
     )
-    assert 'httpx.get(f"{httpbin.url}/get")' in "".join(http_record.initiator.stack)
 
 
 @pytest.mark.httpx
 def test_httpx_request(httpbin_both):
     with httpdbg() as records:
         httpx.post(f"{httpbin_both.url}/post", content="abc", verify=False)
 
@@ -280,34 +282,34 @@
 
     assert http_record.url == f"{httpbin_both.url}/get"
     assert http_record.method.upper() == "GET"
     assert http_record.status_code == 200
     assert http_record.reason.upper() == "OK"
 
 
+@pytest.mark.initiator
 @pytest.mark.httpx
 @pytest.mark.asyncio
 @pytest.mark.xfail(
     platform.system().lower() == "windows",
     reason="Async HTTP requests not intercepted on Windows",
 )
-async def test_httpx_initiator_asyncclient(httpbin):
-    with httpdbg() as records:
-        async with httpx.AsyncClient() as client:
-            await client.get(f"{httpbin.url}/get")
+async def test_httpx_initiator_asyncclient(httpbin, monkeypatch):
+    with monkeypatch.context() as m:
+        m.delenv("PYTEST_CURRENT_TEST")
+        with httpdbg() as records:
+            async with httpx.AsyncClient() as client:
+                await client.get(f"{httpbin.url}/get")
 
     assert len(records) == 1
     http_record = records[0]
 
-    assert http_record.initiator.short_label == "test_httpx_initiator_asyncclient"
-    assert (
-        http_record.initiator.long_label
-        == "tests/test_hook_httpx.py::test_httpx_initiator_asyncclient"
-    )
-    assert 'await client.get(f"{httpbin.url}/get")' in "".join(
+    assert http_record.initiator.short_label == 'await client.get(f"{httpbin.url}/get")'
+    assert http_record.initiator.long_label is None
+    assert 'await client.get(f"{httpbin.url}/get") <===' in "".join(
         http_record.initiator.stack
     )
 
 
 @pytest.mark.httpx
 @pytest.mark.asyncio
 @pytest.mark.xfail(
```

### Comparing `httpdbg-0.8.5/tests/test_hook_requests.py` & `httpdbg-0.9.0/tests/test_hook_requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,28 +18,30 @@
 
     assert http_record.url == f"{httpbin_both.url}/get"
     assert http_record.method.upper() == "GET"
     assert http_record.status_code == 200
     assert http_record.reason.upper() == "OK"
 
 
+@pytest.mark.initiator
 @pytest.mark.requests
-def test_requests_initiator(httpbin):
-    with httpdbg() as records:
-        requests.get(f"{httpbin.url}/get")
+def test_requests_initiator(httpbin, monkeypatch):
+    with monkeypatch.context() as m:
+        m.delenv("PYTEST_CURRENT_TEST")
+        with httpdbg() as records:
+            requests.get(f"{httpbin.url}/get")
 
     assert len(records) == 1
     http_record = records[0]
 
-    assert http_record.initiator.short_label == "test_requests_initiator"
-    assert (
-        http_record.initiator.long_label
-        == "tests/test_hook_requests.py::test_requests_initiator"
+    assert http_record.initiator.short_label == 'requests.get(f"{httpbin.url}/get")'
+    assert http_record.initiator.long_label is None
+    assert 'requests.get(f"{httpbin.url}/get") <===' in "".join(
+        http_record.initiator.stack
     )
-    assert 'requests.get(f"{httpbin.url}/get")' in "".join(http_record.initiator.stack)
 
 
 @pytest.mark.requests
 def test_requests_request(httpbin_both):
     with httpdbg() as records:
         requests.post(f"{httpbin_both.url}/post", data="abc", verify=False)
 
@@ -61,15 +63,14 @@
 
     assert len(records) == 1
     http_record = records[0]
 
     assert http_record.method.upper() == "PUT"
     assert http_record.status_code == 200
 
-    print(http_record.response.headers)
     assert (
         HTTPDBGHeader("Content-Type", "application/json")
         in http_record.response.headers
     )
     assert http_record.response.cookies == []
     assert b'"args":{"azerty":""}' in http_record.response.content
     assert b'"data":"def"' in http_record.response.content
```

### Comparing `httpdbg-0.8.5/tests/test_hook_urllib3.py` & `httpdbg-0.9.0/tests/test_hook_urllib3.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,32 +18,39 @@
 
     assert http_record.url == f"{httpbin_both.url}/get"
     assert http_record.method.upper() == "GET"
     assert http_record.status_code == 200
     assert http_record.reason.upper() == "OK"
 
 
+@pytest.mark.initiator
 @pytest.mark.urllib3
-def test_urllib3_initiator(httpbin):
-    with httpdbg() as records:
-        with urllib3.PoolManager(cert_reqs="CERT_NONE") as http:
-            http.request("GET", f"{httpbin.url}/get")
+def test_urllib3_initiator(httpbin, monkeypatch):
+    with monkeypatch.context() as m:
+        m.delenv("PYTEST_CURRENT_TEST")
+        with httpdbg() as records:
+            with urllib3.PoolManager(cert_reqs="CERT_NONE") as http:
+                http.request("GET", f"{httpbin.url}/get")
+            with urllib3.HTTPConnectionPool(f"{httpbin.url[7:]}") as http:
+                http.request("GET", "/get")
 
-    assert len(records) == 1
-    http_record = records[0]
+    assert len(records) == 2
 
-    assert http_record.initiator.short_label == "test_urllib3_initiator"
     assert (
-        http_record.initiator.long_label
-        == "tests/test_hook_urllib3.py::test_urllib3_initiator"
+        records[0].initiator.short_label == 'http.request("GET", f"{httpbin.url}/get")'
     )
-    assert 'http.request("GET", f"{httpbin.url}/get")' in "".join(
-        http_record.initiator.stack
+    assert records[0].initiator.long_label is None
+    assert 'http.request("GET", f"{httpbin.url}/get") <===' in "".join(
+        records[0].initiator.stack
     )
 
+    assert records[1].initiator.short_label == 'http.request("GET", "/get")'
+    assert records[1].initiator.long_label is None
+    assert 'http.request("GET", "/get") <===' in "".join(records[1].initiator.stack)
+
 
 @pytest.mark.urllib3
 def test_urllib3_request(httpbin_both):
     with httpdbg() as records:
         with urllib3.PoolManager(cert_reqs="CERT_NONE") as http:
             http.request(
                 "POST",
```

### Comparing `httpdbg-0.8.5/tests/test_mode_console.py` & `httpdbg-0.9.0/tests/test_mode_console.py`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/tests/test_mode_module_pytest.py` & `httpdbg-0.9.0/tests/test_mode_module_pytest.py`

 * *Files identical despite different names*

### Comparing `httpdbg-0.8.5/tests/test_mode_script.py` & `httpdbg-0.9.0/tests/test_mode_script.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,32 +71,29 @@
         run_script(["not_a_path_to_a_python_script"])
 
 
 @pytest.mark.api
 @pytest.mark.script
 def test_run_script_initiator(httpbin, httpdbg_port):
     with httpdbg_srv(httpdbg_port) as records:
-        PYTEST_CURRENT_TEST = os.environ["PYTEST_CURRENT_TEST"]
-        os.environ.pop("PYTEST_CURRENT_TEST")
-
         with httpdbg(records):
             script_to_run = os.path.join(
                 os.path.dirname(os.path.realpath(__file__)), "demo_run_script.py"
             )
             run_script([script_to_run, httpbin.url])
 
-        os.environ["PYTEST_CURRENT_TEST"] = PYTEST_CURRENT_TEST
-
         ret = requests.get(f"http://127.0.0.1:{httpdbg_port}/requests")
 
     reqs = ret.json()["requests"]
 
     assert (
-        reqs[list(reqs.keys())[0]]["initiator"].get("short_label")
-        == '    _ = requests.get(f"{base_url}/get")'
+        reqs[list(reqs.keys())[0]]["initiator"]["short_label"]
+        == "test_run_script_initiator"
+    )
+    assert (
+        reqs[list(reqs.keys())[0]]["initiator"]["long_label"]
+        == "tests/test_mode_script.py::test_run_script_initiator"
+    )
+    assert (
+        '_ = requests.get(f"{base_url}/get")'
+        in reqs[list(reqs.keys())[0]]["initiator"]["short_stack"]
     )
-    assert 'demo_run_script.py", line 8,' in reqs[list(reqs.keys())[0]][
-        "initiator"
-    ].get("long_label")
-    assert '_ = requests.get(f"{base_url}/get")' in reqs[list(reqs.keys())[0]][
-        "initiator"
-    ].get("long_label")
```

### Comparing `httpdbg-0.8.5/tests/test_preview.py` & `httpdbg-0.9.0/tests/test_preview.py`

 * *Files identical despite different names*

