# Comparing `tmp/lftools-0.9.0.tar.gz` & `tmp/lftools-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lftools-0.9.0.tar", last modified: Tue Sep  5 17:34:55 2017, max compression
+gzip compressed data, was "dist/lftools-0.9.1.tar", last modified: Fri Sep 29 16:39:36 2017, max compression
```

## Comparing `lftools-0.9.0.tar` & `lftools-0.9.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)        0 2017-09-05 17:34:55.000000 lftools-0.9.0/
-drwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)        0 2017-09-05 17:34:55.000000 lftools-0.9.0/etc/
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)      335 2017-09-01 19:06:25.000000 lftools-0.9.0/etc/logging.ini
-drwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)        0 2017-09-05 17:34:55.000000 lftools-0.9.0/lftools/
-drwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)        0 2017-09-05 17:34:55.000000 lftools-0.9.0/lftools/cli/
-drwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)        0 2017-09-05 17:34:55.000000 lftools-0.9.0/lftools/cli/jenkins/
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     2224 2017-09-01 19:06:25.000000 lftools-0.9.0/lftools/cli/jenkins/__init__.py
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     1445 2017-09-01 19:06:25.000000 lftools-0.9.0/lftools/cli/jenkins/builds.py
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     1171 2017-09-01 19:06:25.000000 lftools-0.9.0/lftools/cli/jenkins/nodes.py
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     3572 2017-09-01 19:06:25.000000 lftools-0.9.0/lftools/cli/jenkins/plugins.py
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     1261 2017-09-01 19:06:25.000000 lftools-0.9.0/lftools/cli/__init__.py
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     7196 2017-09-01 19:06:25.000000 lftools-0.9.0/lftools/cli/deploy.py
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     2165 2017-09-01 19:06:25.000000 lftools-0.9.0/lftools/cli/license.py
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     1646 2017-09-01 19:06:25.000000 lftools-0.9.0/lftools/cli/nexus.py
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     2654 2017-09-01 19:06:25.000000 lftools-0.9.0/lftools/cli/sign.py
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     3574 2017-09-01 19:06:25.000000 lftools-0.9.0/lftools/cli/version.py
-drwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)        0 2017-09-05 17:34:55.000000 lftools-0.9.0/lftools/nexus/
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     7383 2017-09-01 19:06:25.000000 lftools-0.9.0/lftools/nexus/__init__.py
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     5156 2017-09-01 19:06:25.000000 lftools-0.9.0/lftools/nexus/cmd.py
-drwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)        0 2017-09-05 17:34:55.000000 lftools-0.9.0/lftools/openstack/
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)      549 2017-09-01 19:06:25.000000 lftools-0.9.0/lftools/openstack/__init__.py
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     2818 2017-09-01 19:06:25.000000 lftools-0.9.0/lftools/openstack/cmd.py
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     3295 2017-09-01 19:06:25.000000 lftools-0.9.0/lftools/openstack/image.py
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     2635 2017-09-01 19:06:25.000000 lftools-0.9.0/lftools/openstack/server.py
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     2148 2017-09-05 16:09:05.000000 lftools-0.9.0/lftools/__init__.py
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     2500 2017-09-01 19:06:25.000000 lftools-0.9.0/lftools/license.py
-drwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)        0 2017-09-05 17:34:55.000000 lftools-0.9.0/lftools.egg-info/
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)      917 2017-09-05 17:34:55.000000 lftools-0.9.0/lftools.egg-info/PKG-INFO
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)      730 2017-09-05 17:34:55.000000 lftools-0.9.0/lftools.egg-info/SOURCES.txt
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)        1 2017-09-05 17:34:55.000000 lftools-0.9.0/lftools.egg-info/dependency_links.txt
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)       64 2017-09-05 17:34:55.000000 lftools-0.9.0/lftools.egg-info/entry_points.txt
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)      163 2017-09-05 17:34:55.000000 lftools-0.9.0/lftools.egg-info/requires.txt
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)        8 2017-09-05 17:34:55.000000 lftools-0.9.0/lftools.egg-info/top_level.txt
-drwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)        0 2017-09-05 17:34:55.000000 lftools-0.9.0/shell/
--rwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)    22102 2017-09-01 19:06:25.000000 lftools-0.9.0/shell/deploy
--rwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)     5159 2017-09-01 19:06:35.000000 lftools-0.9.0/shell/sign
--rwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)     7566 2017-09-01 19:06:25.000000 lftools-0.9.0/shell/version
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)       49 2017-09-01 19:06:25.000000 lftools-0.9.0/MANIFEST.in
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)      215 2017-09-01 19:06:25.000000 lftools-0.9.0/requirements.txt
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     2081 2017-09-01 19:06:25.000000 lftools-0.9.0/setup.py
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)      917 2017-09-05 17:34:55.000000 lftools-0.9.0/PKG-INFO
--rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)       38 2017-09-05 17:34:55.000000 lftools-0.9.0/setup.cfg
+drwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)        0 2017-09-29 16:39:36.000000 lftools-0.9.1/
+drwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)        0 2017-09-29 16:39:36.000000 lftools-0.9.1/etc/
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)      335 2017-09-01 19:06:25.000000 lftools-0.9.1/etc/logging.ini
+drwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)        0 2017-09-29 16:39:36.000000 lftools-0.9.1/lftools/
+drwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)        0 2017-09-29 16:39:36.000000 lftools-0.9.1/lftools/cli/
+drwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)        0 2017-09-29 16:39:36.000000 lftools-0.9.1/lftools/cli/jenkins/
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     2224 2017-09-01 19:06:25.000000 lftools-0.9.1/lftools/cli/jenkins/__init__.py
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     1445 2017-09-01 19:06:25.000000 lftools-0.9.1/lftools/cli/jenkins/builds.py
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     1171 2017-09-01 19:06:25.000000 lftools-0.9.1/lftools/cli/jenkins/nodes.py
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     3572 2017-09-01 19:06:25.000000 lftools-0.9.1/lftools/cli/jenkins/plugins.py
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     1261 2017-09-01 19:06:25.000000 lftools-0.9.1/lftools/cli/__init__.py
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     7196 2017-09-01 19:06:25.000000 lftools-0.9.1/lftools/cli/deploy.py
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     2165 2017-09-01 19:06:25.000000 lftools-0.9.1/lftools/cli/license.py
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     1646 2017-09-01 19:06:25.000000 lftools-0.9.1/lftools/cli/nexus.py
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     2654 2017-09-01 19:06:25.000000 lftools-0.9.1/lftools/cli/sign.py
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     3574 2017-09-01 19:06:25.000000 lftools-0.9.1/lftools/cli/version.py
+drwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)        0 2017-09-29 16:39:36.000000 lftools-0.9.1/lftools/nexus/
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     7383 2017-09-01 19:06:25.000000 lftools-0.9.1/lftools/nexus/__init__.py
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     5156 2017-09-01 19:06:25.000000 lftools-0.9.1/lftools/nexus/cmd.py
+drwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)        0 2017-09-29 16:39:36.000000 lftools-0.9.1/lftools/openstack/
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)      549 2017-09-01 19:06:25.000000 lftools-0.9.1/lftools/openstack/__init__.py
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     2818 2017-09-01 19:06:25.000000 lftools-0.9.1/lftools/openstack/cmd.py
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     3295 2017-09-01 19:06:25.000000 lftools-0.9.1/lftools/openstack/image.py
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     2635 2017-09-01 19:06:25.000000 lftools-0.9.1/lftools/openstack/server.py
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     2148 2017-09-29 16:39:04.000000 lftools-0.9.1/lftools/__init__.py
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     2500 2017-09-01 19:06:25.000000 lftools-0.9.1/lftools/license.py
+drwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)        0 2017-09-29 16:39:36.000000 lftools-0.9.1/lftools.egg-info/
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)      917 2017-09-29 16:39:36.000000 lftools-0.9.1/lftools.egg-info/PKG-INFO
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)      740 2017-09-29 16:39:36.000000 lftools-0.9.1/lftools.egg-info/SOURCES.txt
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)        1 2017-09-29 16:39:36.000000 lftools-0.9.1/lftools.egg-info/dependency_links.txt
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)       64 2017-09-29 16:39:36.000000 lftools-0.9.1/lftools.egg-info/entry_points.txt
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)      163 2017-09-29 16:39:36.000000 lftools-0.9.1/lftools.egg-info/requires.txt
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)        8 2017-09-29 16:39:36.000000 lftools-0.9.1/lftools.egg-info/top_level.txt
+drwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)        0 2017-09-29 16:39:36.000000 lftools-0.9.1/shell/
+-rwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)    22106 2017-09-29 16:16:41.000000 lftools-0.9.1/shell/deploy
+-rwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)     5159 2017-09-01 19:06:35.000000 lftools-0.9.1/shell/sign
+-rwxr-xr-x   0 zxiiro    (1000) zxiiro    (1000)     7566 2017-09-01 19:06:25.000000 lftools-0.9.1/shell/version
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)       49 2017-09-29 16:39:04.000000 lftools-0.9.1/MANIFEST.in
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)      117 2017-09-29 16:39:04.000000 lftools-0.9.1/README.md
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)      215 2017-09-01 19:06:25.000000 lftools-0.9.1/requirements.txt
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)     2081 2017-09-29 16:39:04.000000 lftools-0.9.1/setup.py
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)      917 2017-09-29 16:39:36.000000 lftools-0.9.1/PKG-INFO
+-rw-r--r--   0 zxiiro    (1000) zxiiro    (1000)       38 2017-09-29 16:39:36.000000 lftools-0.9.1/setup.cfg
```

### Comparing `lftools-0.9.0/lftools/cli/jenkins/__init__.py` & `lftools-0.9.1/lftools/cli/jenkins/__init__.py`

 * *Files identical despite different names*

### Comparing `lftools-0.9.0/lftools/cli/jenkins/builds.py` & `lftools-0.9.1/lftools/cli/jenkins/builds.py`

 * *Files identical despite different names*

### Comparing `lftools-0.9.0/lftools/cli/jenkins/nodes.py` & `lftools-0.9.1/lftools/cli/jenkins/nodes.py`

 * *Files identical despite different names*

### Comparing `lftools-0.9.0/lftools/cli/jenkins/plugins.py` & `lftools-0.9.1/lftools/cli/jenkins/plugins.py`

 * *Files identical despite different names*

### Comparing `lftools-0.9.0/lftools/cli/__init__.py` & `lftools-0.9.1/lftools/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `lftools-0.9.0/lftools/cli/deploy.py` & `lftools-0.9.1/lftools/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `lftools-0.9.0/lftools/cli/license.py` & `lftools-0.9.1/lftools/cli/license.py`

 * *Files identical despite different names*

### Comparing `lftools-0.9.0/lftools/cli/nexus.py` & `lftools-0.9.1/lftools/cli/nexus.py`

 * *Files identical despite different names*

### Comparing `lftools-0.9.0/lftools/cli/sign.py` & `lftools-0.9.1/lftools/cli/sign.py`

 * *Files identical despite different names*

### Comparing `lftools-0.9.0/lftools/cli/version.py` & `lftools-0.9.1/lftools/cli/version.py`

 * *Files identical despite different names*

### Comparing `lftools-0.9.0/lftools/nexus/__init__.py` & `lftools-0.9.1/lftools/nexus/__init__.py`

 * *Files identical despite different names*

### Comparing `lftools-0.9.0/lftools/nexus/cmd.py` & `lftools-0.9.1/lftools/nexus/cmd.py`

 * *Files identical despite different names*

### Comparing `lftools-0.9.0/lftools/openstack/__init__.py` & `lftools-0.9.1/lftools/openstack/__init__.py`

 * *Files identical despite different names*

### Comparing `lftools-0.9.0/lftools/openstack/cmd.py` & `lftools-0.9.1/lftools/openstack/cmd.py`

 * *Files identical despite different names*

### Comparing `lftools-0.9.0/lftools/openstack/image.py` & `lftools-0.9.1/lftools/openstack/image.py`

 * *Files identical despite different names*

### Comparing `lftools-0.9.0/lftools/openstack/server.py` & `lftools-0.9.1/lftools/openstack/server.py`

 * *Files identical despite different names*

### Comparing `lftools-0.9.0/lftools/__init__.py` & `lftools-0.9.1/lftools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Contributors:
 #   Thanh Ha - Initial implementation
 ##############################################################################
 """lftools package."""
 
 __author__ = 'Thanh Ha'
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 import logging
 import logging.config
 import os
 import sys
 
 log = logging.getLogger(__name__)
```

### Comparing `lftools-0.9.0/lftools/license.py` & `lftools-0.9.1/lftools/license.py`

 * *Files identical despite different names*

### Comparing `lftools-0.9.0/lftools.egg-info/PKG-INFO` & `lftools-0.9.1/lftools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: lftools
-Version: 0.9.0
+Version: 0.9.1
 Summary: Linux Foundation Release Engineering Tools
 Website: https://lf-releng-tools.readthedocs.io/en/latest/
 
 Home-page: UNKNOWN
 Author: Thanh Ha
 Author-email: thanh.ha@linuxfoundation.org
 License: EPL
```

### Comparing `lftools-0.9.0/lftools.egg-info/SOURCES.txt` & `lftools-0.9.1/lftools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 MANIFEST.in
+README.md
 requirements.txt
 setup.py
 etc/logging.ini
 lftools/__init__.py
 lftools/license.py
 lftools.egg-info/PKG-INFO
 lftools.egg-info/SOURCES.txt
```

### Comparing `lftools-0.9.0/shell/deploy` & `lftools-0.9.1/shell/deploy`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
     tmpdir=$(mktemp -d)
     pushd "$tmpdir"
 
     touch "_build-details.log"
     {
         echo "build-url: ${build_url}"
     } 2>&1 | tee -a "_build-details.log"
-    env | grep -v -E "SSH|HUDSON|COOKIE|TOKEN|DOCKER|PASSWORD" | sort > "_build-enviroment-variables.log"
+    env | grep -v -E "COOKIE|DOCKER|HUDSON|KEY|PASSWORD|SSH|TOKEN" | sort > "_build-enviroment-variables.log"
 
     # Print system info before collecting logs
     touch "_sys-info.log"
     {
         local sys_cmds
         sys_cmds=(
             "uname -a"
```

### Comparing `lftools-0.9.0/shell/sign` & `lftools-0.9.1/shell/sign`

 * *Files identical despite different names*

### Comparing `lftools-0.9.0/shell/version` & `lftools-0.9.1/shell/version`

 * *Files identical despite different names*

### Comparing `lftools-0.9.0/setup.py` & `lftools-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `lftools-0.9.0/PKG-INFO` & `lftools-0.9.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: lftools
-Version: 0.9.0
+Version: 0.9.1
 Summary: Linux Foundation Release Engineering Tools
 Website: https://lf-releng-tools.readthedocs.io/en/latest/
 
 Home-page: UNKNOWN
 Author: Thanh Ha
 Author-email: thanh.ha@linuxfoundation.org
 License: EPL
```

