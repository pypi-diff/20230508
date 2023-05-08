# Comparing `tmp/espwrap-2.0.8.tar.gz` & `tmp/espwrap-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/espwrap-2.0.8.tar", last modified: Wed Mar 18 19:23:46 2020, max compression
+gzip compressed data, was "dist/espwrap-2.0.9.tar", last modified: Thu Apr 16 18:37:43 2020, max compression
```

## Comparing `espwrap-2.0.8.tar` & `espwrap-2.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2020-03-18 19:23:46.000000 espwrap-2.0.8/
--rw-r--r--   0 jim        (501) staff       (20)      377 2020-03-18 19:23:46.000000 espwrap-2.0.8/PKG-INFO
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2020-03-18 19:23:46.000000 espwrap-2.0.8/espwrap/
--rw-r--r--   0 jim        (501) staff       (20)       22 2020-03-18 19:23:36.000000 espwrap-2.0.8/espwrap/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2020-03-18 19:23:46.000000 espwrap-2.0.8/espwrap/adaptors/
--rw-r--r--   0 jim        (501) staff       (20)     8504 2020-03-18 19:23:36.000000 espwrap-2.0.8/espwrap/adaptors/sendgrid_v3.py
--rw-r--r--   0 jim        (501) staff       (20)        0 2020-02-11 20:10:17.000000 espwrap-2.0.8/espwrap/adaptors/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      165 2020-02-11 20:10:17.000000 espwrap-2.0.8/espwrap/adaptors/noop.py
--rw-r--r--   0 jim        (501) staff       (20)     4681 2020-02-11 20:10:17.000000 espwrap-2.0.8/espwrap/adaptors/sendgrid.py
--rw-r--r--   0 jim        (501) staff       (20)     2635 2020-02-11 20:10:17.000000 espwrap-2.0.8/espwrap/adaptors/mandrill.py
--rw-r--r--   0 jim        (501) staff       (20)      376 2020-02-11 20:10:17.000000 espwrap-2.0.8/espwrap/adaptors/sendgrid_common.py
--rw-r--r--   0 jim        (501) staff       (20)     6731 2020-03-18 19:23:36.000000 espwrap-2.0.8/espwrap/base.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2020-03-18 19:23:46.000000 espwrap-2.0.8/espwrap.egg-info/
--rw-r--r--   0 jim        (501) staff       (20)      377 2020-03-18 19:23:46.000000 espwrap-2.0.8/espwrap.egg-info/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)      398 2020-03-18 19:23:46.000000 espwrap-2.0.8/espwrap.egg-info/SOURCES.txt
--rw-r--r--   0 jim        (501) staff       (20)       72 2020-03-18 19:23:46.000000 espwrap-2.0.8/espwrap.egg-info/requires.txt
--rw-r--r--   0 jim        (501) staff       (20)        8 2020-03-18 19:23:46.000000 espwrap-2.0.8/espwrap.egg-info/top_level.txt
--rw-r--r--   0 jim        (501) staff       (20)        1 2020-03-18 19:23:46.000000 espwrap-2.0.8/espwrap.egg-info/dependency_links.txt
--rw-r--r--   0 jim        (501) staff       (20)    10321 2020-02-11 20:10:17.000000 espwrap-2.0.8/README.md
--rw-r--r--   0 jim        (501) staff       (20)      960 2020-02-11 20:10:17.000000 espwrap-2.0.8/setup.py
--rw-r--r--   0 jim        (501) staff       (20)       63 2020-03-18 19:23:46.000000 espwrap-2.0.8/setup.cfg
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2020-04-16 18:37:43.000000 espwrap-2.0.9/
+-rw-r--r--   0 jim        (501) staff       (20)      377 2020-04-16 18:37:43.000000 espwrap-2.0.9/PKG-INFO
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2020-04-16 18:37:43.000000 espwrap-2.0.9/espwrap/
+-rw-r--r--   0 jim        (501) staff       (20)       22 2020-04-16 18:31:09.000000 espwrap-2.0.9/espwrap/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2020-04-16 18:37:43.000000 espwrap-2.0.9/espwrap/adaptors/
+-rw-r--r--   0 jim        (501) staff       (20)     8629 2020-04-16 18:31:09.000000 espwrap-2.0.9/espwrap/adaptors/sendgrid_v3.py
+-rw-r--r--   0 jim        (501) staff       (20)        0 2020-02-11 20:10:17.000000 espwrap-2.0.9/espwrap/adaptors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      165 2020-02-11 20:10:17.000000 espwrap-2.0.9/espwrap/adaptors/noop.py
+-rw-r--r--   0 jim        (501) staff       (20)     4681 2020-02-11 20:10:17.000000 espwrap-2.0.9/espwrap/adaptors/sendgrid.py
+-rw-r--r--   0 jim        (501) staff       (20)     2635 2020-02-11 20:10:17.000000 espwrap-2.0.9/espwrap/adaptors/mandrill.py
+-rw-r--r--   0 jim        (501) staff       (20)      376 2020-02-11 20:10:17.000000 espwrap-2.0.9/espwrap/adaptors/sendgrid_common.py
+-rw-r--r--   0 jim        (501) staff       (20)     6731 2020-03-18 19:23:36.000000 espwrap-2.0.9/espwrap/base.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2020-04-16 18:37:43.000000 espwrap-2.0.9/espwrap.egg-info/
+-rw-r--r--   0 jim        (501) staff       (20)      377 2020-04-16 18:37:43.000000 espwrap-2.0.9/espwrap.egg-info/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)      398 2020-04-16 18:37:43.000000 espwrap-2.0.9/espwrap.egg-info/SOURCES.txt
+-rw-r--r--   0 jim        (501) staff       (20)       72 2020-04-16 18:37:43.000000 espwrap-2.0.9/espwrap.egg-info/requires.txt
+-rw-r--r--   0 jim        (501) staff       (20)        8 2020-04-16 18:37:43.000000 espwrap-2.0.9/espwrap.egg-info/top_level.txt
+-rw-r--r--   0 jim        (501) staff       (20)        1 2020-04-16 18:37:43.000000 espwrap-2.0.9/espwrap.egg-info/dependency_links.txt
+-rw-r--r--   0 jim        (501) staff       (20)    10321 2020-02-11 20:10:17.000000 espwrap-2.0.9/README.md
+-rw-r--r--   0 jim        (501) staff       (20)      960 2020-02-11 20:10:17.000000 espwrap-2.0.9/setup.py
+-rw-r--r--   0 jim        (501) staff       (20)       63 2020-04-16 18:37:43.000000 espwrap-2.0.9/setup.cfg
```

### Comparing `espwrap-2.0.8/espwrap/adaptors/sendgrid_v3.py` & `espwrap-2.0.9/espwrap/adaptors/sendgrid_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,19 @@
         # Clicks
         if self.track_clicks:
             tracking_settings.click_tracking = ClickTracking(
                 self.track_clicks,
                 self.track_clicks
             )
         message.tracking_settings = tracking_settings
-        message.from_email = From(email=self.from_addr, name=self.from_name)
+
+        if self.from_addr and self.from_name:
+            message.from_email = From(email=self.from_addr, name=self.from_name)
+        else:
+            message.from_email = From(email=self.from_addr)
 
         for subgrps in to_send:
             for subgrp in subgrps:
                 substitutions = subgrp['merge_vars']
                 substitutions = {
                     '{1}{0}{2}'.format(x, *self.delimiters): substitutions[x]
                     for x in substitutions
```

### Comparing `espwrap-2.0.8/espwrap/adaptors/sendgrid.py` & `espwrap-2.0.9/espwrap/adaptors/sendgrid.py`

 * *Files identical despite different names*

### Comparing `espwrap-2.0.8/espwrap/adaptors/mandrill.py` & `espwrap-2.0.9/espwrap/adaptors/mandrill.py`

 * *Files identical despite different names*

### Comparing `espwrap-2.0.8/espwrap/base.py` & `espwrap-2.0.9/espwrap/base.py`

 * *Files identical despite different names*

### Comparing `espwrap-2.0.8/README.md` & `espwrap-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `espwrap-2.0.8/setup.py` & `espwrap-2.0.9/setup.py`

 * *Files identical despite different names*

