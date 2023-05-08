# Comparing `tmp/hestia-earth-schema-9.7.0.tar.gz` & `tmp/hestia-earth-schema-9.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hestia-earth-schema-9.7.0.tar", last modified: Tue Aug  2 10:06:24 2022, max compression
+gzip compressed data, was "hestia-earth-schema-9.7.1.tar", last modified: Thu Aug  4 13:11:47 2022, max compression
```

## Comparing `hestia-earth-schema-9.7.0.tar` & `hestia-earth-schema-9.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 10:06:24.905558 hestia-earth-schema-9.7.0/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2022-08-02 10:06:15.000000 hestia-earth-schema-9.7.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      815 2022-08-02 10:06:24.905558 hestia-earth-schema-9.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      957 2022-08-02 10:06:15.000000 hestia-earth-schema-9.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 10:06:24.903558 hestia-earth-schema-9.7.0/hestia_earth/
--rw-rw-rw-   0 root         (0) root         (0)       56 2022-08-02 10:06:15.000000 hestia-earth-schema-9.7.0/hestia_earth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 10:06:24.903558 hestia-earth-schema-9.7.0/hestia_earth/schema/
--rw-r--r--   0 root         (0) root         (0)    64147 2022-08-02 10:05:26.000000 hestia-earth-schema-9.7.0/hestia_earth/schema/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 10:06:24.904558 hestia-earth-schema-9.7.0/hestia_earth/schema/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      229 2022-08-02 10:05:04.000000 hestia-earth-schema-9.7.0/hestia_earth/schema/migrations/1654666500000_remove_ImpactAssessment_systemBoundary.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2022-08-02 10:05:04.000000 hestia-earth-schema-9.7.0/hestia_earth/schema/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 10:06:24.905558 hestia-earth-schema-9.7.0/hestia_earth_schema.egg-info/
--rw-r--r--   0 root         (0) root         (0)      815 2022-08-02 10:06:24.000000 hestia-earth-schema-9.7.0/hestia_earth_schema.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      395 2022-08-02 10:06:24.000000 hestia-earth-schema-9.7.0/hestia_earth_schema.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-02 10:06:24.000000 hestia-earth-schema-9.7.0/hestia_earth_schema.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-08-02 10:06:24.000000 hestia-earth-schema-9.7.0/hestia_earth_schema.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       79 2022-08-02 10:06:24.906558 hestia-earth-schema-9.7.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      619 2022-08-02 10:06:15.000000 hestia-earth-schema-9.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 13:11:47.721705 hestia-earth-schema-9.7.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2022-08-04 13:11:38.000000 hestia-earth-schema-9.7.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      795 2022-08-04 13:11:47.721705 hestia-earth-schema-9.7.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      957 2022-08-04 13:11:38.000000 hestia-earth-schema-9.7.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 13:11:47.718705 hestia-earth-schema-9.7.1/hestia_earth/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2022-08-04 13:11:38.000000 hestia-earth-schema-9.7.1/hestia_earth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 13:11:47.719705 hestia-earth-schema-9.7.1/hestia_earth/schema/
+-rw-r--r--   0 root         (0) root         (0)    64147 2022-08-04 13:10:47.000000 hestia-earth-schema-9.7.1/hestia_earth/schema/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 13:11:47.719705 hestia-earth-schema-9.7.1/hestia_earth/schema/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      229 2022-08-04 13:10:24.000000 hestia-earth-schema-9.7.1/hestia_earth/schema/migrations/1654666500000_remove_ImpactAssessment_systemBoundary.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2022-08-04 13:10:24.000000 hestia-earth-schema-9.7.1/hestia_earth/schema/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 13:11:47.721705 hestia-earth-schema-9.7.1/hestia_earth_schema.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      795 2022-08-04 13:11:47.000000 hestia-earth-schema-9.7.1/hestia_earth_schema.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      395 2022-08-04 13:11:47.000000 hestia-earth-schema-9.7.1/hestia_earth_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-04 13:11:47.000000 hestia-earth-schema-9.7.1/hestia_earth_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-08-04 13:11:47.000000 hestia-earth-schema-9.7.1/hestia_earth_schema.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       79 2022-08-04 13:11:47.722705 hestia-earth-schema-9.7.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      619 2022-08-04 13:11:38.000000 hestia-earth-schema-9.7.1/setup.py
```

### Comparing `hestia-earth-schema-9.7.0/LICENSE` & `hestia-earth-schema-9.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hestia-earth-schema-9.7.0/README.md` & `hestia-earth-schema-9.7.1/README.md`

 * *Files identical despite different names*

### Comparing `hestia-earth-schema-9.7.0/hestia_earth/schema/__init__.py` & `hestia-earth-schema-9.7.1/hestia_earth/schema/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # auto-generated content
 from collections import OrderedDict
 from enum import Enum
 from pkgutil import extend_path
 
 
 __path__ = extend_path(__path__, __name__)
-SCHEMA_VERSION = '9.7.0'
+SCHEMA_VERSION = '9.7.1'
 NESTED_SEARCHABLE_KEYS = [
     'otherSites',
     'inputs',
     'emissions',
     'products',
     'practices',
     'transformations',
```

### Comparing `hestia-earth-schema-9.7.0/setup.py` & `hestia-earth-schema-9.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open('docs/python.md', 'r') as fh:
     long_description = fh.read()
 
 
 setup(
     name='hestia-earth-schema',
     packages=find_packages(),
-    version='9.7.0',
+    version='9.7.1',
     description='Hestia Schema library',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Guillaume Royer',
     author_email='guillaumeroyer.mail@gmail.com',
     license='GPL-3.0-or-later',
     url='https://gitlab.com/hestia-earth/hestia-schema',
```

