# Comparing `tmp/varbox-1.0.tar.gz` & `tmp/varbox-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varbox-1.0.tar", last modified: Mon May  8 16:02:14 2023, max compression
+gzip compressed data, was "varbox-1.1.tar", last modified: Mon May  8 16:15:50 2023, max compression
```

## Comparing `varbox-1.0.tar` & `varbox-1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 16:02:14.724038 varbox-1.0/
--rw-rw-rw-   0        0        0      438 2023-05-08 16:02:14.722675 varbox-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-08 16:02:14.724038 varbox-1.0/setup.cfg
--rw-rw-rw-   0        0        0      747 2023-05-08 15:56:41.000000 varbox-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 16:02:14.706901 varbox-1.0/varbox/
--rw-rw-rw-   0        0        0     2837 2023-05-08 14:25:49.000000 varbox-1.0/varbox/cipher.py
--rw-rw-rw-   0        0        0      314 2023-05-08 15:53:32.000000 varbox-1.0/varbox/test.py
-drwxrwxrwx   0        0        0        0 2023-05-08 16:02:14.720677 varbox-1.0/varbox/varbox.egg-info/
--rw-rw-rw-   0        0        0      438 2023-05-08 16:02:14.000000 varbox-1.0/varbox/varbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-05-08 16:02:14.000000 varbox-1.0/varbox/varbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 16:02:14.000000 varbox-1.0/varbox/varbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-08 16:02:14.000000 varbox-1.0/varbox/varbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-08 16:02:14.000000 varbox-1.0/varbox/varbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4271 2023-05-08 14:37:36.000000 varbox-1.0/varbox/varbox.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:15:50.669690 varbox-1.1/
+-rw-rw-rw-   0        0        0      438 2023-05-08 16:15:50.669690 varbox-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-08 16:15:50.669690 varbox-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      951 2023-05-08 16:14:42.000000 varbox-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:15:50.654114 varbox-1.1/varbox/
+-rw-rw-rw-   0        0        0     2837 2023-05-08 14:25:49.000000 varbox-1.1/varbox/cipher.py
+-rw-rw-rw-   0        0        0      314 2023-05-08 15:53:32.000000 varbox-1.1/varbox/test.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:15:50.669690 varbox-1.1/varbox/varbox.egg-info/
+-rw-rw-rw-   0        0        0      438 2023-05-08 16:15:50.000000 varbox-1.1/varbox/varbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-05-08 16:15:50.000000 varbox-1.1/varbox/varbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 16:15:50.000000 varbox-1.1/varbox/varbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-08 16:13:12.000000 varbox-1.1/varbox/varbox.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2023-05-08 16:15:50.000000 varbox-1.1/varbox/varbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-08 16:15:50.000000 varbox-1.1/varbox/varbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4271 2023-05-08 14:37:36.000000 varbox-1.1/varbox/varbox.py
```

### Comparing `varbox-1.0/varbox/cipher.py` & `varbox-1.1/varbox/cipher.py`

 * *Files identical despite different names*

### Comparing `varbox-1.0/varbox/varbox.py` & `varbox-1.1/varbox/varbox.py`

 * *Files identical despite different names*

