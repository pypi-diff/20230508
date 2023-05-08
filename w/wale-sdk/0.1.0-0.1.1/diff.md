# Comparing `tmp/wale-sdk-0.1.0.tar.gz` & `tmp/wale-sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wale-sdk-0.1.0.tar", last modified: Sun May  7 22:44:17 2023, max compression
+gzip compressed data, was "wale-sdk-0.1.1.tar", last modified: Mon May  8 00:00:32 2023, max compression
```

## Comparing `wale-sdk-0.1.0.tar` & `wale-sdk-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 zachzhao   (501) staff       (20)        0 2023-05-07 22:44:17.741481 wale-sdk-0.1.0/
--rw-r--r--   0 zachzhao   (501) staff       (20)      554 2023-05-07 22:44:17.741345 wale-sdk-0.1.0/PKG-INFO
--rw-r--r--   0 zachzhao   (501) staff       (20)        0 2023-05-07 21:20:17.000000 wale-sdk-0.1.0/README.md
--rw-r--r--   0 zachzhao   (501) staff       (20)       38 2023-05-07 22:44:17.741521 wale-sdk-0.1.0/setup.cfg
--rw-r--r--   0 zachzhao   (501) staff       (20)      797 2023-05-07 22:35:39.000000 wale-sdk-0.1.0/setup.py
-drwxr-xr-x   0 zachzhao   (501) staff       (20)        0 2023-05-07 22:44:17.740456 wale-sdk-0.1.0/wale/
--rw-r--r--   0 zachzhao   (501) staff       (20)       42 2023-05-07 22:10:59.000000 wale-sdk-0.1.0/wale/__init__.py
--rw-r--r--   0 zachzhao   (501) staff       (20)     1589 2023-05-07 22:11:09.000000 wale-sdk-0.1.0/wale/wale.py
-drwxr-xr-x   0 zachzhao   (501) staff       (20)        0 2023-05-07 22:44:17.741172 wale-sdk-0.1.0/wale_sdk.egg-info/
--rw-r--r--   0 zachzhao   (501) staff       (20)      554 2023-05-07 22:44:17.000000 wale-sdk-0.1.0/wale_sdk.egg-info/PKG-INFO
--rw-r--r--   0 zachzhao   (501) staff       (20)      207 2023-05-07 22:44:17.000000 wale-sdk-0.1.0/wale_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 zachzhao   (501) staff       (20)        1 2023-05-07 22:44:17.000000 wale-sdk-0.1.0/wale_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 zachzhao   (501) staff       (20)       86 2023-05-07 22:44:17.000000 wale-sdk-0.1.0/wale_sdk.egg-info/requires.txt
--rw-r--r--   0 zachzhao   (501) staff       (20)        5 2023-05-07 22:44:17.000000 wale-sdk-0.1.0/wale_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 zachzhao   (501) staff       (20)        0 2023-05-08 00:00:32.116950 wale-sdk-0.1.1/
+-rw-r--r--   0 zachzhao   (501) staff       (20)      554 2023-05-08 00:00:32.116815 wale-sdk-0.1.1/PKG-INFO
+-rw-r--r--   0 zachzhao   (501) staff       (20)     1332 2023-05-07 22:50:13.000000 wale-sdk-0.1.1/README.md
+-rw-r--r--   0 zachzhao   (501) staff       (20)       38 2023-05-08 00:00:32.116990 wale-sdk-0.1.1/setup.cfg
+-rw-r--r--   0 zachzhao   (501) staff       (20)      797 2023-05-07 23:51:05.000000 wale-sdk-0.1.1/setup.py
+drwxr-xr-x   0 zachzhao   (501) staff       (20)        0 2023-05-08 00:00:32.115708 wale-sdk-0.1.1/wale/
+-rw-r--r--   0 zachzhao   (501) staff       (20)       42 2023-05-07 22:10:59.000000 wale-sdk-0.1.1/wale/__init__.py
+-rw-r--r--   0 zachzhao   (501) staff       (20)     1926 2023-05-07 23:36:52.000000 wale-sdk-0.1.1/wale/wale.py
+drwxr-xr-x   0 zachzhao   (501) staff       (20)        0 2023-05-08 00:00:32.116629 wale-sdk-0.1.1/wale_sdk.egg-info/
+-rw-r--r--   0 zachzhao   (501) staff       (20)      554 2023-05-08 00:00:32.000000 wale-sdk-0.1.1/wale_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 zachzhao   (501) staff       (20)      207 2023-05-08 00:00:32.000000 wale-sdk-0.1.1/wale_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 zachzhao   (501) staff       (20)        1 2023-05-08 00:00:32.000000 wale-sdk-0.1.1/wale_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 zachzhao   (501) staff       (20)      125 2023-05-08 00:00:32.000000 wale-sdk-0.1.1/wale_sdk.egg-info/requires.txt
+-rw-r--r--   0 zachzhao   (501) staff       (20)        5 2023-05-08 00:00:32.000000 wale-sdk-0.1.1/wale_sdk.egg-info/top_level.txt
```

### Comparing `wale-sdk-0.1.0/PKG-INFO` & `wale-sdk-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wale-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Telemetry for LLMs
 Home-page: https://github.com/trywale
 Author: Zach Zhao
 Author-email: zach@trywale.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wale-sdk-0.1.0/setup.py` & `wale-sdk-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='wale-sdk',
-    version='0.1.0',
+    version='0.1.1',
     description='Telemetry for LLMs',
     author='Zach Zhao',
     author_email='zach@trywale.com',
     url='https://github.com/trywale',
     packages=find_packages(exclude=['tests']),
     install_requires=requirements,
     classifiers=[
```

### Comparing `wale-sdk-0.1.0/wale_sdk.egg-info/PKG-INFO` & `wale-sdk-0.1.1/wale_sdk.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wale-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Telemetry for LLMs
 Home-page: https://github.com/trywale
 Author: Zach Zhao
 Author-email: zach@trywale.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

