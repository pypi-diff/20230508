# Comparing `tmp/gravitypy-1.0.8.tar.gz` & `tmp/gravitypy-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitypy-1.0.8.tar", last modified: Sun May  7 19:28:42 2023, max compression
+gzip compressed data, was "gravitypy-1.0.9.tar", last modified: Sun May  7 19:30:33 2023, max compression
```

## Comparing `gravitypy-1.0.8.tar` & `gravitypy-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:28:42.730007 gravitypy-1.0.8/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 16:26:56.000000 gravitypy-1.0.8/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 16:26:56.000000 gravitypy-1.0.8/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 19:28:42.730007 gravitypy-1.0.8/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1005 2023-05-07 16:26:56.000000 gravitypy-1.0.8/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:28:42.726007 gravitypy-1.0.8/gravitypy/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 16:26:56.000000 gravitypy-1.0.8/gravitypy/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-07 19:25:11.000000 gravitypy-1.0.8/gravitypy/__main__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15448 2023-05-07 19:20:12.000000 gravitypy-1.0.8/gravitypy/main.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:28:42.726007 gravitypy-1.0.8/gravitypy/resources/
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:28:42.730007 gravitypy-1.0.8/gravitypy/resources/fonts/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 16:26:56.000000 gravitypy-1.0.8/gravitypy/resources/fonts/minecraft_font.ttf
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:28:42.730007 gravitypy-1.0.8/gravitypy.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 19:28:42.000000 gravitypy-1.0.8/gravitypy.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      362 2023-05-07 19:28:42.000000 gravitypy-1.0.8/gravitypy.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-07 19:28:42.000000 gravitypy-1.0.8/gravitypy.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-05-07 19:28:42.000000 gravitypy-1.0.8/gravitypy.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 19:28:42.000000 gravitypy-1.0.8/gravitypy.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-05-07 19:28:42.000000 gravitypy-1.0.8/gravitypy.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 16:26:56.000000 gravitypy-1.0.8/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-07 19:28:42.730007 gravitypy-1.0.8/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      905 2023-05-07 19:28:18.000000 gravitypy-1.0.8/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:30:33.421872 gravitypy-1.0.9/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 16:26:56.000000 gravitypy-1.0.9/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 16:26:56.000000 gravitypy-1.0.9/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 19:30:33.421872 gravitypy-1.0.9/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1005 2023-05-07 16:26:56.000000 gravitypy-1.0.9/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:30:33.421872 gravitypy-1.0.9/gravitypy/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 16:26:56.000000 gravitypy-1.0.9/gravitypy/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-07 19:25:11.000000 gravitypy-1.0.9/gravitypy/__main__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15441 2023-05-07 19:30:04.000000 gravitypy-1.0.9/gravitypy/main.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:30:33.421872 gravitypy-1.0.9/gravitypy/resources/
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:30:33.421872 gravitypy-1.0.9/gravitypy/resources/fonts/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 16:26:56.000000 gravitypy-1.0.9/gravitypy/resources/fonts/minecraft_font.ttf
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:30:33.421872 gravitypy-1.0.9/gravitypy.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 19:30:33.000000 gravitypy-1.0.9/gravitypy.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      362 2023-05-07 19:30:33.000000 gravitypy-1.0.9/gravitypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-07 19:30:33.000000 gravitypy-1.0.9/gravitypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-05-07 19:30:33.000000 gravitypy-1.0.9/gravitypy.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 19:30:33.000000 gravitypy-1.0.9/gravitypy.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-05-07 19:30:33.000000 gravitypy-1.0.9/gravitypy.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 16:26:56.000000 gravitypy-1.0.9/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-07 19:30:33.421872 gravitypy-1.0.9/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      905 2023-05-07 19:30:11.000000 gravitypy-1.0.9/setup.py
```

### Comparing `gravitypy-1.0.8/LICENSE` & `gravitypy-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gravitypy-1.0.8/README.md` & `gravitypy-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gravitypy-1.0.8/gravitypy/main.py` & `gravitypy-1.0.9/gravitypy/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 pygame.display.set_caption("GravityPy")
 
 WIDTH, HEIGHT = 1200, 800
 SCREEN = pygame.display.set_mode((WIDTH, HEIGHT))
 CLOCK = pygame.time.Clock()
 font_path = os.path.join(os.path.dirname(__file__), 'gravitypy/resources/fonts/minecraft_font.ttf')
 
-FONT = pygame.font.Font(font_path, font_size)
+FONT = pygame.font.Font(font_path, 16)
 G = 100
 SCALE = 1.0
 PARTICLES = []
 ADDED_RADIUS = 20
 ADDED_MASS = 20
 ADDED_VELOCITY = pygame.Vector2(0, 0)
 NUM_PARTICLES = 30
```

### Comparing `gravitypy-1.0.8/gravitypy/resources/fonts/minecraft_font.ttf` & `gravitypy-1.0.9/gravitypy/resources/fonts/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `gravitypy-1.0.8/setup.py` & `gravitypy-1.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 req_file = os.path.join(here, 'requirements.txt')
 with open(req_file, 'r') as f:
     REQUIREMENTS = [line.strip() for line in f.readlines()]
 LONG_DESCRIPTION = 'Pygame N-Body gravity simulation app'
 
 setup(
    name='gravitypy',
-   version='1.0.8',
+   version='1.0.9',
    description='Particles Gravity',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/Particles_Gravity",
    long_description_content_type="text/markdown",
    long_description=LONG_DESCRIPTION,
```

