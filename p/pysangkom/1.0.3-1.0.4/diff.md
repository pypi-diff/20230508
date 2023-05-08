# Comparing `tmp/pysangkom-1.0.3.tar.gz` & `tmp/pysangkom-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysangkom-1.0.3.tar", last modified: Mon May  8 10:32:13 2023, max compression
+gzip compressed data, was "pysangkom-1.0.4.tar", last modified: Mon May  8 10:38:47 2023, max compression
```

## Comparing `pysangkom-1.0.3.tar` & `pysangkom-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:32:13.269567 pysangkom-1.0.3/
--rw-r--r--   0 kang49     (501) staff       (20)      522 2023-05-08 10:32:13.269354 pysangkom-1.0.3/PKG-INFO
--rw-r--r--   0 kang49     (501) staff       (20)      535 2023-05-08 10:29:19.000000 pysangkom-1.0.3/README.md
-drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:32:13.267880 pysangkom-1.0.3/pysangkom/
--rw-r--r--   0 kang49     (501) staff       (20)        0 2023-05-08 09:36:30.000000 pysangkom-1.0.3/pysangkom/__init__.py
--rw-r--r--   0 kang49     (501) staff       (20)    40090 2023-05-08 10:15:04.000000 pysangkom-1.0.3/pysangkom/forkyou.py
-drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:32:13.269131 pysangkom-1.0.3/pysangkom.egg-info/
--rw-r--r--   0 kang49     (501) staff       (20)      522 2023-05-08 10:32:13.000000 pysangkom-1.0.3/pysangkom.egg-info/PKG-INFO
--rw-r--r--   0 kang49     (501) staff       (20)      225 2023-05-08 10:32:13.000000 pysangkom-1.0.3/pysangkom.egg-info/SOURCES.txt
--rw-r--r--   0 kang49     (501) staff       (20)        1 2023-05-08 10:32:13.000000 pysangkom-1.0.3/pysangkom.egg-info/dependency_links.txt
--rw-r--r--   0 kang49     (501) staff       (20)       31 2023-05-08 10:32:13.000000 pysangkom-1.0.3/pysangkom.egg-info/requires.txt
--rw-r--r--   0 kang49     (501) staff       (20)       10 2023-05-08 10:32:13.000000 pysangkom-1.0.3/pysangkom.egg-info/top_level.txt
--rw-r--r--   0 kang49     (501) staff       (20)       38 2023-05-08 10:32:13.269617 pysangkom-1.0.3/setup.cfg
--rw-r--r--   0 kang49     (501) staff       (20)      744 2023-05-08 10:32:08.000000 pysangkom-1.0.3/setup.py
+drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:38:47.819733 pysangkom-1.0.4/
+-rw-r--r--   0 kang49     (501) staff       (20)     1099 2023-05-08 10:38:47.819542 pysangkom-1.0.4/PKG-INFO
+-rw-r--r--   0 kang49     (501) staff       (20)      535 2023-05-08 10:29:19.000000 pysangkom-1.0.4/README.md
+drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:38:47.818331 pysangkom-1.0.4/pysangkom/
+-rw-r--r--   0 kang49     (501) staff       (20)        0 2023-05-08 09:36:30.000000 pysangkom-1.0.4/pysangkom/__init__.py
+-rw-r--r--   0 kang49     (501) staff       (20)    40090 2023-05-08 10:15:04.000000 pysangkom-1.0.4/pysangkom/forkyou.py
+drwxr-xr-x   0 kang49     (501) staff       (20)        0 2023-05-08 10:38:47.819350 pysangkom-1.0.4/pysangkom.egg-info/
+-rw-r--r--   0 kang49     (501) staff       (20)     1099 2023-05-08 10:38:47.000000 pysangkom-1.0.4/pysangkom.egg-info/PKG-INFO
+-rw-r--r--   0 kang49     (501) staff       (20)      225 2023-05-08 10:38:47.000000 pysangkom-1.0.4/pysangkom.egg-info/SOURCES.txt
+-rw-r--r--   0 kang49     (501) staff       (20)        1 2023-05-08 10:38:47.000000 pysangkom-1.0.4/pysangkom.egg-info/dependency_links.txt
+-rw-r--r--   0 kang49     (501) staff       (20)       31 2023-05-08 10:38:47.000000 pysangkom-1.0.4/pysangkom.egg-info/requires.txt
+-rw-r--r--   0 kang49     (501) staff       (20)       10 2023-05-08 10:38:47.000000 pysangkom-1.0.4/pysangkom.egg-info/top_level.txt
+-rw-r--r--   0 kang49     (501) staff       (20)       38 2023-05-08 10:38:47.819783 pysangkom-1.0.4/setup.cfg
+-rw-r--r--   0 kang49     (501) staff       (20)      902 2023-05-08 10:38:44.000000 pysangkom-1.0.4/setup.py
```

### Comparing `pysangkom-1.0.3/README.md` & `pysangkom-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pysangkom-1.0.3/pysangkom/forkyou.py` & `pysangkom-1.0.4/pysangkom/forkyou.py`

 * *Files identical despite different names*

