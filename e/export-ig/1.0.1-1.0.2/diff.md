# Comparing `tmp/export_ig-1.0.1.tar.gz` & `tmp/export_ig-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "export_ig-1.0.1.tar", last modified: Mon May  8 05:24:39 2023, max compression
+gzip compressed data, was "export_ig-1.0.2.tar", last modified: Mon May  8 05:34:56 2023, max compression
```

## Comparing `export_ig-1.0.1.tar` & `export_ig-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 synch      (501) staff       (20)        0 2023-05-08 05:24:39.791681 export_ig-1.0.1/
--rw-r--r--   0 synch      (501) staff       (20)    11357 2023-05-08 05:17:43.000000 export_ig-1.0.1/LICENSE
--rw-r--r--   0 synch      (501) staff       (20)     1696 2023-05-08 05:24:39.791548 export_ig-1.0.1/PKG-INFO
--rw-r--r--   0 synch      (501) staff       (20)     1331 2023-05-08 05:22:50.000000 export_ig-1.0.1/README.md
-drwxr-xr-x   0 synch      (501) staff       (20)        0 2023-05-08 05:24:39.790614 export_ig-1.0.1/export_ig/
--rw-r--r--   0 synch      (501) staff       (20)        0 2023-05-08 05:08:54.000000 export_ig-1.0.1/export_ig/__init__.py
--rw-r--r--   0 synch      (501) staff       (20)      555 2023-05-08 05:05:42.000000 export_ig-1.0.1/export_ig/color_utils.py
--rw-r--r--   0 synch      (501) staff       (20)     4416 2023-05-08 05:12:10.000000 export_ig-1.0.1/export_ig/export_ig.py
-drwxr-xr-x   0 synch      (501) staff       (20)        0 2023-05-08 05:24:39.791394 export_ig-1.0.1/export_ig.egg-info/
--rw-r--r--   0 synch      (501) staff       (20)     1696 2023-05-08 05:24:39.000000 export_ig-1.0.1/export_ig.egg-info/PKG-INFO
--rw-r--r--   0 synch      (501) staff       (20)      328 2023-05-08 05:24:39.000000 export_ig-1.0.1/export_ig.egg-info/SOURCES.txt
--rw-r--r--   0 synch      (501) staff       (20)        1 2023-05-08 05:24:39.000000 export_ig-1.0.1/export_ig.egg-info/dependency_links.txt
--rw-r--r--   0 synch      (501) staff       (20)       54 2023-05-08 05:24:39.000000 export_ig-1.0.1/export_ig.egg-info/entry_points.txt
--rw-r--r--   0 synch      (501) staff       (20)        1 2023-05-08 05:13:33.000000 export_ig-1.0.1/export_ig.egg-info/not-zip-safe
--rw-r--r--   0 synch      (501) staff       (20)       19 2023-05-08 05:24:39.000000 export_ig-1.0.1/export_ig.egg-info/requires.txt
--rw-r--r--   0 synch      (501) staff       (20)       10 2023-05-08 05:24:39.000000 export_ig-1.0.1/export_ig.egg-info/top_level.txt
--rw-r--r--   0 synch      (501) staff       (20)       38 2023-05-08 05:24:39.791720 export_ig-1.0.1/setup.cfg
--rw-r--r--   0 synch      (501) staff       (20)      791 2023-05-08 05:23:27.000000 export_ig-1.0.1/setup.py
+drwxr-xr-x   0 synch      (501) staff       (20)        0 2023-05-08 05:34:56.508825 export_ig-1.0.2/
+-rw-r--r--   0 synch      (501) staff       (20)    11357 2023-05-08 05:17:43.000000 export_ig-1.0.2/LICENSE
+-rw-r--r--   0 synch      (501) staff       (20)     1701 2023-05-08 05:34:56.508672 export_ig-1.0.2/PKG-INFO
+-rw-r--r--   0 synch      (501) staff       (20)     1331 2023-05-08 05:22:50.000000 export_ig-1.0.2/README.md
+drwxr-xr-x   0 synch      (501) staff       (20)        0 2023-05-08 05:34:56.507211 export_ig-1.0.2/export_ig/
+-rw-r--r--   0 synch      (501) staff       (20)        0 2023-05-08 05:08:54.000000 export_ig-1.0.2/export_ig/__init__.py
+-rw-r--r--   0 synch      (501) staff       (20)      556 2023-05-08 05:27:19.000000 export_ig-1.0.2/export_ig/color_utils.py
+-rw-r--r--   0 synch      (501) staff       (20)     4416 2023-05-08 05:12:10.000000 export_ig-1.0.2/export_ig/export_ig.py
+drwxr-xr-x   0 synch      (501) staff       (20)        0 2023-05-08 05:34:56.508488 export_ig-1.0.2/export_ig.egg-info/
+-rw-r--r--   0 synch      (501) staff       (20)     1701 2023-05-08 05:34:56.000000 export_ig-1.0.2/export_ig.egg-info/PKG-INFO
+-rw-r--r--   0 synch      (501) staff       (20)      328 2023-05-08 05:34:56.000000 export_ig-1.0.2/export_ig.egg-info/SOURCES.txt
+-rw-r--r--   0 synch      (501) staff       (20)        1 2023-05-08 05:34:56.000000 export_ig-1.0.2/export_ig.egg-info/dependency_links.txt
+-rw-r--r--   0 synch      (501) staff       (20)       54 2023-05-08 05:34:56.000000 export_ig-1.0.2/export_ig.egg-info/entry_points.txt
+-rw-r--r--   0 synch      (501) staff       (20)        1 2023-05-08 05:13:33.000000 export_ig-1.0.2/export_ig.egg-info/not-zip-safe
+-rw-r--r--   0 synch      (501) staff       (20)       19 2023-05-08 05:34:56.000000 export_ig-1.0.2/export_ig.egg-info/requires.txt
+-rw-r--r--   0 synch      (501) staff       (20)       10 2023-05-08 05:34:56.000000 export_ig-1.0.2/export_ig.egg-info/top_level.txt
+-rw-r--r--   0 synch      (501) staff       (20)       38 2023-05-08 05:34:56.508869 export_ig-1.0.2/setup.cfg
+-rw-r--r--   0 synch      (501) staff       (20)      867 2023-05-08 05:33:34.000000 export_ig-1.0.2/setup.py
```

### Comparing `export_ig-1.0.1/LICENSE` & `export_ig-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `export_ig-1.0.1/PKG-INFO` & `export_ig-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: export_ig
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package for processing images for Instagram upload.
-Home-page: https://instagram.com/synch.poto
+Home-page: https://github.com/syncdoth/export_ig
 Author: Sehyun Choi
 Author-email: choisehyun98@gmail.com
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `export_ig-1.0.1/README.md` & `export_ig-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `export_ig-1.0.1/export_ig/color_utils.py` & `export_ig-1.0.2/export_ig/color_utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
     if hex_color.startswith("#"):
         hex_color = hex_color[1:]
 
     if len(hex_color) == 3:
         hex_color = "".join([c * 2 for c in hex_color])
     if len(hex_color) != 6:
         raise ValueError("Invalid hex color")
-    return tuple(int(hex_color[i:i + 2], 16) for i in (0, 2, 4))
+    return tuple(int(hex_color[i:i + 2], 16) for i in (0, 2, 4))
```

### Comparing `export_ig-1.0.1/export_ig/export_ig.py` & `export_ig-1.0.2/export_ig/export_ig.py`

 * *Files identical despite different names*

### Comparing `export_ig-1.0.1/export_ig.egg-info/PKG-INFO` & `export_ig-1.0.2/export_ig.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: export-ig
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package for processing images for Instagram upload.
-Home-page: https://instagram.com/synch.poto
+Home-page: https://github.com/syncdoth/export_ig
 Author: Sehyun Choi
 Author-email: choisehyun98@gmail.com
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `export_ig-1.0.1/setup.py` & `export_ig-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import find_packages, setup
 
 setup(
     name="export_ig",
-    version="1.0.1",
+    version="1.0.2",
     description="Package for processing images for Instagram upload.",
-    long_description=open("README.md").read(),
+    # pylint: disable-next=consider-using-with
+    long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
-    url="https://instagram.com/synch.poto",
+    url="https://github.com/syncdoth/export_ig",
     author="Sehyun Choi",
     author_email="choisehyun98@gmail.com",
     license="Apache",
     packages=find_packages(exclude=[
         ".github",
         "imgs",
     ]),
@@ -22,8 +23,8 @@
         "joblib",
         "fire",
     ],
     entry_points={"console_scripts": ["export_ig=export_ig.export_ig:run"]},
     include_package_data=True,
     python_requires=">=3.8",
     zip_safe=False,
-)
+)
```

