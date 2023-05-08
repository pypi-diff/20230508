# Comparing `tmp/getmonitorresolution-0.10.tar.gz` & `tmp/getmonitorresolution-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getmonitorresolution-0.10.tar", last modified: Mon May  8 02:38:18 2023, max compression
+gzip compressed data, was "getmonitorresolution-0.11.tar", last modified: Mon May  8 02:49:56 2023, max compression
```

## Comparing `getmonitorresolution-0.10.tar` & `getmonitorresolution-0.11.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 02:38:18.413563 getmonitorresolution-0.10/
--rw-rw-rw-   0        0        0     1148 2023-05-08 02:38:14.000000 getmonitorresolution-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      131 2023-05-08 02:38:13.000000 getmonitorresolution-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     3437 2023-05-08 02:38:18.413563 getmonitorresolution-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     2764 2023-05-08 02:35:54.000000 getmonitorresolution-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 02:38:18.409573 getmonitorresolution-0.10/getmonitorresolution/
--rw-rw-rw-   0        0        0     2764 2023-05-08 02:35:54.000000 getmonitorresolution-0.10/getmonitorresolution/README.md
--rw-rw-rw-   0        0        0     2774 2023-05-08 02:32:47.000000 getmonitorresolution-0.10/getmonitorresolution/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-08 02:38:17.000000 getmonitorresolution-0.10/getmonitorresolution/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-05-08 02:38:17.000000 getmonitorresolution-0.10/getmonitorresolution/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-05-08 02:38:18.413563 getmonitorresolution-0.10/getmonitorresolution.egg-info/
--rw-rw-rw-   0        0        0     3437 2023-05-08 02:38:18.000000 getmonitorresolution-0.10/getmonitorresolution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-05-08 02:38:18.000000 getmonitorresolution-0.10/getmonitorresolution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 02:38:18.000000 getmonitorresolution-0.10/getmonitorresolution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-08 02:38:18.000000 getmonitorresolution-0.10/getmonitorresolution.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-05-08 02:38:18.414560 getmonitorresolution-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1330 2023-05-08 02:38:17.000000 getmonitorresolution-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 02:49:56.033936 getmonitorresolution-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-05-08 02:49:50.000000 getmonitorresolution-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      131 2023-05-08 02:49:48.000000 getmonitorresolution-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     3437 2023-05-08 02:49:56.033936 getmonitorresolution-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     2764 2023-05-08 02:41:04.000000 getmonitorresolution-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 02:49:56.028948 getmonitorresolution-0.11/getmonitorresolution/
+-rw-rw-rw-   0        0        0     2764 2023-05-08 02:41:04.000000 getmonitorresolution-0.11/getmonitorresolution/README.md
+-rw-rw-rw-   0        0        0     2775 2023-05-08 02:49:01.000000 getmonitorresolution-0.11/getmonitorresolution/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-08 02:49:55.000000 getmonitorresolution-0.11/getmonitorresolution/requirements.txt
+-rw-rw-rw-   0        0        0        2 2023-05-08 02:49:55.000000 getmonitorresolution-0.11/getmonitorresolution/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-05-08 02:49:56.032939 getmonitorresolution-0.11/getmonitorresolution.egg-info/
+-rw-rw-rw-   0        0        0     3437 2023-05-08 02:49:55.000000 getmonitorresolution-0.11/getmonitorresolution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-05-08 02:49:55.000000 getmonitorresolution-0.11/getmonitorresolution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 02:49:55.000000 getmonitorresolution-0.11/getmonitorresolution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-08 02:49:55.000000 getmonitorresolution-0.11/getmonitorresolution.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-08 02:49:56.033936 getmonitorresolution-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1330 2023-05-08 02:49:55.000000 getmonitorresolution-0.11/setup.py
```

### Comparing `getmonitorresolution-0.10/LICENSE.rst` & `getmonitorresolution-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `getmonitorresolution-0.10/PKG-INFO` & `getmonitorresolution-0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getmonitorresolution
-Version: 0.10
+Version: 0.11
 Summary: Uses ctypes to get the resolution information of all available monitors
 Home-page: https://github.com/hansalemaos/getmonitorresolution
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: ctypes,monitor,resolution
 Classifier: Development Status :: 4 - Beta
```

### Comparing `getmonitorresolution-0.10/README.md` & `getmonitorresolution-0.11/README.md`

 * *Files identical despite different names*

### Comparing `getmonitorresolution-0.10/getmonitorresolution/README.md` & `getmonitorresolution-0.11/getmonitorresolution/README.md`

 * *Files identical despite different names*

### Comparing `getmonitorresolution-0.10/getmonitorresolution/__init__.py` & `getmonitorresolution-0.11/getmonitorresolution/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     resolutions = _get_monitors_resolution()
     allmoni = {}
     for i, res in enumerate(resolutions):
         allmoni[i] = {"width": res[0], "height": res[1]}
     moninfos = {
         'width_all_monitors': sum([q[1]["width"] for q in allmoni.items()]),
-        'height_all_monitors': max([q[1]["width"] for q in allmoni.items()]),
+        'height_all_monitors': max([q[1]["height"] for q in allmoni.items()]),
         'max_monitor_width': max([q[1]["width"] for q in allmoni.items()]),
         'min_monitor_width': min([q[1]["width"] for q in allmoni.items()]),
         'max_monitor_height': max([q[1]["height"] for q in allmoni.items()]),
         'min_monitor_height': min([q[1]["height"] for q in allmoni.items()]),
 
     }
     return allmoni, moninfos
```

### Comparing `getmonitorresolution-0.10/getmonitorresolution.egg-info/PKG-INFO` & `getmonitorresolution-0.11/getmonitorresolution.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getmonitorresolution
-Version: 0.10
+Version: 0.11
 Summary: Uses ctypes to get the resolution information of all available monitors
 Home-page: https://github.com/hansalemaos/getmonitorresolution
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: ctypes,monitor,resolution
 Classifier: Development Status :: 4 - Beta
```

### Comparing `getmonitorresolution-0.10/setup.py` & `getmonitorresolution-0.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''Uses ctypes to get the resolution information of all available monitors'''
 
 # Setting up
 setup(
     name="getmonitorresolution",
     version=VERSION,
     license='MIT',
```

