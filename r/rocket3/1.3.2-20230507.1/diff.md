# Comparing `tmp/rocket3-1.3.2.tar.gz` & `tmp/rocket3-20230507.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocket3-1.3.2.tar", last modified: Sat Oct  9 07:52:48 2021, max compression
+gzip compressed data, was "rocket3-20230507.1.tar", last modified: Mon May  8 00:08:54 2023, max compression
```

## Comparing `rocket3-1.3.2.tar` & `rocket3-20230507.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2021-10-09 07:52:48.574868 rocket3-1.3.2/
--rw-rw-r--   0 mdp       (1000) mdp       (1000)     1301 2021-10-09 07:52:48.574868 rocket3-1.3.2/PKG-INFO
--rw-r--r--   0 mdp       (1000) mdp       (1000)      741 2021-02-08 03:06:36.000000 rocket3-1.3.2/README.md
-drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2021-10-09 07:52:48.574868 rocket3-1.3.2/rocket3/
--rw-rw-r--   0 mdp       (1000) mdp       (1000)    55024 2021-10-09 07:49:59.000000 rocket3-1.3.2/rocket3/__init__.py
-drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2021-10-09 07:52:48.574868 rocket3-1.3.2/rocket3.egg-info/
--rw-rw-r--   0 mdp       (1000) mdp       (1000)     1301 2021-10-09 07:52:48.000000 rocket3-1.3.2/rocket3.egg-info/PKG-INFO
--rw-rw-r--   0 mdp       (1000) mdp       (1000)      192 2021-10-09 07:52:48.000000 rocket3-1.3.2/rocket3.egg-info/SOURCES.txt
--rw-rw-r--   0 mdp       (1000) mdp       (1000)        1 2021-10-09 07:52:48.000000 rocket3-1.3.2/rocket3.egg-info/dependency_links.txt
--rw-rw-r--   0 mdp       (1000) mdp       (1000)        1 2021-02-08 03:09:26.000000 rocket3-1.3.2/rocket3.egg-info/not-zip-safe
--rw-rw-r--   0 mdp       (1000) mdp       (1000)        8 2021-10-09 07:52:48.000000 rocket3-1.3.2/rocket3.egg-info/top_level.txt
--rw-rw-r--   0 mdp       (1000) mdp       (1000)       38 2021-10-09 07:52:48.574868 rocket3-1.3.2/setup.cfg
--rw-r--r--   0 mdp       (1000) mdp       (1000)     1575 2021-02-08 02:45:15.000000 rocket3-1.3.2/setup.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 00:08:54.053000 rocket3-20230507.1/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     1555 2021-02-08 02:11:58.000000 rocket3-20230507.1/LICENSE.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1283 2023-05-08 00:08:54.053000 rocket3-20230507.1/PKG-INFO
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      741 2021-02-08 03:06:36.000000 rocket3-20230507.1/README.md
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      514 2023-05-08 00:06:08.000000 rocket3-20230507.1/pyproject.toml
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 00:08:54.036999 rocket3-20230507.1/rocket3/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)    55029 2023-05-07 23:57:14.000000 rocket3-20230507.1/rocket3/__init__.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 00:08:54.053000 rocket3-20230507.1/rocket3.egg-info/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     1283 2023-05-08 00:08:54.000000 rocket3-20230507.1/rocket3.egg-info/PKG-INFO
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      201 2023-05-08 00:08:54.000000 rocket3-20230507.1/rocket3.egg-info/SOURCES.txt
+-rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2023-05-08 00:08:54.000000 rocket3-20230507.1/rocket3.egg-info/dependency_links.txt
+-rw-r--r--   0 massimo   (1000) massimo   (1000)        8 2023-05-08 00:08:54.000000 rocket3-20230507.1/rocket3.egg-info/top_level.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)       38 2023-05-08 00:08:54.053000 rocket3-20230507.1/setup.cfg
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 00:08:54.053000 rocket3-20230507.1/tests/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      693 2021-10-09 07:48:58.000000 rocket3-20230507.1/tests/test_rocket.py
```

### Comparing `rocket3-1.3.2/README.md` & `rocket3-20230507.1/README.md`

 * *Files identical despite different names*

### Comparing `rocket3-1.3.2/rocket3/__init__.py` & `rocket3-20230507.1/rocket3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         pass
 
 
 log = logging.getLogger("Rocket")
 log.addHandler(NullHandler())
 
 # Define Constants
-__version__ = "1.3.2"
+__version__ = "20230507.1"
 SERVER_NAME = socket.gethostname()
 SERVER_SOFTWARE = "Rocket3 %s" % __version__
 HTTP_SERVER_SOFTWARE = "%s Python/%s" % (SERVER_SOFTWARE, sys.version.split(" ")[0])
 BUF_SIZE = 16384
 SOCKET_TIMEOUT = 10  # in secs
 THREAD_STOP_CHECK_INTERVAL = (
     1  # in secs, How often should threads check for a server stop message?
```

