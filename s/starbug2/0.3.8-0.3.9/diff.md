# Comparing `tmp/starbug2-0.3.8.tar.gz` & `tmp/starbug2-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starbug2-0.3.8.tar", last modified: Tue Apr 25 15:37:46 2023, max compression
+gzip compressed data, was "starbug2-0.3.9.tar", last modified: Wed Apr 26 09:25:29 2023, max compression
```

## Comparing `starbug2-0.3.8.tar` & `starbug2-0.3.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:37:46.520021 starbug2-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-25 15:37:12.000000 starbug2-0.3.8/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 15:37:12.000000 starbug2-0.3.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-25 15:37:12.000000 starbug2-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-25 15:37:46.520021 starbug2-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-25 15:37:12.000000 starbug2-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:37:46.516021 starbug2-0.3.8/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10896 2023-04-25 15:37:12.000000 starbug2-0.3.8/bin/starbug2
--rwxr-xr-x   0 runner    (1001) docker     (123)     3644 2023-04-25 15:37:12.000000 starbug2-0.3.8/bin/starbug2-match
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:37:46.516021 starbug2-0.3.8/extras/
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-25 15:37:12.000000 starbug2-0.3.8/extras/starbug2.completion
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-25 15:37:12.000000 starbug2-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-25 15:37:46.520021 starbug2-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-25 15:37:12.000000 starbug2-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:37:46.516021 starbug2-0.3.8/starbug2/
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-25 15:37:12.000000 starbug2-0.3.8/starbug2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14164 2023-04-25 15:37:12.000000 starbug2-0.3.8/starbug2/matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-04-25 15:37:12.000000 starbug2-0.3.8/starbug2/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:37:46.516021 starbug2-0.3.8/starbug2/param/
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-25 15:37:12.000000 starbug2-0.3.8/starbug2/param/default.param
--rw-r--r--   0 runner    (1001) docker     (123)    28078 2023-04-25 15:37:12.000000 starbug2-0.3.8/starbug2/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    28295 2023-04-25 15:37:12.000000 starbug2-0.3.8/starbug2/starbug.py
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-04-25 15:37:12.000000 starbug2-0.3.8/starbug2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:37:46.516021 starbug2-0.3.8/starbug2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-25 15:37:46.000000 starbug2-0.3.8/starbug2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-25 15:37:46.000000 starbug2-0.3.8/starbug2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:37:46.000000 starbug2-0.3.8/starbug2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-25 15:37:46.000000 starbug2-0.3.8/starbug2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 15:37:46.000000 starbug2-0.3.8/starbug2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:37:46.520021 starbug2-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-25 15:37:12.000000 starbug2-0.3.8/tests/test_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-25 15:37:12.000000 starbug2-0.3.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:25:29.438328 starbug2-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-26 09:25:08.000000 starbug2-0.3.9/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 09:25:08.000000 starbug2-0.3.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-26 09:25:08.000000 starbug2-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-26 09:25:29.438328 starbug2-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-26 09:25:08.000000 starbug2-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:25:29.434328 starbug2-0.3.9/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10896 2023-04-26 09:25:08.000000 starbug2-0.3.9/bin/starbug2
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3644 2023-04-26 09:25:08.000000 starbug2-0.3.9/bin/starbug2-match
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:25:29.434328 starbug2-0.3.9/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-26 09:25:08.000000 starbug2-0.3.9/extras/starbug2.completion
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-26 09:25:08.000000 starbug2-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-26 09:25:29.438328 starbug2-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-26 09:25:08.000000 starbug2-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:25:29.434328 starbug2-0.3.9/starbug2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-26 09:25:08.000000 starbug2-0.3.9/starbug2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14164 2023-04-26 09:25:08.000000 starbug2-0.3.9/starbug2/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-04-26 09:25:08.000000 starbug2-0.3.9/starbug2/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:25:29.438328 starbug2-0.3.9/starbug2/param/
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-26 09:25:08.000000 starbug2-0.3.9/starbug2/param/default.param
+-rw-r--r--   0 runner    (1001) docker     (123)    28226 2023-04-26 09:25:08.000000 starbug2-0.3.9/starbug2/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28295 2023-04-26 09:25:08.000000 starbug2-0.3.9/starbug2/starbug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-04-26 09:25:08.000000 starbug2-0.3.9/starbug2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:25:29.438328 starbug2-0.3.9/starbug2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-26 09:25:29.000000 starbug2-0.3.9/starbug2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-26 09:25:29.000000 starbug2-0.3.9/starbug2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:25:29.000000 starbug2-0.3.9/starbug2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-26 09:25:29.000000 starbug2-0.3.9/starbug2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 09:25:29.000000 starbug2-0.3.9/starbug2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:25:29.438328 starbug2-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-26 09:25:08.000000 starbug2-0.3.9/tests/test_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-26 09:25:08.000000 starbug2-0.3.9/tests/test_utils.py
```

### Comparing `starbug2-0.3.8/LICENSE.txt` & `starbug2-0.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.8/PKG-INFO` & `starbug2-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starbug2
-Version: 0.3.8
+Version: 0.3.9
 Summary: JWST PSF photometry in complex crowded fields.
 Author: Conor Nally
 Author-email: conor.nally@ed.ac.uk
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 
 # StarBugII
```

### Comparing `starbug2-0.3.8/README.md` & `starbug2-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.8/bin/starbug2` & `starbug2-0.3.9/bin/starbug2`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.8/bin/starbug2-match` & `starbug2-0.3.9/bin/starbug2-match`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.8/extras/starbug2.completion` & `starbug2-0.3.9/extras/starbug2.completion`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.8/starbug2/__init__.py` & `starbug2-0.3.9/starbug2/__init__.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.8/starbug2/matching.py` & `starbug2-0.3.9/starbug2/matching.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.8/starbug2/misc.py` & `starbug2-0.3.9/starbug2/misc.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.8/starbug2/param/default.param` & `starbug2-0.3.9/starbug2/param/default.param`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.8/starbug2/routines.py` & `starbug2-0.3.9/starbug2/routines.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,21 +360,23 @@
     def __call__(self, *args):
         res=super().__call__(*args)
         self.ngroups=max(res["group_id"])
 
         #### hacking recursion error
         for gid in set(res["group_id"]):
             n_members=sum(res["group_id"]==gid)
-            if n_members > sys.getrecursionlimit():
+            ## It seems to not quite hit the recursion limit
+            ## Crashed on 980 with a limit of 1000, so im going to try 90%
+            if n_members > (0.9*sys.getrecursionlimit()):
                 warn()
                 perror("This run will exceed the recursion depth of the system. "
-                        "Starbug will intervene and override the recursion limit but "
-                        "the parameter \"CRIT_SEP\" should be reduced to avoid this.\n"
-                        "Setting recursion limit %d -> %d\n"%(sys.getrecursionlimit(), n_members))
-                sys.setrecursionlimit(n_members)
+                       "Starbug will intervene and override the recursion limit but "
+                       "the parameter \"CRIT_SEP\" should be reduced to avoid this.\n"
+                       "Setting recursion limit %d -> %d\n"%(sys.getrecursionlimit(), n_members))
+                sys.setrecursionlimit(int(1.1*n_members))
         return res
 
 class _fitmodel(LevMarLSQFitter):
     load=None
     def __init__(self, grouper=None, verbose=1):
         super().__init__()
         self.grouper=grouper
```

### Comparing `starbug2-0.3.8/starbug2/starbug.py` & `starbug2-0.3.9/starbug2/starbug.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.8/starbug2/utils.py` & `starbug2-0.3.9/starbug2/utils.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.8/starbug2.egg-info/PKG-INFO` & `starbug2-0.3.9/starbug2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starbug2
-Version: 0.3.8
+Version: 0.3.9
 Summary: JWST PSF photometry in complex crowded fields.
 Author: Conor Nally
 Author-email: conor.nally@ed.ac.uk
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 
 # StarBugII
```

### Comparing `starbug2-0.3.8/tests/test_routines.py` & `starbug2-0.3.9/tests/test_routines.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.8/tests/test_utils.py` & `starbug2-0.3.9/tests/test_utils.py`

 * *Files identical despite different names*

