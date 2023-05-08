# Comparing `tmp/mygui-0.2.2.tar.gz` & `tmp/mygui-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mygui-0.2.2.tar", last modified: Thu Sep 29 18:25:17 2022, max compression
+gzip compressed data, was "mygui-0.2.3.tar", last modified: Mon May  8 13:50:42 2023, max compression
```

## Comparing `mygui-0.2.2.tar` & `mygui-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-09-29 18:25:17.987334 mygui-0.2.2/
--rw-rw-rw-   0        0        0     1143 2022-07-22 19:19:58.000000 mygui-0.2.2/LICENSE.md
--rw-rw-rw-   0        0        0     1503 2022-09-29 18:25:17.987334 mygui-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      629 2022-09-29 18:24:11.000000 mygui-0.2.2/README.md
--rw-rw-rw-   0        0        0       94 2022-07-01 15:14:17.000000 mygui-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0      971 2022-09-29 18:25:17.987334 mygui-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-09-29 18:25:17.956071 mygui-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2022-09-29 18:25:17.971661 mygui-0.2.2/src/mygui/
-drwxrwxrwx   0        0        0        0 2022-09-29 18:25:17.987334 mygui-0.2.2/src/mygui/Examples/
--rw-rw-rw-   0        0        0      304 2022-06-10 17:13:36.000000 mygui-0.2.2/src/mygui/Examples/LgridExamples.py
--rw-rw-rw-   0        0        0      180 2022-06-15 17:08:58.000000 mygui-0.2.2/src/mygui/Examples/MYGUI-egrid.py
--rw-rw-rw-   0        0        0      275 2022-06-15 17:06:42.000000 mygui-0.2.2/src/mygui/Examples/MYGUI-lgrid.py
--rw-rw-rw-   0        0        0      238 2022-06-10 17:11:27.000000 mygui-0.2.2/src/mygui/Examples/testmygui.py
--rw-rw-rw-   0        0        0      838 2022-09-29 18:16:50.000000 mygui-0.2.2/src/mygui/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-29 18:25:17.987334 mygui-0.2.2/src/mygui/test/
--rw-rw-rw-   0        0        0      866 2022-06-15 18:45:44.000000 mygui-0.2.2/src/mygui/test/lgridegridtest.py
--rw-rw-rw-   0        0        0      268 2022-09-29 18:18:15.000000 mygui-0.2.2/src/mygui/test/testmygui.py
-drwxrwxrwx   0        0        0        0 2022-09-29 18:25:17.971661 mygui-0.2.2/src/mygui.egg-info/
--rw-rw-rw-   0        0        0     1503 2022-09-29 18:25:17.000000 mygui-0.2.2/src/mygui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2022-09-29 18:25:17.000000 mygui-0.2.2/src/mygui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-29 18:25:17.000000 mygui-0.2.2/src/mygui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2022-09-29 18:25:17.000000 mygui-0.2.2/src/mygui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 13:50:42.098042 mygui-0.2.3/
+-rw-rw-rw-   0        0        0     1143 2022-07-22 19:19:58.000000 mygui-0.2.3/LICENSE.md
+-rw-rw-rw-   0        0        0     1462 2023-05-08 13:50:42.098042 mygui-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2022-09-29 18:24:11.000000 mygui-0.2.3/README.md
+-rw-rw-rw-   0        0        0       94 2022-07-01 15:14:17.000000 mygui-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0      971 2023-05-08 13:50:42.098042 mygui-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 13:50:42.082416 mygui-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 13:50:42.082416 mygui-0.2.3/src/mygui/
+drwxrwxrwx   0        0        0        0 2023-05-08 13:50:42.098042 mygui-0.2.3/src/mygui/Examples/
+-rw-rw-rw-   0        0        0      304 2022-06-10 17:13:36.000000 mygui-0.2.3/src/mygui/Examples/LgridExamples.py
+-rw-rw-rw-   0        0        0      180 2022-06-15 17:08:58.000000 mygui-0.2.3/src/mygui/Examples/MYGUI-egrid.py
+-rw-rw-rw-   0        0        0      275 2022-06-15 17:06:42.000000 mygui-0.2.3/src/mygui/Examples/MYGUI-lgrid.py
+-rw-rw-rw-   0        0        0      238 2022-06-10 17:11:27.000000 mygui-0.2.3/src/mygui/Examples/testmygui.py
+-rw-rw-rw-   0        0        0      838 2022-09-29 18:16:50.000000 mygui-0.2.3/src/mygui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:50:42.098042 mygui-0.2.3/src/mygui/test/
+-rw-rw-rw-   0        0        0      866 2022-06-15 18:45:44.000000 mygui-0.2.3/src/mygui/test/lgridegridtest.py
+-rw-rw-rw-   0        0        0      268 2022-09-29 18:18:15.000000 mygui-0.2.3/src/mygui/test/testmygui.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:50:42.098042 mygui-0.2.3/src/mygui.egg-info/
+-rw-rw-rw-   0        0        0     1462 2023-05-08 13:50:42.000000 mygui-0.2.3/src/mygui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-05-08 13:50:42.000000 mygui-0.2.3/src/mygui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 13:50:42.000000 mygui-0.2.3/src/mygui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-08 13:50:42.000000 mygui-0.2.3/src/mygui.egg-info/top_level.txt
```

### Comparing `mygui-0.2.2/LICENSE.md` & `mygui-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mygui-0.2.2/PKG-INFO` & `mygui-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: mygui
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Simple icon to replace the tkinter feather for your programs
 Home-page: https://github.com/Caveman-Software/mygui
 Author: Michael E Mulvey
 Author-email: michael.e.mulvey@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Caveman-Software/mygui/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -53,9 +51,7 @@
 
     root = Tk()
     root.minsize(300, 100)
     egrid(root,0,0)
     root.mainloop()
 
 ---
-
-
```

### Comparing `mygui-0.2.2/README.md` & `mygui-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `mygui-0.2.2/setup.cfg` & `mygui-0.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 7967 7569 0d0a 7665 7273 696f   = mygui..versio
-00000020: 6e20 3d20 302e 322e 320d 0a61 7574 686f  n = 0.2.2..autho
+00000020: 6e20 3d20 302e 322e 330d 0a61 7574 686f  n = 0.2.3..autho
 00000030: 7220 3d20 4d69 6368 6165 6c20 4520 4d75  r = Michael E Mu
 00000040: 6c76 6579 0d0a 6175 7468 6f72 5f65 6d61  lvey..author_ema
 00000050: 696c 203d 206d 6963 6861 656c 2e65 2e6d  il = michael.e.m
 00000060: 756c 7665 7940 676d 6169 6c2e 636f 6d0d  ulvey@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000080: 2053 696d 706c 6520 6963 6f6e 2074 6f20   Simple icon to 
 00000090: 7265 706c 6163 6520 7468 6520 746b 696e  replace the tkin
```

### Comparing `mygui-0.2.2/src/mygui/__init__.py` & `mygui-0.2.3/src/mygui/__init__.py`

 * *Files identical despite different names*

### Comparing `mygui-0.2.2/src/mygui/test/lgridegridtest.py` & `mygui-0.2.3/src/mygui/test/lgridegridtest.py`

 * *Files identical despite different names*

### Comparing `mygui-0.2.2/src/mygui.egg-info/PKG-INFO` & `mygui-0.2.3/src/mygui.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: mygui
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Simple icon to replace the tkinter feather for your programs
 Home-page: https://github.com/Caveman-Software/mygui
 Author: Michael E Mulvey
 Author-email: michael.e.mulvey@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Caveman-Software/mygui/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -53,9 +51,7 @@
 
     root = Tk()
     root.minsize(300, 100)
     egrid(root,0,0)
     root.mainloop()
 
 ---
-
-
```

