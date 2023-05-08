# Comparing `tmp/approximate_cluster_identities-0.1.tar.gz` & `tmp/approximate_cluster_identities-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approximate_cluster_identities-0.1.tar", last modified: Mon May  8 10:01:06 2023, max compression
+gzip compressed data, was "approximate_cluster_identities-0.1.1.tar", last modified: Mon May  8 11:10:03 2023, max compression
```

## Comparing `approximate_cluster_identities-0.1.tar` & `approximate_cluster_identities-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2023-05-08 10:01:06.373141 approximate_cluster_identities-0.1/
--rw-rw-r--   0 daniel    (1001) daniel    (1001)      613 2023-05-08 10:01:06.373141 approximate_cluster_identities-0.1/PKG-INFO
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     2920 2023-05-08 09:47:54.000000 approximate_cluster_identities-0.1/README.md
-drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2023-05-08 10:01:06.373141 approximate_cluster_identities-0.1/approximate_cluster_identities/
--rw-rw-r--   0 daniel    (1001) daniel    (1001)        0 2023-05-05 19:20:08.000000 approximate_cluster_identities-0.1/approximate_cluster_identities/__init__.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)    10978 2023-05-08 09:48:40.000000 approximate_cluster_identities-0.1/approximate_cluster_identities/__main__.py
-drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2023-05-08 10:01:06.373141 approximate_cluster_identities-0.1/approximate_cluster_identities.egg-info/
--rw-rw-r--   0 daniel    (1001) daniel    (1001)      613 2023-05-08 10:01:06.000000 approximate_cluster_identities-0.1/approximate_cluster_identities.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1001) daniel    (1001)      430 2023-05-08 10:01:06.000000 approximate_cluster_identities-0.1/approximate_cluster_identities.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1001) daniel    (1001)        1 2023-05-08 10:01:06.000000 approximate_cluster_identities-0.1/approximate_cluster_identities.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1001) daniel    (1001)       61 2023-05-08 10:01:06.000000 approximate_cluster_identities-0.1/approximate_cluster_identities.egg-info/entry_points.txt
--rw-rw-r--   0 daniel    (1001) daniel    (1001)       55 2023-05-08 10:01:06.000000 approximate_cluster_identities-0.1/approximate_cluster_identities.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1001) daniel    (1001)       31 2023-05-08 10:01:06.000000 approximate_cluster_identities-0.1/approximate_cluster_identities.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1001) daniel    (1001)       38 2023-05-08 10:01:06.373141 approximate_cluster_identities-0.1/setup.cfg
--rw-rw-r--   0 daniel    (1001) daniel    (1001)      936 2023-05-08 10:00:30.000000 approximate_cluster_identities-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:10:03.701268 approximate_cluster_identities-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 11:09:48.000000 approximate_cluster_identities-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-08 11:10:03.701268 approximate_cluster_identities-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-08 11:09:48.000000 approximate_cluster_identities-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:10:03.701268 approximate_cluster_identities-0.1.1/approximate_cluster_identities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:09:48.000000 approximate_cluster_identities-0.1.1/approximate_cluster_identities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-05-08 11:09:48.000000 approximate_cluster_identities-0.1.1/approximate_cluster_identities/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:10:03.701268 approximate_cluster_identities-0.1.1/approximate_cluster_identities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-08 11:10:03.000000 approximate_cluster_identities-0.1.1/approximate_cluster_identities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-08 11:10:03.000000 approximate_cluster_identities-0.1.1/approximate_cluster_identities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:10:03.000000 approximate_cluster_identities-0.1.1/approximate_cluster_identities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-08 11:10:03.000000 approximate_cluster_identities-0.1.1/approximate_cluster_identities.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 11:10:03.000000 approximate_cluster_identities-0.1.1/approximate_cluster_identities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-08 11:10:03.000000 approximate_cluster_identities-0.1.1/approximate_cluster_identities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 11:10:03.701268 approximate_cluster_identities-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-08 11:09:48.000000 approximate_cluster_identities-0.1.1/setup.py
```

### Comparing `approximate_cluster_identities-0.1/README.md` & `approximate_cluster_identities-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Approximate Cluster Identities (ACI)
 
 A python package to visualise the approximate within and between cluster identities of short sequences as assigned by e.g. mmseqs2, cd-hit or panaroo.
 
 # Installation
 ```
-pip install approximate_cluster_identities
+pip install approximate-cluster-identities
 ```
 
 # Usage
 
 ```
 aci -h
```

### Comparing `approximate_cluster_identities-0.1/approximate_cluster_identities/__main__.py` & `approximate_cluster_identities-0.1.1/approximate_cluster_identities/__main__.py`

 * *Files identical despite different names*

