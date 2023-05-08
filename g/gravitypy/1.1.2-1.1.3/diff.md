# Comparing `tmp/gravitypy-1.1.2.tar.gz` & `tmp/gravitypy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitypy-1.1.2.tar", last modified: Mon May  8 18:51:02 2023, max compression
+gzip compressed data, was "gravitypy-1.1.3.tar", last modified: Mon May  8 19:11:33 2023, max compression
```

## Comparing `gravitypy-1.1.2.tar` & `gravitypy-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 18:51:02.120184 gravitypy-1.1.2/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 20:40:23.000000 gravitypy-1.1.2/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 20:40:23.000000 gravitypy-1.1.2/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-08 18:51:02.120184 gravitypy-1.1.2/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1340 2023-05-07 20:40:23.000000 gravitypy-1.1.2/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 18:51:02.120184 gravitypy-1.1.2/gravitypy/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 20:40:23.000000 gravitypy-1.1.2/gravitypy/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-08 18:43:26.000000 gravitypy-1.1.2/gravitypy/__main__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15495 2023-05-08 18:34:31.000000 gravitypy-1.1.2/gravitypy/main.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 18:51:02.120184 gravitypy-1.1.2/gravitypy/resources/
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 18:51:02.120184 gravitypy-1.1.2/gravitypy/resources/fonts/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 20:40:23.000000 gravitypy-1.1.2/gravitypy/resources/fonts/minecraft_font.ttf
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 18:51:02.120184 gravitypy-1.1.2/gravitypy.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-08 18:51:02.000000 gravitypy-1.1.2/gravitypy.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      362 2023-05-08 18:51:02.000000 gravitypy-1.1.2/gravitypy.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-08 18:51:02.000000 gravitypy-1.1.2/gravitypy.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-05-08 18:51:02.000000 gravitypy-1.1.2/gravitypy.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-08 18:51:02.000000 gravitypy-1.1.2/gravitypy.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-05-08 18:51:02.000000 gravitypy-1.1.2/gravitypy.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 20:40:23.000000 gravitypy-1.1.2/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-08 18:51:02.120184 gravitypy-1.1.2/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      973 2023-05-08 18:50:29.000000 gravitypy-1.1.2/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 19:11:33.897231 gravitypy-1.1.3/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 20:40:23.000000 gravitypy-1.1.3/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 20:40:23.000000 gravitypy-1.1.3/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-08 19:11:33.897231 gravitypy-1.1.3/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1340 2023-05-07 20:40:23.000000 gravitypy-1.1.3/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 19:11:33.893231 gravitypy-1.1.3/gravitypy/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 20:40:23.000000 gravitypy-1.1.3/gravitypy/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-08 19:10:52.000000 gravitypy-1.1.3/gravitypy/__main__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15604 2023-05-08 19:10:49.000000 gravitypy-1.1.3/gravitypy/main.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 19:11:33.893231 gravitypy-1.1.3/gravitypy/resources/
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 19:11:33.897231 gravitypy-1.1.3/gravitypy/resources/fonts/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 20:40:23.000000 gravitypy-1.1.3/gravitypy/resources/fonts/minecraft_font.ttf
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 19:11:33.897231 gravitypy-1.1.3/gravitypy.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-08 19:11:33.000000 gravitypy-1.1.3/gravitypy.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      362 2023-05-08 19:11:33.000000 gravitypy-1.1.3/gravitypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-08 19:11:33.000000 gravitypy-1.1.3/gravitypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-05-08 19:11:33.000000 gravitypy-1.1.3/gravitypy.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-08 19:11:33.000000 gravitypy-1.1.3/gravitypy.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-05-08 19:11:33.000000 gravitypy-1.1.3/gravitypy.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 20:40:23.000000 gravitypy-1.1.3/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-08 19:11:33.897231 gravitypy-1.1.3/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      973 2023-05-08 19:11:02.000000 gravitypy-1.1.3/setup.py
```

### Comparing `gravitypy-1.1.2/LICENSE` & `gravitypy-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.2/README.md` & `gravitypy-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.2/gravitypy/main.py` & `gravitypy-1.1.3/gravitypy/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,20 +291,21 @@
 
         if add_button_statement:
             actual_mouse_x, actuale_mouse_y = pygame.mouse.get_pos()
             scaled_mouse_x = int(MOUSE_X + (actual_mouse_x - MOUSE_X) * SCALE)
             scaled_mouse_y = int(MOUSE_Y + (actuale_mouse_y - MOUSE_Y) * SCALE)
             circle_center = (scaled_mouse_x, scaled_mouse_y)
             circle_radius = int(ADDED_RADIUS * SCALE)
-            pygame.draw.circle(
-                SCREEN, 
-                ADDED_COLOR , 
-                circle_center, 
-                circle_radius
-                )
+            if 0 < scaled_mouse_y < HEIGHT and 0 < scaled_mouse_x < WIDTH: 
+                pygame.draw.circle(
+                    SCREEN, 
+                    ADDED_COLOR , 
+                    circle_center, 
+                    circle_radius
+                    )
 
         if add_button_statement_put:
             particle_velocity = ADDED_VELOCITY.copy()
             PARTICLES.append(
                 Particle(
                     actual_mouse_x,
                     actuale_mouse_y,
@@ -328,14 +329,15 @@
             else:
                 particle.update()
             
                 for other_particle in PARTICLES:
                     if particle != other_particle:
                         particle.apply_gravitational_force(other_particle, G)
             particle.draw_scaled(MOUSE_X, MOUSE_Y)
+        
         # Buttons
         button_increse_r = Buttons(50,50,"Increse R", pygame.Rect(50,50,120,25))
         button_decrese_r = Buttons(150,50,"Decrese R", pygame.Rect(50,85,120,25))
         button_increse_m = Buttons(250,50,"Increse M", pygame.Rect(200,50,120,25))
         button_decrese_m = Buttons(350,50,"Decrese M", pygame.Rect(200,85,120,25))
         button_increse_vx = Buttons(250,50,"+ Vx", pygame.Rect(350,50,50,25))
         button_decrese_vx = Buttons(350,50,"- Vx", pygame.Rect(350,85,50,25))
```

### Comparing `gravitypy-1.1.2/gravitypy/resources/fonts/minecraft_font.ttf` & `gravitypy-1.1.3/gravitypy/resources/fonts/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.2/setup.py` & `gravitypy-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 req_file = os.path.join(here, 'requirements.txt')
 with open(req_file, 'r') as f:
     REQUIREMENTS = [line.strip() for line in f.readlines()]
 LONG_DESCRIPTION = 'Pygame N-Body gravity simulation app'
 
 setup(
    name='gravitypy',
-   version='1.1.2',
+   version='1.1.3',
    description='Particles Gravity',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/Particles_Gravity",
    long_description_content_type="text/markdown",
    package_data={'gravitypy': ['*']},
```

