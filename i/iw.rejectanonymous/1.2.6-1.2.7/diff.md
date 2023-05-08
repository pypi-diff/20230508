# Comparing `tmp/iw.rejectanonymous-1.2.6.tar.gz` & `tmp/iw.rejectanonymous-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iw.rejectanonymous-1.2.6.tar", last modified: Wed May 11 10:45:33 2022, max compression
+gzip compressed data, was "iw.rejectanonymous-1.2.7.tar", last modified: Mon May  8 08:42:14 2023, max compression
```

## Comparing `iw.rejectanonymous-1.2.6.tar` & `iw.rejectanonymous-1.2.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-05-11 10:45:33.717739 iw.rejectanonymous-1.2.6/
--rw-rw-r--   0 ale       (1000) ale       (1000)       34 2022-05-11 10:45:32.000000 iw.rejectanonymous-1.2.6/.gitignore
--rw-rw-r--   0 ale       (1000) ale       (1000)     2161 2022-05-11 10:45:32.000000 iw.rejectanonymous-1.2.6/CHANGES.rst
--rw-rw-r--   0 ale       (1000) ale       (1000)       75 2022-05-11 10:45:32.000000 iw.rejectanonymous-1.2.6/MANIFEST.in
--rw-rw-r--   0 ale       (1000) ale       (1000)     6402 2022-05-11 10:45:33.717739 iw.rejectanonymous-1.2.6/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)     3476 2022-05-11 10:45:32.000000 iw.rejectanonymous-1.2.6/README.rst
--rw-rw-r--   0 ale       (1000) ale       (1000)     1737 2022-05-11 10:45:32.000000 iw.rejectanonymous-1.2.6/bootstrap.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-05-11 10:45:33.717739 iw.rejectanonymous-1.2.6/iw/
--rw-rw-r--   0 ale       (1000) ale       (1000)      244 2022-05-11 10:45:32.000000 iw.rejectanonymous-1.2.6/iw/__init__.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-05-11 10:45:33.717739 iw.rejectanonymous-1.2.6/iw/rejectanonymous/
--rw-rw-r--   0 ale       (1000) ale       (1000)     4168 2022-05-11 10:45:32.000000 iw.rejectanonymous-1.2.6/iw/rejectanonymous/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      871 2022-05-11 10:45:32.000000 iw.rejectanonymous-1.2.6/iw/rejectanonymous/configure.zcml
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-05-11 10:45:33.717739 iw.rejectanonymous-1.2.6/iw/rejectanonymous/doctests/
--rw-rw-r--   0 ale       (1000) ale       (1000)     5647 2022-05-11 10:45:32.000000 iw.rejectanonymous-1.2.6/iw/rejectanonymous/doctests/README.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)     2353 2022-05-11 10:45:32.000000 iw.rejectanonymous-1.2.6/iw/rejectanonymous/plonecontrolpanel.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-05-11 10:45:33.717739 iw.rejectanonymous-1.2.6/iw/rejectanonymous/tests/
--rw-rw-r--   0 ale       (1000) ale       (1000)       18 2022-05-11 10:45:32.000000 iw.rejectanonymous-1.2.6/iw/rejectanonymous/tests/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1359 2022-05-11 10:45:32.000000 iw.rejectanonymous-1.2.6/iw/rejectanonymous/tests/base.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2726 2022-05-11 10:45:32.000000 iw.rejectanonymous-1.2.6/iw/rejectanonymous/tests/test_rejectanonymousdocs.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      335 2022-05-11 10:45:32.000000 iw.rejectanonymous-1.2.6/iw/rejectanonymous/utils.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-05-11 10:45:33.717739 iw.rejectanonymous-1.2.6/iw.rejectanonymous.egg-info/
--rw-rw-r--   0 ale       (1000) ale       (1000)     6402 2022-05-11 10:45:33.000000 iw.rejectanonymous-1.2.6/iw.rejectanonymous.egg-info/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)      723 2022-05-11 10:45:33.000000 iw.rejectanonymous-1.2.6/iw.rejectanonymous.egg-info/SOURCES.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2022-05-11 10:45:33.000000 iw.rejectanonymous-1.2.6/iw.rejectanonymous.egg-info/dependency_links.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)       40 2022-05-11 10:45:33.000000 iw.rejectanonymous-1.2.6/iw.rejectanonymous.egg-info/entry_points.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        3 2022-05-11 10:45:33.000000 iw.rejectanonymous-1.2.6/iw.rejectanonymous.egg-info/namespace_packages.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2022-05-11 10:45:33.000000 iw.rejectanonymous-1.2.6/iw.rejectanonymous.egg-info/not-zip-safe
--rw-rw-r--   0 ale       (1000) ale       (1000)       11 2022-05-11 10:45:33.000000 iw.rejectanonymous-1.2.6/iw.rejectanonymous.egg-info/requires.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        3 2022-05-11 10:45:33.000000 iw.rejectanonymous-1.2.6/iw.rejectanonymous.egg-info/top_level.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)       38 2022-05-11 10:45:33.717739 iw.rejectanonymous-1.2.6/setup.cfg
--rw-rw-r--   0 ale       (1000) ale       (1000)     1631 2022-05-11 10:45:32.000000 iw.rejectanonymous-1.2.6/setup.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-08 08:42:14.881175 iw.rejectanonymous-1.2.7/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       34 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/.gitignore
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2284 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/CHANGES.rst
+-rw-rw-r--   0 ale       (1000) ale       (1000)       75 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/MANIFEST.in
+-rw-rw-r--   0 ale       (1000) ale       (1000)     6527 2023-05-08 08:42:14.881175 iw.rejectanonymous-1.2.7/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3476 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/README.rst
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1737 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/bootstrap.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-08 08:42:14.881175 iw.rejectanonymous-1.2.7/iw/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      244 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/iw/__init__.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-08 08:42:14.881175 iw.rejectanonymous-1.2.7/iw/rejectanonymous/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4181 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/iw/rejectanonymous/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      871 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/iw/rejectanonymous/configure.zcml
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-08 08:42:14.881175 iw.rejectanonymous-1.2.7/iw/rejectanonymous/doctests/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     5647 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/iw/rejectanonymous/doctests/README.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2353 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/iw/rejectanonymous/plonecontrolpanel.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-08 08:42:14.881175 iw.rejectanonymous-1.2.7/iw/rejectanonymous/tests/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       18 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/iw/rejectanonymous/tests/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1359 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/iw/rejectanonymous/tests/base.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2726 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/iw/rejectanonymous/tests/test_rejectanonymousdocs.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      335 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/iw/rejectanonymous/utils.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-08 08:42:14.881175 iw.rejectanonymous-1.2.7/iw.rejectanonymous.egg-info/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     6527 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/iw.rejectanonymous.egg-info/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)      723 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/iw.rejectanonymous.egg-info/SOURCES.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/iw.rejectanonymous.egg-info/dependency_links.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       40 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/iw.rejectanonymous.egg-info/entry_points.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        3 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/iw.rejectanonymous.egg-info/namespace_packages.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/iw.rejectanonymous.egg-info/not-zip-safe
+-rw-rw-r--   0 ale       (1000) ale       (1000)       42 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/iw.rejectanonymous.egg-info/requires.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        3 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/iw.rejectanonymous.egg-info/top_level.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       38 2023-05-08 08:42:14.881175 iw.rejectanonymous-1.2.7/setup.cfg
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1730 2023-05-08 08:42:14.000000 iw.rejectanonymous-1.2.7/setup.py
```

### Comparing `iw.rejectanonymous-1.2.6/CHANGES.rst` & `iw.rejectanonymous-1.2.7/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changes log
 ===========
 
+1.2.7 (2023-05-08)
+------------------
+
+- Add ++webresource++ and ++plone++ to valid_subpart_prefixes (Plone 6)
+  [mamico]
+
 1.2.6 (2022-05-11)
 ------------------
 
 - Add @@ok to valid_ids
   [ale-rt]
 
 - Add custom.css to valid_ids (needed since Plone 5.2.2)
```

### Comparing `iw.rejectanonymous-1.2.6/PKG-INFO` & `iw.rejectanonymous-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: iw.rejectanonymous
-Version: 1.2.6
+Version: 1.2.7
 Summary: Disallow access to a Plone site and its children if user is anonymous
 Home-page: https://svn.plone.org/svn/collective/iw.rejectanonymous
 Author: Ingeniweb
 Author-email: support@ingeniweb.com
 License: GPL
 Keywords: plone extranet
-Platform: UNKNOWN
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 3.2
 Classifier: Framework :: Plone :: 3.3
 Classifier: Framework :: Plone :: 4.0
 Classifier: Framework :: Plone :: 4.1
 Classifier: Framework :: Plone :: 5.0
 Classifier: Framework :: Plone :: 5.1
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Zope2
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: test
 
 ==================
 iw.rejectanonymous
 ==================
 
 
 What is iw.rejectanonymous ?
@@ -166,14 +166,20 @@
 * Thomas Desvenain
 * Gilles Lenfant
 * Elisabeth Leddy
 
 Changes log
 ===========
 
+1.2.7 (2023-05-08)
+------------------
+
+- Add ++webresource++ and ++plone++ to valid_subpart_prefixes (Plone 6)
+  [mamico]
+
 1.2.6 (2022-05-11)
 ------------------
 
 - Add @@ok to valid_ids
   [ale-rt]
 
 - Add custom.css to valid_ids (needed since Plone 5.2.2)
@@ -287,8 +293,7 @@
 
 
 1.0.0 - 2008-02-11
 ------------------
 
 - Initial release
   [bmathieu]
-
```

### Comparing `iw.rejectanonymous-1.2.6/README.rst` & `iw.rejectanonymous-1.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `iw.rejectanonymous-1.2.6/bootstrap.py` & `iw.rejectanonymous-1.2.7/bootstrap.py`

 * *Files identical despite different names*

### Comparing `iw.rejectanonymous-1.2.6/iw/rejectanonymous/__init__.py` & `iw.rejectanonymous-1.2.7/iw/rejectanonymous/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 if HAS_RESTAPI:
     valid_ids = valid_ids.union(('reset-password', '@login', '@login-renew', '@logout'))
 
 valid_subparts = frozenset((
     'portal_css', 'portal_javascripts', 'passwordreset', 'portal_kss'
 ))
 
-valid_subpart_prefixes = frozenset(('++resource++', '++theme++', '++plone++static',
-    '++unique++',
+valid_subpart_prefixes = frozenset(('++resource++', '++theme++', '++plone++',
+    '++unique++', '++webresource++',
 ))
 
 
 # Customization functions
 def addValidIds(*new_ids):
     """A customized Plone site may need to publish other ids as resources
     of the login process. The policy or third party component just need to
```

### Comparing `iw.rejectanonymous-1.2.6/iw/rejectanonymous/configure.zcml` & `iw.rejectanonymous-1.2.7/iw/rejectanonymous/configure.zcml`

 * *Files identical despite different names*

### Comparing `iw.rejectanonymous-1.2.6/iw/rejectanonymous/doctests/README.txt` & `iw.rejectanonymous-1.2.7/iw/rejectanonymous/doctests/README.txt`

 * *Files identical despite different names*

### Comparing `iw.rejectanonymous-1.2.6/iw/rejectanonymous/plonecontrolpanel.py` & `iw.rejectanonymous-1.2.7/iw/rejectanonymous/plonecontrolpanel.py`

 * *Files identical despite different names*

### Comparing `iw.rejectanonymous-1.2.6/iw/rejectanonymous/tests/base.py` & `iw.rejectanonymous-1.2.7/iw/rejectanonymous/tests/base.py`

 * *Files identical despite different names*

### Comparing `iw.rejectanonymous-1.2.6/iw/rejectanonymous/tests/test_rejectanonymousdocs.py` & `iw.rejectanonymous-1.2.7/iw/rejectanonymous/tests/test_rejectanonymousdocs.py`

 * *Files identical despite different names*

### Comparing `iw.rejectanonymous-1.2.6/iw.rejectanonymous.egg-info/PKG-INFO` & `iw.rejectanonymous-1.2.7/iw.rejectanonymous.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: iw.rejectanonymous
-Version: 1.2.6
+Version: 1.2.7
 Summary: Disallow access to a Plone site and its children if user is anonymous
 Home-page: https://svn.plone.org/svn/collective/iw.rejectanonymous
 Author: Ingeniweb
 Author-email: support@ingeniweb.com
 License: GPL
 Keywords: plone extranet
-Platform: UNKNOWN
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 3.2
 Classifier: Framework :: Plone :: 3.3
 Classifier: Framework :: Plone :: 4.0
 Classifier: Framework :: Plone :: 4.1
 Classifier: Framework :: Plone :: 5.0
 Classifier: Framework :: Plone :: 5.1
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Zope2
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: test
 
 ==================
 iw.rejectanonymous
 ==================
 
 
 What is iw.rejectanonymous ?
@@ -166,14 +166,20 @@
 * Thomas Desvenain
 * Gilles Lenfant
 * Elisabeth Leddy
 
 Changes log
 ===========
 
+1.2.7 (2023-05-08)
+------------------
+
+- Add ++webresource++ and ++plone++ to valid_subpart_prefixes (Plone 6)
+  [mamico]
+
 1.2.6 (2022-05-11)
 ------------------
 
 - Add @@ok to valid_ids
   [ale-rt]
 
 - Add custom.css to valid_ids (needed since Plone 5.2.2)
@@ -287,8 +293,7 @@
 
 
 1.0.0 - 2008-02-11
 ------------------
 
 - Initial release
   [bmathieu]
-
```

### Comparing `iw.rejectanonymous-1.2.6/iw.rejectanonymous.egg-info/SOURCES.txt` & `iw.rejectanonymous-1.2.7/iw.rejectanonymous.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iw.rejectanonymous-1.2.6/setup.py` & `iw.rejectanonymous-1.2.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def read(*names):
     here = os.path.dirname(os.path.abspath(__file__))
     path = os.path.join(here, *names)
     return open(path, 'r').read().strip()
 
-version = '1.2.6'
+version = '1.2.7'
 
 setup(name='iw.rejectanonymous',
       version=version,
       description="Disallow access to a Plone site and its children if user is anonymous",
       long_description=(read('README.rst')
                         + '\n\n'
                         + read('CHANGES.rst')),
@@ -39,13 +39,18 @@
       namespace_packages=['iw'],
       include_package_data=True,
       zip_safe=False,
       install_requires=[
           'setuptools',
           # -*- Extra requirements: -*-
           ],
+      extras_require={
+        "test": [
+            "Products.PloneTestCase",
+        ],
+      },
       entry_points="""
       # -*- Entry points: -*-
       [z3c.autoinclude.plugin]
       target = plone
       """
       )
```

