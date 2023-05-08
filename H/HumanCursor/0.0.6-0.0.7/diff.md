# Comparing `tmp/HumanCursor-0.0.6.tar.gz` & `tmp/HumanCursor-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HumanCursor-0.0.6.tar", last modified: Sun May  7 16:22:49 2023, max compression
+gzip compressed data, was "HumanCursor-0.0.7.tar", last modified: Mon May  8 15:05:33 2023, max compression
```

## Comparing `HumanCursor-0.0.6.tar` & `HumanCursor-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 16:22:49.904893 HumanCursor-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-05-07 16:22:49.826840 HumanCursor-0.0.6/HumanCursor.egg-info/
--rw-rw-rw-   0        0        0     5384 2023-05-07 16:22:49.000000 HumanCursor-0.0.6/HumanCursor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2023-05-07 16:22:49.000000 HumanCursor-0.0.6/HumanCursor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 16:22:49.000000 HumanCursor-0.0.6/HumanCursor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-07 16:22:49.000000 HumanCursor-0.0.6/HumanCursor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-07 16:22:49.000000 HumanCursor-0.0.6/HumanCursor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2023-04-25 17:10:16.000000 HumanCursor-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     5384 2023-05-07 16:22:49.903858 HumanCursor-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4903 2023-05-05 15:45:08.000000 HumanCursor-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 16:22:49.843884 HumanCursor-0.0.6/humancursor/
--rw-rw-rw-   0        0        0       98 2023-04-26 15:30:38.000000 HumanCursor-0.0.6/humancursor/__init__.py
--rw-rw-rw-   0        0        0     2282 2023-05-07 16:22:16.000000 HumanCursor-0.0.6/humancursor/system_cursor.py
-drwxrwxrwx   0        0        0        0 2023-05-07 16:22:49.868708 HumanCursor-0.0.6/humancursor/test/
--rw-rw-rw-   0        0        0      275 2023-05-05 15:45:08.000000 HumanCursor-0.0.6/humancursor/test/system.py
--rw-rw-rw-   0        0        0     1119 2023-05-05 15:45:08.000000 HumanCursor-0.0.6/humancursor/test/web.py
-drwxrwxrwx   0        0        0        0 2023-05-07 16:22:49.902015 HumanCursor-0.0.6/humancursor/utilities/
--rw-rw-rw-   0        0        0     3318 2023-05-05 14:44:20.000000 HumanCursor-0.0.6/humancursor/utilities/calc.py
--rw-rw-rw-   0        0        0     7876 2023-05-05 14:39:43.000000 HumanCursor-0.0.6/humancursor/utilities/human_curve_generator.py
--rw-rw-rw-   0        0        0     5346 2023-05-05 14:46:47.000000 HumanCursor-0.0.6/humancursor/utilities/web_adjuster.py
--rw-rw-rw-   0        0        0     6923 2023-04-26 15:30:38.000000 HumanCursor-0.0.6/humancursor/web_cursor.py
--rw-rw-rw-   0        0        0      667 2023-05-07 16:22:16.000000 HumanCursor-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 16:22:49.904893 HumanCursor-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 15:05:33.610781 HumanCursor-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-05-08 15:05:33.558203 HumanCursor-0.0.7/HumanCursor.egg-info/
+-rw-rw-rw-   0        0        0     5384 2023-05-08 15:05:33.000000 HumanCursor-0.0.7/HumanCursor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      451 2023-05-08 15:05:33.000000 HumanCursor-0.0.7/HumanCursor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 15:05:33.000000 HumanCursor-0.0.7/HumanCursor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-08 15:05:33.000000 HumanCursor-0.0.7/HumanCursor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-08 15:05:33.000000 HumanCursor-0.0.7/HumanCursor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2023-04-25 17:10:16.000000 HumanCursor-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     5384 2023-05-08 15:05:33.610781 HumanCursor-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4903 2023-05-05 15:45:08.000000 HumanCursor-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 15:05:33.589446 HumanCursor-0.0.7/humancursor/
+-rw-rw-rw-   0        0        0       98 2023-04-26 15:30:38.000000 HumanCursor-0.0.7/humancursor/__init__.py
+-rw-rw-rw-   0        0        0     2282 2023-05-07 16:22:16.000000 HumanCursor-0.0.7/humancursor/system_cursor.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:05:33.589446 HumanCursor-0.0.7/humancursor/test/
+-rw-rw-rw-   0        0        0      275 2023-05-08 15:04:08.000000 HumanCursor-0.0.7/humancursor/test/system.py
+-rw-rw-rw-   0        0        0     1119 2023-05-08 14:57:57.000000 HumanCursor-0.0.7/humancursor/test/web.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:05:33.610781 HumanCursor-0.0.7/humancursor/utilities/
+-rw-rw-rw-   0        0        0     3354 2023-05-08 14:54:55.000000 HumanCursor-0.0.7/humancursor/utilities/calc.py
+-rw-rw-rw-   0        0        0     7876 2023-05-05 14:39:43.000000 HumanCursor-0.0.7/humancursor/utilities/human_curve_generator.py
+-rw-rw-rw-   0        0        0     5357 2023-05-08 14:57:57.000000 HumanCursor-0.0.7/humancursor/utilities/web_adjuster.py
+-rw-rw-rw-   0        0        0     6923 2023-04-26 15:30:38.000000 HumanCursor-0.0.7/humancursor/web_cursor.py
+-rw-rw-rw-   0        0        0      667 2023-05-08 15:04:08.000000 HumanCursor-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 15:05:33.610781 HumanCursor-0.0.7/setup.cfg
```

### Comparing `HumanCursor-0.0.6/HumanCursor.egg-info/PKG-INFO` & `HumanCursor-0.0.7/HumanCursor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HumanCursor
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simulate Human Cursor Movement for Automated Scripts
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Homepage, https://github.com/riflosnake/HumanCursor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `HumanCursor-0.0.6/LICENSE` & `HumanCursor-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.6/PKG-INFO` & `HumanCursor-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HumanCursor
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simulate Human Cursor Movement for Automated Scripts
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Homepage, https://github.com/riflosnake/HumanCursor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `HumanCursor-0.0.6/README.md` & `HumanCursor-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.6/humancursor/system_cursor.py` & `HumanCursor-0.0.7/humancursor/system_cursor.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.6/humancursor/test/web.py` & `HumanCursor-0.0.7/humancursor/test/web.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.6/humancursor/utilities/calc.py` & `HumanCursor-0.0.7/humancursor/utilities/calc.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,38 +39,38 @@
         pytweening.easeOutCubic,
         pytweening.easeOutCirc,
     ]
 
     tween = random.choice(tween_options)
     offset_boundary_x = random.choice(
         random.choices(
-            [range(0, 20), range(20, 60), range(60, 80)], [0.25, 0.6, 0.15]
+            [range(20, 45), range(45, 75), range(75, 100)], [0.2, 0.65, 15]
         )[0]
     )
     offset_boundary_y = random.choice(
         random.choices(
-            [range(0, 20), range(20, 60), range(60, 80)], [0.25, 0.6, 0.15]
+            [range(20, 45), range(45, 75), range(75, 100)], [0.2, 0.65, 15]
         )[0]
     )
-
     knots_count = random.choices(
         [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
-        [0.1, 0.35, 0.12, 0.1, 0.1, 0.08, 0.04, 0.04, 0.04, 0.03],
-    )
+        [0.15, 0.36, 0.17, 0.12, 0.08, 0.04, 0.03, 0.02, 0.015, 0.005],
+    )[0]
 
-    distortion_mean = random.choice(range(40, 100)) / 100
-    distortion_st_dev = random.choice(range(40, 100)) / 100
-    distortion_frequency = random.choice(range(25, 75)) / 100
+    distortion_mean = random.choice(range(80, 110)) / 100
+    distortion_st_dev = random.choice(range(85, 110)) / 100
+    distortion_frequency = random.choice(range(25, 70)) / 100
 
     if web:
         target_points = random.choice(
             random.choices(
                 [range(25, 35), range(35, 70), range(70, 90)], [0.53, 0.32, 0.15]
             )[0]
         )
+        print(target_points)
     else:
         target_points = random.choice(
                 range(90, 110)
         )
 
     if (
             min_width > pre_origin[0]
```

### Comparing `HumanCursor-0.0.6/humancursor/utilities/human_curve_generator.py` & `HumanCursor-0.0.7/humancursor/utilities/human_curve_generator.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.6/humancursor/utilities/web_adjuster.py` & `HumanCursor-0.0.7/humancursor/utilities/web_adjuster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import random
 
-from selenium.common import MoveTargetOutOfBoundsException
+from selenium.common.exceptions import MoveTargetOutOfBoundsException
 from selenium.webdriver.common.action_chains import ActionChains
 
 from humancursor.utilities.human_curve_generator import HumanizeMouseTrajectory
 from humancursor.utilities.calc import generate_random_curve_parameters, calculate_absolute_offset
 
 
 class WebAdjuster:
```

### Comparing `HumanCursor-0.0.6/humancursor/web_cursor.py` & `HumanCursor-0.0.7/humancursor/web_cursor.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.6/pyproject.toml` & `HumanCursor-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HumanCursor"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Flori Batusha", email="floribatusha0@gmail.com" },
 ]
 description = "Simulate Human Cursor Movement for Automated Scripts"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

