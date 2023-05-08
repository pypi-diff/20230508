# Comparing `tmp/pqinput-0.0.3.tar.gz` & `tmp/pqinput-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqinput-0.0.3.tar", last modified: Mon May  8 09:03:02 2023, max compression
+gzip compressed data, was "pqinput-0.0.31.tar", last modified: Mon May  8 09:27:50 2023, max compression
```

## Comparing `pqinput-0.0.3.tar` & `pqinput-0.0.31.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-08 09:03:02.726419 pqinput-0.0.3/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1075 2023-02-09 10:07:34.000000 pqinput-0.0.3/LICENSE.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1934 2023-05-08 09:03:02.726419 pqinput-0.0.3/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1363 2023-02-20 12:29:30.000000 pqinput-0.0.3/README.md
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-08 09:03:02.726419 pqinput-0.0.3/pqinput/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      119 2023-05-04 15:25:36.000000 pqinput-0.0.3/pqinput/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     8411 2023-05-08 08:52:27.000000 pqinput-0.0.3/pqinput/drawPES.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    13687 2023-05-04 15:14:28.000000 pqinput-0.0.3/pqinput/inpxml.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-08 09:03:02.726419 pqinput-0.0.3/pqinput.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1934 2023-05-08 09:03:02.000000 pqinput-0.0.3/pqinput.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      226 2023-05-08 09:03:02.000000 pqinput-0.0.3/pqinput.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-08 09:03:02.000000 pqinput-0.0.3/pqinput.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        8 2023-05-08 09:03:02.000000 pqinput-0.0.3/pqinput.egg-info/top_level.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      540 2023-05-08 09:01:24.000000 pqinput-0.0.3/pyproject.toml
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-08 09:03:02.726419 pqinput-0.0.3/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      651 2023-05-08 09:01:57.000000 pqinput-0.0.3/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-08 09:27:50.498871 pqinput-0.0.31/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1075 2023-02-09 10:07:34.000000 pqinput-0.0.31/LICENSE.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1935 2023-05-08 09:27:50.498871 pqinput-0.0.31/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1363 2023-02-20 12:29:30.000000 pqinput-0.0.31/README.md
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-08 09:27:50.498871 pqinput-0.0.31/pqinput/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      119 2023-05-04 15:25:36.000000 pqinput-0.0.31/pqinput/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     8411 2023-05-08 08:52:27.000000 pqinput-0.0.31/pqinput/drawPES.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    13861 2023-05-08 09:26:13.000000 pqinput-0.0.31/pqinput/inpxml.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-08 09:27:50.498871 pqinput-0.0.31/pqinput.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1935 2023-05-08 09:27:50.000000 pqinput-0.0.31/pqinput.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      226 2023-05-08 09:27:50.000000 pqinput-0.0.31/pqinput.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-08 09:27:50.000000 pqinput-0.0.31/pqinput.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        8 2023-05-08 09:27:50.000000 pqinput-0.0.31/pqinput.egg-info/top_level.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      541 2023-05-08 09:27:24.000000 pqinput-0.0.31/pyproject.toml
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-08 09:27:50.498871 pqinput-0.0.31/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      652 2023-05-08 09:27:17.000000 pqinput-0.0.31/setup.py
```

### Comparing `pqinput-0.0.3/LICENSE.txt` & `pqinput-0.0.31/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.3/PKG-INFO` & `pqinput-0.0.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqinput
-Version: 0.0.3
+Version: 0.0.31
 Summary: Create input files for QDng calculations
 Home-page: https://gitlab.fysik.su.se/lucas.borges/inputxml
 Author: Lucas Borges
 Author-email: Lucas Borges <lucas.borges@fysik.su.se>
 License: MIT
 Project-URL: Homepage, https://gitlab.fysik.su.se/lucas.borges/pqinput
 Keywords: qdng
```

### Comparing `pqinput-0.0.3/README.md` & `pqinput-0.0.31/README.md`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.3/pqinput/drawPES.py` & `pqinput-0.0.31/pqinput/drawPES.py`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.3/pqinput/inpxml.py` & `pqinput-0.0.31/pqinput/inpxml.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,19 +84,24 @@
         return printx(getattr(self, storage_name))
     
     @propriety.setter
     def propriety(self, args):
         # modify key with new_value of propriedade using path 
         # args = [path, key, new_value] or "path_key_new_value"
         if isinstance(args, str): args = args.split('_') # single string format
-        path, key, new_value = args
-        element = getattr(self, storage_name).find(path)
-        if element is None: raise AttributeError('setter path do not point to a defined attribute.')
-        element.set(key, str(new_value))
-        printx(element)
+        
+        if len(args)==3:
+            path, key, new_value = args
+            element = getattr(self, storage_name).find(path)
+            if element is None: raise AttributeError('setter path do not point to a defined attribute.')
+            element.set(key, str(new_value))
+        else:
+            key, new_value = args
+            getattr(self, storage_name).set(key, new_value)
+        
         
         # READ MORE ABOUT XPATH AND IF ITS USEFUL
         
     return propriety
 # %% 
 '''-------------------------------------------------------------------------'''
 '''                                Class                                    '''
@@ -326,12 +331,14 @@
                    'm{}'.format(ind):{'name':'GridPotential', 'file':'MgH/mu/mu_Sig0Sig1'}}
                    for ind in [2.1,] ]
     #%%
     prop = InpXML()
     prop.program('propa', nparams, WFparams)
     prop.propagation('Cheby', Hparams)
     prop.filter('filterpost', filteropes)
+    prop.hamilt = 'name', 'b'
+
 
     prop.show
     # prop.writexml(txt=True)
```

### Comparing `pqinput-0.0.3/pqinput.egg-info/PKG-INFO` & `pqinput-0.0.31/pqinput.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqinput
-Version: 0.0.3
+Version: 0.0.31
 Summary: Create input files for QDng calculations
 Home-page: https://gitlab.fysik.su.se/lucas.borges/inputxml
 Author: Lucas Borges
 Author-email: Lucas Borges <lucas.borges@fysik.su.se>
 License: MIT
 Project-URL: Homepage, https://gitlab.fysik.su.se/lucas.borges/pqinput
 Keywords: qdng
```

### Comparing `pqinput-0.0.3/pyproject.toml` & `pqinput-0.0.31/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pqinput"
-version = "0.0.3"
+version = "0.0.31"
 authors = [
   { name="Lucas Borges", email="lucas.borges@fysik.su.se" },
 ]
 description = "Create input files for QDng calculations"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pqinput-0.0.3/setup.py` & `pqinput-0.0.31/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setuptools.setup(
     name = "pqinput",
-    version = "0.0.3",
+    version = "0.0.31",
     author = "Lucas Borges",
     author_email = "lucas.borges@fysik.su.se",
     description = ("additional functions for QDng calculations setups."),
     license = "MIT",
     keywords = "qdng",
     url = "https://gitlab.fysik.su.se/lucas.borges/inputxml",
     packages=setuptools.find_packages(),
```

