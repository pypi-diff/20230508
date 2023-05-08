# Comparing `tmp/policyengine-canada-0.8.0.tar.gz` & `tmp/policyengine-canada-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "policyengine-canada-0.8.0.tar", last modified: Mon Dec 12 18:54:07 2022, max compression
+gzip compressed data, was "policyengine-canada-0.9.0.tar", last modified: Mon Dec 12 19:21:11 2022, max compression
```

## Comparing `policyengine-canada-0.8.0.tar` & `policyengine-canada-0.9.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 18:54:07.874368 policyengine-canada-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2022-12-12 18:53:07.000000 policyengine-canada-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      965 2022-12-12 18:54:07.874368 policyengine-canada-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-12 18:53:07.000000 policyengine-canada-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 18:54:07.874368 policyengine-canada-0.8.0/policyengine_canada.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      965 2022-12-12 18:54:07.000000 policyengine-canada-0.8.0/policyengine_canada.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2022-12-12 18:54:07.000000 policyengine-canada-0.8.0/policyengine_canada.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 18:54:07.000000 policyengine-canada-0.8.0/policyengine_canada.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      418 2022-12-12 18:54:07.000000 policyengine-canada-0.8.0/policyengine_canada.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 18:54:07.000000 policyengine-canada-0.8.0/policyengine_canada.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-12 18:54:07.874368 policyengine-canada-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2022-12-12 18:53:07.000000 policyengine-canada-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 19:21:11.895285 policyengine-canada-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2022-12-12 19:20:05.000000 policyengine-canada-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2022-12-12 19:21:11.895285 policyengine-canada-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-12 19:20:05.000000 policyengine-canada-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 19:21:11.895285 policyengine-canada-0.9.0/policyengine_canada.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2022-12-12 19:21:11.000000 policyengine-canada-0.9.0/policyengine_canada.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2022-12-12 19:21:11.000000 policyengine-canada-0.9.0/policyengine_canada.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 19:21:11.000000 policyengine-canada-0.9.0/policyengine_canada.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2022-12-12 19:21:11.000000 policyengine-canada-0.9.0/policyengine_canada.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 19:21:11.000000 policyengine-canada-0.9.0/policyengine_canada.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-12 19:21:11.895285 policyengine-canada-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2022-12-12 19:20:05.000000 policyengine-canada-0.9.0/setup.py
```

### Comparing `policyengine-canada-0.8.0/LICENSE` & `policyengine-canada-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.8.0/PKG-INFO` & `policyengine-canada-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyengine-canada
-Version: 0.8.0
+Version: 0.9.0
 Summary: Microsimulation model for Canada's tax-benefit system.
 Home-page: https://github.com/policyengine/policyengine-canada
 Author: PolicyEngine
 Author-email: hello@policyengine.org
 License: https://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit microsimulation framework
 Platform: UNKNOWN
```

### Comparing `policyengine-canada-0.8.0/policyengine_canada.egg-info/PKG-INFO` & `policyengine-canada-0.9.0/policyengine_canada.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyengine-canada
-Version: 0.8.0
+Version: 0.9.0
 Summary: Microsimulation model for Canada's tax-benefit system.
 Home-page: https://github.com/policyengine/policyengine-canada
 Author: PolicyEngine
 Author-email: hello@policyengine.org
 License: https://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit microsimulation framework
 Platform: UNKNOWN
```

### Comparing `policyengine-canada-0.8.0/setup.py` & `policyengine-canada-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "sphinx>=4.5.0,<5",
     "sphinx-argparse>=0.3.2,<1",
     "sphinx-math-dollar>=1.2.1,<2",
 ]
 
 setup(
     name="policyengine-canada",
-    version="0.8.0",
+    version="0.9.0",
     author="PolicyEngine",
     author_email="hello@policyengine.org",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: POSIX",
         "Programming Language :: Python",
```

