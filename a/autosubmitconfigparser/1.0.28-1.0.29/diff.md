# Comparing `tmp/autosubmitconfigparser-1.0.28.tar.gz` & `tmp/autosubmitconfigparser-1.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosubmitconfigparser-1.0.28.tar", last modified: Fri May  5 11:22:21 2023, max compression
+gzip compressed data, was "autosubmitconfigparser-1.0.29.tar", last modified: Mon May  8 14:17:15 2023, max compression
```

## Comparing `autosubmitconfigparser-1.0.28.tar` & `autosubmitconfigparser-1.0.29.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-05 11:22:21.890628 autosubmitconfigparser-1.0.28/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-09-23 10:01:03.000000 autosubmitconfigparser-1.0.28/CHANGELOG
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       41 2023-03-03 13:49:23.000000 autosubmitconfigparser-1.0.28/MANIFEST.in
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-05-05 11:22:21.890628 autosubmitconfigparser-1.0.28/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1493 2022-12-05 09:31:33.000000 autosubmitconfigparser-1.0.28/README.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        6 2023-05-04 13:40:57.000000 autosubmitconfigparser-1.0.28/VERSION
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmitconfigparser-1.0.28/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-05 11:22:21.882628 autosubmitconfigparser-1.0.28/autosubmitconfigparser/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-05 11:22:21.886628 autosubmitconfigparser-1.0.28/autosubmitconfigparser/__pycache__/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      162 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/__pycache__/__init__.cpython-37.pyc
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-05 11:22:21.886628 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-05 11:22:21.886628 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/__pycache__/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      169 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4187 2022-12-19 09:28:49.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/__pycache__/basicconfig.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    74789 2023-04-05 09:03:32.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/__pycache__/configcommon.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1104 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/__pycache__/yamlparser.cpython-37.pyc
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     7990 2023-04-25 12:49:03.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/basicconfig.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   100720 2023-05-04 13:02:37.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/configcommon.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-05 11:22:21.886628 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/autosubmit-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/autosubmit.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      562 2023-02-14 09:24:09.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/expdef-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      557 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/expdef.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      401 2023-03-03 11:06:17.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/git-minimal.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/jobs-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/jobs.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      321 2023-03-03 12:26:14.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/local-minimal.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/platforms-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/platforms.yml
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      408 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/yamlparser.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-05 11:22:21.882628 autosubmitconfigparser-1.0.28/autosubmitconfigparser.egg-info/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-05-05 11:22:21.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser.egg-info/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1514 2023-05-05 11:22:21.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser.egg-info/SOURCES.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-05-05 11:22:21.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser.egg-info/dependency_links.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      314 2023-05-05 11:22:21.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser.egg-info/requires.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2023-05-05 11:22:21.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser.egg-info/top_level.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      600 2023-05-05 11:20:51.000000 autosubmitconfigparser-1.0.28/environment.yml
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-05 11:22:21.890628 autosubmitconfigparser-1.0.28/log/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.28/log/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-05 11:22:21.890628 autosubmitconfigparser-1.0.28/log/__pycache__/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      143 2022-10-26 14:22:27.000000 autosubmitconfigparser-1.0.28/log/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12336 2022-10-26 14:22:27.000000 autosubmitconfigparser-1.0.28/log/__pycache__/log.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.28/log/fd_show.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13106 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.28/log/log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      425 2023-05-05 11:20:51.000000 autosubmitconfigparser-1.0.28/requeriments.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-05-05 11:22:21.890628 autosubmitconfigparser-1.0.28/setup.cfg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1474 2023-05-05 11:20:51.000000 autosubmitconfigparser-1.0.28/setup.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1254 2023-01-31 09:30:38.000000 autosubmitconfigparser-1.0.28/test_config.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:17:15.407431 autosubmitconfigparser-1.0.29/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-09-23 10:01:03.000000 autosubmitconfigparser-1.0.29/CHANGELOG
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       41 2023-03-03 13:49:23.000000 autosubmitconfigparser-1.0.29/MANIFEST.in
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-05-08 14:17:15.407431 autosubmitconfigparser-1.0.29/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1493 2022-12-05 09:31:33.000000 autosubmitconfigparser-1.0.29/README.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        6 2023-05-08 14:15:56.000000 autosubmitconfigparser-1.0.29/VERSION
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmitconfigparser-1.0.29/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:17:15.403431 autosubmitconfigparser-1.0.29/autosubmitconfigparser/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:17:15.403431 autosubmitconfigparser-1.0.29/autosubmitconfigparser/__pycache__/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      162 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser/__pycache__/__init__.cpython-37.pyc
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:17:15.403431 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:17:15.403431 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/__pycache__/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      169 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4187 2022-12-19 09:28:49.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/__pycache__/basicconfig.cpython-37.pyc
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    74789 2023-04-05 09:03:32.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/__pycache__/configcommon.cpython-37.pyc
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1104 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/__pycache__/yamlparser.cpython-37.pyc
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     7990 2023-04-25 12:49:03.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/basicconfig.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   101050 2023-05-08 13:46:44.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/configcommon.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:17:15.407431 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/files/
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/files/autosubmit-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/files/autosubmit.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      562 2023-02-14 09:24:09.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/files/expdef-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      557 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/files/expdef.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      401 2023-03-03 11:06:17.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/files/git-minimal.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/files/jobs-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/files/jobs.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      321 2023-03-03 12:26:14.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/files/local-minimal.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/files/platforms-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/files/platforms.yml
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      408 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/yamlparser.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:17:15.403431 autosubmitconfigparser-1.0.29/autosubmitconfigparser.egg-info/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-05-08 14:17:14.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser.egg-info/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1514 2023-05-08 14:17:15.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser.egg-info/SOURCES.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-05-08 14:17:14.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser.egg-info/dependency_links.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      314 2023-05-08 14:17:14.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser.egg-info/requires.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2023-05-08 14:17:15.000000 autosubmitconfigparser-1.0.29/autosubmitconfigparser.egg-info/top_level.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      600 2023-05-05 11:20:51.000000 autosubmitconfigparser-1.0.29/environment.yml
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:17:15.407431 autosubmitconfigparser-1.0.29/log/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.29/log/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-08 14:17:15.407431 autosubmitconfigparser-1.0.29/log/__pycache__/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      143 2022-10-26 14:22:27.000000 autosubmitconfigparser-1.0.29/log/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12336 2022-10-26 14:22:27.000000 autosubmitconfigparser-1.0.29/log/__pycache__/log.cpython-37.pyc
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.29/log/fd_show.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13106 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.29/log/log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      425 2023-05-05 11:20:51.000000 autosubmitconfigparser-1.0.29/requeriments.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-05-08 14:17:15.407431 autosubmitconfigparser-1.0.29/setup.cfg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1474 2023-05-08 14:15:56.000000 autosubmitconfigparser-1.0.29/setup.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1254 2023-01-31 09:30:38.000000 autosubmitconfigparser-1.0.29/test_config.py
```

### Comparing `autosubmitconfigparser-1.0.28/PKG-INFO` & `autosubmitconfigparser-1.0.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmitconfigparser
-Version: 1.0.28
+Version: 1.0.29
 Summary: An utility library that allows to read an Autosubmit 4 experiment configuration.
 Home-page: https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 Keywords: climate,weather,workflow,HPC
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `autosubmitconfigparser-1.0.28/README.md` & `autosubmitconfigparser-1.0.29/README.md`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/__pycache__/basicconfig.cpython-37.pyc` & `autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/__pycache__/basicconfig.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/__pycache__/configcommon.cpython-37.pyc` & `autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/__pycache__/configcommon.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/__pycache__/yamlparser.cpython-37.pyc` & `autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/__pycache__/yamlparser.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/basicconfig.py` & `autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/basicconfig.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/configcommon.py` & `autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/configcommon.py`

 * *Files 1% similar despite different names*

```diff
@@ -476,14 +476,19 @@
         return normalized_data
 
     def deep_update(self,unified_config, new_dict):
         """
         Update a nested dictionary or similar mapping.
         Modify ``source`` in place.
         """
+        if not isinstance(unified_config,collections.abc.Mapping):
+            unified_config = {}
+        for key in new_dict.keys():
+            if key not in unified_config:
+                unified_config[key] = ""
         for key, val in new_dict.items():
             if isinstance(val, collections.abc.Mapping ):
                 tmp = self.deep_update(unified_config.get(key, {}), val)
                 unified_config[key] = tmp
             elif isinstance(val, list):
                 current_list = set(unified_config.get(key, []))
                 if current_list != set(val):
@@ -624,18 +629,21 @@
                     if ',' in custom_conf_directive["POST"]:
                         filenames_to_load["POST"] = custom_conf_directive["POST"].split(',')
                     else:
                         filenames_to_load["POST"] = custom_conf_directive["POST"].split(' ')
         aux_filenames_to_load = filenames_to_load.copy()
         for file_to_load in aux_filenames_to_load["PRE"]:
             if file_to_load in self.current_loaded_files:
-                del filenames_to_load[file_to_load]
+                f_list = filenames_to_load["PRE"]
+                f_list.remove(file_to_load)
         for file_to_load in aux_filenames_to_load["POST"]:
             if file_to_load in self.current_loaded_files:
-                del filenames_to_load[file_to_load]
+                if file_to_load in self.current_loaded_files:
+                    f_list = filenames_to_load["POST"]
+                    f_list.remove(file_to_load)
         return filenames_to_load
 
     def unify_conf(self,current_data,new_data):
         '''
         Unifies all configuration files into a single dictionary.
         :param current_data: dict with current configuration
         :param new_data: dict with new configuration
@@ -1266,67 +1274,70 @@
     def load_custom_config(self,current_data,filenames_to_load):
         """
         Loads custom config files
         :param current_data: dict with current data
         :param filenames_to_load: list of filenames to load
         :return: current_data_pre,current_data_post with unified data
         """
-
         current_data_pre = {}
+        current_data_aux = {}
         current_data_post = {}
-        if current_data.get('DEFAULT', {}).get('CUSTOM_CONFIG', None) is not None:
-            del current_data["DEFAULT"]["CUSTOM_CONFIG"]
         # at this point, filenames_to_load should be a list of filenames of an specific section PRE or POST.
         for filename in filenames_to_load:
             filename = filename.strip(", ")  # Remove commas and spaces if any
             if filename.startswith("~"):
                 filename = os.path.expanduser(filename)
-            current_data["AS_TEMP"] = {}
-            current_data["AS_TEMP"]["FILENAME_TO_LOAD"] = filename
+            current_data_aux = self.unify_conf(self.starter_conf,current_data)
+            current_data_aux["AS_TEMP"] = {}
+            current_data_aux["AS_TEMP"]["FILENAME_TO_LOAD"] = filename
             self.dynamic_variables.append(("AS_TEMP.FILENAME_TO_LOAD", filename))
-            current_data = self.substitute_dynamic_variables(current_data)
-            filename = Path(current_data["AS_TEMP"]["FILENAME_TO_LOAD"])
-
+            current_data_aux = self.substitute_dynamic_variables(current_data_aux)
+            filename = Path(current_data_aux["AS_TEMP"]["FILENAME_TO_LOAD"])
             if filename.exists() and str(filename) not in self.current_loaded_files:
                 # Check if this file is already loaded. If not, load it
                 self.current_loaded_files[str(filename)] = filename.stat().st_mtime
                 # Load a folder or a file
                 if not filename.is_file():
                     # Load a folder by calling recursively to this function as a list of files
-                    if "AS_TEMP" in current_data:
-                        del current_data["AS_TEMP"]
-                    current_data_pre,current_data_post = self.load_config_folder(current_data,filename)
+                    current_data_pre,current_data_post = self.load_config_folder(copy.deepcopy(current_data),filename)
                     current_data = self.substitute_dynamic_variables(self.unify_conf(current_data_pre,current_data))
                     current_data = self.substitute_dynamic_variables(self.unify_conf(current_data,current_data_post))
                 else:
                     # Load a file and unify the current_data with the loaded data
                     current_data = self.substitute_dynamic_variables(self.unify_conf(self.substitute_dynamic_variables(current_data), self.load_config_file(current_data,filename)))
                     # Load next level if any
                     custom_conf_directive = current_data.get('DEFAULT', {}).get('CUSTOM_CONFIG', None)
                     filenames_to_load_level = self.parse_custom_conf_directive(custom_conf_directive)
-                    if "AS_TEMP" in current_data:
-                        del current_data["AS_TEMP"]
-                    current_data_pre = self.unify_conf(current_data_pre,self.unify_conf(self.load_custom_config_section(current_data, filenames_to_load_level["PRE"]),current_data))
-                    current_data_post = self.unify_conf(current_data_post,self.unify_conf(current_data,self.load_custom_config_section(current_data, filenames_to_load_level["POST"])))
-        if len(current_data_pre) == 0 and len(current_data_post) == 0:
-            return current_data, current_data
-        else:
-            return current_data_pre, current_data_post
+                    if current_data.get('DEFAULT', {}).get('CUSTOM_CONFIG', None) is not None:
+                        del current_data["DEFAULT"]["CUSTOM_CONFIG"]
+                    if len(filenames_to_load_level["PRE"]) > 0:
+                        current_data_pre = self.unify_conf(current_data_pre,self.load_custom_config_section(copy.deepcopy(current_data), filenames_to_load_level["PRE"]))
+                    else:
+                        current_data_pre = current_data
+                    current_data = self.unify_conf(current_data_pre, current_data)
+
+                    if len(filenames_to_load_level["POST"]) > 0:
+                        current_data_post = self.unify_conf(current_data_post,self.unify_conf(current_data,self.load_custom_config_section(current_data, filenames_to_load_level["POST"])))
+                    else:
+                        current_data_post = current_data
+
+        del current_data_aux
+        return current_data_pre, current_data_post
 
     def load_custom_config_section(self,current_data,filenames_to_load):
         """
         Loads a section (PRE or POST ), simple str are also PRE data of the custom config files
         :param current_data: data until now
         :param filenames_to_load: files to load in this section
         :return:
         """
         # This is a recursive call
         current_data_pre,current_data_post = self.load_custom_config(current_data, filenames_to_load)
         # Unifies all pre and post data of the current pre or post data. Think of it as a tree with two branches that needs to be unified at each level
-        return self.substitute_dynamic_variables(self.unify_conf(current_data_pre,current_data_post))
+        return self.substitute_dynamic_variables(self.unify_conf(self.unify_conf(current_data_pre,current_data),current_data_post))
 
     def reload(self,force_load=False,only_experiment_data = False):
         """
         Reloads the configuration files
         :param force_load: If True, reloads all the files, if False, reloads only the modified files
         """
         # Check if the files have been modified or if they need a reload
@@ -1345,37 +1356,34 @@
                 Log.result(f"Reloading configuration files, due a change in the following files: {files_to_reload}")
             starter_conf = {}
             self.current_loaded_files = {} # reset loaded files
             for filename in self.get_yaml_filenames_to_load(self.conf_folder_yaml):
                 starter_conf = self.unify_conf(starter_conf, self.load_config_file(starter_conf, Path(filename)))
             starter_conf = self.load_common_parameters(starter_conf)
             starter_conf = self.substitute_dynamic_variables(starter_conf)
-
+            self.starter_conf = starter_conf
             # Same data without the minimal config ( if any ), need to be here to due current_loaded_files variable
             non_minimal_conf = {}
             non_minimal_files = {}
             for filename in self.get_yaml_filenames_to_load(self.conf_folder_yaml,ignore_minimal=True):
                 non_minimal_files[str(filename)] = Path(filename).stat().st_mtime
                 non_minimal_conf = self.unify_conf(non_minimal_conf, self.load_config_file(non_minimal_conf, Path(filename)))
             non_minimal_conf = self.load_common_parameters(non_minimal_conf)
             non_minimal_conf = self.substitute_dynamic_variables(non_minimal_conf, max_deep=25)
             # Start loading the custom config files
             # Gets the files to load
             filenames_to_load = self.parse_custom_conf_directive(starter_conf.get("DEFAULT",{}).get("CUSTOM_CONFIG",None))
-            # Loads all configuration associated with the project data "pre"
-            #custom_conf_pre = self.load_custom_config_section({key:starter_conf[key] for key in ["PROJDIR","ROOTDIR","DEFAULT"]},filenames_to_load["PRE"])
-            custom_conf_pre = self.load_custom_config_section(starter_conf, filenames_to_load["PRE"])
-            # Loads all configuration associated with the user data "post"
-            custom_conf_post = self.load_custom_config_section(starter_conf,filenames_to_load["POST"])
-            # Unify the dictionaries PROJ(PRE) - $EXPID/CONF - PROJ(POST)
+            #debug
             if not only_experiment_data:
-                self.experiment_data = self.unify_conf(self.unify_conf(custom_conf_pre,non_minimal_conf),custom_conf_post)
+                # Loads all configuration associated with the project data "pre"
+                custom_conf_pre = self.load_custom_config_section({}, filenames_to_load["PRE"])
+                # Loads all configuration associated with the user data "post"
+                self.experiment_data = self.load_custom_config_section(self.unify_conf(custom_conf_pre,non_minimal_conf),filenames_to_load["POST"])
             else:
                 self.experiment_data = starter_conf
-            # This part is useless, as it is already done
             self.experiment_data = self.substitute_dynamic_variables(self.experiment_data, max_deep=25)
             user_data = self.load_custom_config_section(self.experiment_data, filenames_to_load["POST"])
             self.experiment_data = self.substitute_dynamic_variables(self.unify_conf(self.experiment_data,user_data))
             ###
             self.current_loaded_files.update(non_minimal_files)
             if "AS_TEMP" in self.experiment_data.keys():
                 del self.experiment_data["AS_TEMP"]
```

### Comparing `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/expdef-dummy.yml` & `autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/files/expdef-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/expdef.yml` & `autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/files/expdef.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/jobs-dummy.yml` & `autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/files/jobs-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/jobs.yml` & `autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/files/jobs.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/platforms-dummy.yml` & `autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/files/platforms-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/platforms.yml` & `autosubmitconfigparser-1.0.29/autosubmitconfigparser/config/files/platforms.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.28/autosubmitconfigparser.egg-info/PKG-INFO` & `autosubmitconfigparser-1.0.29/autosubmitconfigparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmitconfigparser
-Version: 1.0.28
+Version: 1.0.29
 Summary: An utility library that allows to read an Autosubmit 4 experiment configuration.
 Home-page: https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 Keywords: climate,weather,workflow,HPC
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `autosubmitconfigparser-1.0.28/autosubmitconfigparser.egg-info/SOURCES.txt` & `autosubmitconfigparser-1.0.29/autosubmitconfigparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.28/environment.yml` & `autosubmitconfigparser-1.0.29/environment.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.28/log/__pycache__/log.cpython-37.pyc` & `autosubmitconfigparser-1.0.29/log/__pycache__/log.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.28/log/fd_show.py` & `autosubmitconfigparser-1.0.29/log/fd_show.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.28/log/log.py` & `autosubmitconfigparser-1.0.29/log/log.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.28/setup.py` & `autosubmitconfigparser-1.0.29/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autosubmitconfigparser",
-    version="1.0.28",
+    version="1.0.29",
     author="Daniel Beltran Mora",
     author_email="daniel.beltran@bsc.es",
     description="An utility library that allows to read an Autosubmit 4 experiment configuration.",
     keywords=['climate', 'weather', 'workflow', 'HPC'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git",
```

### Comparing `autosubmitconfigparser-1.0.28/test_config.py` & `autosubmitconfigparser-1.0.29/test_config.py`

 * *Files identical despite different names*

