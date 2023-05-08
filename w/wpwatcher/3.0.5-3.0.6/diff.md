# Comparing `tmp/wpwatcher-3.0.5.tar.gz` & `tmp/wpwatcher-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wpwatcher-3.0.5.tar", last modified: Tue Jan  3 20:06:05 2023, max compression
+gzip compressed data, was "wpwatcher-3.0.6.tar", last modified: Mon May  8 19:41:26 2023, max compression
```

## Comparing `wpwatcher-3.0.5.tar` & `wpwatcher-3.0.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 20:06:04.996547 wpwatcher-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-01-03 20:06:04.992547 wpwatcher-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-03 20:06:04.996547 wpwatcher-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 20:06:04.992547 wpwatcher-3.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/tests/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/tests/config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/tests/core_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/tests/db_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/tests/notification_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/tests/scan_random_sites.py
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/tests/scan_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/tests/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/tests/wpscan_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 20:06:04.992547 wpwatcher-3.0.5/wpwatcher/
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/wpwatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/wpwatcher/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/wpwatcher/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/wpwatcher/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/wpwatcher/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/wpwatcher/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/wpwatcher/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/wpwatcher/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    15226 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/wpwatcher/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/wpwatcher/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/wpwatcher/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/wpwatcher/site.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/wpwatcher/syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/wpwatcher/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-01-03 20:06:00.000000 wpwatcher-3.0.5/wpwatcher/wpscan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 20:06:04.992547 wpwatcher-3.0.5/wpwatcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-01-03 20:06:04.000000 wpwatcher-3.0.5/wpwatcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-01-03 20:06:04.000000 wpwatcher-3.0.5/wpwatcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 20:06:04.000000 wpwatcher-3.0.5/wpwatcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-03 20:06:04.000000 wpwatcher-3.0.5/wpwatcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-01-03 20:06:04.000000 wpwatcher-3.0.5/wpwatcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-03 20:06:04.000000 wpwatcher-3.0.5/wpwatcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:41:26.027489 wpwatcher-3.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-08 19:41:26.027489 wpwatcher-3.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 19:41:26.027489 wpwatcher-3.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:41:26.027489 wpwatcher-3.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/tests/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/tests/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/tests/core_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/tests/db_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/tests/notification_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/tests/scan_random_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/tests/scan_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/tests/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/tests/wpscan_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:41:26.027489 wpwatcher-3.0.6/wpwatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/wpwatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/wpwatcher/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/wpwatcher/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/wpwatcher/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/wpwatcher/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/wpwatcher/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/wpwatcher/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/wpwatcher/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15226 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/wpwatcher/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/wpwatcher/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/wpwatcher/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/wpwatcher/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/wpwatcher/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/wpwatcher/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-05-08 19:41:16.000000 wpwatcher-3.0.6/wpwatcher/wpscan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:41:26.027489 wpwatcher-3.0.6/wpwatcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-08 19:41:26.000000 wpwatcher-3.0.6/wpwatcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-08 19:41:26.000000 wpwatcher-3.0.6/wpwatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:41:26.000000 wpwatcher-3.0.6/wpwatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-08 19:41:26.000000 wpwatcher-3.0.6/wpwatcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-08 19:41:26.000000 wpwatcher-3.0.6/wpwatcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 19:41:26.000000 wpwatcher-3.0.6/wpwatcher.egg-info/top_level.txt
```

### Comparing `wpwatcher-3.0.5/LICENSE` & `wpwatcher-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/PKG-INFO` & `wpwatcher-3.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpwatcher
-Version: 3.0.5
+Version: 3.0.6
 Summary: WPWatcher - Automating WPScan to scan and report vulnerable Wordpress sites
 Home-page: https://github.com/tristanlatr/WPWatcher
 Maintainer: Florian Roth, Tristan Landes
 License: Apache License 2.0
 Keywords: wpscan auto multiple bulk batch scan wordpress email report alerts warnings service automate mass vulnerable sites asynchronous syslog
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wpwatcher Version: 3.0.5 Summary: WPWatcher -
+Metadata-Version: 2.1 Name: wpwatcher Version: 3.0.6 Summary: WPWatcher -
 Automating WPScan to scan and report vulnerable Wordpress sites Home-page:
 https://github.com/tristanlatr/WPWatcher Maintainer: Florian Roth, Tristan
 Landes License: Apache License 2.0 Keywords: wpscan auto multiple bulk batch
 scan wordpress email report alerts warnings service automate mass vulnerable
 sites asynchronous syslog Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Information Technology Classifier:
 Environment :: Console Classifier: Topic :: Security Classifier: Topic ::
```

### Comparing `wpwatcher-3.0.5/README.md` & `wpwatcher-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/setup.py` & `wpwatcher-3.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/tests/cli_test.py` & `wpwatcher-3.0.6/tests/cli_test.py`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/tests/config_test.py` & `wpwatcher-3.0.6/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/tests/core_test.py` & `wpwatcher-3.0.6/tests/core_test.py`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/tests/db_test.py` & `wpwatcher-3.0.6/tests/db_test.py`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/tests/notification_test.py` & `wpwatcher-3.0.6/tests/notification_test.py`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/tests/scan_random_sites.py` & `wpwatcher-3.0.6/tests/scan_random_sites.py`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/tests/scan_test.py` & `wpwatcher-3.0.6/tests/scan_test.py`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/wpwatcher/__init__.py` & `wpwatcher-3.0.6/wpwatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/wpwatcher/__version__.py` & `wpwatcher-3.0.6/wpwatcher/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Wordpress Watcher
 Automating WPscan to scan and report vulnerable Wordpress sites
 
 Project version and meta informations.
 """
 
-__version__ = "3.0.5"
+__version__ = "3.0.6"
 __title__ = "wpwatcher"
 __description__ = "WPWatcher - Automating WPScan to scan and report vulnerable Wordpress sites"
 __author__ = "Florian Roth, Tristan Landes"
 __author_email__ = ""
 __license__ = "Apache License 2.0"
 __url__ = "https://github.com/tristanlatr/WPWatcher"
 __keywords__ = "wpscan auto multiple bulk batch scan wordpress email report alerts warnings service automate mass vulnerable sites asynchronous syslog"
```

### Comparing `wpwatcher-3.0.5/wpwatcher/cli.py` & `wpwatcher-3.0.6/wpwatcher/cli.py`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/wpwatcher/config.py` & `wpwatcher-3.0.6/wpwatcher/config.py`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/wpwatcher/core.py` & `wpwatcher-3.0.6/wpwatcher/core.py`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/wpwatcher/daemon.py` & `wpwatcher-3.0.6/wpwatcher/daemon.py`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/wpwatcher/db.py` & `wpwatcher-3.0.6/wpwatcher/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,17 +37,21 @@
 
         self._data = ReportCollection()
         self._data.extend(self._build_db(self.filepath))
 
         # Writing into the database file is thread safe
         self._wp_report_lock: threading.Lock = threading.Lock()
 
-        # Only once instance of WPWatcher can use a database file at a time. 
-        self._wp_report_file_lock: FileLock = FileLock(f"{self.filepath}.lock")
+        try:
+            lock = FileLock(f"{self.filepath}.lock", thread_local=False)
+        except:
+            lock = FileLock(f"{self.filepath}.lock")
         
+        # Only one instance of WPWatcher can use a database file at a time. 
+        self._wp_report_file_lock: FileLock = lock
 
     def open(self) -> None:
         """
         Acquire the file lock for the DB file. 
         """
         try:
             self._wp_report_file_lock.acquire(timeout=1)
```

### Comparing `wpwatcher-3.0.5/wpwatcher/email.py` & `wpwatcher-3.0.6/wpwatcher/email.py`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/wpwatcher/report.py` & `wpwatcher-3.0.6/wpwatcher/report.py`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/wpwatcher/scan.py` & `wpwatcher-3.0.6/wpwatcher/scan.py`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/wpwatcher/site.py` & `wpwatcher-3.0.6/wpwatcher/site.py`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/wpwatcher/syslog.py` & `wpwatcher-3.0.6/wpwatcher/syslog.py`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/wpwatcher/utils.py` & `wpwatcher-3.0.6/wpwatcher/utils.py`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/wpwatcher/wpscan.py` & `wpwatcher-3.0.6/wpwatcher/wpscan.py`

 * *Files identical despite different names*

### Comparing `wpwatcher-3.0.5/wpwatcher.egg-info/PKG-INFO` & `wpwatcher-3.0.6/wpwatcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpwatcher
-Version: 3.0.5
+Version: 3.0.6
 Summary: WPWatcher - Automating WPScan to scan and report vulnerable Wordpress sites
 Home-page: https://github.com/tristanlatr/WPWatcher
 Maintainer: Florian Roth, Tristan Landes
 License: Apache License 2.0
 Keywords: wpscan auto multiple bulk batch scan wordpress email report alerts warnings service automate mass vulnerable sites asynchronous syslog
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wpwatcher Version: 3.0.5 Summary: WPWatcher -
+Metadata-Version: 2.1 Name: wpwatcher Version: 3.0.6 Summary: WPWatcher -
 Automating WPScan to scan and report vulnerable Wordpress sites Home-page:
 https://github.com/tristanlatr/WPWatcher Maintainer: Florian Roth, Tristan
 Landes License: Apache License 2.0 Keywords: wpscan auto multiple bulk batch
 scan wordpress email report alerts warnings service automate mass vulnerable
 sites asynchronous syslog Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Information Technology Classifier:
 Environment :: Console Classifier: Topic :: Security Classifier: Topic ::
```

### Comparing `wpwatcher-3.0.5/wpwatcher.egg-info/SOURCES.txt` & `wpwatcher-3.0.6/wpwatcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

