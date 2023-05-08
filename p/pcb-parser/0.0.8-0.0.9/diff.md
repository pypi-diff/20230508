# Comparing `tmp/pcb-parser-0.0.8.tar.gz` & `tmp/pcb-parser-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcb-parser-0.0.8.tar", last modified: Thu Apr 13 13:57:32 2023, max compression
+gzip compressed data, was "pcb-parser-0.0.9.tar", last modified: Wed Apr 19 09:20:28 2023, max compression
```

## Comparing `pcb-parser-0.0.8.tar` & `pcb-parser-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:57:32.479419 pcb-parser-0.0.8/
--rwxrwxrwx   0 root         (0) root         (0)     1065 2023-02-20 02:12:16.000000 pcb-parser-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      412 2023-04-13 13:57:32.479419 pcb-parser-0.0.8/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-03 04:33:47.000000 pcb-parser-0.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 13:57:32.480419 pcb-parser-0.0.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      688 2023-04-13 13:56:58.000000 pcb-parser-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:57:32.478419 pcb-parser-0.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:57:32.479419 pcb-parser-0.0.8/src/pcb_parser/
--rwxrwxrwx   0 root         (0) root         (0)       72 2023-03-02 23:43:20.000000 pcb-parser-0.0.8/src/pcb_parser/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      924 2023-03-30 05:32:08.000000 pcb-parser-0.0.8/src/pcb_parser/abs.py
--rwxr-xr-x   0 root         (0) root         (0)    30746 2023-04-13 13:56:15.000000 pcb-parser-0.0.8/src/pcb_parser/geometry.py
--rwxr-xr-x   0 root         (0) root         (0)     6779 2023-04-13 13:56:01.000000 pcb-parser-0.0.8/src/pcb_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     1194 2023-04-13 13:56:14.000000 pcb-parser-0.0.8/src/pcb_parser/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:57:32.479419 pcb-parser-0.0.8/src/pcb_parser.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-13 13:57:32.000000 pcb-parser-0.0.8/src/pcb_parser.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      303 2023-04-13 13:57:32.000000 pcb-parser-0.0.8/src/pcb_parser.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-13 13:57:32.000000 pcb-parser-0.0.8/src/pcb_parser.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       11 2023-04-13 13:57:32.000000 pcb-parser-0.0.8/src/pcb_parser.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:20:28.333265 pcb-parser-0.0.9/
+-rwxrwxrwx   0 root         (0) root         (0)     1065 2023-02-20 02:12:16.000000 pcb-parser-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      412 2023-04-19 09:20:28.332265 pcb-parser-0.0.9/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-03 04:33:47.000000 pcb-parser-0.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 09:20:28.333265 pcb-parser-0.0.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      688 2023-04-19 09:19:44.000000 pcb-parser-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:20:28.330265 pcb-parser-0.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:20:28.331265 pcb-parser-0.0.9/src/pcb_parser/
+-rwxrwxrwx   0 root         (0) root         (0)       72 2023-03-02 23:43:20.000000 pcb-parser-0.0.9/src/pcb_parser/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      924 2023-03-30 05:32:08.000000 pcb-parser-0.0.9/src/pcb_parser/abs.py
+-rwxr-xr-x   0 root         (0) root         (0)    30895 2023-04-19 09:16:05.000000 pcb-parser-0.0.9/src/pcb_parser/geometry.py
+-rwxr-xr-x   0 root         (0) root         (0)     6779 2023-04-14 00:50:36.000000 pcb-parser-0.0.9/src/pcb_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-04-13 13:56:14.000000 pcb-parser-0.0.9/src/pcb_parser/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:20:28.332265 pcb-parser-0.0.9/src/pcb_parser.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-19 09:20:28.000000 pcb-parser-0.0.9/src/pcb_parser.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      303 2023-04-19 09:20:28.000000 pcb-parser-0.0.9/src/pcb_parser.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-19 09:20:28.000000 pcb-parser-0.0.9/src/pcb_parser.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       11 2023-04-19 09:20:28.000000 pcb-parser-0.0.9/src/pcb_parser.egg-info/top_level.txt
```

### Comparing `pcb-parser-0.0.8/LICENSE` & `pcb-parser-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pcb-parser-0.0.8/setup.py` & `pcb-parser-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open('README.md', 'r') as f:
     long_description = f.read()
     
 setuptools.setup(
     name = 'pcb-parser',
-    version = 'v0.0.8',
+    version = 'v0.0.9',
     author = 'Changyun Choi',
     author_email = "cyun9601@gmail.com",
     description = "PCB Parser",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/cyun9601/PCB_Parser",
     package_dir={"": "src"},
```

### Comparing `pcb-parser-0.0.8/src/pcb_parser/abs.py` & `pcb-parser-0.0.9/src/pcb_parser/abs.py`

 * *Files identical despite different names*

### Comparing `pcb-parser-0.0.8/src/pcb_parser/geometry.py` & `pcb-parser-0.0.9/src/pcb_parser/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,19 +464,14 @@
         - Output -
         """
         
         # Line 과 Arc가 존재하지 않으면 None 반환 
         if len(self) == 0: 
             return None 
         
-        # 기존에 그린게 있으면 해당 값을 반환
-        # if 'self.cv_img' in locals(): 
-        #     if (self.cv_resolution == resolution) & (self.cv_fill == fill):
-        #         return self.cv_img
-        
         # 원점으로 이동 
         polygon = self.move(-self.min_x, -self.min_y)
 
         h = int(round(polygon.h / self.p_resolution, 0)) + 1 
         w = int(round(polygon.w / self.p_resolution, 0)) + 1
         polygon_img = np.ones((h, w)) * 255
         polygon_img = polygon_img.astype(np.uint8)
@@ -597,14 +592,20 @@
             self.hole_area = Polygon(data['HoleArea'], p_resolution).move(self.center.x, self.center.y)
             self.pin_dict = data['PinDict']
             self.fixed = data['Fixed']
             self.group = data['Group']
         else:
             NotImplementedError
 
+        self.top_area.draw_cv('fill')
+        self.bottom_area.draw_cv('fill')
+        self.top_prohibit_area.draw_cv('fill')
+        self.bottom_prohibit_area.draw_cv('fill') 
+        self.hole_area.draw_cv('fill')
+        
         self.p_resolution = p_resolution
 
         # Component 초기화 
         self.initialize()
         
     def initialize(self) -> None:
         # unfixed component 에 대한 처리
@@ -687,16 +688,20 @@
                 bottom_max_pix_h = total_h - 1 - int(round((bottom_moved_min_y / self.p_resolution), 0))
                 bottom_min_pix_w = int(round((bottom_moved_min_x / self.p_resolution), 0))
                 bottom_max_pix_w = int(round((bottom_moved_max_x / self.p_resolution), 0))
                 
                 ## 이미지 삽입 
                 total_bottom_img[bottom_min_pix_h:bottom_min_pix_h + bottom_img.shape[0], bottom_min_pix_w:bottom_min_pix_w + bottom_img.shape[1]] = bottom_img 
 
-            self.cv_top_img = total_top_img    
-            self.cv_bottom_img = total_bottom_img   
+                im = Image.fromarray(total_bottom_img)
+                os.makedirs(img_path, exist_ok=True)
+                im.save(bottom_img_path)
+
+        self.cv_top_img = total_top_img    
+        self.cv_bottom_img = total_bottom_img   
             
         return self.cv_top_img, self.cv_bottom_img     
         
     def draw_mat(self, ax, layer, shift_x=0, shift_y=0, color='k'): 
         if layer == 'TOP':
             self.top_area.draw_mat(ax, shift_x=shift_x, shift_y=shift_y, color=color)
         elif layer == 'BOTTOM':
@@ -796,14 +801,15 @@
             if 'cv_bottom_img' in dir(self):
                 self.cv_bottom_img = img_rot_90(self.cv_bottom_img, k)
             return self
         else:
             new_comp = copy.deepcopy(self)
             return new_comp.rotation(angle, inplace=True)
 
+'''
 def merge_polygon(base_img:np.array, background:Polygon, foreground:Polygon, resolution = 0.05, inplace = False) -> np.array:
     if inplace == False:
         base_img = copy.deepcopy(base_img)
     
     back_pix_h = int(round(background.h / resolution, 0)) + 1
     back_pix_w = int(round(background.w / resolution, 0)) + 1
     
@@ -826,8 +832,9 @@
     ## 이미지 삽입 
     partial_base_img = base_img[min_pix_h:min_pix_h+foreground.cv_img.shape[0], min_pix_w:min_pix_w+foreground.cv_img.shape[1]]
     if ((partial_base_img == 0) & (foreground.cv_img == 0)).sum() > 0: 
         collision = True
     else:
         collision = False
     base_img[min_pix_h:min_pix_h+foreground.cv_img.shape[0], min_pix_w:min_pix_w+foreground.cv_img.shape[1]] = foreground.cv_img 
-    return base_img, collision
+    return base_img, collision
+'''
```

### Comparing `pcb-parser-0.0.8/src/pcb_parser/parser.py` & `pcb-parser-0.0.9/src/pcb_parser/parser.py`

 * *Files identical despite different names*

### Comparing `pcb-parser-0.0.8/src/pcb_parser/utils.py` & `pcb-parser-0.0.9/src/pcb_parser/utils.py`

 * *Files identical despite different names*

