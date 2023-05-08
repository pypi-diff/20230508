# Comparing `tmp/robotframework-browser-9.0.1.tar.gz` & `tmp/robotframework-browser-9.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-browser-9.0.1.tar", last modified: Thu Oct 14 11:29:03 2021, max compression
+gzip compressed data, was "robotframework-browser-9.0.2.tar", last modified: Thu Oct 21 18:05:57 2021, max compression
```

## Comparing `robotframework-browser-9.0.1.tar` & `robotframework-browser-9.0.2.tar`

### file list

```diff
@@ -1,65 +1,55 @@
-drwxr-xr-x   0 kerkko     (501) staff       (20)        0 2021-10-14 11:29:03.291814 robotframework-browser-9.0.1/
-drwxr-xr-x   0 kerkko     (501) staff       (20)        0 2021-10-14 11:29:03.277353 robotframework-browser-9.0.1/Browser/
--rw-r--r--   0 kerkko     (501) staff       (20)     1164 2021-05-10 06:35:26.000000 robotframework-browser-9.0.1/Browser/__init__.py
--rw-r--r--   0 kerkko     (501) staff       (20)    16326 2021-10-14 11:29:02.000000 robotframework-browser-9.0.1/Browser/__init__.pyi
--rw-r--r--   0 kerkko     (501) staff       (20)     1908 2021-05-10 06:35:26.000000 robotframework-browser-9.0.1/Browser/assertion_engine.py
-drwxr-xr-x   0 kerkko     (501) staff       (20)        0 2021-10-14 11:29:03.278410 robotframework-browser-9.0.1/Browser/base/
--rw-r--r--   0 kerkko     (501) staff       (20)      715 2020-12-04 07:30:30.000000 robotframework-browser-9.0.1/Browser/base/__init__.py
--rw-r--r--   0 kerkko     (501) staff       (20)      321 2020-12-04 07:30:30.000000 robotframework-browser-9.0.1/Browser/base/cache.py
--rw-r--r--   0 kerkko     (501) staff       (20)     4614 2021-10-14 09:51:58.000000 robotframework-browser-9.0.1/Browser/base/librarycomponent.py
--rwxr-xr-x   0 kerkko     (501) staff       (20)    42995 2021-10-14 09:51:58.000000 robotframework-browser-9.0.1/Browser/browser.py
--rw-r--r--   0 kerkko     (501) staff       (20)      679 2021-10-14 09:51:58.000000 robotframework-browser-9.0.1/Browser/dev-requirements.txt
--rw-r--r--   0 kerkko     (501) staff       (20)     6817 2021-10-14 09:51:58.000000 robotframework-browser-9.0.1/Browser/entry.py
--rw-r--r--   0 kerkko     (501) staff       (20)     5560 2021-10-14 09:51:58.000000 robotframework-browser-9.0.1/Browser/gen_stub.py
-drwxr-xr-x   0 kerkko     (501) staff       (20)        0 2021-10-14 11:29:03.279824 robotframework-browser-9.0.1/Browser/generated/
--rw-r--r--   0 kerkko     (501) staff       (20)        0 2021-10-14 11:28:51.000000 robotframework-browser-9.0.1/Browser/generated/__init__.py
--rw-r--r--   0 kerkko     (501) staff       (20)   127195 2021-10-14 11:28:51.000000 robotframework-browser-9.0.1/Browser/generated/playwright_pb2.py
--rw-r--r--   0 kerkko     (501) staff       (20)    31255 2021-10-14 11:28:51.000000 robotframework-browser-9.0.1/Browser/generated/playwright_pb2.pyi
--rw-r--r--   0 kerkko     (501) staff       (20)   118557 2021-10-14 11:28:51.000000 robotframework-browser-9.0.1/Browser/generated/playwright_pb2_grpc.py
-drwxr-xr-x   0 kerkko     (501) staff       (20)        0 2021-10-14 11:29:03.284518 robotframework-browser-9.0.1/Browser/keywords/
--rw-r--r--   0 kerkko     (501) staff       (20)     1299 2021-09-30 08:07:46.000000 robotframework-browser-9.0.1/Browser/keywords/__init__.py
--rw-r--r--   0 kerkko     (501) staff       (20)    13088 2021-10-14 09:51:58.000000 robotframework-browser-9.0.1/Browser/keywords/browser_control.py
--rw-r--r--   0 kerkko     (501) staff       (20)    10032 2021-09-30 08:07:46.000000 robotframework-browser-9.0.1/Browser/keywords/cookie.py
--rw-r--r--   0 kerkko     (501) staff       (20)     3965 2021-09-30 08:07:46.000000 robotframework-browser-9.0.1/Browser/keywords/crawling.py
--rw-r--r--   0 kerkko     (501) staff       (20)     2409 2021-09-30 08:07:46.000000 robotframework-browser-9.0.1/Browser/keywords/device_descriptors.py
--rw-r--r--   0 kerkko     (501) staff       (20)     5209 2021-09-30 08:07:46.000000 robotframework-browser-9.0.1/Browser/keywords/evaluation.py
--rw-r--r--   0 kerkko     (501) staff       (20)    45419 2021-10-07 07:57:40.000000 robotframework-browser-9.0.1/Browser/keywords/getters.py
--rw-r--r--   0 kerkko     (501) staff       (20)    42542 2021-10-14 09:51:58.000000 robotframework-browser-9.0.1/Browser/keywords/interaction.py
--rw-r--r--   0 kerkko     (501) staff       (20)    10224 2021-10-07 09:39:03.000000 robotframework-browser-9.0.1/Browser/keywords/network.py
--rwxr-xr-x   0 kerkko     (501) staff       (20)    48742 2021-10-14 11:24:57.000000 robotframework-browser-9.0.1/Browser/keywords/playwright_state.py
--rw-r--r--   0 kerkko     (501) staff       (20)     6962 2021-09-30 10:54:18.000000 robotframework-browser-9.0.1/Browser/keywords/promises.py
--rw-r--r--   0 kerkko     (501) staff       (20)     2952 2021-10-14 09:51:58.000000 robotframework-browser-9.0.1/Browser/keywords/runonfailure.py
--rw-r--r--   0 kerkko     (501) staff       (20)     1498 2021-10-14 09:51:58.000000 robotframework-browser-9.0.1/Browser/keywords/strict_mode.py
--rw-r--r--   0 kerkko     (501) staff       (20)     8842 2021-09-30 08:07:46.000000 robotframework-browser-9.0.1/Browser/keywords/waiter.py
--rw-r--r--   0 kerkko     (501) staff       (20)     7351 2021-09-30 08:07:46.000000 robotframework-browser-9.0.1/Browser/keywords/webapp_state.py
--rw-r--r--   0 kerkko     (501) staff       (20)      209 2020-12-04 07:30:30.000000 robotframework-browser-9.0.1/Browser/mypy.ini
--rw-r--r--   0 kerkko     (501) staff       (20)     6711 2021-10-06 13:44:43.000000 robotframework-browser-9.0.1/Browser/playwright.py
--rw-r--r--   0 kerkko     (501) staff       (20)      286 2021-09-23 06:37:40.000000 robotframework-browser-9.0.1/Browser/pyproject.toml
--rw-r--r--   0 kerkko     (501) staff       (20)      257 2021-10-14 09:51:58.000000 robotframework-browser-9.0.1/Browser/requirements.txt
-drwxr-xr-x   0 kerkko     (501) staff       (20)        0 2021-10-14 11:29:03.286135 robotframework-browser-9.0.1/Browser/utils/
--rw-r--r--   0 kerkko     (501) staff       (20)     1356 2021-09-30 10:54:18.000000 robotframework-browser-9.0.1/Browser/utils/__init__.py
--rw-r--r--   0 kerkko     (501) staff       (20)    14535 2021-10-14 09:51:58.000000 robotframework-browser-9.0.1/Browser/utils/data_types.py
--rw-r--r--   0 kerkko     (501) staff       (20)     2147 2021-01-07 07:45:41.000000 robotframework-browser-9.0.1/Browser/utils/deprecated.py
--rw-r--r--   0 kerkko     (501) staff       (20)     2206 2020-12-04 07:30:30.000000 robotframework-browser-9.0.1/Browser/utils/js_utilities.py
--rw-r--r--   0 kerkko     (501) staff       (20)     2062 2020-12-04 07:30:30.000000 robotframework-browser-9.0.1/Browser/utils/logger.py
--rw-r--r--   0 kerkko     (501) staff       (20)     1572 2020-12-04 07:30:30.000000 robotframework-browser-9.0.1/Browser/utils/meta_python.py
--rw-r--r--   0 kerkko     (501) staff       (20)     1727 2021-10-14 09:51:58.000000 robotframework-browser-9.0.1/Browser/utils/misc.py
--rw-r--r--   0 kerkko     (501) staff       (20)     1012 2020-12-04 07:30:30.000000 robotframework-browser-9.0.1/Browser/utils/robot_booleans.py
--rw-r--r--   0 kerkko     (501) staff       (20)       22 2021-10-14 11:24:57.000000 robotframework-browser-9.0.1/Browser/version.py
-drwxr-xr-x   0 kerkko     (501) staff       (20)        0 2021-10-14 11:29:03.289889 robotframework-browser-9.0.1/Browser/wrapper/
--rw-r--r--   0 kerkko     (501) staff       (20)  3075281 2021-10-14 11:25:12.000000 robotframework-browser-9.0.1/Browser/wrapper/index.js
--rw-r--r--   0 kerkko     (501) staff       (20)   181760 2021-09-30 08:32:02.000000 robotframework-browser-9.0.1/Browser/wrapper/package-lock.json
--rw-r--r--   0 kerkko     (501) staff       (20)     1569 2021-10-14 11:29:02.000000 robotframework-browser-9.0.1/Browser/wrapper/package.json
--rw-r--r--   0 kerkko     (501) staff       (20)    11361 2020-12-04 07:30:30.000000 robotframework-browser-9.0.1/LICENSE
--rw-r--r--   0 kerkko     (501) staff       (20)       16 2021-05-10 06:35:26.000000 robotframework-browser-9.0.1/MANIFEST.in
--rw-r--r--   0 kerkko     (501) staff       (20)    23129 2021-10-14 11:29:03.291578 robotframework-browser-9.0.1/PKG-INFO
--rw-r--r--   0 kerkko     (501) staff       (20)    22312 2021-10-14 09:51:58.000000 robotframework-browser-9.0.1/README.md
-drwxr-xr-x   0 kerkko     (501) staff       (20)        0 2021-10-14 11:29:03.291173 robotframework-browser-9.0.1/robotframework_browser.egg-info/
--rw-r--r--   0 kerkko     (501) staff       (20)    23129 2021-10-14 11:29:03.000000 robotframework-browser-9.0.1/robotframework_browser.egg-info/PKG-INFO
--rw-r--r--   0 kerkko     (501) staff       (20)     1577 2021-10-14 11:29:03.000000 robotframework-browser-9.0.1/robotframework_browser.egg-info/SOURCES.txt
--rw-r--r--   0 kerkko     (501) staff       (20)        1 2021-10-14 11:29:03.000000 robotframework-browser-9.0.1/robotframework_browser.egg-info/dependency_links.txt
--rw-r--r--   0 kerkko     (501) staff       (20)       49 2021-10-14 11:29:03.000000 robotframework-browser-9.0.1/robotframework_browser.egg-info/entry_points.txt
--rw-r--r--   0 kerkko     (501) staff       (20)      241 2021-10-14 11:29:03.000000 robotframework-browser-9.0.1/robotframework_browser.egg-info/requires.txt
--rw-r--r--   0 kerkko     (501) staff       (20)        8 2021-10-14 11:29:03.000000 robotframework-browser-9.0.1/robotframework_browser.egg-info/top_level.txt
--rw-r--r--   0 kerkko     (501) staff       (20)       38 2021-10-14 11:29:03.291881 robotframework-browser-9.0.1/setup.cfg
--rw-r--r--   0 kerkko     (501) staff       (20)     1731 2021-10-14 11:24:57.000000 robotframework-browser-9.0.1/setup.py
+drwxrwxr-x   0 tatu      (1000) tatu      (1000)        0 2021-10-21 18:05:57.625337 robotframework-browser-9.0.2/
+drwxrwxr-x   0 tatu      (1000) tatu      (1000)        0 2021-10-21 18:05:57.613337 robotframework-browser-9.0.2/Browser/
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     1164 2021-03-20 17:46:49.000000 robotframework-browser-9.0.2/Browser/__init__.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     1908 2021-03-20 17:46:49.000000 robotframework-browser-9.0.2/Browser/assertion_engine.py
+drwxrwxr-x   0 tatu      (1000) tatu      (1000)        0 2021-10-21 18:05:57.617337 robotframework-browser-9.0.2/Browser/base/
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)      715 2021-01-30 22:16:32.000000 robotframework-browser-9.0.2/Browser/base/__init__.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)      321 2021-01-30 22:16:32.000000 robotframework-browser-9.0.2/Browser/base/cache.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     4614 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/base/librarycomponent.py
+-rwxrwxr-x   0 tatu      (1000) tatu      (1000)    43252 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/browser.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     6817 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/entry.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     5560 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/gen_stub.py
+drwxrwxr-x   0 tatu      (1000) tatu      (1000)        0 2021-10-21 18:05:57.617337 robotframework-browser-9.0.2/Browser/generated/
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)        0 2021-10-21 18:05:33.000000 robotframework-browser-9.0.2/Browser/generated/__init__.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)   127195 2021-10-21 18:05:33.000000 robotframework-browser-9.0.2/Browser/generated/playwright_pb2.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)   118557 2021-10-21 18:05:33.000000 robotframework-browser-9.0.2/Browser/generated/playwright_pb2_grpc.py
+drwxrwxr-x   0 tatu      (1000) tatu      (1000)        0 2021-10-21 18:05:57.621337 robotframework-browser-9.0.2/Browser/keywords/
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     1299 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/keywords/__init__.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)    13088 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/keywords/browser_control.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)    10033 2021-10-21 17:37:16.000000 robotframework-browser-9.0.2/Browser/keywords/cookie.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     3965 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/keywords/crawling.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     2409 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/keywords/device_descriptors.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     5209 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/keywords/evaluation.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)    45419 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/keywords/getters.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)    42542 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/keywords/interaction.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)    10224 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/keywords/network.py
+-rwxrwxr-x   0 tatu      (1000) tatu      (1000)    48742 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/keywords/playwright_state.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     6962 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/keywords/promises.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     3137 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/keywords/runonfailure.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     1498 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/keywords/strict_mode.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     8842 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/keywords/waiter.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     7351 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/keywords/webapp_state.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     6711 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/playwright.py
+drwxrwxr-x   0 tatu      (1000) tatu      (1000)        0 2021-10-21 18:05:57.621337 robotframework-browser-9.0.2/Browser/utils/
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     1356 2021-03-25 18:56:30.000000 robotframework-browser-9.0.2/Browser/utils/__init__.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)    14706 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/utils/data_types.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     2147 2021-01-30 22:16:32.000000 robotframework-browser-9.0.2/Browser/utils/deprecated.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     2206 2021-01-30 22:16:32.000000 robotframework-browser-9.0.2/Browser/utils/js_utilities.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     2062 2021-01-30 22:16:32.000000 robotframework-browser-9.0.2/Browser/utils/logger.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     1572 2021-01-30 22:16:32.000000 robotframework-browser-9.0.2/Browser/utils/meta_python.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     1727 2021-10-21 17:36:08.000000 robotframework-browser-9.0.2/Browser/utils/misc.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     1012 2021-01-30 22:16:32.000000 robotframework-browser-9.0.2/Browser/utils/robot_booleans.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)       22 2021-10-21 17:55:52.000000 robotframework-browser-9.0.2/Browser/version.py
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)    11361 2021-01-30 22:16:32.000000 robotframework-browser-9.0.2/LICENSE
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)       16 2021-03-25 18:56:30.000000 robotframework-browser-9.0.2/MANIFEST.in
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)    25224 2021-10-21 18:05:57.625337 robotframework-browser-9.0.2/PKG-INFO
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)    22634 2021-10-21 17:37:16.000000 robotframework-browser-9.0.2/README.md
+drwxrwxr-x   0 tatu      (1000) tatu      (1000)        0 2021-10-21 18:05:57.621337 robotframework-browser-9.0.2/robotframework_browser.egg-info/
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)    25224 2021-10-21 18:05:57.000000 robotframework-browser-9.0.2/robotframework_browser.egg-info/PKG-INFO
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     1337 2021-10-21 18:05:57.000000 robotframework-browser-9.0.2/robotframework_browser.egg-info/SOURCES.txt
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)        1 2021-10-21 18:05:57.000000 robotframework-browser-9.0.2/robotframework_browser.egg-info/dependency_links.txt
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)       49 2021-10-21 18:05:57.000000 robotframework-browser-9.0.2/robotframework_browser.egg-info/entry_points.txt
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)      241 2021-10-21 18:05:57.000000 robotframework-browser-9.0.2/robotframework_browser.egg-info/requires.txt
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)        8 2021-10-21 18:05:57.000000 robotframework-browser-9.0.2/robotframework_browser.egg-info/top_level.txt
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)       38 2021-10-21 18:05:57.625337 robotframework-browser-9.0.2/setup.cfg
+-rw-rw-r--   0 tatu      (1000) tatu      (1000)     1731 2021-10-21 17:55:52.000000 robotframework-browser-9.0.2/setup.py
```

### Comparing `robotframework-browser-9.0.1/Browser/__init__.py` & `robotframework-browser-9.0.2/Browser/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/assertion_engine.py` & `robotframework-browser-9.0.2/Browser/assertion_engine.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/base/__init__.py` & `robotframework-browser-9.0.2/Browser/base/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/base/librarycomponent.py` & `robotframework-browser-9.0.2/Browser/base/librarycomponent.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/browser.py` & `robotframework-browser-9.0.2/Browser/browser.py`

 * *Files 4% similar despite different names*

```diff
@@ -724,28 +724,32 @@
         # Parsing needs keywords to be discovered.
         self.run_on_failure_keyword = self._parse_run_on_failure_keyword(run_on_failure)
 
     def _parse_run_on_failure_keyword(
         self, keyword_name: Union[str, None]
     ) -> DelayedKeyword:
         if keyword_name is None or is_falsy(keyword_name):
-            return DelayedKeyword(None, None, tuple())
+            return DelayedKeyword(None, None, tuple(), {})
         parts = keyword_name.split("  ")
         keyword_name = parts[0]
         normalized_keyword_name = get_normalized_keyword(keyword_name)
         args = parts[1:]
         if normalized_keyword_name not in self.keywords:
-            return DelayedKeyword(keyword_name, keyword_name, tuple(args))
+            return DelayedKeyword(keyword_name, keyword_name, tuple(args), {})
         spec = PythonArgumentParser().parse(self.keywords[normalized_keyword_name])
-        converted_args = []
+        varargs = []
+        kwargs = {}
         for arg in spec.resolve(args):
             for item in arg:
-                converted_args.append(item)
+                if isinstance(item, tuple):
+                    kwargs[item[0]] = item[1]
+                else:
+                    varargs.append(item)
         return DelayedKeyword(
-            normalized_keyword_name, keyword_name, tuple(converted_args)
+            normalized_keyword_name, keyword_name, tuple(varargs), kwargs
         )
 
     def _initialize_jsextension(self, jsextension: str) -> LibraryComponent:
         component = LibraryComponent(self)
         with self.playwright.grpc_channel() as stub:
             response = stub.InitializeExtension(
                 Request().FilePath(path=os.path.abspath(jsextension))
@@ -896,24 +900,27 @@
                 self.screenshot_on_failure(test.name)
 
     def keyword_error(self):
         """Runs keyword on failure."""
         if self._running_on_failure_keyword or not self.run_on_failure_keyword.name:
             return
         self._running_on_failure_keyword = True
-        args = self.run_on_failure_keyword.args
+        varargs = self.run_on_failure_keyword.args
+        kwargs = self.run_on_failure_keyword.kwargs
         try:
             if self.run_on_failure_keyword.name in self.keywords:
-                if self.run_on_failure_keyword.name == "take_screenshot" and not args:
-                    args = [self._failure_screenshot_path()]
-                self.keywords[self.run_on_failure_keyword.name](*args)
+                if (
+                    self.run_on_failure_keyword.name == "take_screenshot"
+                    and not varargs
+                ):
+                    varargs = [self._failure_screenshot_path()]
+                self.keywords[self.run_on_failure_keyword.name](*varargs, **kwargs)
             else:
                 BuiltIn().run_keyword(
-                    self.run_on_failure_keyword.name,
-                    *args,
+                    self.run_on_failure_keyword.name, *varargs, **kwargs
                 )
         except Exception as err:
             logger.warn(
                 f"Keyword '{self.run_on_failure_keyword}' could not be run on failure:\n{err}"
             )
         finally:
             self._running_on_failure_keyword = False
```

### Comparing `robotframework-browser-9.0.1/Browser/entry.py` & `robotframework-browser-9.0.2/Browser/entry.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/gen_stub.py` & `robotframework-browser-9.0.2/Browser/gen_stub.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/generated/playwright_pb2.py` & `robotframework-browser-9.0.2/Browser/generated/playwright_pb2.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/generated/playwright_pb2_grpc.py` & `robotframework-browser-9.0.2/Browser/generated/playwright_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/keywords/__init__.py` & `robotframework-browser-9.0.2/Browser/keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/keywords/browser_control.py` & `robotframework-browser-9.0.2/Browser/keywords/browser_control.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/keywords/cookie.py` & `robotframework-browser-9.0.2/Browser/keywords/cookie.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         dot_dict = DotDict()
         for key in cookie:
             if key == "expires":
                 # In Windows OS, expires value might be -1 and it causes OSError.
                 try:
                     dot_dict[key] = datetime.fromtimestamp(cookie[key])
                 except OSError:
-                    logger.warn(
+                    logger.debug(
                         f"Invalid expiry seen in: {cookie}, setting expiry as None"
                     )
                     dot_dict[key] = None
             else:
                 dot_dict[key] = cookie[key]
         return dot_dict
 
@@ -189,15 +189,15 @@
 
         | *Value*  | *Explanation*                                                                              |
         | name     | The name of a cookie, mandatory.                                                           |
         | value    | Value of the cookie, mandatory.                                                            |
         | url      | Define the scope of the cookie, what URLs the cookies should be sent to.                   |
         | domain   | Specifies which hosts are allowed to receive the cookie.                                   |
         | path     | Indicates a URL path that must exist in the requested URL, for example `/`.                |
-        | expiry   | Lifetime of a cookie. Returned as datatime object.                                         |
+        | expiry   | Lifetime of a cookie. Returned as datatime object or None if not valid time received.      |
         | httpOnly | When true, the cookie is not accessible via JavaScript.                                    |
         | secure   | When true, the cookie is only used with HTTPS connections.                                 |
         | sameSite | Attribute lets servers require that a cookie shouldn't be sent with cross-origin requests. |
 
         See
         [https://playwright.dev/docs/api/class-browsercontext#browsercontextaddcookiescookies|playwright documentation]
         for details about each attribute.
```

### Comparing `robotframework-browser-9.0.1/Browser/keywords/crawling.py` & `robotframework-browser-9.0.2/Browser/keywords/crawling.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/keywords/device_descriptors.py` & `robotframework-browser-9.0.2/Browser/keywords/device_descriptors.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/keywords/evaluation.py` & `robotframework-browser-9.0.2/Browser/keywords/evaluation.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/keywords/getters.py` & `robotframework-browser-9.0.2/Browser/keywords/getters.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/keywords/interaction.py` & `robotframework-browser-9.0.2/Browser/keywords/interaction.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/keywords/network.py` & `robotframework-browser-9.0.2/Browser/keywords/network.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/keywords/playwright_state.py` & `robotframework-browser-9.0.2/Browser/keywords/playwright_state.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/keywords/promises.py` & `robotframework-browser-9.0.2/Browser/keywords/promises.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/keywords/runonfailure.py` & `robotframework-browser-9.0.2/Browser/keywords/runonfailure.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,16 @@
         restore the original value later. The returned object contains
         keyword name and the possible arguments used to for the keyword.
 
         Example:
         | `Register Keyword To Run On Failure`    Take Screenshot
         | ${previous kw}=    `Register Keyword To Run On Failure`    NONE
         | `Register Keyword To Run On Failure`    ${previous kw}
+        | `Register Keyword To Run On Failure`    Take Screenshot    fullPage=True
+        | `Register Keyword To Run On Failure`    Take Screenshot    failure-{index}    fullPage=True
 
         """
         old_keyword = self.library.run_on_failure_keyword
         new_keyword = self.parse_run_on_failure_keyword(
             f"{keyword}  {'  '.join(args)}".strip()
         )
         self.library.run_on_failure_keyword = new_keyword
```

### Comparing `robotframework-browser-9.0.1/Browser/keywords/strict_mode.py` & `robotframework-browser-9.0.2/Browser/keywords/strict_mode.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/keywords/waiter.py` & `robotframework-browser-9.0.2/Browser/keywords/waiter.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/keywords/webapp_state.py` & `robotframework-browser-9.0.2/Browser/keywords/webapp_state.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/playwright.py` & `robotframework-browser-9.0.2/Browser/playwright.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/utils/__init__.py` & `robotframework-browser-9.0.2/Browser/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/utils/data_types.py` & `robotframework-browser-9.0.2/Browser/utils/data_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,23 +56,29 @@
                 typed_dict[opt_key] = struct[opt_key](lower_case_dict[opt_key.lower()])  # type: ignore
             params[arg_name] = typed_dict
     return params
 
 
 class DelayedKeyword:
     def __init__(
-        self, name: Union[str, None], original_name: Union[str, None], args: tuple
+        self,
+        name: Union[str, None],
+        original_name: Union[str, None],
+        args: tuple,
+        kwargs: dict,
     ):
         self.name = name
         self.original_name = original_name
         self.args = args
+        self.kwargs = kwargs
 
     def __str__(self):
         args = [str(arg) for arg in self.args]
-        return f"{self.original_name}  {'  '.join(args)}".strip()
+        kwargs = [f"{key}={value}" for key, value in self.kwargs.items()]
+        return f"{self.original_name}  {'  '.join(args)}  {'  '.join(kwargs)}".strip()
 
 
 class BoundingBox(TypedDict, total=False):
     x: float
     y: float
     width: float
     height: float
```

### Comparing `robotframework-browser-9.0.1/Browser/utils/deprecated.py` & `robotframework-browser-9.0.2/Browser/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/utils/js_utilities.py` & `robotframework-browser-9.0.2/Browser/utils/js_utilities.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/utils/logger.py` & `robotframework-browser-9.0.2/Browser/utils/logger.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/utils/meta_python.py` & `robotframework-browser-9.0.2/Browser/utils/meta_python.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/utils/misc.py` & `robotframework-browser-9.0.2/Browser/utils/misc.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/Browser/utils/robot_booleans.py` & `robotframework-browser-9.0.2/Browser/utils/robot_booleans.py`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/LICENSE` & `robotframework-browser-9.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-browser-9.0.1/PKG-INFO` & `robotframework-browser-9.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,10 @@
-Metadata-Version: 2.1
-Name: robotframework-browser
-Version: 9.0.1
-Summary: Robot Framework Browser library powered by Playwright. Aiming for speed, reliability and visibility.
-Home-page: https://github.com/MarketSquare/robotframework-browser
-Author: MarketSquare - Robot Framework community
-Author-email: mikko.korpela@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Testing
-Classifier: Framework :: Robot Framework
-Classifier: Framework :: Robot Framework :: Library
-Requires-Python: >=3.7,<4.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # robotframework-browser
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-50-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-51-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 [![Version](https://img.shields.io/pypi/v/robotframework-browser.svg)](https://pypi.python.org/pypi/robotframework-browser)
 [![Actions Status](https://github.com/MarketSquare/robotframework-browser/workflows/Continuous%20integration/badge.svg)](https://github.com/MarketSquare/robotframework-browser/actions)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 ----
 
@@ -229,16 +209,15 @@
     <td align="center"><a href="https://github.com/AllanMedeiros"><img src="https://avatars.githubusercontent.com/u/34678196?v=4?s=100" width="100px;" alt=""/><br /><sub><b>AllanMedeiros</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AAllanMedeiros" title="Bug reports">🐛</a></td>
     <td align="center"><a href="https://github.com/ealap"><img src="https://avatars.githubusercontent.com/u/15620712?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Emmanuel Alap</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aealap" title="Bug reports">🐛</a></td>
     <td align="center"><a href="https://github.com/ankurbhalla-gmail"><img src="https://avatars.githubusercontent.com/u/90744440?v=4?s=100" width="100px;" alt=""/><br /><sub><b>ankurbhalla-gmail</b></sub></a><br /><a href="#ideas-ankurbhalla-gmail" title="Ideas, Planning, & Feedback">🤔</a></td>
     <td align="center"><a href="https://github.com/UliSei"><img src="https://avatars.githubusercontent.com/u/89480399?v=4?s=100" width="100px;" alt=""/><br /><sub><b>UliSei</b></sub></a><br /><a href="#ideas-UliSei" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AUliSei" title="Bug reports">🐛</a> <a href="https://github.com/MarketSquare/robotframework-browser/commits?author=UliSei" title="Code">💻</a></td>
   </tr>
   <tr>
     <td align="center"><a href="https://github.com/tomekTieto"><img src="https://avatars.githubusercontent.com/u/39945193?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Tomasz Pawlak</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AtomekTieto" title="Bug reports">🐛</a></td>
+    <td align="center"><a href="https://github.com/mtoskamp"><img src="https://avatars.githubusercontent.com/u/58772827?v=4?s=100" width="100px;" alt=""/><br /><sub><b>mtoskamp</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Amtoskamp" title="Bug reports">🐛</a></td>
   </tr>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
-
-
```

### Comparing `robotframework-browser-9.0.1/README.md` & `robotframework-browser-9.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,222 +1,242 @@
-# robotframework-browser
-<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-50-orange.svg?style=flat-square)](#contributors-)
-<!-- ALL-CONTRIBUTORS-BADGE:END -->
-[![Version](https://img.shields.io/pypi/v/robotframework-browser.svg)](https://pypi.python.org/pypi/robotframework-browser)
-[![Actions Status](https://github.com/MarketSquare/robotframework-browser/workflows/Continuous%20integration/badge.svg)](https://github.com/MarketSquare/robotframework-browser/actions)
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-
-----
-
-[Robot Framework](https://robotframework.org) Browser library powered by [Playwright](https://playwright.dev/). Moving browser automation to year 2021!
-
-Aiming for :rocket: speed, :white_check_mark: reliability and :microscope: visibility.
-
-See [keyword documentation](https://marketsquare.github.io/robotframework-browser/Browser.html) and
-[web page](https://robotframework-browser.org/) for more details.
-
-# Installation instructions
-
-Only Python 3.7 or newer is supported.
-
-1. Install node.js e.g. from https://nodejs.org/en/download/ (only < v15 supported; if unsure, use 14.15.0 LTS)
-2. Update pip `pip install -U pip` to ensure latest version is used
-3. Install robotframework-browser from the commandline: `pip install robotframework-browser`
-4. Install the node dependencies: run `rfbrowser init` in your shell
-  - if `rfbrowser` is not found, try `python -m Browser.entry init`
-
-Please note that by default Chromium, Firefox and WebKit browser are installed, even those would be already
-installed in the system. The installation size depends on the operating system, but usually is +700Mb.
-It is possible to skip browser binaries installation with `rfbrowser init --skip-browsers` command, but then user
-is responsible for browser binary installation.
-
-Or use the [docker images](https://github.com/MarketSquare/robotframework-browser/packages). Documented at [docker/README.md](https://github.com/MarketSquare/robotframework-browser/blob/main/docker/README.md).
-
-## Update instructions
-
-To upgrade your already installed robotframework-browser library
-
-1. Update from commandline: `pip install -U robotframework-browser`
-2. Clean old node side dependencies and browser binaries: `rfbrowser clean-node`
-3. Install the node dependencies for the newly installed version: `rfbrowser init`
-
-## Uninstall instructions
-
-To completely install library, including the browser binaries installed by Playwright,
-run following commands:
-1. Clean old node side dependencies and browser binaries: `rfbrowser clean-node`
-2. Uninstall with pip: `pip uninstall robotframework-browser`
-
-# Examples
-
-### Testing with [Robot Framework](https://robotframework.org)
-```RobotFramework
-*** Settings ***
-Library   Browser
-
-*** Test Cases ***
-Example Test
-    New Page    https://playwright.dev
-    Get Text    h1    contains    Playwright
-```
-### and testing with [Python](https://python.org).
-```python
-import Browser
-browser = Browser.Browser()
-browser.new_page("https://playwright.dev")
-assert 'Playwright' in browser.get_text("h1")
-browser.close_browser()
-```
-
-### and extending with JavaScript
-
-```JavaScript
-async function myGoToKeyword(page, args) {
-  return await page.goto(args[0]);
-}
-exports.__esModule = true;
-exports.myGoToKeyword = myGoToKeyword;
-```
-
-```RobotFramework
-*** Settings ***
-Library   Browser  jsextension=${CURDIR}/mymodule.js
-
-*** Test Cases ***
-Example Test
-   New Page
-   myGoToKeyword   https://www.robotframework.org
-```
-
-Ready made extensions and a place to share your own at [robotframework-browser-extensions](https://github.com/MarketSquare/robotframework-browser-extensions).
-
-### Ergonomic selector syntax, supports chaining of `text`, `css`  and `xpath` selectors
-
-```RobotFramework
-# Select element containing text "Login" with text selector strategy 
-# and select it's parent `input` element with xpath
-Click    "Login" >> xpath=../input
-# Select element with CSS strategy and select button in it with text strategy
-Click    div.dialog >> "Ok"
-```
-### Evaluate in browser page
-```RobotFramework
-New Page   ${LOGIN_URL}
-${ref}=    Get Element    h1
-Get Property    ${ref}    innerText    ==    Login Page
-Execute JavaScript    (elem) => elem.innerText = "abc"    ${ref}
-Get Property    ${ref}    innerText    ==    abc
-```
-### Asynchronously waiting for HTTP requests and responses
-```RobotFramework
-# The button with id `delayed_request` fires a delayed request. We use a promise to capture it.
-${promise}=    Promise To    Wait For Response    matcher=    timeout=3s
-Click    \#delayed_request
-${body}=    Wait For    ${promise}
-```
-### Device Descriptors
-```RobotFramework
-${device}=  Get Device  iPhone X
-New Context  &{device}
-New Page
-Get Viewport Size  # returns { "width": 375, "height": 812 }
-```
-### Sending HTTP requests and parsing their responses
-```RobotFramework
-&{response}=    HTTP    /api/post    POST    {"name": "John"}
-Should Be Equal    ${response.status}    ${200}
-```
-# Development
-
-See [CONTRIBUTING.md](CONTRIBUTING.md) for development instructions.
-
-## Core team
-
-In order of appearance.
-
-  * Mikko Korpela
-  * Tatu Aalto
-  * Janne Härkönen (Alumnus)
-  * Kerkko Pelttari
-  * René Rohner
-
-## Contributors
-
-This project is community driven and becomes a reality only through the work of all the people who contribute.
-Supported by [Robocorp](https://robocorp.com/) through [Robot Framework Foundation](https://robotframework.org/foundation/).
-<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
-<!-- prettier-ignore-start -->
-<!-- markdownlint-disable -->
-<table>
-  <tr>
-    <td align="center"><a href="https://github.com/mkorpela"><img src="https://avatars1.githubusercontent.com/u/136885?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Mikko Korpela</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=mkorpela" title="Code">💻</a></td>
-    <td align="center"><a href="https://github.com/aaltat"><img src="https://avatars0.githubusercontent.com/u/2665023?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Tatu Aalto</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=aaltat" title="Code">💻</a></td>
-    <td align="center"><a href="https://robocorp.com"><img src="https://avatars1.githubusercontent.com/u/8512727?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Antti Karjalainen</b></sub></a><br /><a href="#fundingFinding-aikarjal" title="Funding Finding">🔍</a></td>
-    <td align="center"><a href="https://www.linkedin.com/in/ismoaro/"><img src="https://avatars2.githubusercontent.com/u/1047173?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ismo Aro</b></sub></a><br /><a href="#fundingFinding-IsNoGood" title="Funding Finding">🔍</a></td>
-    <td align="center"><a href="https://twitter.com/janneharkonen"><img src="https://avatars3.githubusercontent.com/u/159146?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Janne Härkönen</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=yanne" title="Code">💻</a></td>
-    <td align="center"><a href="http://xylix.fi"><img src="https://avatars1.githubusercontent.com/u/13387304?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Kerkko Pelttari</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=xylix" title="Code">💻</a></td>
-    <td align="center"><a href="https://robocorp.com"><img src="https://avatars3.githubusercontent.com/u/54288445?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Robocorp</b></sub></a><br /><a href="#financial-robocorp" title="Financial">💵</a></td>
-  </tr>
-  <tr>
-    <td align="center"><a href="https://github.com/Snooz82"><img src="https://avatars0.githubusercontent.com/u/41592183?v=4?s=100" width="100px;" alt=""/><br /><sub><b>René</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=Snooz82" title="Code">💻</a></td>
-    <td align="center"><a href="https://wordpress.com/read/feeds/39696435"><img src="https://avatars0.githubusercontent.com/u/1123938?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Bryan Oakley</b></sub></a><br /><a href="#ideas-boakley" title="Ideas, Planning, & Feedback">🤔</a></td>
-    <td align="center"><a href="https://github.com/idxn"><img src="https://avatars3.githubusercontent.com/u/2438992?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Tanakiat Srisaranyakul</b></sub></a><br /><a href="#ideas-idxn" title="Ideas, Planning, & Feedback">🤔</a></td>
-    <td align="center"><a href="http://visible-quality.blogspot.com"><img src="https://avatars1.githubusercontent.com/u/5338157?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Maaret Pyhäjärvi</b></sub></a><br /><a href="#userTesting-maaretp" title="User Testing">📓</a></td>
-    <td align="center"><a href="http://www.tentamen.eu"><img src="https://avatars2.githubusercontent.com/u/777520?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Karlo Smid</b></sub></a><br /><a href="#userTesting-karlosmid" title="User Testing">📓</a></td>
-    <td align="center"><a href="https://github.com/aspargillus"><img src="https://avatars0.githubusercontent.com/u/4592889?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Frank Schimmel</b></sub></a><br /><a href="#userTesting-Aspargillus" title="User Testing">📓</a></td>
-    <td align="center"><a href="https://github.com/tuxmux28"><img src="https://avatars3.githubusercontent.com/u/2794048?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Christoph</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=tuxmux28" title="Tests">⚠️</a></td>
-  </tr>
-  <tr>
-    <td align="center"><a href="https://github.com/mikahanninen"><img src="https://avatars2.githubusercontent.com/u/1019528?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Mika Hänninen</b></sub></a><br /><a href="#question-mikahanninen" title="Answering Questions">💬</a></td>
-    <td align="center"><a href="https://www.imbus.de"><img src="https://avatars0.githubusercontent.com/u/67375753?v=4?s=100" width="100px;" alt=""/><br /><sub><b>imbus</b></sub></a><br /><a href="#financial-imbus" title="Financial">💵</a></td>
-    <td align="center"><a href="https://github.com/Finalrykku"><img src="https://avatars0.githubusercontent.com/u/19802569?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Niklas</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=Finalrykku" title="Documentation">📖</a></td>
-    <td align="center"><a href="https://github.com/gdroes"><img src="https://avatars1.githubusercontent.com/u/6716450?v=4?s=100" width="100px;" alt=""/><br /><sub><b>gdroes</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=gdroes" title="Tests">⚠️</a></td>
-    <td align="center"><a href="https://reaktor.com"><img src="https://avatars2.githubusercontent.com/u/71799?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Reaktor</b></sub></a><br /><a href="#financial-reaktor" title="Financial">💵</a></td>
-    <td align="center"><a href="https://github.com/adrianyorke"><img src="https://avatars1.githubusercontent.com/u/30093433?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Adrian Yorke</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=adrianyorke" title="Documentation">📖</a> <a href="https://github.com/MarketSquare/robotframework-browser/pulls?q=is%3Apr+reviewed-by%3Aadrianyorke" title="Reviewed Pull Requests">👀</a></td>
-    <td align="center"><a href="https://github.com/wangzimeiyingtao"><img src="https://avatars0.githubusercontent.com/u/70925596?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nanakawa</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=wangzimeiyingtao" title="Tests">⚠️</a></td>
-  </tr>
-  <tr>
-    <td align="center"><a href="https://github.com/emanlove"><img src="https://avatars1.githubusercontent.com/u/993527?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ed Manlove</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=emanlove" title="Documentation">📖</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aemanlove" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/estimation"><img src="https://avatars1.githubusercontent.com/u/16793171?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Brian Tsao</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aestimation" title="Bug reports">🐛</a> <a href="#userTesting-estimation" title="User Testing">📓</a></td>
-    <td align="center"><a href="https://github.com/mawentao119"><img src="https://avatars0.githubusercontent.com/u/26617186?v=4?s=100" width="100px;" alt=""/><br /><sub><b>charis</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=mawentao119" title="Code">💻</a></td>
-    <td align="center"><a href="https://github.com/s-galante"><img src="https://avatars2.githubusercontent.com/u/4580052?v=4?s=100" width="100px;" alt=""/><br /><sub><b>s-galante</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3As-galante" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="http://www.elabit.de"><img src="https://avatars3.githubusercontent.com/u/1897410?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Simon Meggle</b></sub></a><br /><a href="#userTesting-simonmeggle" title="User Testing">📓</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Asimonmeggle" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/Anna-Gunda"><img src="https://avatars3.githubusercontent.com/u/13298792?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Anna-Gunda</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AAnna-Gunda" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/anton264"><img src="https://avatars0.githubusercontent.com/u/10194266?v=4?s=100" width="100px;" alt=""/><br /><sub><b>anton264</b></sub></a><br /><a href="#userTesting-anton264" title="User Testing">📓</a></td>
-  </tr>
-  <tr>
-    <td align="center"><a href="https://github.com/emakaay"><img src="https://avatars.githubusercontent.com/u/72747481?v=4?s=100" width="100px;" alt=""/><br /><sub><b>emakaay</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aemakaay" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://virvatuli.itch.io/"><img src="https://avatars.githubusercontent.com/u/29060467?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nea Ohvo</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AVirvatuli" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/leeuwe"><img src="https://avatars.githubusercontent.com/u/66635066?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Elout van Leeuwen</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=leeuwe" title="Documentation">📖</a></td>
-    <td align="center"><a href="https://github.com/LDerikx"><img src="https://avatars.githubusercontent.com/u/26576024?v=4?s=100" width="100px;" alt=""/><br /><sub><b>LDerikx</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=LDerikx" title="Documentation">📖</a></td>
-    <td align="center"><a href="https://github.com/olga-"><img src="https://avatars.githubusercontent.com/u/9334057?v=4?s=100" width="100px;" alt=""/><br /><sub><b>olga-</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=olga-" title="Documentation">📖</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aolga-" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/bollwyvl"><img src="https://avatars.githubusercontent.com/u/45380?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nicholas Bollweg</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=bollwyvl" title="Documentation">📖</a></td>
-    <td align="center"><a href="http://villesalonen.fi"><img src="https://avatars.githubusercontent.com/u/1070813?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ville Salonen</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AVilleSalonen" title="Bug reports">🐛</a></td>
-  </tr>
-  <tr>
-    <td align="center"><a href="https://rasjani.github.io"><img src="https://avatars.githubusercontent.com/u/27887?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jani Mikkonen</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Arasjani" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/JaPyR"><img src="https://avatars.githubusercontent.com/u/7773301?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Aleh Borysiewicz</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AJaPyR" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="http://www.binary-overflow.de"><img src="https://avatars.githubusercontent.com/u/25060709?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jürgen Knauth</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Ajkpubsrc" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/dalaakso"><img src="https://avatars.githubusercontent.com/u/50731554?v=4?s=100" width="100px;" alt=""/><br /><sub><b>dalaakso</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Adalaakso" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/msirkka"><img src="https://avatars.githubusercontent.com/u/84907426?v=4?s=100" width="100px;" alt=""/><br /><sub><b>msirkka</b></sub></a><br /><a href="#ideas-msirkka" title="Ideas, Planning, & Feedback">🤔</a></td>
-    <td align="center"><a href="https://github.com/osrjv"><img src="https://avatars.githubusercontent.com/u/29481017?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ossi R.</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=osrjv" title="Code">💻</a></td>
-    <td align="center"><a href="https://github.com/adrian-evo"><img src="https://avatars.githubusercontent.com/u/19324942?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Adrian V.</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=adrian-evo" title="Code">💻</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aadrian-evo" title="Bug reports">🐛</a> <a href="#ideas-adrian-evo" title="Ideas, Planning, & Feedback">🤔</a></td>
-  </tr>
-  <tr>
-    <td align="center"><a href="https://github.com/ssallmen"><img src="https://avatars.githubusercontent.com/u/39527407?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Sami Sallmén</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Assallmen" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="http://eliga.fi"><img src="https://avatars.githubusercontent.com/u/114985?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Pekka Klärck</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=pekkaklarck" title="Code">💻</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Apekkaklarck" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/janipalsamaki"><img src="https://avatars.githubusercontent.com/u/1157184?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jani Palsamäki</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Ajanipalsamaki" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/AllanMedeiros"><img src="https://avatars.githubusercontent.com/u/34678196?v=4?s=100" width="100px;" alt=""/><br /><sub><b>AllanMedeiros</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AAllanMedeiros" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/ealap"><img src="https://avatars.githubusercontent.com/u/15620712?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Emmanuel Alap</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aealap" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/ankurbhalla-gmail"><img src="https://avatars.githubusercontent.com/u/90744440?v=4?s=100" width="100px;" alt=""/><br /><sub><b>ankurbhalla-gmail</b></sub></a><br /><a href="#ideas-ankurbhalla-gmail" title="Ideas, Planning, & Feedback">🤔</a></td>
-    <td align="center"><a href="https://github.com/UliSei"><img src="https://avatars.githubusercontent.com/u/89480399?v=4?s=100" width="100px;" alt=""/><br /><sub><b>UliSei</b></sub></a><br /><a href="#ideas-UliSei" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AUliSei" title="Bug reports">🐛</a> <a href="https://github.com/MarketSquare/robotframework-browser/commits?author=UliSei" title="Code">💻</a></td>
-  </tr>
-  <tr>
-    <td align="center"><a href="https://github.com/tomekTieto"><img src="https://avatars.githubusercontent.com/u/39945193?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Tomasz Pawlak</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AtomekTieto" title="Bug reports">🐛</a></td>
-  </tr>
-</table>
-
-<!-- markdownlint-restore -->
-<!-- prettier-ignore-end -->
-
-<!-- ALL-CONTRIBUTORS-LIST:END -->
+Metadata-Version: 2.1
+Name: robotframework-browser
+Version: 9.0.2
+Summary: Robot Framework Browser library powered by Playwright. Aiming for speed, reliability and visibility.
+Home-page: https://github.com/MarketSquare/robotframework-browser
+Author: MarketSquare - Robot Framework community
+Author-email: mikko.korpela@gmail.com
+License: UNKNOWN
+Description: # robotframework-browser
+        <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+        [![All Contributors](https://img.shields.io/badge/all_contributors-51-orange.svg?style=flat-square)](#contributors-)
+        <!-- ALL-CONTRIBUTORS-BADGE:END -->
+        [![Version](https://img.shields.io/pypi/v/robotframework-browser.svg)](https://pypi.python.org/pypi/robotframework-browser)
+        [![Actions Status](https://github.com/MarketSquare/robotframework-browser/workflows/Continuous%20integration/badge.svg)](https://github.com/MarketSquare/robotframework-browser/actions)
+        [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+        
+        ----
+        
+        [Robot Framework](https://robotframework.org) Browser library powered by [Playwright](https://playwright.dev/). Moving browser automation to year 2021!
+        
+        Aiming for :rocket: speed, :white_check_mark: reliability and :microscope: visibility.
+        
+        See [keyword documentation](https://marketsquare.github.io/robotframework-browser/Browser.html) and
+        [web page](https://robotframework-browser.org/) for more details.
+        
+        # Installation instructions
+        
+        Only Python 3.7 or newer is supported.
+        
+        1. Install node.js e.g. from https://nodejs.org/en/download/ (only < v15 supported; if unsure, use 14.15.0 LTS)
+        2. Update pip `pip install -U pip` to ensure latest version is used
+        3. Install robotframework-browser from the commandline: `pip install robotframework-browser`
+        4. Install the node dependencies: run `rfbrowser init` in your shell
+          - if `rfbrowser` is not found, try `python -m Browser.entry init`
+        
+        Please note that by default Chromium, Firefox and WebKit browser are installed, even those would be already
+        installed in the system. The installation size depends on the operating system, but usually is +700Mb.
+        It is possible to skip browser binaries installation with `rfbrowser init --skip-browsers` command, but then user
+        is responsible for browser binary installation.
+        
+        Or use the [docker images](https://github.com/MarketSquare/robotframework-browser/packages). Documented at [docker/README.md](https://github.com/MarketSquare/robotframework-browser/blob/main/docker/README.md).
+        
+        ## Update instructions
+        
+        To upgrade your already installed robotframework-browser library
+        
+        1. Update from commandline: `pip install -U robotframework-browser`
+        2. Clean old node side dependencies and browser binaries: `rfbrowser clean-node`
+        3. Install the node dependencies for the newly installed version: `rfbrowser init`
+        
+        ## Uninstall instructions
+        
+        To completely install library, including the browser binaries installed by Playwright,
+        run following commands:
+        1. Clean old node side dependencies and browser binaries: `rfbrowser clean-node`
+        2. Uninstall with pip: `pip uninstall robotframework-browser`
+        
+        # Examples
+        
+        ### Testing with [Robot Framework](https://robotframework.org)
+        ```RobotFramework
+        *** Settings ***
+        Library   Browser
+        
+        *** Test Cases ***
+        Example Test
+            New Page    https://playwright.dev
+            Get Text    h1    contains    Playwright
+        ```
+        ### and testing with [Python](https://python.org).
+        ```python
+        import Browser
+        browser = Browser.Browser()
+        browser.new_page("https://playwright.dev")
+        assert 'Playwright' in browser.get_text("h1")
+        browser.close_browser()
+        ```
+        
+        ### and extending with JavaScript
+        
+        ```JavaScript
+        async function myGoToKeyword(page, args) {
+          return await page.goto(args[0]);
+        }
+        exports.__esModule = true;
+        exports.myGoToKeyword = myGoToKeyword;
+        ```
+        
+        ```RobotFramework
+        *** Settings ***
+        Library   Browser  jsextension=${CURDIR}/mymodule.js
+        
+        *** Test Cases ***
+        Example Test
+           New Page
+           myGoToKeyword   https://www.robotframework.org
+        ```
+        
+        Ready made extensions and a place to share your own at [robotframework-browser-extensions](https://github.com/MarketSquare/robotframework-browser-extensions).
+        
+        ### Ergonomic selector syntax, supports chaining of `text`, `css`  and `xpath` selectors
+        
+        ```RobotFramework
+        # Select element containing text "Login" with text selector strategy 
+        # and select it's parent `input` element with xpath
+        Click    "Login" >> xpath=../input
+        # Select element with CSS strategy and select button in it with text strategy
+        Click    div.dialog >> "Ok"
+        ```
+        ### Evaluate in browser page
+        ```RobotFramework
+        New Page   ${LOGIN_URL}
+        ${ref}=    Get Element    h1
+        Get Property    ${ref}    innerText    ==    Login Page
+        Execute JavaScript    (elem) => elem.innerText = "abc"    ${ref}
+        Get Property    ${ref}    innerText    ==    abc
+        ```
+        ### Asynchronously waiting for HTTP requests and responses
+        ```RobotFramework
+        # The button with id `delayed_request` fires a delayed request. We use a promise to capture it.
+        ${promise}=    Promise To    Wait For Response    matcher=    timeout=3s
+        Click    \#delayed_request
+        ${body}=    Wait For    ${promise}
+        ```
+        ### Device Descriptors
+        ```RobotFramework
+        ${device}=  Get Device  iPhone X
+        New Context  &{device}
+        New Page
+        Get Viewport Size  # returns { "width": 375, "height": 812 }
+        ```
+        ### Sending HTTP requests and parsing their responses
+        ```RobotFramework
+        &{response}=    HTTP    /api/post    POST    {"name": "John"}
+        Should Be Equal    ${response.status}    ${200}
+        ```
+        # Development
+        
+        See [CONTRIBUTING.md](CONTRIBUTING.md) for development instructions.
+        
+        ## Core team
+        
+        In order of appearance.
+        
+          * Mikko Korpela
+          * Tatu Aalto
+          * Janne Härkönen (Alumnus)
+          * Kerkko Pelttari
+          * René Rohner
+        
+        ## Contributors
+        
+        This project is community driven and becomes a reality only through the work of all the people who contribute.
+        Supported by [Robocorp](https://robocorp.com/) through [Robot Framework Foundation](https://robotframework.org/foundation/).
+        <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+        <!-- prettier-ignore-start -->
+        <!-- markdownlint-disable -->
+        <table>
+          <tr>
+            <td align="center"><a href="https://github.com/mkorpela"><img src="https://avatars1.githubusercontent.com/u/136885?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Mikko Korpela</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=mkorpela" title="Code">💻</a></td>
+            <td align="center"><a href="https://github.com/aaltat"><img src="https://avatars0.githubusercontent.com/u/2665023?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Tatu Aalto</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=aaltat" title="Code">💻</a></td>
+            <td align="center"><a href="https://robocorp.com"><img src="https://avatars1.githubusercontent.com/u/8512727?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Antti Karjalainen</b></sub></a><br /><a href="#fundingFinding-aikarjal" title="Funding Finding">🔍</a></td>
+            <td align="center"><a href="https://www.linkedin.com/in/ismoaro/"><img src="https://avatars2.githubusercontent.com/u/1047173?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ismo Aro</b></sub></a><br /><a href="#fundingFinding-IsNoGood" title="Funding Finding">🔍</a></td>
+            <td align="center"><a href="https://twitter.com/janneharkonen"><img src="https://avatars3.githubusercontent.com/u/159146?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Janne Härkönen</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=yanne" title="Code">💻</a></td>
+            <td align="center"><a href="http://xylix.fi"><img src="https://avatars1.githubusercontent.com/u/13387304?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Kerkko Pelttari</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=xylix" title="Code">💻</a></td>
+            <td align="center"><a href="https://robocorp.com"><img src="https://avatars3.githubusercontent.com/u/54288445?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Robocorp</b></sub></a><br /><a href="#financial-robocorp" title="Financial">💵</a></td>
+          </tr>
+          <tr>
+            <td align="center"><a href="https://github.com/Snooz82"><img src="https://avatars0.githubusercontent.com/u/41592183?v=4?s=100" width="100px;" alt=""/><br /><sub><b>René</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=Snooz82" title="Code">💻</a></td>
+            <td align="center"><a href="https://wordpress.com/read/feeds/39696435"><img src="https://avatars0.githubusercontent.com/u/1123938?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Bryan Oakley</b></sub></a><br /><a href="#ideas-boakley" title="Ideas, Planning, & Feedback">🤔</a></td>
+            <td align="center"><a href="https://github.com/idxn"><img src="https://avatars3.githubusercontent.com/u/2438992?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Tanakiat Srisaranyakul</b></sub></a><br /><a href="#ideas-idxn" title="Ideas, Planning, & Feedback">🤔</a></td>
+            <td align="center"><a href="http://visible-quality.blogspot.com"><img src="https://avatars1.githubusercontent.com/u/5338157?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Maaret Pyhäjärvi</b></sub></a><br /><a href="#userTesting-maaretp" title="User Testing">📓</a></td>
+            <td align="center"><a href="http://www.tentamen.eu"><img src="https://avatars2.githubusercontent.com/u/777520?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Karlo Smid</b></sub></a><br /><a href="#userTesting-karlosmid" title="User Testing">📓</a></td>
+            <td align="center"><a href="https://github.com/aspargillus"><img src="https://avatars0.githubusercontent.com/u/4592889?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Frank Schimmel</b></sub></a><br /><a href="#userTesting-Aspargillus" title="User Testing">📓</a></td>
+            <td align="center"><a href="https://github.com/tuxmux28"><img src="https://avatars3.githubusercontent.com/u/2794048?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Christoph</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=tuxmux28" title="Tests">⚠️</a></td>
+          </tr>
+          <tr>
+            <td align="center"><a href="https://github.com/mikahanninen"><img src="https://avatars2.githubusercontent.com/u/1019528?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Mika Hänninen</b></sub></a><br /><a href="#question-mikahanninen" title="Answering Questions">💬</a></td>
+            <td align="center"><a href="https://www.imbus.de"><img src="https://avatars0.githubusercontent.com/u/67375753?v=4?s=100" width="100px;" alt=""/><br /><sub><b>imbus</b></sub></a><br /><a href="#financial-imbus" title="Financial">💵</a></td>
+            <td align="center"><a href="https://github.com/Finalrykku"><img src="https://avatars0.githubusercontent.com/u/19802569?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Niklas</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=Finalrykku" title="Documentation">📖</a></td>
+            <td align="center"><a href="https://github.com/gdroes"><img src="https://avatars1.githubusercontent.com/u/6716450?v=4?s=100" width="100px;" alt=""/><br /><sub><b>gdroes</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=gdroes" title="Tests">⚠️</a></td>
+            <td align="center"><a href="https://reaktor.com"><img src="https://avatars2.githubusercontent.com/u/71799?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Reaktor</b></sub></a><br /><a href="#financial-reaktor" title="Financial">💵</a></td>
+            <td align="center"><a href="https://github.com/adrianyorke"><img src="https://avatars1.githubusercontent.com/u/30093433?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Adrian Yorke</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=adrianyorke" title="Documentation">📖</a> <a href="https://github.com/MarketSquare/robotframework-browser/pulls?q=is%3Apr+reviewed-by%3Aadrianyorke" title="Reviewed Pull Requests">👀</a></td>
+            <td align="center"><a href="https://github.com/wangzimeiyingtao"><img src="https://avatars0.githubusercontent.com/u/70925596?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nanakawa</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=wangzimeiyingtao" title="Tests">⚠️</a></td>
+          </tr>
+          <tr>
+            <td align="center"><a href="https://github.com/emanlove"><img src="https://avatars1.githubusercontent.com/u/993527?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ed Manlove</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=emanlove" title="Documentation">📖</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aemanlove" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/estimation"><img src="https://avatars1.githubusercontent.com/u/16793171?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Brian Tsao</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aestimation" title="Bug reports">🐛</a> <a href="#userTesting-estimation" title="User Testing">📓</a></td>
+            <td align="center"><a href="https://github.com/mawentao119"><img src="https://avatars0.githubusercontent.com/u/26617186?v=4?s=100" width="100px;" alt=""/><br /><sub><b>charis</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=mawentao119" title="Code">💻</a></td>
+            <td align="center"><a href="https://github.com/s-galante"><img src="https://avatars2.githubusercontent.com/u/4580052?v=4?s=100" width="100px;" alt=""/><br /><sub><b>s-galante</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3As-galante" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="http://www.elabit.de"><img src="https://avatars3.githubusercontent.com/u/1897410?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Simon Meggle</b></sub></a><br /><a href="#userTesting-simonmeggle" title="User Testing">📓</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Asimonmeggle" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/Anna-Gunda"><img src="https://avatars3.githubusercontent.com/u/13298792?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Anna-Gunda</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AAnna-Gunda" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/anton264"><img src="https://avatars0.githubusercontent.com/u/10194266?v=4?s=100" width="100px;" alt=""/><br /><sub><b>anton264</b></sub></a><br /><a href="#userTesting-anton264" title="User Testing">📓</a></td>
+          </tr>
+          <tr>
+            <td align="center"><a href="https://github.com/emakaay"><img src="https://avatars.githubusercontent.com/u/72747481?v=4?s=100" width="100px;" alt=""/><br /><sub><b>emakaay</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aemakaay" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://virvatuli.itch.io/"><img src="https://avatars.githubusercontent.com/u/29060467?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nea Ohvo</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AVirvatuli" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/leeuwe"><img src="https://avatars.githubusercontent.com/u/66635066?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Elout van Leeuwen</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=leeuwe" title="Documentation">📖</a></td>
+            <td align="center"><a href="https://github.com/LDerikx"><img src="https://avatars.githubusercontent.com/u/26576024?v=4?s=100" width="100px;" alt=""/><br /><sub><b>LDerikx</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=LDerikx" title="Documentation">📖</a></td>
+            <td align="center"><a href="https://github.com/olga-"><img src="https://avatars.githubusercontent.com/u/9334057?v=4?s=100" width="100px;" alt=""/><br /><sub><b>olga-</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=olga-" title="Documentation">📖</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aolga-" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/bollwyvl"><img src="https://avatars.githubusercontent.com/u/45380?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nicholas Bollweg</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=bollwyvl" title="Documentation">📖</a></td>
+            <td align="center"><a href="http://villesalonen.fi"><img src="https://avatars.githubusercontent.com/u/1070813?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ville Salonen</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AVilleSalonen" title="Bug reports">🐛</a></td>
+          </tr>
+          <tr>
+            <td align="center"><a href="https://rasjani.github.io"><img src="https://avatars.githubusercontent.com/u/27887?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jani Mikkonen</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Arasjani" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/JaPyR"><img src="https://avatars.githubusercontent.com/u/7773301?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Aleh Borysiewicz</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AJaPyR" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="http://www.binary-overflow.de"><img src="https://avatars.githubusercontent.com/u/25060709?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jürgen Knauth</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Ajkpubsrc" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/dalaakso"><img src="https://avatars.githubusercontent.com/u/50731554?v=4?s=100" width="100px;" alt=""/><br /><sub><b>dalaakso</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Adalaakso" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/msirkka"><img src="https://avatars.githubusercontent.com/u/84907426?v=4?s=100" width="100px;" alt=""/><br /><sub><b>msirkka</b></sub></a><br /><a href="#ideas-msirkka" title="Ideas, Planning, & Feedback">🤔</a></td>
+            <td align="center"><a href="https://github.com/osrjv"><img src="https://avatars.githubusercontent.com/u/29481017?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ossi R.</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=osrjv" title="Code">💻</a></td>
+            <td align="center"><a href="https://github.com/adrian-evo"><img src="https://avatars.githubusercontent.com/u/19324942?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Adrian V.</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=adrian-evo" title="Code">💻</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aadrian-evo" title="Bug reports">🐛</a> <a href="#ideas-adrian-evo" title="Ideas, Planning, & Feedback">🤔</a></td>
+          </tr>
+          <tr>
+            <td align="center"><a href="https://github.com/ssallmen"><img src="https://avatars.githubusercontent.com/u/39527407?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Sami Sallmén</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Assallmen" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="http://eliga.fi"><img src="https://avatars.githubusercontent.com/u/114985?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Pekka Klärck</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=pekkaklarck" title="Code">💻</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Apekkaklarck" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/janipalsamaki"><img src="https://avatars.githubusercontent.com/u/1157184?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jani Palsamäki</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Ajanipalsamaki" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/AllanMedeiros"><img src="https://avatars.githubusercontent.com/u/34678196?v=4?s=100" width="100px;" alt=""/><br /><sub><b>AllanMedeiros</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AAllanMedeiros" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/ealap"><img src="https://avatars.githubusercontent.com/u/15620712?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Emmanuel Alap</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aealap" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/ankurbhalla-gmail"><img src="https://avatars.githubusercontent.com/u/90744440?v=4?s=100" width="100px;" alt=""/><br /><sub><b>ankurbhalla-gmail</b></sub></a><br /><a href="#ideas-ankurbhalla-gmail" title="Ideas, Planning, & Feedback">🤔</a></td>
+            <td align="center"><a href="https://github.com/UliSei"><img src="https://avatars.githubusercontent.com/u/89480399?v=4?s=100" width="100px;" alt=""/><br /><sub><b>UliSei</b></sub></a><br /><a href="#ideas-UliSei" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AUliSei" title="Bug reports">🐛</a> <a href="https://github.com/MarketSquare/robotframework-browser/commits?author=UliSei" title="Code">💻</a></td>
+          </tr>
+          <tr>
+            <td align="center"><a href="https://github.com/tomekTieto"><img src="https://avatars.githubusercontent.com/u/39945193?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Tomasz Pawlak</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AtomekTieto" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/mtoskamp"><img src="https://avatars.githubusercontent.com/u/58772827?v=4?s=100" width="100px;" alt=""/><br /><sub><b>mtoskamp</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Amtoskamp" title="Bug reports">🐛</a></td>
+          </tr>
+        </table>
+        
+        <!-- markdownlint-restore -->
+        <!-- prettier-ignore-end -->
+        
+        <!-- ALL-CONTRIBUTORS-LIST:END -->
+        
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Testing
+Classifier: Framework :: Robot Framework
+Classifier: Framework :: Robot Framework :: Library
+Requires-Python: >=3.7,<4.0
+Description-Content-Type: text/markdown
```

### Comparing `robotframework-browser-9.0.1/robotframework_browser.egg-info/PKG-INFO` & `robotframework-browser-9.0.2/robotframework_browser.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,244 +1,242 @@
 Metadata-Version: 2.1
 Name: robotframework-browser
-Version: 9.0.1
+Version: 9.0.2
 Summary: Robot Framework Browser library powered by Playwright. Aiming for speed, reliability and visibility.
 Home-page: https://github.com/MarketSquare/robotframework-browser
 Author: MarketSquare - Robot Framework community
 Author-email: mikko.korpela@gmail.com
 License: UNKNOWN
+Description: # robotframework-browser
+        <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+        [![All Contributors](https://img.shields.io/badge/all_contributors-51-orange.svg?style=flat-square)](#contributors-)
+        <!-- ALL-CONTRIBUTORS-BADGE:END -->
+        [![Version](https://img.shields.io/pypi/v/robotframework-browser.svg)](https://pypi.python.org/pypi/robotframework-browser)
+        [![Actions Status](https://github.com/MarketSquare/robotframework-browser/workflows/Continuous%20integration/badge.svg)](https://github.com/MarketSquare/robotframework-browser/actions)
+        [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+        
+        ----
+        
+        [Robot Framework](https://robotframework.org) Browser library powered by [Playwright](https://playwright.dev/). Moving browser automation to year 2021!
+        
+        Aiming for :rocket: speed, :white_check_mark: reliability and :microscope: visibility.
+        
+        See [keyword documentation](https://marketsquare.github.io/robotframework-browser/Browser.html) and
+        [web page](https://robotframework-browser.org/) for more details.
+        
+        # Installation instructions
+        
+        Only Python 3.7 or newer is supported.
+        
+        1. Install node.js e.g. from https://nodejs.org/en/download/ (only < v15 supported; if unsure, use 14.15.0 LTS)
+        2. Update pip `pip install -U pip` to ensure latest version is used
+        3. Install robotframework-browser from the commandline: `pip install robotframework-browser`
+        4. Install the node dependencies: run `rfbrowser init` in your shell
+          - if `rfbrowser` is not found, try `python -m Browser.entry init`
+        
+        Please note that by default Chromium, Firefox and WebKit browser are installed, even those would be already
+        installed in the system. The installation size depends on the operating system, but usually is +700Mb.
+        It is possible to skip browser binaries installation with `rfbrowser init --skip-browsers` command, but then user
+        is responsible for browser binary installation.
+        
+        Or use the [docker images](https://github.com/MarketSquare/robotframework-browser/packages). Documented at [docker/README.md](https://github.com/MarketSquare/robotframework-browser/blob/main/docker/README.md).
+        
+        ## Update instructions
+        
+        To upgrade your already installed robotframework-browser library
+        
+        1. Update from commandline: `pip install -U robotframework-browser`
+        2. Clean old node side dependencies and browser binaries: `rfbrowser clean-node`
+        3. Install the node dependencies for the newly installed version: `rfbrowser init`
+        
+        ## Uninstall instructions
+        
+        To completely install library, including the browser binaries installed by Playwright,
+        run following commands:
+        1. Clean old node side dependencies and browser binaries: `rfbrowser clean-node`
+        2. Uninstall with pip: `pip uninstall robotframework-browser`
+        
+        # Examples
+        
+        ### Testing with [Robot Framework](https://robotframework.org)
+        ```RobotFramework
+        *** Settings ***
+        Library   Browser
+        
+        *** Test Cases ***
+        Example Test
+            New Page    https://playwright.dev
+            Get Text    h1    contains    Playwright
+        ```
+        ### and testing with [Python](https://python.org).
+        ```python
+        import Browser
+        browser = Browser.Browser()
+        browser.new_page("https://playwright.dev")
+        assert 'Playwright' in browser.get_text("h1")
+        browser.close_browser()
+        ```
+        
+        ### and extending with JavaScript
+        
+        ```JavaScript
+        async function myGoToKeyword(page, args) {
+          return await page.goto(args[0]);
+        }
+        exports.__esModule = true;
+        exports.myGoToKeyword = myGoToKeyword;
+        ```
+        
+        ```RobotFramework
+        *** Settings ***
+        Library   Browser  jsextension=${CURDIR}/mymodule.js
+        
+        *** Test Cases ***
+        Example Test
+           New Page
+           myGoToKeyword   https://www.robotframework.org
+        ```
+        
+        Ready made extensions and a place to share your own at [robotframework-browser-extensions](https://github.com/MarketSquare/robotframework-browser-extensions).
+        
+        ### Ergonomic selector syntax, supports chaining of `text`, `css`  and `xpath` selectors
+        
+        ```RobotFramework
+        # Select element containing text "Login" with text selector strategy 
+        # and select it's parent `input` element with xpath
+        Click    "Login" >> xpath=../input
+        # Select element with CSS strategy and select button in it with text strategy
+        Click    div.dialog >> "Ok"
+        ```
+        ### Evaluate in browser page
+        ```RobotFramework
+        New Page   ${LOGIN_URL}
+        ${ref}=    Get Element    h1
+        Get Property    ${ref}    innerText    ==    Login Page
+        Execute JavaScript    (elem) => elem.innerText = "abc"    ${ref}
+        Get Property    ${ref}    innerText    ==    abc
+        ```
+        ### Asynchronously waiting for HTTP requests and responses
+        ```RobotFramework
+        # The button with id `delayed_request` fires a delayed request. We use a promise to capture it.
+        ${promise}=    Promise To    Wait For Response    matcher=    timeout=3s
+        Click    \#delayed_request
+        ${body}=    Wait For    ${promise}
+        ```
+        ### Device Descriptors
+        ```RobotFramework
+        ${device}=  Get Device  iPhone X
+        New Context  &{device}
+        New Page
+        Get Viewport Size  # returns { "width": 375, "height": 812 }
+        ```
+        ### Sending HTTP requests and parsing their responses
+        ```RobotFramework
+        &{response}=    HTTP    /api/post    POST    {"name": "John"}
+        Should Be Equal    ${response.status}    ${200}
+        ```
+        # Development
+        
+        See [CONTRIBUTING.md](CONTRIBUTING.md) for development instructions.
+        
+        ## Core team
+        
+        In order of appearance.
+        
+          * Mikko Korpela
+          * Tatu Aalto
+          * Janne Härkönen (Alumnus)
+          * Kerkko Pelttari
+          * René Rohner
+        
+        ## Contributors
+        
+        This project is community driven and becomes a reality only through the work of all the people who contribute.
+        Supported by [Robocorp](https://robocorp.com/) through [Robot Framework Foundation](https://robotframework.org/foundation/).
+        <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+        <!-- prettier-ignore-start -->
+        <!-- markdownlint-disable -->
+        <table>
+          <tr>
+            <td align="center"><a href="https://github.com/mkorpela"><img src="https://avatars1.githubusercontent.com/u/136885?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Mikko Korpela</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=mkorpela" title="Code">💻</a></td>
+            <td align="center"><a href="https://github.com/aaltat"><img src="https://avatars0.githubusercontent.com/u/2665023?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Tatu Aalto</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=aaltat" title="Code">💻</a></td>
+            <td align="center"><a href="https://robocorp.com"><img src="https://avatars1.githubusercontent.com/u/8512727?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Antti Karjalainen</b></sub></a><br /><a href="#fundingFinding-aikarjal" title="Funding Finding">🔍</a></td>
+            <td align="center"><a href="https://www.linkedin.com/in/ismoaro/"><img src="https://avatars2.githubusercontent.com/u/1047173?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ismo Aro</b></sub></a><br /><a href="#fundingFinding-IsNoGood" title="Funding Finding">🔍</a></td>
+            <td align="center"><a href="https://twitter.com/janneharkonen"><img src="https://avatars3.githubusercontent.com/u/159146?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Janne Härkönen</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=yanne" title="Code">💻</a></td>
+            <td align="center"><a href="http://xylix.fi"><img src="https://avatars1.githubusercontent.com/u/13387304?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Kerkko Pelttari</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=xylix" title="Code">💻</a></td>
+            <td align="center"><a href="https://robocorp.com"><img src="https://avatars3.githubusercontent.com/u/54288445?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Robocorp</b></sub></a><br /><a href="#financial-robocorp" title="Financial">💵</a></td>
+          </tr>
+          <tr>
+            <td align="center"><a href="https://github.com/Snooz82"><img src="https://avatars0.githubusercontent.com/u/41592183?v=4?s=100" width="100px;" alt=""/><br /><sub><b>René</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=Snooz82" title="Code">💻</a></td>
+            <td align="center"><a href="https://wordpress.com/read/feeds/39696435"><img src="https://avatars0.githubusercontent.com/u/1123938?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Bryan Oakley</b></sub></a><br /><a href="#ideas-boakley" title="Ideas, Planning, & Feedback">🤔</a></td>
+            <td align="center"><a href="https://github.com/idxn"><img src="https://avatars3.githubusercontent.com/u/2438992?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Tanakiat Srisaranyakul</b></sub></a><br /><a href="#ideas-idxn" title="Ideas, Planning, & Feedback">🤔</a></td>
+            <td align="center"><a href="http://visible-quality.blogspot.com"><img src="https://avatars1.githubusercontent.com/u/5338157?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Maaret Pyhäjärvi</b></sub></a><br /><a href="#userTesting-maaretp" title="User Testing">📓</a></td>
+            <td align="center"><a href="http://www.tentamen.eu"><img src="https://avatars2.githubusercontent.com/u/777520?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Karlo Smid</b></sub></a><br /><a href="#userTesting-karlosmid" title="User Testing">📓</a></td>
+            <td align="center"><a href="https://github.com/aspargillus"><img src="https://avatars0.githubusercontent.com/u/4592889?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Frank Schimmel</b></sub></a><br /><a href="#userTesting-Aspargillus" title="User Testing">📓</a></td>
+            <td align="center"><a href="https://github.com/tuxmux28"><img src="https://avatars3.githubusercontent.com/u/2794048?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Christoph</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=tuxmux28" title="Tests">⚠️</a></td>
+          </tr>
+          <tr>
+            <td align="center"><a href="https://github.com/mikahanninen"><img src="https://avatars2.githubusercontent.com/u/1019528?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Mika Hänninen</b></sub></a><br /><a href="#question-mikahanninen" title="Answering Questions">💬</a></td>
+            <td align="center"><a href="https://www.imbus.de"><img src="https://avatars0.githubusercontent.com/u/67375753?v=4?s=100" width="100px;" alt=""/><br /><sub><b>imbus</b></sub></a><br /><a href="#financial-imbus" title="Financial">💵</a></td>
+            <td align="center"><a href="https://github.com/Finalrykku"><img src="https://avatars0.githubusercontent.com/u/19802569?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Niklas</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=Finalrykku" title="Documentation">📖</a></td>
+            <td align="center"><a href="https://github.com/gdroes"><img src="https://avatars1.githubusercontent.com/u/6716450?v=4?s=100" width="100px;" alt=""/><br /><sub><b>gdroes</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=gdroes" title="Tests">⚠️</a></td>
+            <td align="center"><a href="https://reaktor.com"><img src="https://avatars2.githubusercontent.com/u/71799?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Reaktor</b></sub></a><br /><a href="#financial-reaktor" title="Financial">💵</a></td>
+            <td align="center"><a href="https://github.com/adrianyorke"><img src="https://avatars1.githubusercontent.com/u/30093433?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Adrian Yorke</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=adrianyorke" title="Documentation">📖</a> <a href="https://github.com/MarketSquare/robotframework-browser/pulls?q=is%3Apr+reviewed-by%3Aadrianyorke" title="Reviewed Pull Requests">👀</a></td>
+            <td align="center"><a href="https://github.com/wangzimeiyingtao"><img src="https://avatars0.githubusercontent.com/u/70925596?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nanakawa</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=wangzimeiyingtao" title="Tests">⚠️</a></td>
+          </tr>
+          <tr>
+            <td align="center"><a href="https://github.com/emanlove"><img src="https://avatars1.githubusercontent.com/u/993527?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ed Manlove</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=emanlove" title="Documentation">📖</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aemanlove" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/estimation"><img src="https://avatars1.githubusercontent.com/u/16793171?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Brian Tsao</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aestimation" title="Bug reports">🐛</a> <a href="#userTesting-estimation" title="User Testing">📓</a></td>
+            <td align="center"><a href="https://github.com/mawentao119"><img src="https://avatars0.githubusercontent.com/u/26617186?v=4?s=100" width="100px;" alt=""/><br /><sub><b>charis</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=mawentao119" title="Code">💻</a></td>
+            <td align="center"><a href="https://github.com/s-galante"><img src="https://avatars2.githubusercontent.com/u/4580052?v=4?s=100" width="100px;" alt=""/><br /><sub><b>s-galante</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3As-galante" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="http://www.elabit.de"><img src="https://avatars3.githubusercontent.com/u/1897410?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Simon Meggle</b></sub></a><br /><a href="#userTesting-simonmeggle" title="User Testing">📓</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Asimonmeggle" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/Anna-Gunda"><img src="https://avatars3.githubusercontent.com/u/13298792?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Anna-Gunda</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AAnna-Gunda" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/anton264"><img src="https://avatars0.githubusercontent.com/u/10194266?v=4?s=100" width="100px;" alt=""/><br /><sub><b>anton264</b></sub></a><br /><a href="#userTesting-anton264" title="User Testing">📓</a></td>
+          </tr>
+          <tr>
+            <td align="center"><a href="https://github.com/emakaay"><img src="https://avatars.githubusercontent.com/u/72747481?v=4?s=100" width="100px;" alt=""/><br /><sub><b>emakaay</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aemakaay" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://virvatuli.itch.io/"><img src="https://avatars.githubusercontent.com/u/29060467?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nea Ohvo</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AVirvatuli" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/leeuwe"><img src="https://avatars.githubusercontent.com/u/66635066?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Elout van Leeuwen</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=leeuwe" title="Documentation">📖</a></td>
+            <td align="center"><a href="https://github.com/LDerikx"><img src="https://avatars.githubusercontent.com/u/26576024?v=4?s=100" width="100px;" alt=""/><br /><sub><b>LDerikx</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=LDerikx" title="Documentation">📖</a></td>
+            <td align="center"><a href="https://github.com/olga-"><img src="https://avatars.githubusercontent.com/u/9334057?v=4?s=100" width="100px;" alt=""/><br /><sub><b>olga-</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=olga-" title="Documentation">📖</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aolga-" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/bollwyvl"><img src="https://avatars.githubusercontent.com/u/45380?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nicholas Bollweg</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=bollwyvl" title="Documentation">📖</a></td>
+            <td align="center"><a href="http://villesalonen.fi"><img src="https://avatars.githubusercontent.com/u/1070813?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ville Salonen</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AVilleSalonen" title="Bug reports">🐛</a></td>
+          </tr>
+          <tr>
+            <td align="center"><a href="https://rasjani.github.io"><img src="https://avatars.githubusercontent.com/u/27887?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jani Mikkonen</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Arasjani" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/JaPyR"><img src="https://avatars.githubusercontent.com/u/7773301?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Aleh Borysiewicz</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AJaPyR" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="http://www.binary-overflow.de"><img src="https://avatars.githubusercontent.com/u/25060709?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jürgen Knauth</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Ajkpubsrc" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/dalaakso"><img src="https://avatars.githubusercontent.com/u/50731554?v=4?s=100" width="100px;" alt=""/><br /><sub><b>dalaakso</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Adalaakso" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/msirkka"><img src="https://avatars.githubusercontent.com/u/84907426?v=4?s=100" width="100px;" alt=""/><br /><sub><b>msirkka</b></sub></a><br /><a href="#ideas-msirkka" title="Ideas, Planning, & Feedback">🤔</a></td>
+            <td align="center"><a href="https://github.com/osrjv"><img src="https://avatars.githubusercontent.com/u/29481017?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ossi R.</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=osrjv" title="Code">💻</a></td>
+            <td align="center"><a href="https://github.com/adrian-evo"><img src="https://avatars.githubusercontent.com/u/19324942?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Adrian V.</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=adrian-evo" title="Code">💻</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aadrian-evo" title="Bug reports">🐛</a> <a href="#ideas-adrian-evo" title="Ideas, Planning, & Feedback">🤔</a></td>
+          </tr>
+          <tr>
+            <td align="center"><a href="https://github.com/ssallmen"><img src="https://avatars.githubusercontent.com/u/39527407?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Sami Sallmén</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Assallmen" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="http://eliga.fi"><img src="https://avatars.githubusercontent.com/u/114985?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Pekka Klärck</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=pekkaklarck" title="Code">💻</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Apekkaklarck" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/janipalsamaki"><img src="https://avatars.githubusercontent.com/u/1157184?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jani Palsamäki</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Ajanipalsamaki" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/AllanMedeiros"><img src="https://avatars.githubusercontent.com/u/34678196?v=4?s=100" width="100px;" alt=""/><br /><sub><b>AllanMedeiros</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AAllanMedeiros" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/ealap"><img src="https://avatars.githubusercontent.com/u/15620712?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Emmanuel Alap</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aealap" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/ankurbhalla-gmail"><img src="https://avatars.githubusercontent.com/u/90744440?v=4?s=100" width="100px;" alt=""/><br /><sub><b>ankurbhalla-gmail</b></sub></a><br /><a href="#ideas-ankurbhalla-gmail" title="Ideas, Planning, & Feedback">🤔</a></td>
+            <td align="center"><a href="https://github.com/UliSei"><img src="https://avatars.githubusercontent.com/u/89480399?v=4?s=100" width="100px;" alt=""/><br /><sub><b>UliSei</b></sub></a><br /><a href="#ideas-UliSei" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AUliSei" title="Bug reports">🐛</a> <a href="https://github.com/MarketSquare/robotframework-browser/commits?author=UliSei" title="Code">💻</a></td>
+          </tr>
+          <tr>
+            <td align="center"><a href="https://github.com/tomekTieto"><img src="https://avatars.githubusercontent.com/u/39945193?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Tomasz Pawlak</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AtomekTieto" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/mtoskamp"><img src="https://avatars.githubusercontent.com/u/58772827?v=4?s=100" width="100px;" alt=""/><br /><sub><b>mtoskamp</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Amtoskamp" title="Bug reports">🐛</a></td>
+          </tr>
+        </table>
+        
+        <!-- markdownlint-restore -->
+        <!-- prettier-ignore-end -->
+        
+        <!-- ALL-CONTRIBUTORS-LIST:END -->
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Testing
 Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library
 Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# robotframework-browser
-<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-50-orange.svg?style=flat-square)](#contributors-)
-<!-- ALL-CONTRIBUTORS-BADGE:END -->
-[![Version](https://img.shields.io/pypi/v/robotframework-browser.svg)](https://pypi.python.org/pypi/robotframework-browser)
-[![Actions Status](https://github.com/MarketSquare/robotframework-browser/workflows/Continuous%20integration/badge.svg)](https://github.com/MarketSquare/robotframework-browser/actions)
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-
-----
-
-[Robot Framework](https://robotframework.org) Browser library powered by [Playwright](https://playwright.dev/). Moving browser automation to year 2021!
-
-Aiming for :rocket: speed, :white_check_mark: reliability and :microscope: visibility.
-
-See [keyword documentation](https://marketsquare.github.io/robotframework-browser/Browser.html) and
-[web page](https://robotframework-browser.org/) for more details.
-
-# Installation instructions
-
-Only Python 3.7 or newer is supported.
-
-1. Install node.js e.g. from https://nodejs.org/en/download/ (only < v15 supported; if unsure, use 14.15.0 LTS)
-2. Update pip `pip install -U pip` to ensure latest version is used
-3. Install robotframework-browser from the commandline: `pip install robotframework-browser`
-4. Install the node dependencies: run `rfbrowser init` in your shell
-  - if `rfbrowser` is not found, try `python -m Browser.entry init`
-
-Please note that by default Chromium, Firefox and WebKit browser are installed, even those would be already
-installed in the system. The installation size depends on the operating system, but usually is +700Mb.
-It is possible to skip browser binaries installation with `rfbrowser init --skip-browsers` command, but then user
-is responsible for browser binary installation.
-
-Or use the [docker images](https://github.com/MarketSquare/robotframework-browser/packages). Documented at [docker/README.md](https://github.com/MarketSquare/robotframework-browser/blob/main/docker/README.md).
-
-## Update instructions
-
-To upgrade your already installed robotframework-browser library
-
-1. Update from commandline: `pip install -U robotframework-browser`
-2. Clean old node side dependencies and browser binaries: `rfbrowser clean-node`
-3. Install the node dependencies for the newly installed version: `rfbrowser init`
-
-## Uninstall instructions
-
-To completely install library, including the browser binaries installed by Playwright,
-run following commands:
-1. Clean old node side dependencies and browser binaries: `rfbrowser clean-node`
-2. Uninstall with pip: `pip uninstall robotframework-browser`
-
-# Examples
-
-### Testing with [Robot Framework](https://robotframework.org)
-```RobotFramework
-*** Settings ***
-Library   Browser
-
-*** Test Cases ***
-Example Test
-    New Page    https://playwright.dev
-    Get Text    h1    contains    Playwright
-```
-### and testing with [Python](https://python.org).
-```python
-import Browser
-browser = Browser.Browser()
-browser.new_page("https://playwright.dev")
-assert 'Playwright' in browser.get_text("h1")
-browser.close_browser()
-```
-
-### and extending with JavaScript
-
-```JavaScript
-async function myGoToKeyword(page, args) {
-  return await page.goto(args[0]);
-}
-exports.__esModule = true;
-exports.myGoToKeyword = myGoToKeyword;
-```
-
-```RobotFramework
-*** Settings ***
-Library   Browser  jsextension=${CURDIR}/mymodule.js
-
-*** Test Cases ***
-Example Test
-   New Page
-   myGoToKeyword   https://www.robotframework.org
-```
-
-Ready made extensions and a place to share your own at [robotframework-browser-extensions](https://github.com/MarketSquare/robotframework-browser-extensions).
-
-### Ergonomic selector syntax, supports chaining of `text`, `css`  and `xpath` selectors
-
-```RobotFramework
-# Select element containing text "Login" with text selector strategy 
-# and select it's parent `input` element with xpath
-Click    "Login" >> xpath=../input
-# Select element with CSS strategy and select button in it with text strategy
-Click    div.dialog >> "Ok"
-```
-### Evaluate in browser page
-```RobotFramework
-New Page   ${LOGIN_URL}
-${ref}=    Get Element    h1
-Get Property    ${ref}    innerText    ==    Login Page
-Execute JavaScript    (elem) => elem.innerText = "abc"    ${ref}
-Get Property    ${ref}    innerText    ==    abc
-```
-### Asynchronously waiting for HTTP requests and responses
-```RobotFramework
-# The button with id `delayed_request` fires a delayed request. We use a promise to capture it.
-${promise}=    Promise To    Wait For Response    matcher=    timeout=3s
-Click    \#delayed_request
-${body}=    Wait For    ${promise}
-```
-### Device Descriptors
-```RobotFramework
-${device}=  Get Device  iPhone X
-New Context  &{device}
-New Page
-Get Viewport Size  # returns { "width": 375, "height": 812 }
-```
-### Sending HTTP requests and parsing their responses
-```RobotFramework
-&{response}=    HTTP    /api/post    POST    {"name": "John"}
-Should Be Equal    ${response.status}    ${200}
-```
-# Development
-
-See [CONTRIBUTING.md](CONTRIBUTING.md) for development instructions.
-
-## Core team
-
-In order of appearance.
-
-  * Mikko Korpela
-  * Tatu Aalto
-  * Janne Härkönen (Alumnus)
-  * Kerkko Pelttari
-  * René Rohner
-
-## Contributors
-
-This project is community driven and becomes a reality only through the work of all the people who contribute.
-Supported by [Robocorp](https://robocorp.com/) through [Robot Framework Foundation](https://robotframework.org/foundation/).
-<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
-<!-- prettier-ignore-start -->
-<!-- markdownlint-disable -->
-<table>
-  <tr>
-    <td align="center"><a href="https://github.com/mkorpela"><img src="https://avatars1.githubusercontent.com/u/136885?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Mikko Korpela</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=mkorpela" title="Code">💻</a></td>
-    <td align="center"><a href="https://github.com/aaltat"><img src="https://avatars0.githubusercontent.com/u/2665023?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Tatu Aalto</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=aaltat" title="Code">💻</a></td>
-    <td align="center"><a href="https://robocorp.com"><img src="https://avatars1.githubusercontent.com/u/8512727?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Antti Karjalainen</b></sub></a><br /><a href="#fundingFinding-aikarjal" title="Funding Finding">🔍</a></td>
-    <td align="center"><a href="https://www.linkedin.com/in/ismoaro/"><img src="https://avatars2.githubusercontent.com/u/1047173?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ismo Aro</b></sub></a><br /><a href="#fundingFinding-IsNoGood" title="Funding Finding">🔍</a></td>
-    <td align="center"><a href="https://twitter.com/janneharkonen"><img src="https://avatars3.githubusercontent.com/u/159146?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Janne Härkönen</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=yanne" title="Code">💻</a></td>
-    <td align="center"><a href="http://xylix.fi"><img src="https://avatars1.githubusercontent.com/u/13387304?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Kerkko Pelttari</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=xylix" title="Code">💻</a></td>
-    <td align="center"><a href="https://robocorp.com"><img src="https://avatars3.githubusercontent.com/u/54288445?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Robocorp</b></sub></a><br /><a href="#financial-robocorp" title="Financial">💵</a></td>
-  </tr>
-  <tr>
-    <td align="center"><a href="https://github.com/Snooz82"><img src="https://avatars0.githubusercontent.com/u/41592183?v=4?s=100" width="100px;" alt=""/><br /><sub><b>René</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=Snooz82" title="Code">💻</a></td>
-    <td align="center"><a href="https://wordpress.com/read/feeds/39696435"><img src="https://avatars0.githubusercontent.com/u/1123938?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Bryan Oakley</b></sub></a><br /><a href="#ideas-boakley" title="Ideas, Planning, & Feedback">🤔</a></td>
-    <td align="center"><a href="https://github.com/idxn"><img src="https://avatars3.githubusercontent.com/u/2438992?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Tanakiat Srisaranyakul</b></sub></a><br /><a href="#ideas-idxn" title="Ideas, Planning, & Feedback">🤔</a></td>
-    <td align="center"><a href="http://visible-quality.blogspot.com"><img src="https://avatars1.githubusercontent.com/u/5338157?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Maaret Pyhäjärvi</b></sub></a><br /><a href="#userTesting-maaretp" title="User Testing">📓</a></td>
-    <td align="center"><a href="http://www.tentamen.eu"><img src="https://avatars2.githubusercontent.com/u/777520?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Karlo Smid</b></sub></a><br /><a href="#userTesting-karlosmid" title="User Testing">📓</a></td>
-    <td align="center"><a href="https://github.com/aspargillus"><img src="https://avatars0.githubusercontent.com/u/4592889?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Frank Schimmel</b></sub></a><br /><a href="#userTesting-Aspargillus" title="User Testing">📓</a></td>
-    <td align="center"><a href="https://github.com/tuxmux28"><img src="https://avatars3.githubusercontent.com/u/2794048?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Christoph</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=tuxmux28" title="Tests">⚠️</a></td>
-  </tr>
-  <tr>
-    <td align="center"><a href="https://github.com/mikahanninen"><img src="https://avatars2.githubusercontent.com/u/1019528?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Mika Hänninen</b></sub></a><br /><a href="#question-mikahanninen" title="Answering Questions">💬</a></td>
-    <td align="center"><a href="https://www.imbus.de"><img src="https://avatars0.githubusercontent.com/u/67375753?v=4?s=100" width="100px;" alt=""/><br /><sub><b>imbus</b></sub></a><br /><a href="#financial-imbus" title="Financial">💵</a></td>
-    <td align="center"><a href="https://github.com/Finalrykku"><img src="https://avatars0.githubusercontent.com/u/19802569?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Niklas</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=Finalrykku" title="Documentation">📖</a></td>
-    <td align="center"><a href="https://github.com/gdroes"><img src="https://avatars1.githubusercontent.com/u/6716450?v=4?s=100" width="100px;" alt=""/><br /><sub><b>gdroes</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=gdroes" title="Tests">⚠️</a></td>
-    <td align="center"><a href="https://reaktor.com"><img src="https://avatars2.githubusercontent.com/u/71799?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Reaktor</b></sub></a><br /><a href="#financial-reaktor" title="Financial">💵</a></td>
-    <td align="center"><a href="https://github.com/adrianyorke"><img src="https://avatars1.githubusercontent.com/u/30093433?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Adrian Yorke</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=adrianyorke" title="Documentation">📖</a> <a href="https://github.com/MarketSquare/robotframework-browser/pulls?q=is%3Apr+reviewed-by%3Aadrianyorke" title="Reviewed Pull Requests">👀</a></td>
-    <td align="center"><a href="https://github.com/wangzimeiyingtao"><img src="https://avatars0.githubusercontent.com/u/70925596?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nanakawa</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=wangzimeiyingtao" title="Tests">⚠️</a></td>
-  </tr>
-  <tr>
-    <td align="center"><a href="https://github.com/emanlove"><img src="https://avatars1.githubusercontent.com/u/993527?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ed Manlove</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=emanlove" title="Documentation">📖</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aemanlove" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/estimation"><img src="https://avatars1.githubusercontent.com/u/16793171?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Brian Tsao</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aestimation" title="Bug reports">🐛</a> <a href="#userTesting-estimation" title="User Testing">📓</a></td>
-    <td align="center"><a href="https://github.com/mawentao119"><img src="https://avatars0.githubusercontent.com/u/26617186?v=4?s=100" width="100px;" alt=""/><br /><sub><b>charis</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=mawentao119" title="Code">💻</a></td>
-    <td align="center"><a href="https://github.com/s-galante"><img src="https://avatars2.githubusercontent.com/u/4580052?v=4?s=100" width="100px;" alt=""/><br /><sub><b>s-galante</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3As-galante" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="http://www.elabit.de"><img src="https://avatars3.githubusercontent.com/u/1897410?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Simon Meggle</b></sub></a><br /><a href="#userTesting-simonmeggle" title="User Testing">📓</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Asimonmeggle" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/Anna-Gunda"><img src="https://avatars3.githubusercontent.com/u/13298792?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Anna-Gunda</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AAnna-Gunda" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/anton264"><img src="https://avatars0.githubusercontent.com/u/10194266?v=4?s=100" width="100px;" alt=""/><br /><sub><b>anton264</b></sub></a><br /><a href="#userTesting-anton264" title="User Testing">📓</a></td>
-  </tr>
-  <tr>
-    <td align="center"><a href="https://github.com/emakaay"><img src="https://avatars.githubusercontent.com/u/72747481?v=4?s=100" width="100px;" alt=""/><br /><sub><b>emakaay</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aemakaay" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://virvatuli.itch.io/"><img src="https://avatars.githubusercontent.com/u/29060467?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nea Ohvo</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AVirvatuli" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/leeuwe"><img src="https://avatars.githubusercontent.com/u/66635066?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Elout van Leeuwen</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=leeuwe" title="Documentation">📖</a></td>
-    <td align="center"><a href="https://github.com/LDerikx"><img src="https://avatars.githubusercontent.com/u/26576024?v=4?s=100" width="100px;" alt=""/><br /><sub><b>LDerikx</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=LDerikx" title="Documentation">📖</a></td>
-    <td align="center"><a href="https://github.com/olga-"><img src="https://avatars.githubusercontent.com/u/9334057?v=4?s=100" width="100px;" alt=""/><br /><sub><b>olga-</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=olga-" title="Documentation">📖</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aolga-" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/bollwyvl"><img src="https://avatars.githubusercontent.com/u/45380?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nicholas Bollweg</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=bollwyvl" title="Documentation">📖</a></td>
-    <td align="center"><a href="http://villesalonen.fi"><img src="https://avatars.githubusercontent.com/u/1070813?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ville Salonen</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AVilleSalonen" title="Bug reports">🐛</a></td>
-  </tr>
-  <tr>
-    <td align="center"><a href="https://rasjani.github.io"><img src="https://avatars.githubusercontent.com/u/27887?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jani Mikkonen</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Arasjani" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/JaPyR"><img src="https://avatars.githubusercontent.com/u/7773301?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Aleh Borysiewicz</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AJaPyR" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="http://www.binary-overflow.de"><img src="https://avatars.githubusercontent.com/u/25060709?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jürgen Knauth</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Ajkpubsrc" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/dalaakso"><img src="https://avatars.githubusercontent.com/u/50731554?v=4?s=100" width="100px;" alt=""/><br /><sub><b>dalaakso</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Adalaakso" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/msirkka"><img src="https://avatars.githubusercontent.com/u/84907426?v=4?s=100" width="100px;" alt=""/><br /><sub><b>msirkka</b></sub></a><br /><a href="#ideas-msirkka" title="Ideas, Planning, & Feedback">🤔</a></td>
-    <td align="center"><a href="https://github.com/osrjv"><img src="https://avatars.githubusercontent.com/u/29481017?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ossi R.</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=osrjv" title="Code">💻</a></td>
-    <td align="center"><a href="https://github.com/adrian-evo"><img src="https://avatars.githubusercontent.com/u/19324942?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Adrian V.</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=adrian-evo" title="Code">💻</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aadrian-evo" title="Bug reports">🐛</a> <a href="#ideas-adrian-evo" title="Ideas, Planning, & Feedback">🤔</a></td>
-  </tr>
-  <tr>
-    <td align="center"><a href="https://github.com/ssallmen"><img src="https://avatars.githubusercontent.com/u/39527407?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Sami Sallmén</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Assallmen" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="http://eliga.fi"><img src="https://avatars.githubusercontent.com/u/114985?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Pekka Klärck</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/commits?author=pekkaklarck" title="Code">💻</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Apekkaklarck" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/janipalsamaki"><img src="https://avatars.githubusercontent.com/u/1157184?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jani Palsamäki</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Ajanipalsamaki" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/AllanMedeiros"><img src="https://avatars.githubusercontent.com/u/34678196?v=4?s=100" width="100px;" alt=""/><br /><sub><b>AllanMedeiros</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AAllanMedeiros" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/ealap"><img src="https://avatars.githubusercontent.com/u/15620712?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Emmanuel Alap</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3Aealap" title="Bug reports">🐛</a></td>
-    <td align="center"><a href="https://github.com/ankurbhalla-gmail"><img src="https://avatars.githubusercontent.com/u/90744440?v=4?s=100" width="100px;" alt=""/><br /><sub><b>ankurbhalla-gmail</b></sub></a><br /><a href="#ideas-ankurbhalla-gmail" title="Ideas, Planning, & Feedback">🤔</a></td>
-    <td align="center"><a href="https://github.com/UliSei"><img src="https://avatars.githubusercontent.com/u/89480399?v=4?s=100" width="100px;" alt=""/><br /><sub><b>UliSei</b></sub></a><br /><a href="#ideas-UliSei" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AUliSei" title="Bug reports">🐛</a> <a href="https://github.com/MarketSquare/robotframework-browser/commits?author=UliSei" title="Code">💻</a></td>
-  </tr>
-  <tr>
-    <td align="center"><a href="https://github.com/tomekTieto"><img src="https://avatars.githubusercontent.com/u/39945193?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Tomasz Pawlak</b></sub></a><br /><a href="https://github.com/MarketSquare/robotframework-browser/issues?q=author%3AtomekTieto" title="Bug reports">🐛</a></td>
-  </tr>
-</table>
-
-<!-- markdownlint-restore -->
-<!-- prettier-ignore-end -->
-
-<!-- ALL-CONTRIBUTORS-LIST:END -->
-
-
```

### Comparing `robotframework-browser-9.0.1/robotframework_browser.egg-info/SOURCES.txt` & `robotframework-browser-9.0.2/robotframework_browser.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 Browser/__init__.py
-Browser/__init__.pyi
 Browser/assertion_engine.py
 Browser/browser.py
-Browser/dev-requirements.txt
 Browser/entry.py
 Browser/gen_stub.py
-Browser/mypy.ini
 Browser/playwright.py
-Browser/pyproject.toml
-Browser/requirements.txt
 Browser/version.py
 Browser/base/__init__.py
 Browser/base/cache.py
 Browser/base/librarycomponent.py
 Browser/generated/__init__.py
 Browser/generated/playwright_pb2.py
-Browser/generated/playwright_pb2.pyi
 Browser/generated/playwright_pb2_grpc.py
 Browser/keywords/__init__.py
 Browser/keywords/browser_control.py
 Browser/keywords/cookie.py
 Browser/keywords/crawling.py
 Browser/keywords/device_descriptors.py
 Browser/keywords/evaluation.py
@@ -40,16 +34,13 @@
 Browser/utils/data_types.py
 Browser/utils/deprecated.py
 Browser/utils/js_utilities.py
 Browser/utils/logger.py
 Browser/utils/meta_python.py
 Browser/utils/misc.py
 Browser/utils/robot_booleans.py
-Browser/wrapper/index.js
-Browser/wrapper/package-lock.json
-Browser/wrapper/package.json
 robotframework_browser.egg-info/PKG-INFO
 robotframework_browser.egg-info/SOURCES.txt
 robotframework_browser.egg-info/dependency_links.txt
 robotframework_browser.egg-info/entry_points.txt
 robotframework_browser.egg-info/requires.txt
 robotframework_browser.egg-info/top_level.txt
```

### Comparing `robotframework-browser-9.0.1/setup.py` & `robotframework-browser-9.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     ],
 }
 
 install_requires = open(os.path.join("Browser", "requirements.txt")).readlines()
 
 setup_kwargs = {
     "name": "robotframework-browser",
-    "version": "9.0.1",
+    "version": "9.0.2",
     "description": "Robot Framework Browser library powered by Playwright. Aiming for speed, reliability and visibility.",
     "long_description": long_description,
     "long_description_content_type": "text/markdown",
     "author": "MarketSquare - Robot Framework community",
     "author_email": "mikko.korpela@gmail.com",
     "maintainer": None,
     "maintainer_email": None,
```

