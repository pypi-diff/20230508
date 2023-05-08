# Comparing `tmp/tight_loops-0.2.2.tar.gz` & `tmp/tight_loops-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tight_loops-0.2.2.tar", last modified: Thu Apr 27 19:19:06 2023, max compression
+gzip compressed data, was "tight_loops-0.2.3.tar", last modified: Mon May  8 17:22:24 2023, max compression
```

## Comparing `tight_loops-0.2.2.tar` & `tight_loops-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:19:05.995091 tight_loops-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-27 19:18:53.000000 tight_loops-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-27 19:18:53.000000 tight_loops-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-27 19:19:05.995091 tight_loops-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-27 19:18:53.000000 tight_loops-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 19:18:53.000000 tight_loops-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-27 19:19:05.995091 tight_loops-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-27 19:18:53.000000 tight_loops-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:19:05.995091 tight_loops-0.2.2/tight_loops/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-27 19:18:53.000000 tight_loops-0.2.2/tight_loops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-27 19:18:53.000000 tight_loops-0.2.2/tight_loops/folium_loops.py
--rw-r--r--   0 runner    (1001) docker     (123)    10869 2023-04-27 19:18:53.000000 tight_loops-0.2.2/tight_loops/tight_loops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:19:05.995091 tight_loops-0.2.2/tight_loops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-27 19:19:05.000000 tight_loops-0.2.2/tight_loops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-27 19:19:05.000000 tight_loops-0.2.2/tight_loops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-27 19:19:05.000000 tight_loops-0.2.2/tight_loops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:19:05.000000 tight_loops-0.2.2/tight_loops.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-27 19:19:05.000000 tight_loops-0.2.2/tight_loops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 19:19:05.000000 tight_loops-0.2.2/tight_loops.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:22:24.096821 tight_loops-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-08 17:22:08.000000 tight_loops-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-08 17:22:08.000000 tight_loops-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-08 17:22:24.096821 tight_loops-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-08 17:22:08.000000 tight_loops-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 17:22:08.000000 tight_loops-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 17:22:24.096821 tight_loops-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-08 17:22:08.000000 tight_loops-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:22:24.096821 tight_loops-0.2.3/tight_loops/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-08 17:22:08.000000 tight_loops-0.2.3/tight_loops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-08 17:22:08.000000 tight_loops-0.2.3/tight_loops/folium_loops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-05-08 17:22:08.000000 tight_loops-0.2.3/tight_loops/tight_loops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:22:24.096821 tight_loops-0.2.3/tight_loops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-08 17:22:24.000000 tight_loops-0.2.3/tight_loops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-08 17:22:24.000000 tight_loops-0.2.3/tight_loops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 17:22:24.000000 tight_loops-0.2.3/tight_loops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:22:24.000000 tight_loops-0.2.3/tight_loops.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 17:22:24.000000 tight_loops-0.2.3/tight_loops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 17:22:24.000000 tight_loops-0.2.3/tight_loops.egg-info/top_level.txt
```

### Comparing `tight_loops-0.2.2/LICENSE` & `tight_loops-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tight_loops-0.2.2/PKG-INFO` & `tight_loops-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tight_loops
-Version: 0.2.2
+Version: 0.2.3
 Summary: This is a demo python package for UTK GEOG510
 Home-page: https://github.com/wnelso18/tight_loops
 Author: Will Nelson
 Author-email: wnelso18@vols.utk.edu
 License: MIT license
 Keywords: tight_loops
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `tight_loops-0.2.2/README.md` & `tight_loops-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tight_loops-0.2.2/setup.py` & `tight_loops-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='tight_loops',
     name='tight_loops',
     packages=find_packages(include=['tight_loops', 'tight_loops.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/wnelso18/tight_loops',
-    version='0.2.2',
+    version='0.2.3',
     zip_safe=False,
 )
```

### Comparing `tight_loops-0.2.2/tight_loops/tight_loops.py` & `tight_loops-0.2.3/tight_loops/tight_loops.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,14 +215,15 @@
         """
 
         widget = widgets.HTML(value=f"<img src={url} width='{width}' height='{height}'>")
         control = WidgetControl(widget=widget, position = position)
         self.add_control(control)
 
     def add_toolbar(self, position="topright"):
+        
 
         widget_width = "250px"
         padding = "0px 0px 0px 5px"  # upper, right, bottom, left
 
         toolbar_button = widgets.ToggleButton(
             value=False,
             tooltip="Toolbar",
```

### Comparing `tight_loops-0.2.2/tight_loops.egg-info/PKG-INFO` & `tight_loops-0.2.3/tight_loops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tight-loops
-Version: 0.2.2
+Version: 0.2.3
 Summary: This is a demo python package for UTK GEOG510
 Home-page: https://github.com/wnelso18/tight_loops
 Author: Will Nelson
 Author-email: wnelso18@vols.utk.edu
 License: MIT license
 Keywords: tight_loops
 Classifier: Development Status :: 2 - Pre-Alpha
```

