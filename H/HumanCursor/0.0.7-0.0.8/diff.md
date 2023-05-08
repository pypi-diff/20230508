# Comparing `tmp/HumanCursor-0.0.7.tar.gz` & `tmp/HumanCursor-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HumanCursor-0.0.7.tar", last modified: Mon May  8 15:05:33 2023, max compression
+gzip compressed data, was "HumanCursor-0.0.8.tar", last modified: Mon May  8 16:52:48 2023, max compression
```

## Comparing `HumanCursor-0.0.7.tar` & `HumanCursor-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 15:05:33.610781 HumanCursor-0.0.7/
-drwxrwxrwx   0        0        0        0 2023-05-08 15:05:33.558203 HumanCursor-0.0.7/HumanCursor.egg-info/
--rw-rw-rw-   0        0        0     5384 2023-05-08 15:05:33.000000 HumanCursor-0.0.7/HumanCursor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2023-05-08 15:05:33.000000 HumanCursor-0.0.7/HumanCursor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 15:05:33.000000 HumanCursor-0.0.7/HumanCursor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-08 15:05:33.000000 HumanCursor-0.0.7/HumanCursor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-08 15:05:33.000000 HumanCursor-0.0.7/HumanCursor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2023-04-25 17:10:16.000000 HumanCursor-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     5384 2023-05-08 15:05:33.610781 HumanCursor-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4903 2023-05-05 15:45:08.000000 HumanCursor-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 15:05:33.589446 HumanCursor-0.0.7/humancursor/
--rw-rw-rw-   0        0        0       98 2023-04-26 15:30:38.000000 HumanCursor-0.0.7/humancursor/__init__.py
--rw-rw-rw-   0        0        0     2282 2023-05-07 16:22:16.000000 HumanCursor-0.0.7/humancursor/system_cursor.py
-drwxrwxrwx   0        0        0        0 2023-05-08 15:05:33.589446 HumanCursor-0.0.7/humancursor/test/
--rw-rw-rw-   0        0        0      275 2023-05-08 15:04:08.000000 HumanCursor-0.0.7/humancursor/test/system.py
--rw-rw-rw-   0        0        0     1119 2023-05-08 14:57:57.000000 HumanCursor-0.0.7/humancursor/test/web.py
-drwxrwxrwx   0        0        0        0 2023-05-08 15:05:33.610781 HumanCursor-0.0.7/humancursor/utilities/
--rw-rw-rw-   0        0        0     3354 2023-05-08 14:54:55.000000 HumanCursor-0.0.7/humancursor/utilities/calc.py
--rw-rw-rw-   0        0        0     7876 2023-05-05 14:39:43.000000 HumanCursor-0.0.7/humancursor/utilities/human_curve_generator.py
--rw-rw-rw-   0        0        0     5357 2023-05-08 14:57:57.000000 HumanCursor-0.0.7/humancursor/utilities/web_adjuster.py
--rw-rw-rw-   0        0        0     6923 2023-04-26 15:30:38.000000 HumanCursor-0.0.7/humancursor/web_cursor.py
--rw-rw-rw-   0        0        0      667 2023-05-08 15:04:08.000000 HumanCursor-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 15:05:33.610781 HumanCursor-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 16:52:48.647774 HumanCursor-0.0.8/
+drwxrwxrwx   0        0        0        0 2023-05-08 16:52:48.631844 HumanCursor-0.0.8/HumanCursor.egg-info/
+-rw-rw-rw-   0        0        0     5470 2023-05-08 16:52:48.000000 HumanCursor-0.0.8/HumanCursor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      451 2023-05-08 16:52:48.000000 HumanCursor-0.0.8/HumanCursor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 16:52:48.000000 HumanCursor-0.0.8/HumanCursor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-08 16:52:48.000000 HumanCursor-0.0.8/HumanCursor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-08 16:52:48.000000 HumanCursor-0.0.8/HumanCursor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2023-04-25 17:10:16.000000 HumanCursor-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     5470 2023-05-08 16:52:48.647774 HumanCursor-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4989 2023-05-08 16:51:06.000000 HumanCursor-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 16:52:48.642254 HumanCursor-0.0.8/humancursor/
+-rw-rw-rw-   0        0        0       98 2023-04-26 15:30:38.000000 HumanCursor-0.0.8/humancursor/__init__.py
+-rw-rw-rw-   0        0        0     2529 2023-05-08 16:47:40.000000 HumanCursor-0.0.8/humancursor/system_cursor.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:52:48.647774 HumanCursor-0.0.8/humancursor/test/
+-rw-rw-rw-   0        0        0      275 2023-05-08 16:51:06.000000 HumanCursor-0.0.8/humancursor/test/system.py
+-rw-rw-rw-   0        0        0     1119 2023-05-08 15:39:56.000000 HumanCursor-0.0.8/humancursor/test/web.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:52:48.647774 HumanCursor-0.0.8/humancursor/utilities/
+-rw-rw-rw-   0        0        0     3324 2023-05-08 15:35:22.000000 HumanCursor-0.0.8/humancursor/utilities/calc.py
+-rw-rw-rw-   0        0        0     7876 2023-05-05 14:39:43.000000 HumanCursor-0.0.8/humancursor/utilities/human_curve_generator.py
+-rw-rw-rw-   0        0        0     5540 2023-05-08 16:47:40.000000 HumanCursor-0.0.8/humancursor/utilities/web_adjuster.py
+-rw-rw-rw-   0        0        0     7186 2023-05-08 16:47:40.000000 HumanCursor-0.0.8/humancursor/web_cursor.py
+-rw-rw-rw-   0        0        0      667 2023-05-08 16:51:06.000000 HumanCursor-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 16:52:48.663424 HumanCursor-0.0.8/setup.cfg
```

### Comparing `HumanCursor-0.0.7/HumanCursor.egg-info/PKG-INFO` & `HumanCursor-0.0.8/HumanCursor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HumanCursor
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simulate Human Cursor Movement for Automated Scripts
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Homepage, https://github.com/riflosnake/HumanCursor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -51,14 +51,15 @@
 These functions can accept as destination, either the WebElement itself, or a list of 'x' and 'y' coordinates.
 
 Some parameters explained:
 
 - `relative_position`: Takes a list of x and y percentages as floats from 0 to 1, which indicate the exact position inside an element
                                        for example, if you set it to [0.5, 0.5], it will move the cursor to the center of the element.
 - `absolute_offset`: If you input a list of coordinates instead of webelement, if you turn this to True, the coordinates will be interpreted as absolute movement by pixels, and not like coordinates in the webpage.
+- `steady`: Tries to make movement in straight line, mimicking human, if set to True
 
 ### SystemCursor
 
 To use HumanCursor for your system mouse, you need to import the `SystemCursor` class, and create an instance just like we did above:
 
 ```python
 from HumanCursor.cursors import SystemCursor
```

### Comparing `HumanCursor-0.0.7/LICENSE` & `HumanCursor-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.7/PKG-INFO` & `HumanCursor-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HumanCursor
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simulate Human Cursor Movement for Automated Scripts
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Homepage, https://github.com/riflosnake/HumanCursor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -51,14 +51,15 @@
 These functions can accept as destination, either the WebElement itself, or a list of 'x' and 'y' coordinates.
 
 Some parameters explained:
 
 - `relative_position`: Takes a list of x and y percentages as floats from 0 to 1, which indicate the exact position inside an element
                                        for example, if you set it to [0.5, 0.5], it will move the cursor to the center of the element.
 - `absolute_offset`: If you input a list of coordinates instead of webelement, if you turn this to True, the coordinates will be interpreted as absolute movement by pixels, and not like coordinates in the webpage.
+- `steady`: Tries to make movement in straight line, mimicking human, if set to True
 
 ### SystemCursor
 
 To use HumanCursor for your system mouse, you need to import the `SystemCursor` class, and create an instance just like we did above:
 
 ```python
 from HumanCursor.cursors import SystemCursor
```

### Comparing `HumanCursor-0.0.7/README.md` & `HumanCursor-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 These functions can accept as destination, either the WebElement itself, or a list of 'x' and 'y' coordinates.
 
 Some parameters explained:
 
 - `relative_position`: Takes a list of x and y percentages as floats from 0 to 1, which indicate the exact position inside an element
                                        for example, if you set it to [0.5, 0.5], it will move the cursor to the center of the element.
 - `absolute_offset`: If you input a list of coordinates instead of webelement, if you turn this to True, the coordinates will be interpreted as absolute movement by pixels, and not like coordinates in the webpage.
+- `steady`: Tries to make movement in straight line, mimicking human, if set to True
 
 ### SystemCursor
 
 To use HumanCursor for your system mouse, you need to import the `SystemCursor` class, and create an instance just like we did above:
 
 ```python
 from HumanCursor.cursors import SystemCursor
```

### Comparing `HumanCursor-0.0.7/humancursor/system_cursor.py` & `HumanCursor-0.0.8/humancursor/system_cursor.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class SystemCursor:
     def __init__(self):
         pyautogui.MINIMUM_DURATION = 0
         pyautogui.MINIMUM_SLEEP = 0
         pyautogui.PAUSE = 0
 
     @staticmethod
-    def move_to(point: list, duration: int = None, human_curve=None):
+    def move_to(point: list, duration: int = None, human_curve=None, steady=False):
         """Moves to certain coordinates of screen"""
         from_point = pyautogui.position()
 
         if not human_curve:
             (
                 offset_boundary_x,
                 offset_boundary_y,
@@ -26,14 +26,17 @@
                 distortion_st_dev,
                 distortion_frequency,
                 tween,
                 target_points,
             ) = generate_random_curve_parameters(
                 pyautogui, from_point, point
             )
+            if steady:
+                offset_boundary_x, offset_boundary_y = 10, 10
+                distortion_mean, distortion_st_dev, distortion_frequency = 1.2, 1.2, 1
             human_curve = HumanizeMouseTrajectory(
                 from_point,
                 point,
                 offset_boundary_x=offset_boundary_x,
                 offset_boundary_y=offset_boundary_y,
                 knots_count=knots_count,
                 distortion_mean=distortion_mean,
@@ -46,20 +49,20 @@
         if duration is None:
             duration = random.uniform(0.5, 2.0)
         pyautogui.PAUSE = duration / len(human_curve.points)
         for pnt in human_curve.points:
             pyautogui.moveTo(pnt)
         pyautogui.moveTo(point)
 
-    def click_on(self, point: list, clicks: int = 1):
+    def click_on(self, point: list, clicks: int = 1, steady=False):
         """Clicks a specified number of times, on the specified coordinates"""
-        self.move_to(point)
+        self.move_to(point, steady=steady)
         for _ in range(clicks):
             pyautogui.click()
             sleep(random.uniform(0.150, 0.300))
 
-    def drag_and_drop(self, from_point: list, to_point: list):
+    def drag_and_drop(self, from_point: list, to_point: list, steady=False):
         """Drags from a certain point, and releases to another"""
         self.move_to(from_point)
         pyautogui.mouseDown()
-        self.move_to(to_point)
+        self.move_to(to_point, steady=steady)
         pyautogui.mouseUp()
```

### Comparing `HumanCursor-0.0.7/humancursor/test/web.py` & `HumanCursor-0.0.8/humancursor/test/web.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.7/humancursor/utilities/calc.py` & `HumanCursor-0.0.8/humancursor/utilities/calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,18 +59,17 @@
     distortion_mean = random.choice(range(80, 110)) / 100
     distortion_st_dev = random.choice(range(85, 110)) / 100
     distortion_frequency = random.choice(range(25, 70)) / 100
 
     if web:
         target_points = random.choice(
             random.choices(
-                [range(25, 35), range(35, 70), range(70, 90)], [0.53, 0.32, 0.15]
+                [range(35, 45), range(45, 60), range(60, 80)], [0.53, 0.32, 0.15]
             )[0]
         )
-        print(target_points)
     else:
         target_points = random.choice(
                 range(90, 110)
         )
 
     if (
             min_width > pre_origin[0]
```

### Comparing `HumanCursor-0.0.7/humancursor/utilities/human_curve_generator.py` & `HumanCursor-0.0.8/humancursor/utilities/human_curve_generator.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.7/humancursor/utilities/web_adjuster.py` & `HumanCursor-0.0.8/humancursor/utilities/web_adjuster.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     def move_to(
         self,
         element_or_pos,
         origin_coordinates=None,
         absolute_offset=False,
         relative_position=None,
         human_curve=None,
+        steady=False
     ):
         """Moves the humancursor, trying to mimic human behaviour!"""
         origin = origin_coordinates
         if origin_coordinates is None:
             origin = self.origin_coordinate
 
         pre_origin = tuple(origin)
@@ -60,15 +61,17 @@
             distortion_st_dev,
             distortion_frequency,
             tween,
             target_points,
         ) = generate_random_curve_parameters(
             self.__driver, [origin[0], origin[1]], [x, y]
         )
-
+        if steady:
+            offset_boundary_x, offset_boundary_y = 10, 10
+            distortion_mean, distortion_st_dev, distortion_frequency = 1.2, 1.2, 1
         if not human_curve:
             human_curve = HumanizeMouseTrajectory(
                 [origin[0], origin[1]],
                 [x, y],
                 offset_boundary_x=offset_boundary_x,
                 offset_boundary_y=offset_boundary_y,
                 knots_count=knots_count,
```

### Comparing `HumanCursor-0.0.7/humancursor/web_cursor.py` & `HumanCursor-0.0.8/humancursor/web_cursor.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,110 +16,118 @@
 
     def move_to(
         self,
         element: WebElement or list,
         relative_position: list = None,
         absolute_offset: bool = False,
         origin_coordinates=None,
+        steady=False
     ):
         """Moves to element or coordinates with human curve"""
         if not self.scroll_into_view_of_element(element):
             return False
         if origin_coordinates is None:
             origin_coordinates = self.origin_coordinates
         self.origin_coordinates = self.human.move_to(
             element,
             origin_coordinates=origin_coordinates,
             absolute_offset=absolute_offset,
             relative_position=relative_position,
+            steady=steady
         )
         return self.origin_coordinates
 
     def click_on(
         self,
         element: WebElement or list,
         number_of_clicks: int = 1,
         relative_position: list = None,
         absolute_offset: bool = False,
         origin_coordinates=None,
+        steady=False
     ):
         """Moves to element or coordinates with human curve, and clicks on it a specified number of times, default is 1"""
         self.move_to(
             element,
             origin_coordinates=origin_coordinates,
             absolute_offset=absolute_offset,
             relative_position=relative_position,
+            steady=steady
         )
         self.click(number_of_clicks)
         return True
 
     def click(self, number_of_clicks=1):
         """Performs the click action"""
         for _ in range(number_of_clicks):
             self.__action.click().pause(random.randint(200, 300) / 1000)
         self.__action.perform()
         return True
 
-    def move_by_offset(self, x: int, y: int):
+    def move_by_offset(self, x: int, y: int, steady=False):
         """Moves the cursor with human curve, by specified number of x and y pixels"""
-        self.origin_coordinates = self.human.move_to([x, y], absolute_offset=True)
+        self.origin_coordinates = self.human.move_to([x, y], absolute_offset=True, steady=steady)
         return True
 
     def drag_and_drop(
         self,
         drag_from_element: WebElement or list,
         drag_to_element: WebElement or list,
         drag_from_relative_position: list = None,
         drag_to_relative_position: list = None,
+        steady=False
     ):
         """Moves to element or coordinates, clicks and holds, dragging it to another element, with human curve"""
         if drag_from_relative_position is None:
             self.move_to(drag_from_element)
         else:
             self.move_to(
                 drag_from_element, relative_position=drag_from_relative_position
             )
 
         if drag_to_element is None:
             self.__action.click().perform()
         else:
             self.__action.click_and_hold().perform()
             if drag_to_relative_position is None:
-                self.move_to(drag_to_element)
+                self.move_to(drag_to_element, steady=steady)
             else:
                 self.move_to(
-                    drag_to_element, relative_position=drag_to_relative_position
+                    drag_to_element, relative_position=drag_to_relative_position, steady=steady
                 )
             self.__action.release().perform()
 
         return True
 
     def control_scroll_bar(
         self,
         scroll_bar_element: WebElement,
         amount_by_percentage: list,
         orientation: str = "horizontal",
+        steady=False
     ):
         """Adjusts any scroll bar on the webpage, by the amount you want in float number from 0 to 1
         representing percentage of fullness, orientation of the scroll bar must also be defined by user
         horizontal or vertical"""
         direction = True if orientation == "horizontal" else False
 
         self.move_to(scroll_bar_element)
         self.__action.click_and_hold().perform()
         # TODO: this needs rework, it will be more natural if it goes out of scroll bar, up or down randomly
         if direction:
             self.move_to(
                 scroll_bar_element,
                 relative_position=[amount_by_percentage, random.randint(0, 100) / 100],
+                steady=steady
             )
         else:
             self.move_to(
                 scroll_bar_element,
                 relative_position=[random.randint(0, 100) / 100, amount_by_percentage],
+                steady=steady
             )
 
         self.__action.release().perform()
 
         return True
 
     def scroll_into_view_of_element(self, element: WebElement):
```

### Comparing `HumanCursor-0.0.7/pyproject.toml` & `HumanCursor-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HumanCursor"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Flori Batusha", email="floribatusha0@gmail.com" },
 ]
 description = "Simulate Human Cursor Movement for Automated Scripts"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

