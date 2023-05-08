# Comparing `tmp/bpy_building_blocks-0.0.23.tar.gz` & `tmp/bpy_building_blocks-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpy_building_blocks-0.0.23.tar", last modified: Tue Feb 14 08:00:31 2023, max compression
+gzip compressed data, was "bpy_building_blocks-0.0.24.tar", last modified: Mon May  8 06:08:24 2023, max compression
```

## Comparing `bpy_building_blocks-0.0.23.tar` & `bpy_building_blocks-0.0.24.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-02-14 08:00:31.298926 bpy_building_blocks-0.0.23/
--rw-rw-rw-   0        0        0     1093 2022-11-04 19:58:39.000000 bpy_building_blocks-0.0.23/LICENSE
--rw-rw-rw-   0        0        0    10567 2023-02-14 08:00:31.298926 bpy_building_blocks-0.0.23/PKG-INFO
--rw-rw-rw-   0        0        0    10032 2023-02-12 19:58:07.000000 bpy_building_blocks-0.0.23/README.md
--rw-rw-rw-   0        0        0       42 2023-02-14 08:00:31.299926 bpy_building_blocks-0.0.23/setup.cfg
--rw-rw-rw-   0        0        0      944 2022-11-04 19:58:39.000000 bpy_building_blocks-0.0.23/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-14 08:00:31.267919 bpy_building_blocks-0.0.23/src/
-drwxrwxrwx   0        0        0        0 2023-02-14 08:00:31.284923 bpy_building_blocks-0.0.23/src/bpy_building_blocks.egg-info/
--rw-rw-rw-   0        0        0    10567 2023-02-14 08:00:31.000000 bpy_building_blocks-0.0.23/src/bpy_building_blocks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-02-14 08:00:31.000000 bpy_building_blocks-0.0.23/src/bpy_building_blocks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-14 08:00:31.000000 bpy_building_blocks-0.0.23/src/bpy_building_blocks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-02-14 08:00:31.000000 bpy_building_blocks-0.0.23/src/bpy_building_blocks.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-14 08:00:31.297927 bpy_building_blocks-0.0.23/src/bpybb/
--rw-rw-rw-   0        0        0      269 2022-11-04 19:58:39.000000 bpy_building_blocks-0.0.23/src/bpybb/__init__.py
--rw-rw-rw-   0        0        0     2046 2022-11-04 19:58:39.000000 bpy_building_blocks-0.0.23/src/bpybb/addon.py
--rw-rw-rw-   0        0        0     3945 2023-02-10 07:59:09.000000 bpy_building_blocks-0.0.23/src/bpybb/animate.py
--rw-rw-rw-   0        0        0      915 2022-11-04 19:58:39.000000 bpy_building_blocks-0.0.23/src/bpybb/collection.py
--rw-rw-rw-   0        0        0     2378 2022-11-04 19:58:39.000000 bpy_building_blocks-0.0.23/src/bpybb/color.py
--rw-rw-rw-   0        0        0      388 2023-02-10 07:41:06.000000 bpy_building_blocks-0.0.23/src/bpybb/empty.py
--rw-rw-rw-   0        0        0     3564 2022-11-04 19:58:39.000000 bpy_building_blocks-0.0.23/src/bpybb/hdri.py
--rw-rw-rw-   0        0        0     2716 2022-11-04 19:58:39.000000 bpy_building_blocks-0.0.23/src/bpybb/material.py
--rw-rw-rw-   0        0        0      713 2022-11-04 20:10:45.000000 bpy_building_blocks-0.0.23/src/bpybb/mesh.py
--rw-rw-rw-   0        0        0     1105 2023-02-10 08:18:37.000000 bpy_building_blocks-0.0.23/src/bpybb/modifier.py
--rw-rw-rw-   0        0        0     2653 2023-02-10 08:20:52.000000 bpy_building_blocks-0.0.23/src/bpybb/object.py
--rw-rw-rw-   0        0        0     3043 2022-11-04 19:58:39.000000 bpy_building_blocks-0.0.23/src/bpybb/output.py
--rw-rw-rw-   0        0        0     1021 2023-02-10 07:27:31.000000 bpy_building_blocks-0.0.23/src/bpybb/random.py
--rw-rw-rw-   0        0        0     6241 2022-11-06 04:38:27.000000 bpy_building_blocks-0.0.23/src/bpybb/utils.py
--rw-rw-rw-   0        0        0      135 2023-01-28 17:06:16.000000 bpy_building_blocks-0.0.23/src/bpybb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:08:24.227404 bpy_building_blocks-0.0.24/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-08 06:08:11.000000 bpy_building_blocks-0.0.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-05-08 06:08:24.227404 bpy_building_blocks-0.0.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-05-08 06:08:11.000000 bpy_building_blocks-0.0.24/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 06:08:24.227404 bpy_building_blocks-0.0.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-08 06:08:11.000000 bpy_building_blocks-0.0.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:08:24.223404 bpy_building_blocks-0.0.24/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:08:24.227404 bpy_building_blocks-0.0.24/src/bpy_building_blocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-05-08 06:08:24.000000 bpy_building_blocks-0.0.24/src/bpy_building_blocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-08 06:08:24.000000 bpy_building_blocks-0.0.24/src/bpy_building_blocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 06:08:24.000000 bpy_building_blocks-0.0.24/src/bpy_building_blocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 06:08:24.000000 bpy_building_blocks-0.0.24/src/bpy_building_blocks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:08:24.227404 bpy_building_blocks-0.0.24/src/bpybb/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-08 06:08:11.000000 bpy_building_blocks-0.0.24/src/bpybb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-08 06:08:11.000000 bpy_building_blocks-0.0.24/src/bpybb/addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-08 06:08:11.000000 bpy_building_blocks-0.0.24/src/bpybb/animate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-08 06:08:11.000000 bpy_building_blocks-0.0.24/src/bpybb/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-08 06:08:11.000000 bpy_building_blocks-0.0.24/src/bpybb/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-08 06:08:11.000000 bpy_building_blocks-0.0.24/src/bpybb/empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-08 06:08:11.000000 bpy_building_blocks-0.0.24/src/bpybb/hdri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-08 06:08:11.000000 bpy_building_blocks-0.0.24/src/bpybb/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-08 06:08:11.000000 bpy_building_blocks-0.0.24/src/bpybb/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-08 06:08:11.000000 bpy_building_blocks-0.0.24/src/bpybb/modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-08 06:08:11.000000 bpy_building_blocks-0.0.24/src/bpybb/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-08 06:08:11.000000 bpy_building_blocks-0.0.24/src/bpybb/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-08 06:08:11.000000 bpy_building_blocks-0.0.24/src/bpybb/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-05-08 06:08:11.000000 bpy_building_blocks-0.0.24/src/bpybb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-08 06:08:11.000000 bpy_building_blocks-0.0.24/src/bpybb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-08 06:08:11.000000 bpy_building_blocks-0.0.24/src/bpybb/world_shader.py
```

### Comparing `bpy_building_blocks-0.0.23/PKG-INFO` & `bpy_building_blocks-0.0.24/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,174 +1,169 @@
-Metadata-Version: 2.1
-Name: bpy_building_blocks
-Version: 0.0.23
-Summary: A collection of helper functions and code used for speeding up Blender 3D Python script development.
-Home-page: https://github.com/CGArtPython/bpy_building_blocks
-Author: Viktor Stepanov
-Author-email: cgartpython@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Summary
-
-A collection of helper functions and code used for speeding up Blender 3D Python script development.
-
-Checkout project examples [YouTube: Art with a Python script](https://www.youtube.com/watch?v=rIhXHSdMWmc&list=PLB8-FQgROBmm-2f6Vyos6rbnjZeEScrX1)
-
-Important: This package assumes you are using [Blender's](https://www.blender.org/) embedded Python interpreter. 
-
-# Installation
-
-## Installation Walkthrough Video 
-
-[YouTube: How to install the bpy Building Blocks Python package](https://www.youtube.com/watch?v=_irmuKXjhS0)
-
-## From the command line via pip (into Blender's embedded Python interpreter)
-
----
-
-### on Windows
-
-**Important:**
-Make sure the `site-packages` folder of Blender's embedded Python interpreter is `writable`.
-_See video ^ if you are not sure how to do that_
-If you won't do this the package will be installed into another folder outside of Blender's embedded Python interpreter.
-And you will see this warning: `Defaulting to user installation because normal site-packages is not writeable`
-
-Run the pip install:
-* `Blender <VERSION>/<VERSION>/python/bin/python.exe -m pip install bpy-building-blocks`
-
-Example:
-* `> cd C:\Program Files\Blender Foundation\Blender 3.2\3.2\python\bin `
-* `> .\python.exe -m pip install bpy-building-blocks`
-
----
-
-### on macOS
-
-**Important:**
-Make sure pip is available.
-
-Run `ensurepip`
-* `/Applications/Blender.app/Contents/Resources/<VERSION>/python/bin/python -m ensurepip`
-
-Run the pip install:
-* `/Applications/Blender.app/Contents/Resources/<VERSION>/python/bin/python -m pip install bpy-building-blocks`
-
----
-
-### on Linux
-
-**Important:**
-Make sure pip is available.
-
-Run `ensurepip`
-* `~/<INSTALL LOCATION OF BLENDER>/<VERSION>/python/bin/python -m ensurepip`
-
-Run the pip install:
-* `~/<INSTALL LOCATION OF BLENDER>/<VERSION>/python/bin/python -m pip install bpy-building-blocks`
-
----
-
-## Via Blender Add-on
-
-[bpy_building_blocks_addon on github](https://github.com/CGArtPython/bpy_building_blocks_addon/releases)
-
-See video for details [YouTube: How to install the bpy Building Blocks Python package](https://www.youtube.com/watch?v=_irmuKXjhS0)
-
-# Package Contents
-
-## Utilities
-
-* active_object() - Get a references to the currently active object 
-* clean_scene() - Removing all of the objects, collection, materials, particles, textures, images, curves, meshes, actions, nodes, and worlds from the scene; Checkout this video explanation with example ["How to clean the scene with Python in Blender (with examples)"](https://youtu.be/3rNqVPtbhzc)
-* purge_orphans() - Remove all orphan data blocks; see this from more info: https://youtu.be/3rNqVPtbhzc?t=149
-* edit_mode() - A context manager to get into and out of edit mode
-* make_active(obj) - Make the passed in object active
-* parent(child_obj, parent_obj, keep_transform=False) - Parent one object to another
-* duplicate_object(obj=None, linked=False)
-* render_animation() - Renders the animation in the currently active scene
-* render_image(write_still=False) - Renders the currently active scene
-
-## Color Utilities
-
-* bpybb.color.convert_srgb_to_linear_rgb(srgb_color_component) - Converting from sRGB to Linear RGB based on [sRGB to CIE XYZ](https://en.wikipedia.org/wiki/SRGB#From_sRGB_to_CIE_XYZ)
-* bpybb.color.hex_color_to_rgb(hex_color) - Converting from a color in the form of a [hex triplet string](en.wikipedia.org/wiki/Web_colors#Hex_triplet) to a Linear RGB (Supports: "#RRGGBB" or "RRGGBB")
-* bpybb.color.hex_color_to_rgba(hex_color, alpha=1.0) - Converting from a color in the form of a hex triplet string to a Linear RGB (Supports: "#RRGGBB" or "RRGGBB") with an Alpha value
-
-## Add-on Utilities
-
-* bpybb.addon.enable_addon(addon_module_name) - enables a given addon; Checkout this video explanation with example ["How to enable add-ons with Python in Blender (with examples)"](https://youtu.be/HnrInoBWT6Q)
-* bpybb.addon.enable_animation_animall() - enable [Animall addon](https://docs.blender.org/manual/en/dev/addons/animation/animall.html)
-* bpybb.addon.enable_ant_landscape() - enable [ANT Landscape addon](https://docs.blender.org/manual/en/3.0/addons/add_mesh/ant_landscape.html)
-* bpybb.addon.enable_extra_curves() - enable [Add Curve Extra Objects addon](https://docs.blender.org/manual/en/3.0/addons/add_curve/extra_objects.html)
-* bpybb.addon.enable_extra_meshes() - enable [Add Mesh Extra Objects addon](https://docs.blender.org/manual/en/3.0/addons/add_mesh/mesh_extra_objects.html)
-* bpybb.addon.enable_import_images_as_planes() - enable [Images as Planes addon](https://docs.blender.org/manual/en/3.0/addons/import_export/images_as_planes.html)
-* bpybb.addon.enable_mod_tools() - enable [Modifier Tools addon](https://docs.blender.org/manual/en/3.0/addons/add_mesh/ant_landscape.html)
-* bpybb.addon.enable_pointcache_pc2() - enable [Pointcache (pc2) addon](https://docs.blender.org/manual/en/3.0/addons/import_export/pc2.html)
-
-## Collection Utilities
-
-* bpybb.collection.create_collection(col_name) - creates a [Blender Scene Collection](https://docs.blender.org/manual/en/latest/scene_layout/collections/collections.html)
-
-## HDRI Utilities
-
-* bpybb.hdri.apply_hdri(path_to_image, bg_color, hdri_light_strength, bg_strength) - creates a HDRI setup based on a technique from a [FlippedNormals tutorial](https://www.youtube.com/watch?v=dbAWTNCJVEs)
-
-## Material Utilities
-
-* bpybb.material.apply_material(material) - apply a material to the currently active object.
-* bpybb.material.make_color_ramp_from_color_list(colors, color_ramp_node) - creates new sliders on a Color Ramp Node and applies the list of colors on each slider
-
-## Mesh Utilities
-
-* bpybb.mesh.get_vert_coordinates_list(obj) - get a list of vertex coordinates for a given object
-* bpybb.mesh.subdivide() - subdivide the current active object
-
-## Random Utilities
-
-* bpybb.random.time_seed() - Sets the random seed based on the time and copies the seed into the clipboard
-* bpybb.random.get_random_rotation() - Returns a random Euler rotation on X, Y, Z
-
-## Object Utilities
-
-* bpybb.object.add_empty(name=None) - Add an Empty object into the scene
-* bpybb.object.apply_location() - Applies the location of the current object
-* bpybb.object.track_empty(obj) - Adds an Empty object and adds a To Track Constraint on the passed in object to track the Empty
-* bpybb.object.add_bezier_circle(radius: float = 1.0, bevel_depth: float = 0.0, resolution_u: int = 12, extrude: float = 0.0) - Adds a Bezier circle curve into the scene.
-* bpybb.object.add_round_cube(radius: float = 1.0) - Adds a Round Cube into the scene.
-* bpybb.object.add_subdivided_round_cube(radius: float = 1.0) - Adds a Round Cube into the scene and applies a Subdivision modifier.
-
-## Animation Utilities
-
-* bpybb.animate.set_fcurve_extrapolation_to_linear(obj=None) - loops over all the fcurves of an action and sets the extrapolation to "LINEAR"
-* bpybb.animate.set_fcurve_interpolation_to_linear(obj=None) - loops over all the fcurve key frame points of an action and sets the interpolation to "LINEAR"
-* bpybb.animate.animate_360_rotation(axis_index, last_frame, obj=None, clockwise=False, linear=True, start_frame=1) - animates the 360 rotation of an object about the given axis
-* bpybb.animate.animate_rotation(angle, axis_index, last_frame, obj=None, clockwise=False, linear=True, start_frame=1) - animates the rotation of an object about the given axis
-* bpybb.animate.create_data_animation_loop(obj, data_path, start_value, mid_value, start_frame, loop_length, linear_extrapolation=True) - make a data property loop
-* bpybb.animate.animate_up_n_down_bob(start_value: mathutils.Vector, mid_value: mathutils.Vector, obj: bpy_types.Object = None, loop_length: int = 90, start_frame: int = random.randint(0, 60)) - animate the up and down bobbing motion of an object
-* bpybb.animate.add_fcruve_cycles_modifier(obj: bpy_types.Object = None) - Apply a cycles modifier to all the fcurve animation data of an object.
-
-## Modifier Utilities
-
-* bpybb.modifier.add_displace_modifier(name: str, texture_type: str, empty_obj: bpy_types.Object = None) - Add a displace modifier and a texture to the currently active object.
-
-## Output Utilities
-
-* bpybb.output.set_1080p_render_res() - Set the resolution of the rendered image to 1080p
-* bpybb.output.set_1080px_square_render_res() - Set the resolution of the rendered image to 1080 by 1080 pixels
-* bpybb.output.set_1440px_square_render_res() - Set the resolution of the rendered image to 1440 by 1440 pixels
-* bpybb.output.set_2048px_square_render_res() - Set the resolution of the rendered image to 2048 by 2048 pixels
-* bpybb.output.set_2k_render_res() - Set the resolution of the rendered image to 2K
-* bpybb.output.set_4096px_square_render_res() - Set the resolution of the rendered image to 4096 by 4096 pixels
-* bpybb.output.set_4k_render_res() - Set the resolution of the rendered image to 4K
-* bpybb.output.set_720px_square_render_res() - Set the resolution of the rendered image to 720 by 720 pixels
-* bpybb.output.set_instagram_portrait_render_res() - Set the resolution of the rendered image to 1080x1350
-* bpybb.output.set_instagram_square_render_res() - Set the resolution of the rendered image to 1080x1080
-* bpybb.output.set_square_render_res(pixels) - Set the resolution of the rendered image to a square
-* bpybb.output.set_twitter_landscape_render_res() - Set the resolution of the rendered image to 1280x720 from Twitter's Media Best Practices ref: https://developer.twitter.com/en/docs/twitter-api/v1/media/upload-media/uploading-media/media-best-practices
-* bpybb.output.set_twitter_square_render_res() - Set the resolution of the rendered image to 720x720 from Twitter's Media Best Practices ref: https://developer.twitter.com/en/docs/twitter-api/v1/media/upload-media/uploading-media/media-best-practices
-* bpybb.output.set_wqhd_render_res() - Set the resolution of the rendered image to 2560x1440 (QHD)
+# Summary
+
+A collection of helper functions and code used for speeding up Blender 3D Python script development.
+
+Checkout project examples [YouTube: Art with a Python script](https://www.youtube.com/watch?v=rIhXHSdMWmc&list=PLB8-FQgROBmm-2f6Vyos6rbnjZeEScrX1)
+
+Important: This package assumes you are using [Blender's](https://www.blender.org/) embedded Python interpreter. 
+
+# Installation
+
+## Installation Walkthrough Video 
+
+[YouTube: How to install the bpy Building Blocks Python package](https://www.youtube.com/watch?v=_irmuKXjhS0)
+
+## From the command line via pip (into Blender's embedded Python interpreter)
+
+---
+
+### on Windows
+
+**Important:**
+Make sure the `site-packages` folder of Blender's embedded Python interpreter is `writable`.
+_See video ^ if you are not sure how to do that_
+If you won't do this the package will be installed into another folder outside of Blender's embedded Python interpreter.
+And you will see this warning: `Defaulting to user installation because normal site-packages is not writeable`
+
+Run the pip install:
+* `Blender <VERSION>/<VERSION>/python/bin/python.exe -m pip install bpy-building-blocks`
+
+Example:
+* `> cd C:\Program Files\Blender Foundation\Blender 3.2\3.2\python\bin `
+* `> .\python.exe -m pip install bpy-building-blocks`
+
+---
+
+### on macOS
+
+**Important:**
+Make sure pip is available.
+
+Run `ensurepip`
+* `/Applications/Blender.app/Contents/Resources/<VERSION>/python/bin/python -m ensurepip`
+
+Run the pip install:
+* `/Applications/Blender.app/Contents/Resources/<VERSION>/python/bin/python -m pip install bpy-building-blocks`
+
+---
+
+### on Linux
+
+**Important:**
+Make sure pip is available.
+
+Run `ensurepip`
+* `~/<INSTALL LOCATION OF BLENDER>/<VERSION>/python/bin/python -m ensurepip`
+
+Run the pip install:
+* `~/<INSTALL LOCATION OF BLENDER>/<VERSION>/python/bin/python -m pip install bpy-building-blocks`
+
+---
+
+## Via Blender Add-on
+
+[bpy_building_blocks_addon on github](https://github.com/CGArtPython/bpy_building_blocks_addon/releases)
+
+See video for details [YouTube: How to install the bpy Building Blocks Python package](https://www.youtube.com/watch?v=_irmuKXjhS0)
+
+# Package Contents
+
+## Utilities
+
+* bpybb.utils.active_object() - Get a references to the currently active object 
+* bpybb.utils.clean_scene() - Removing all of the objects, collection, materials, particles, textures, images, curves, meshes, actions, nodes, and worlds from the scene; Checkout this video explanation with example ["How to clean the scene with Python in Blender (with examples)"](https://youtu.be/3rNqVPtbhzc)
+* bpybb.utils.purge_orphans() - Remove all orphan data blocks; see this from more info: https://youtu.be/3rNqVPtbhzc?t=149
+* bpybb.utils.edit_mode() - A context manager to get into and out of edit mode
+* bpybb.utils.make_active(obj) - Make the passed in object active
+* bpybb.utils.parent(child_obj, parent_obj, keep_transform=False) - Parent one object to another
+* bpybb.utils.duplicate_object(obj=None, linked=False)
+* bpybb.utils.render_animation() - Renders the animation in the currently active scene
+* bpybb.utils.render_image(write_still=False) - Renders the currently active scene
+* bpybb.utils.remove_libraries() - Remove libraries that were linked into the Blend file
+* bpybb.utils.deselect_all_objects() - Similar to bpy.ops.object.select_all(action="DESELECT")
+
+## Color Utilities
+
+* bpybb.color.convert_srgb_to_linear_rgb(srgb_color_component) - Converting from sRGB to Linear RGB based on [sRGB to CIE XYZ](https://en.wikipedia.org/wiki/SRGB#From_sRGB_to_CIE_XYZ)
+* bpybb.color.hex_color_to_rgb(hex_color) - Converting from a color in the form of a [hex triplet string](en.wikipedia.org/wiki/Web_colors#Hex_triplet) to a Linear RGB (Supports: "#RRGGBB" or "RRGGBB")
+* bpybb.color.hex_color_to_rgba(hex_color, alpha=1.0) - Converting from a color in the form of a hex triplet string to a Linear RGB (Supports: "#RRGGBB" or "RRGGBB") with an Alpha value
+
+## Add-on Utilities
+
+* bpybb.addon.enable_addon(addon_module_name) - enables a given addon; Checkout this video explanation with example ["How to enable add-ons with Python in Blender (with examples)"](https://youtu.be/HnrInoBWT6Q)
+* bpybb.addon.enable_animation_animall() - enable [Animall addon](https://docs.blender.org/manual/en/dev/addons/animation/animall.html)
+* bpybb.addon.enable_ant_landscape() - enable [ANT Landscape addon](https://docs.blender.org/manual/en/3.0/addons/add_mesh/ant_landscape.html)
+* bpybb.addon.enable_extra_curves() - enable [Add Curve Extra Objects addon](https://docs.blender.org/manual/en/3.0/addons/add_curve/extra_objects.html)
+* bpybb.addon.enable_extra_meshes() - enable [Add Mesh Extra Objects addon](https://docs.blender.org/manual/en/3.0/addons/add_mesh/mesh_extra_objects.html)
+* bpybb.addon.enable_import_images_as_planes() - enable [Images as Planes addon](https://docs.blender.org/manual/en/3.0/addons/import_export/images_as_planes.html)
+* bpybb.addon.enable_mod_tools() - enable [Modifier Tools addon](https://docs.blender.org/manual/en/3.0/addons/add_mesh/ant_landscape.html)
+* bpybb.addon.enable_pointcache_pc2() - enable [Pointcache (pc2) addon](https://docs.blender.org/manual/en/3.0/addons/import_export/pc2.html)
+
+## Collection Utilities
+
+* bpybb.collection.create_collection(col_name) - creates a [Blender Scene Collection](https://docs.blender.org/manual/en/latest/scene_layout/collections/collections.html)
+* bpybb.collection.create_collection(collection_name: str, location: mathutils.Vector, rotation_euler: Optional[mathutils.Euler] = None, base_collection: Optional[bpy_types.Collection] = None) -> bpy_types.Object - creates an instance of a collection
+
+## HDRI Utilities
+
+* bpybb.hdri.apply_hdri(path_to_image, bg_color, hdri_light_strength, bg_strength) - creates a HDRI setup based on a technique from a [FlippedNormals tutorial](https://www.youtube.com/watch?v=dbAWTNCJVEs)
+
+## Material Utilities
+
+* bpybb.material.apply_material(material) - apply a material to the currently active object.
+* bpybb.material.make_color_ramp_from_color_list(colors, color_ramp_node) - creates new sliders on a Color Ramp Node and applies the list of colors on each slider
+
+## Mesh Utilities
+
+* bpybb.mesh.get_vert_coordinates_list(obj) - get a list of vertex coordinates for a given object
+* bpybb.mesh.subdivide() - subdivide the current active object
+
+## Random Utilities
+
+* bpybb.random.time_seed() - Sets the random seed based on the time and copies the seed into the clipboard
+* bpybb.random.get_random_rotation() - Returns a random Euler rotation on X, Y, Z
+
+## Object Utilities
+
+* bpybb.object.add_empty(name=None) - Add an Empty object into the scene
+* bpybb.object.apply_location() - Applies the location of the current object
+* bpybb.object.rotate_object(axis: int, degrees: float) - Rotate the active object about a given axis
+* bpybb.object.track_empty(obj) - Adds an Empty object and adds a To Track Constraint on the passed in object to track the Empty
+* bpybb.object.add_bezier_circle(radius: float = 1.0, bevel_depth: float = 0.0, resolution_u: int = 12, extrude: float = 0.0) - Adds a Bezier circle curve into the scene.
+* bpybb.object.add_round_cube(radius: float = 1.0) - Adds a Round Cube into the scene.
+* bpybb.object.add_subdivided_round_cube(radius: float = 1.0) - Adds a Round Cube into the scene and applies a Subdivision modifier.
+* join_objects(objects: list[bpy_types.Object]) -> bpy_types.Object - Joins the provided objects into one object
+
+## Animation Utilities
+
+* bpybb.animate.set_fcurve_extrapolation_to_linear(obj=None) - loops over all the fcurves of an action and sets the extrapolation to "LINEAR"
+* bpybb.animate.set_fcurve_interpolation_to_linear(obj=None) - loops over all the fcurve key frame points of an action and sets the interpolation to "LINEAR"
+* bpybb.animate.animate_360_rotation(axis_index, last_frame, obj=None, clockwise=False, linear=True, start_frame=1) - animates the 360 rotation of an object about the given axis
+* bpybb.animate.animate_rotation(angle, axis_index, last_frame, obj=None, clockwise=False, linear=True, start_frame=1) - animates the rotation of an object about the given axis
+* bpybb.animate.create_data_animation_loop(obj, data_path, start_value, mid_value, start_frame, loop_length, linear_extrapolation=True) - make a data property loop
+* bpybb.animate.animate_up_n_down_bob(start_value: mathutils.Vector, mid_value: mathutils.Vector, obj: bpy_types.Object = None, loop_length: int = 90, start_frame: int = random.randint(0, 60)) - animate the up and down bobbing motion of an object
+* bpybb.animate.add_fcruve_cycles_modifier(obj: bpy_types.Object = None) - Apply a cycles modifier to all the fcurve animation data of an object.
+
+## Modifier Utilities
+
+* bpybb.modifier.add_displace_modifier(name: str, texture_type: str, empty_obj: bpy_types.Object = None) - Add a displace modifier and a texture to the currently active object.
+
+## Output Utilities
+
+* bpybb.output.set_1080p_render_res() - Set the resolution of the rendered image to 1080p
+* bpybb.output.set_1080px_square_render_res() - Set the resolution of the rendered image to 1080 by 1080 pixels
+* bpybb.output.set_1440px_square_render_res() - Set the resolution of the rendered image to 1440 by 1440 pixels
+* bpybb.output.set_2048px_square_render_res() - Set the resolution of the rendered image to 2048 by 2048 pixels
+* bpybb.output.set_2k_render_res() - Set the resolution of the rendered image to 2K
+* bpybb.output.set_4096px_square_render_res() - Set the resolution of the rendered image to 4096 by 4096 pixels
+* bpybb.output.set_4k_render_res() - Set the resolution of the rendered image to 4K
+* bpybb.output.set_720px_square_render_res() - Set the resolution of the rendered image to 720 by 720 pixels
+* bpybb.output.set_instagram_portrait_render_res() - Set the resolution of the rendered image to 1080x1350
+* bpybb.output.set_instagram_square_render_res() - Set the resolution of the rendered image to 1080x1080
+* bpybb.output.set_square_render_res(pixels) - Set the resolution of the rendered image to a square
+* bpybb.output.set_twitter_landscape_render_res() - Set the resolution of the rendered image to 1280x720 from Twitter's Media Best Practices ref: https://developer.twitter.com/en/docs/twitter-api/v1/media/upload-media/uploading-media/media-best-practices
+* bpybb.output.set_twitter_square_render_res() - Set the resolution of the rendered image to 720x720 from Twitter's Media Best Practices ref: https://developer.twitter.com/en/docs/twitter-api/v1/media/upload-media/uploading-media/media-best-practices
+* bpybb.output.set_wqhd_render_res() - Set the resolution of the rendered image to 2560x1440 (QHD)
+
+## World Shader Utilities
+
+* bpybb.world_shader.set_up_world_sun_light() - Set up the lighing in a scene using the ShaderNodeTexSky world shader node
```

### Comparing `bpy_building_blocks-0.0.23/README.md` & `bpy_building_blocks-0.0.24/src/bpy_building_blocks.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,160 +1,183 @@
-# Summary
-
-A collection of helper functions and code used for speeding up Blender 3D Python script development.
-
-Checkout project examples [YouTube: Art with a Python script](https://www.youtube.com/watch?v=rIhXHSdMWmc&list=PLB8-FQgROBmm-2f6Vyos6rbnjZeEScrX1)
-
-Important: This package assumes you are using [Blender's](https://www.blender.org/) embedded Python interpreter. 
-
-# Installation
-
-## Installation Walkthrough Video 
-
-[YouTube: How to install the bpy Building Blocks Python package](https://www.youtube.com/watch?v=_irmuKXjhS0)
-
-## From the command line via pip (into Blender's embedded Python interpreter)
-
----
-
-### on Windows
-
-**Important:**
-Make sure the `site-packages` folder of Blender's embedded Python interpreter is `writable`.
-_See video ^ if you are not sure how to do that_
-If you won't do this the package will be installed into another folder outside of Blender's embedded Python interpreter.
-And you will see this warning: `Defaulting to user installation because normal site-packages is not writeable`
-
-Run the pip install:
-* `Blender <VERSION>/<VERSION>/python/bin/python.exe -m pip install bpy-building-blocks`
-
-Example:
-* `> cd C:\Program Files\Blender Foundation\Blender 3.2\3.2\python\bin `
-* `> .\python.exe -m pip install bpy-building-blocks`
-
----
-
-### on macOS
-
-**Important:**
-Make sure pip is available.
-
-Run `ensurepip`
-* `/Applications/Blender.app/Contents/Resources/<VERSION>/python/bin/python -m ensurepip`
-
-Run the pip install:
-* `/Applications/Blender.app/Contents/Resources/<VERSION>/python/bin/python -m pip install bpy-building-blocks`
-
----
-
-### on Linux
-
-**Important:**
-Make sure pip is available.
-
-Run `ensurepip`
-* `~/<INSTALL LOCATION OF BLENDER>/<VERSION>/python/bin/python -m ensurepip`
-
-Run the pip install:
-* `~/<INSTALL LOCATION OF BLENDER>/<VERSION>/python/bin/python -m pip install bpy-building-blocks`
-
----
-
-## Via Blender Add-on
-
-[bpy_building_blocks_addon on github](https://github.com/CGArtPython/bpy_building_blocks_addon/releases)
-
-See video for details [YouTube: How to install the bpy Building Blocks Python package](https://www.youtube.com/watch?v=_irmuKXjhS0)
-
-# Package Contents
-
-## Utilities
-
-* active_object() - Get a references to the currently active object 
-* clean_scene() - Removing all of the objects, collection, materials, particles, textures, images, curves, meshes, actions, nodes, and worlds from the scene; Checkout this video explanation with example ["How to clean the scene with Python in Blender (with examples)"](https://youtu.be/3rNqVPtbhzc)
-* purge_orphans() - Remove all orphan data blocks; see this from more info: https://youtu.be/3rNqVPtbhzc?t=149
-* edit_mode() - A context manager to get into and out of edit mode
-* make_active(obj) - Make the passed in object active
-* parent(child_obj, parent_obj, keep_transform=False) - Parent one object to another
-* duplicate_object(obj=None, linked=False)
-* render_animation() - Renders the animation in the currently active scene
-* render_image(write_still=False) - Renders the currently active scene
-
-## Color Utilities
-
-* bpybb.color.convert_srgb_to_linear_rgb(srgb_color_component) - Converting from sRGB to Linear RGB based on [sRGB to CIE XYZ](https://en.wikipedia.org/wiki/SRGB#From_sRGB_to_CIE_XYZ)
-* bpybb.color.hex_color_to_rgb(hex_color) - Converting from a color in the form of a [hex triplet string](en.wikipedia.org/wiki/Web_colors#Hex_triplet) to a Linear RGB (Supports: "#RRGGBB" or "RRGGBB")
-* bpybb.color.hex_color_to_rgba(hex_color, alpha=1.0) - Converting from a color in the form of a hex triplet string to a Linear RGB (Supports: "#RRGGBB" or "RRGGBB") with an Alpha value
-
-## Add-on Utilities
-
-* bpybb.addon.enable_addon(addon_module_name) - enables a given addon; Checkout this video explanation with example ["How to enable add-ons with Python in Blender (with examples)"](https://youtu.be/HnrInoBWT6Q)
-* bpybb.addon.enable_animation_animall() - enable [Animall addon](https://docs.blender.org/manual/en/dev/addons/animation/animall.html)
-* bpybb.addon.enable_ant_landscape() - enable [ANT Landscape addon](https://docs.blender.org/manual/en/3.0/addons/add_mesh/ant_landscape.html)
-* bpybb.addon.enable_extra_curves() - enable [Add Curve Extra Objects addon](https://docs.blender.org/manual/en/3.0/addons/add_curve/extra_objects.html)
-* bpybb.addon.enable_extra_meshes() - enable [Add Mesh Extra Objects addon](https://docs.blender.org/manual/en/3.0/addons/add_mesh/mesh_extra_objects.html)
-* bpybb.addon.enable_import_images_as_planes() - enable [Images as Planes addon](https://docs.blender.org/manual/en/3.0/addons/import_export/images_as_planes.html)
-* bpybb.addon.enable_mod_tools() - enable [Modifier Tools addon](https://docs.blender.org/manual/en/3.0/addons/add_mesh/ant_landscape.html)
-* bpybb.addon.enable_pointcache_pc2() - enable [Pointcache (pc2) addon](https://docs.blender.org/manual/en/3.0/addons/import_export/pc2.html)
-
-## Collection Utilities
-
-* bpybb.collection.create_collection(col_name) - creates a [Blender Scene Collection](https://docs.blender.org/manual/en/latest/scene_layout/collections/collections.html)
-
-## HDRI Utilities
-
-* bpybb.hdri.apply_hdri(path_to_image, bg_color, hdri_light_strength, bg_strength) - creates a HDRI setup based on a technique from a [FlippedNormals tutorial](https://www.youtube.com/watch?v=dbAWTNCJVEs)
-
-## Material Utilities
-
-* bpybb.material.apply_material(material) - apply a material to the currently active object.
-* bpybb.material.make_color_ramp_from_color_list(colors, color_ramp_node) - creates new sliders on a Color Ramp Node and applies the list of colors on each slider
-
-## Mesh Utilities
-
-* bpybb.mesh.get_vert_coordinates_list(obj) - get a list of vertex coordinates for a given object
-* bpybb.mesh.subdivide() - subdivide the current active object
-
-## Random Utilities
-
-* bpybb.random.time_seed() - Sets the random seed based on the time and copies the seed into the clipboard
-* bpybb.random.get_random_rotation() - Returns a random Euler rotation on X, Y, Z
-
-## Object Utilities
-
-* bpybb.object.add_empty(name=None) - Add an Empty object into the scene
-* bpybb.object.apply_location() - Applies the location of the current object
-* bpybb.object.track_empty(obj) - Adds an Empty object and adds a To Track Constraint on the passed in object to track the Empty
-* bpybb.object.add_bezier_circle(radius: float = 1.0, bevel_depth: float = 0.0, resolution_u: int = 12, extrude: float = 0.0) - Adds a Bezier circle curve into the scene.
-* bpybb.object.add_round_cube(radius: float = 1.0) - Adds a Round Cube into the scene.
-* bpybb.object.add_subdivided_round_cube(radius: float = 1.0) - Adds a Round Cube into the scene and applies a Subdivision modifier.
-
-## Animation Utilities
-
-* bpybb.animate.set_fcurve_extrapolation_to_linear(obj=None) - loops over all the fcurves of an action and sets the extrapolation to "LINEAR"
-* bpybb.animate.set_fcurve_interpolation_to_linear(obj=None) - loops over all the fcurve key frame points of an action and sets the interpolation to "LINEAR"
-* bpybb.animate.animate_360_rotation(axis_index, last_frame, obj=None, clockwise=False, linear=True, start_frame=1) - animates the 360 rotation of an object about the given axis
-* bpybb.animate.animate_rotation(angle, axis_index, last_frame, obj=None, clockwise=False, linear=True, start_frame=1) - animates the rotation of an object about the given axis
-* bpybb.animate.create_data_animation_loop(obj, data_path, start_value, mid_value, start_frame, loop_length, linear_extrapolation=True) - make a data property loop
-* bpybb.animate.animate_up_n_down_bob(start_value: mathutils.Vector, mid_value: mathutils.Vector, obj: bpy_types.Object = None, loop_length: int = 90, start_frame: int = random.randint(0, 60)) - animate the up and down bobbing motion of an object
-* bpybb.animate.add_fcruve_cycles_modifier(obj: bpy_types.Object = None) - Apply a cycles modifier to all the fcurve animation data of an object.
-
-## Modifier Utilities
-
-* bpybb.modifier.add_displace_modifier(name: str, texture_type: str, empty_obj: bpy_types.Object = None) - Add a displace modifier and a texture to the currently active object.
-
-## Output Utilities
-
-* bpybb.output.set_1080p_render_res() - Set the resolution of the rendered image to 1080p
-* bpybb.output.set_1080px_square_render_res() - Set the resolution of the rendered image to 1080 by 1080 pixels
-* bpybb.output.set_1440px_square_render_res() - Set the resolution of the rendered image to 1440 by 1440 pixels
-* bpybb.output.set_2048px_square_render_res() - Set the resolution of the rendered image to 2048 by 2048 pixels
-* bpybb.output.set_2k_render_res() - Set the resolution of the rendered image to 2K
-* bpybb.output.set_4096px_square_render_res() - Set the resolution of the rendered image to 4096 by 4096 pixels
-* bpybb.output.set_4k_render_res() - Set the resolution of the rendered image to 4K
-* bpybb.output.set_720px_square_render_res() - Set the resolution of the rendered image to 720 by 720 pixels
-* bpybb.output.set_instagram_portrait_render_res() - Set the resolution of the rendered image to 1080x1350
-* bpybb.output.set_instagram_square_render_res() - Set the resolution of the rendered image to 1080x1080
-* bpybb.output.set_square_render_res(pixels) - Set the resolution of the rendered image to a square
-* bpybb.output.set_twitter_landscape_render_res() - Set the resolution of the rendered image to 1280x720 from Twitter's Media Best Practices ref: https://developer.twitter.com/en/docs/twitter-api/v1/media/upload-media/uploading-media/media-best-practices
-* bpybb.output.set_twitter_square_render_res() - Set the resolution of the rendered image to 720x720 from Twitter's Media Best Practices ref: https://developer.twitter.com/en/docs/twitter-api/v1/media/upload-media/uploading-media/media-best-practices
-* bpybb.output.set_wqhd_render_res() - Set the resolution of the rendered image to 2560x1440 (QHD)
+Metadata-Version: 2.1
+Name: bpy-building-blocks
+Version: 0.0.24
+Summary: A collection of helper functions and code used for speeding up Blender 3D Python script development.
+Home-page: https://github.com/CGArtPython/bpy_building_blocks
+Author: Viktor Stepanov
+Author-email: cgartpython@gmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Summary
+
+A collection of helper functions and code used for speeding up Blender 3D Python script development.
+
+Checkout project examples [YouTube: Art with a Python script](https://www.youtube.com/watch?v=rIhXHSdMWmc&list=PLB8-FQgROBmm-2f6Vyos6rbnjZeEScrX1)
+
+Important: This package assumes you are using [Blender's](https://www.blender.org/) embedded Python interpreter. 
+
+# Installation
+
+## Installation Walkthrough Video 
+
+[YouTube: How to install the bpy Building Blocks Python package](https://www.youtube.com/watch?v=_irmuKXjhS0)
+
+## From the command line via pip (into Blender's embedded Python interpreter)
+
+---
+
+### on Windows
+
+**Important:**
+Make sure the `site-packages` folder of Blender's embedded Python interpreter is `writable`.
+_See video ^ if you are not sure how to do that_
+If you won't do this the package will be installed into another folder outside of Blender's embedded Python interpreter.
+And you will see this warning: `Defaulting to user installation because normal site-packages is not writeable`
+
+Run the pip install:
+* `Blender <VERSION>/<VERSION>/python/bin/python.exe -m pip install bpy-building-blocks`
+
+Example:
+* `> cd C:\Program Files\Blender Foundation\Blender 3.2\3.2\python\bin `
+* `> .\python.exe -m pip install bpy-building-blocks`
+
+---
+
+### on macOS
+
+**Important:**
+Make sure pip is available.
+
+Run `ensurepip`
+* `/Applications/Blender.app/Contents/Resources/<VERSION>/python/bin/python -m ensurepip`
+
+Run the pip install:
+* `/Applications/Blender.app/Contents/Resources/<VERSION>/python/bin/python -m pip install bpy-building-blocks`
+
+---
+
+### on Linux
+
+**Important:**
+Make sure pip is available.
+
+Run `ensurepip`
+* `~/<INSTALL LOCATION OF BLENDER>/<VERSION>/python/bin/python -m ensurepip`
+
+Run the pip install:
+* `~/<INSTALL LOCATION OF BLENDER>/<VERSION>/python/bin/python -m pip install bpy-building-blocks`
+
+---
+
+## Via Blender Add-on
+
+[bpy_building_blocks_addon on github](https://github.com/CGArtPython/bpy_building_blocks_addon/releases)
+
+See video for details [YouTube: How to install the bpy Building Blocks Python package](https://www.youtube.com/watch?v=_irmuKXjhS0)
+
+# Package Contents
+
+## Utilities
+
+* bpybb.utils.active_object() - Get a references to the currently active object 
+* bpybb.utils.clean_scene() - Removing all of the objects, collection, materials, particles, textures, images, curves, meshes, actions, nodes, and worlds from the scene; Checkout this video explanation with example ["How to clean the scene with Python in Blender (with examples)"](https://youtu.be/3rNqVPtbhzc)
+* bpybb.utils.purge_orphans() - Remove all orphan data blocks; see this from more info: https://youtu.be/3rNqVPtbhzc?t=149
+* bpybb.utils.edit_mode() - A context manager to get into and out of edit mode
+* bpybb.utils.make_active(obj) - Make the passed in object active
+* bpybb.utils.parent(child_obj, parent_obj, keep_transform=False) - Parent one object to another
+* bpybb.utils.duplicate_object(obj=None, linked=False)
+* bpybb.utils.render_animation() - Renders the animation in the currently active scene
+* bpybb.utils.render_image(write_still=False) - Renders the currently active scene
+* bpybb.utils.remove_libraries() - Remove libraries that were linked into the Blend file
+* bpybb.utils.deselect_all_objects() - Similar to bpy.ops.object.select_all(action="DESELECT")
+
+## Color Utilities
+
+* bpybb.color.convert_srgb_to_linear_rgb(srgb_color_component) - Converting from sRGB to Linear RGB based on [sRGB to CIE XYZ](https://en.wikipedia.org/wiki/SRGB#From_sRGB_to_CIE_XYZ)
+* bpybb.color.hex_color_to_rgb(hex_color) - Converting from a color in the form of a [hex triplet string](en.wikipedia.org/wiki/Web_colors#Hex_triplet) to a Linear RGB (Supports: "#RRGGBB" or "RRGGBB")
+* bpybb.color.hex_color_to_rgba(hex_color, alpha=1.0) - Converting from a color in the form of a hex triplet string to a Linear RGB (Supports: "#RRGGBB" or "RRGGBB") with an Alpha value
+
+## Add-on Utilities
+
+* bpybb.addon.enable_addon(addon_module_name) - enables a given addon; Checkout this video explanation with example ["How to enable add-ons with Python in Blender (with examples)"](https://youtu.be/HnrInoBWT6Q)
+* bpybb.addon.enable_animation_animall() - enable [Animall addon](https://docs.blender.org/manual/en/dev/addons/animation/animall.html)
+* bpybb.addon.enable_ant_landscape() - enable [ANT Landscape addon](https://docs.blender.org/manual/en/3.0/addons/add_mesh/ant_landscape.html)
+* bpybb.addon.enable_extra_curves() - enable [Add Curve Extra Objects addon](https://docs.blender.org/manual/en/3.0/addons/add_curve/extra_objects.html)
+* bpybb.addon.enable_extra_meshes() - enable [Add Mesh Extra Objects addon](https://docs.blender.org/manual/en/3.0/addons/add_mesh/mesh_extra_objects.html)
+* bpybb.addon.enable_import_images_as_planes() - enable [Images as Planes addon](https://docs.blender.org/manual/en/3.0/addons/import_export/images_as_planes.html)
+* bpybb.addon.enable_mod_tools() - enable [Modifier Tools addon](https://docs.blender.org/manual/en/3.0/addons/add_mesh/ant_landscape.html)
+* bpybb.addon.enable_pointcache_pc2() - enable [Pointcache (pc2) addon](https://docs.blender.org/manual/en/3.0/addons/import_export/pc2.html)
+
+## Collection Utilities
+
+* bpybb.collection.create_collection(col_name) - creates a [Blender Scene Collection](https://docs.blender.org/manual/en/latest/scene_layout/collections/collections.html)
+* bpybb.collection.create_collection(collection_name: str, location: mathutils.Vector, rotation_euler: Optional[mathutils.Euler] = None, base_collection: Optional[bpy_types.Collection] = None) -> bpy_types.Object - creates an instance of a collection
+
+## HDRI Utilities
+
+* bpybb.hdri.apply_hdri(path_to_image, bg_color, hdri_light_strength, bg_strength) - creates a HDRI setup based on a technique from a [FlippedNormals tutorial](https://www.youtube.com/watch?v=dbAWTNCJVEs)
+
+## Material Utilities
+
+* bpybb.material.apply_material(material) - apply a material to the currently active object.
+* bpybb.material.make_color_ramp_from_color_list(colors, color_ramp_node) - creates new sliders on a Color Ramp Node and applies the list of colors on each slider
+
+## Mesh Utilities
+
+* bpybb.mesh.get_vert_coordinates_list(obj) - get a list of vertex coordinates for a given object
+* bpybb.mesh.subdivide() - subdivide the current active object
+
+## Random Utilities
+
+* bpybb.random.time_seed() - Sets the random seed based on the time and copies the seed into the clipboard
+* bpybb.random.get_random_rotation() - Returns a random Euler rotation on X, Y, Z
+
+## Object Utilities
+
+* bpybb.object.add_empty(name=None) - Add an Empty object into the scene
+* bpybb.object.apply_location() - Applies the location of the current object
+* bpybb.object.rotate_object(axis: int, degrees: float) - Rotate the active object about a given axis
+* bpybb.object.track_empty(obj) - Adds an Empty object and adds a To Track Constraint on the passed in object to track the Empty
+* bpybb.object.add_bezier_circle(radius: float = 1.0, bevel_depth: float = 0.0, resolution_u: int = 12, extrude: float = 0.0) - Adds a Bezier circle curve into the scene.
+* bpybb.object.add_round_cube(radius: float = 1.0) - Adds a Round Cube into the scene.
+* bpybb.object.add_subdivided_round_cube(radius: float = 1.0) - Adds a Round Cube into the scene and applies a Subdivision modifier.
+* join_objects(objects: list[bpy_types.Object]) -> bpy_types.Object - Joins the provided objects into one object
+
+## Animation Utilities
+
+* bpybb.animate.set_fcurve_extrapolation_to_linear(obj=None) - loops over all the fcurves of an action and sets the extrapolation to "LINEAR"
+* bpybb.animate.set_fcurve_interpolation_to_linear(obj=None) - loops over all the fcurve key frame points of an action and sets the interpolation to "LINEAR"
+* bpybb.animate.animate_360_rotation(axis_index, last_frame, obj=None, clockwise=False, linear=True, start_frame=1) - animates the 360 rotation of an object about the given axis
+* bpybb.animate.animate_rotation(angle, axis_index, last_frame, obj=None, clockwise=False, linear=True, start_frame=1) - animates the rotation of an object about the given axis
+* bpybb.animate.create_data_animation_loop(obj, data_path, start_value, mid_value, start_frame, loop_length, linear_extrapolation=True) - make a data property loop
+* bpybb.animate.animate_up_n_down_bob(start_value: mathutils.Vector, mid_value: mathutils.Vector, obj: bpy_types.Object = None, loop_length: int = 90, start_frame: int = random.randint(0, 60)) - animate the up and down bobbing motion of an object
+* bpybb.animate.add_fcruve_cycles_modifier(obj: bpy_types.Object = None) - Apply a cycles modifier to all the fcurve animation data of an object.
+
+## Modifier Utilities
+
+* bpybb.modifier.add_displace_modifier(name: str, texture_type: str, empty_obj: bpy_types.Object = None) - Add a displace modifier and a texture to the currently active object.
+
+## Output Utilities
+
+* bpybb.output.set_1080p_render_res() - Set the resolution of the rendered image to 1080p
+* bpybb.output.set_1080px_square_render_res() - Set the resolution of the rendered image to 1080 by 1080 pixels
+* bpybb.output.set_1440px_square_render_res() - Set the resolution of the rendered image to 1440 by 1440 pixels
+* bpybb.output.set_2048px_square_render_res() - Set the resolution of the rendered image to 2048 by 2048 pixels
+* bpybb.output.set_2k_render_res() - Set the resolution of the rendered image to 2K
+* bpybb.output.set_4096px_square_render_res() - Set the resolution of the rendered image to 4096 by 4096 pixels
+* bpybb.output.set_4k_render_res() - Set the resolution of the rendered image to 4K
+* bpybb.output.set_720px_square_render_res() - Set the resolution of the rendered image to 720 by 720 pixels
+* bpybb.output.set_instagram_portrait_render_res() - Set the resolution of the rendered image to 1080x1350
+* bpybb.output.set_instagram_square_render_res() - Set the resolution of the rendered image to 1080x1080
+* bpybb.output.set_square_render_res(pixels) - Set the resolution of the rendered image to a square
+* bpybb.output.set_twitter_landscape_render_res() - Set the resolution of the rendered image to 1280x720 from Twitter's Media Best Practices ref: https://developer.twitter.com/en/docs/twitter-api/v1/media/upload-media/uploading-media/media-best-practices
+* bpybb.output.set_twitter_square_render_res() - Set the resolution of the rendered image to 720x720 from Twitter's Media Best Practices ref: https://developer.twitter.com/en/docs/twitter-api/v1/media/upload-media/uploading-media/media-best-practices
+* bpybb.output.set_wqhd_render_res() - Set the resolution of the rendered image to 2560x1440 (QHD)
+
+## World Shader Utilities
+
+* bpybb.world_shader.set_up_world_sun_light() - Set up the lighing in a scene using the ShaderNodeTexSky world shader node
```

### Comparing `bpy_building_blocks-0.0.23/setup.py` & `bpy_building_blocks-0.0.24/setup.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from setuptools import setup
-import pathlib
-
-README_TEXT = pathlib.Path(__file__).parent.joinpath("README.md").read_text()
-
-# imports __version__ without importing the bpybb package
-exec(pathlib.Path(__file__).parent.joinpath("src", "bpybb", "version.py").read_text())
-
-setup(
-    name="bpy_building_blocks",
-    version=__version__,
-    description="A collection of helper functions and code used for speeding up Blender 3D Python script development.",
-    long_description=README_TEXT,
-    long_description_content_type="text/markdown",
-    url="https://github.com/CGArtPython/bpy_building_blocks",
-    author="Viktor Stepanov",
-    author_email="cgartpython@gmail.com",
-    license="MIT",
-    classifiers=[
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.9",
-    ],
-    packages=["bpybb"],
-    package_dir={"": "src"},
-)
+from setuptools import setup
+import pathlib
+
+README_TEXT = pathlib.Path(__file__).parent.joinpath("README.md").read_text()
+
+# imports __version__ without importing the bpybb package
+exec(pathlib.Path(__file__).parent.joinpath("src", "bpybb", "version.py").read_text())
+
+setup(
+    name="bpy_building_blocks",
+    version=__version__,
+    description="A collection of helper functions and code used for speeding up Blender 3D Python script development.",
+    long_description=README_TEXT,
+    long_description_content_type="text/markdown",
+    url="https://github.com/CGArtPython/bpy_building_blocks",
+    author="Viktor Stepanov",
+    author_email="cgartpython@gmail.com",
+    license="MIT",
+    classifiers=[
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.9",
+    ],
+    packages=["bpybb"],
+    package_dir={"": "src"},
+)
```

### Comparing `bpy_building_blocks-0.0.23/src/bpy_building_blocks.egg-info/PKG-INFO` & `bpy_building_blocks-0.0.24/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,174 +1,183 @@
-Metadata-Version: 2.1
-Name: bpy-building-blocks
-Version: 0.0.23
-Summary: A collection of helper functions and code used for speeding up Blender 3D Python script development.
-Home-page: https://github.com/CGArtPython/bpy_building_blocks
-Author: Viktor Stepanov
-Author-email: cgartpython@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Summary
-
-A collection of helper functions and code used for speeding up Blender 3D Python script development.
-
-Checkout project examples [YouTube: Art with a Python script](https://www.youtube.com/watch?v=rIhXHSdMWmc&list=PLB8-FQgROBmm-2f6Vyos6rbnjZeEScrX1)
-
-Important: This package assumes you are using [Blender's](https://www.blender.org/) embedded Python interpreter. 
-
-# Installation
-
-## Installation Walkthrough Video 
-
-[YouTube: How to install the bpy Building Blocks Python package](https://www.youtube.com/watch?v=_irmuKXjhS0)
-
-## From the command line via pip (into Blender's embedded Python interpreter)
-
----
-
-### on Windows
-
-**Important:**
-Make sure the `site-packages` folder of Blender's embedded Python interpreter is `writable`.
-_See video ^ if you are not sure how to do that_
-If you won't do this the package will be installed into another folder outside of Blender's embedded Python interpreter.
-And you will see this warning: `Defaulting to user installation because normal site-packages is not writeable`
-
-Run the pip install:
-* `Blender <VERSION>/<VERSION>/python/bin/python.exe -m pip install bpy-building-blocks`
-
-Example:
-* `> cd C:\Program Files\Blender Foundation\Blender 3.2\3.2\python\bin `
-* `> .\python.exe -m pip install bpy-building-blocks`
-
----
-
-### on macOS
-
-**Important:**
-Make sure pip is available.
-
-Run `ensurepip`
-* `/Applications/Blender.app/Contents/Resources/<VERSION>/python/bin/python -m ensurepip`
-
-Run the pip install:
-* `/Applications/Blender.app/Contents/Resources/<VERSION>/python/bin/python -m pip install bpy-building-blocks`
-
----
-
-### on Linux
-
-**Important:**
-Make sure pip is available.
-
-Run `ensurepip`
-* `~/<INSTALL LOCATION OF BLENDER>/<VERSION>/python/bin/python -m ensurepip`
-
-Run the pip install:
-* `~/<INSTALL LOCATION OF BLENDER>/<VERSION>/python/bin/python -m pip install bpy-building-blocks`
-
----
-
-## Via Blender Add-on
-
-[bpy_building_blocks_addon on github](https://github.com/CGArtPython/bpy_building_blocks_addon/releases)
-
-See video for details [YouTube: How to install the bpy Building Blocks Python package](https://www.youtube.com/watch?v=_irmuKXjhS0)
-
-# Package Contents
-
-## Utilities
-
-* active_object() - Get a references to the currently active object 
-* clean_scene() - Removing all of the objects, collection, materials, particles, textures, images, curves, meshes, actions, nodes, and worlds from the scene; Checkout this video explanation with example ["How to clean the scene with Python in Blender (with examples)"](https://youtu.be/3rNqVPtbhzc)
-* purge_orphans() - Remove all orphan data blocks; see this from more info: https://youtu.be/3rNqVPtbhzc?t=149
-* edit_mode() - A context manager to get into and out of edit mode
-* make_active(obj) - Make the passed in object active
-* parent(child_obj, parent_obj, keep_transform=False) - Parent one object to another
-* duplicate_object(obj=None, linked=False)
-* render_animation() - Renders the animation in the currently active scene
-* render_image(write_still=False) - Renders the currently active scene
-
-## Color Utilities
-
-* bpybb.color.convert_srgb_to_linear_rgb(srgb_color_component) - Converting from sRGB to Linear RGB based on [sRGB to CIE XYZ](https://en.wikipedia.org/wiki/SRGB#From_sRGB_to_CIE_XYZ)
-* bpybb.color.hex_color_to_rgb(hex_color) - Converting from a color in the form of a [hex triplet string](en.wikipedia.org/wiki/Web_colors#Hex_triplet) to a Linear RGB (Supports: "#RRGGBB" or "RRGGBB")
-* bpybb.color.hex_color_to_rgba(hex_color, alpha=1.0) - Converting from a color in the form of a hex triplet string to a Linear RGB (Supports: "#RRGGBB" or "RRGGBB") with an Alpha value
-
-## Add-on Utilities
-
-* bpybb.addon.enable_addon(addon_module_name) - enables a given addon; Checkout this video explanation with example ["How to enable add-ons with Python in Blender (with examples)"](https://youtu.be/HnrInoBWT6Q)
-* bpybb.addon.enable_animation_animall() - enable [Animall addon](https://docs.blender.org/manual/en/dev/addons/animation/animall.html)
-* bpybb.addon.enable_ant_landscape() - enable [ANT Landscape addon](https://docs.blender.org/manual/en/3.0/addons/add_mesh/ant_landscape.html)
-* bpybb.addon.enable_extra_curves() - enable [Add Curve Extra Objects addon](https://docs.blender.org/manual/en/3.0/addons/add_curve/extra_objects.html)
-* bpybb.addon.enable_extra_meshes() - enable [Add Mesh Extra Objects addon](https://docs.blender.org/manual/en/3.0/addons/add_mesh/mesh_extra_objects.html)
-* bpybb.addon.enable_import_images_as_planes() - enable [Images as Planes addon](https://docs.blender.org/manual/en/3.0/addons/import_export/images_as_planes.html)
-* bpybb.addon.enable_mod_tools() - enable [Modifier Tools addon](https://docs.blender.org/manual/en/3.0/addons/add_mesh/ant_landscape.html)
-* bpybb.addon.enable_pointcache_pc2() - enable [Pointcache (pc2) addon](https://docs.blender.org/manual/en/3.0/addons/import_export/pc2.html)
-
-## Collection Utilities
-
-* bpybb.collection.create_collection(col_name) - creates a [Blender Scene Collection](https://docs.blender.org/manual/en/latest/scene_layout/collections/collections.html)
-
-## HDRI Utilities
-
-* bpybb.hdri.apply_hdri(path_to_image, bg_color, hdri_light_strength, bg_strength) - creates a HDRI setup based on a technique from a [FlippedNormals tutorial](https://www.youtube.com/watch?v=dbAWTNCJVEs)
-
-## Material Utilities
-
-* bpybb.material.apply_material(material) - apply a material to the currently active object.
-* bpybb.material.make_color_ramp_from_color_list(colors, color_ramp_node) - creates new sliders on a Color Ramp Node and applies the list of colors on each slider
-
-## Mesh Utilities
-
-* bpybb.mesh.get_vert_coordinates_list(obj) - get a list of vertex coordinates for a given object
-* bpybb.mesh.subdivide() - subdivide the current active object
-
-## Random Utilities
-
-* bpybb.random.time_seed() - Sets the random seed based on the time and copies the seed into the clipboard
-* bpybb.random.get_random_rotation() - Returns a random Euler rotation on X, Y, Z
-
-## Object Utilities
-
-* bpybb.object.add_empty(name=None) - Add an Empty object into the scene
-* bpybb.object.apply_location() - Applies the location of the current object
-* bpybb.object.track_empty(obj) - Adds an Empty object and adds a To Track Constraint on the passed in object to track the Empty
-* bpybb.object.add_bezier_circle(radius: float = 1.0, bevel_depth: float = 0.0, resolution_u: int = 12, extrude: float = 0.0) - Adds a Bezier circle curve into the scene.
-* bpybb.object.add_round_cube(radius: float = 1.0) - Adds a Round Cube into the scene.
-* bpybb.object.add_subdivided_round_cube(radius: float = 1.0) - Adds a Round Cube into the scene and applies a Subdivision modifier.
-
-## Animation Utilities
-
-* bpybb.animate.set_fcurve_extrapolation_to_linear(obj=None) - loops over all the fcurves of an action and sets the extrapolation to "LINEAR"
-* bpybb.animate.set_fcurve_interpolation_to_linear(obj=None) - loops over all the fcurve key frame points of an action and sets the interpolation to "LINEAR"
-* bpybb.animate.animate_360_rotation(axis_index, last_frame, obj=None, clockwise=False, linear=True, start_frame=1) - animates the 360 rotation of an object about the given axis
-* bpybb.animate.animate_rotation(angle, axis_index, last_frame, obj=None, clockwise=False, linear=True, start_frame=1) - animates the rotation of an object about the given axis
-* bpybb.animate.create_data_animation_loop(obj, data_path, start_value, mid_value, start_frame, loop_length, linear_extrapolation=True) - make a data property loop
-* bpybb.animate.animate_up_n_down_bob(start_value: mathutils.Vector, mid_value: mathutils.Vector, obj: bpy_types.Object = None, loop_length: int = 90, start_frame: int = random.randint(0, 60)) - animate the up and down bobbing motion of an object
-* bpybb.animate.add_fcruve_cycles_modifier(obj: bpy_types.Object = None) - Apply a cycles modifier to all the fcurve animation data of an object.
-
-## Modifier Utilities
-
-* bpybb.modifier.add_displace_modifier(name: str, texture_type: str, empty_obj: bpy_types.Object = None) - Add a displace modifier and a texture to the currently active object.
-
-## Output Utilities
-
-* bpybb.output.set_1080p_render_res() - Set the resolution of the rendered image to 1080p
-* bpybb.output.set_1080px_square_render_res() - Set the resolution of the rendered image to 1080 by 1080 pixels
-* bpybb.output.set_1440px_square_render_res() - Set the resolution of the rendered image to 1440 by 1440 pixels
-* bpybb.output.set_2048px_square_render_res() - Set the resolution of the rendered image to 2048 by 2048 pixels
-* bpybb.output.set_2k_render_res() - Set the resolution of the rendered image to 2K
-* bpybb.output.set_4096px_square_render_res() - Set the resolution of the rendered image to 4096 by 4096 pixels
-* bpybb.output.set_4k_render_res() - Set the resolution of the rendered image to 4K
-* bpybb.output.set_720px_square_render_res() - Set the resolution of the rendered image to 720 by 720 pixels
-* bpybb.output.set_instagram_portrait_render_res() - Set the resolution of the rendered image to 1080x1350
-* bpybb.output.set_instagram_square_render_res() - Set the resolution of the rendered image to 1080x1080
-* bpybb.output.set_square_render_res(pixels) - Set the resolution of the rendered image to a square
-* bpybb.output.set_twitter_landscape_render_res() - Set the resolution of the rendered image to 1280x720 from Twitter's Media Best Practices ref: https://developer.twitter.com/en/docs/twitter-api/v1/media/upload-media/uploading-media/media-best-practices
-* bpybb.output.set_twitter_square_render_res() - Set the resolution of the rendered image to 720x720 from Twitter's Media Best Practices ref: https://developer.twitter.com/en/docs/twitter-api/v1/media/upload-media/uploading-media/media-best-practices
-* bpybb.output.set_wqhd_render_res() - Set the resolution of the rendered image to 2560x1440 (QHD)
+Metadata-Version: 2.1
+Name: bpy_building_blocks
+Version: 0.0.24
+Summary: A collection of helper functions and code used for speeding up Blender 3D Python script development.
+Home-page: https://github.com/CGArtPython/bpy_building_blocks
+Author: Viktor Stepanov
+Author-email: cgartpython@gmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Summary
+
+A collection of helper functions and code used for speeding up Blender 3D Python script development.
+
+Checkout project examples [YouTube: Art with a Python script](https://www.youtube.com/watch?v=rIhXHSdMWmc&list=PLB8-FQgROBmm-2f6Vyos6rbnjZeEScrX1)
+
+Important: This package assumes you are using [Blender's](https://www.blender.org/) embedded Python interpreter. 
+
+# Installation
+
+## Installation Walkthrough Video 
+
+[YouTube: How to install the bpy Building Blocks Python package](https://www.youtube.com/watch?v=_irmuKXjhS0)
+
+## From the command line via pip (into Blender's embedded Python interpreter)
+
+---
+
+### on Windows
+
+**Important:**
+Make sure the `site-packages` folder of Blender's embedded Python interpreter is `writable`.
+_See video ^ if you are not sure how to do that_
+If you won't do this the package will be installed into another folder outside of Blender's embedded Python interpreter.
+And you will see this warning: `Defaulting to user installation because normal site-packages is not writeable`
+
+Run the pip install:
+* `Blender <VERSION>/<VERSION>/python/bin/python.exe -m pip install bpy-building-blocks`
+
+Example:
+* `> cd C:\Program Files\Blender Foundation\Blender 3.2\3.2\python\bin `
+* `> .\python.exe -m pip install bpy-building-blocks`
+
+---
+
+### on macOS
+
+**Important:**
+Make sure pip is available.
+
+Run `ensurepip`
+* `/Applications/Blender.app/Contents/Resources/<VERSION>/python/bin/python -m ensurepip`
+
+Run the pip install:
+* `/Applications/Blender.app/Contents/Resources/<VERSION>/python/bin/python -m pip install bpy-building-blocks`
+
+---
+
+### on Linux
+
+**Important:**
+Make sure pip is available.
+
+Run `ensurepip`
+* `~/<INSTALL LOCATION OF BLENDER>/<VERSION>/python/bin/python -m ensurepip`
+
+Run the pip install:
+* `~/<INSTALL LOCATION OF BLENDER>/<VERSION>/python/bin/python -m pip install bpy-building-blocks`
+
+---
+
+## Via Blender Add-on
+
+[bpy_building_blocks_addon on github](https://github.com/CGArtPython/bpy_building_blocks_addon/releases)
+
+See video for details [YouTube: How to install the bpy Building Blocks Python package](https://www.youtube.com/watch?v=_irmuKXjhS0)
+
+# Package Contents
+
+## Utilities
+
+* bpybb.utils.active_object() - Get a references to the currently active object 
+* bpybb.utils.clean_scene() - Removing all of the objects, collection, materials, particles, textures, images, curves, meshes, actions, nodes, and worlds from the scene; Checkout this video explanation with example ["How to clean the scene with Python in Blender (with examples)"](https://youtu.be/3rNqVPtbhzc)
+* bpybb.utils.purge_orphans() - Remove all orphan data blocks; see this from more info: https://youtu.be/3rNqVPtbhzc?t=149
+* bpybb.utils.edit_mode() - A context manager to get into and out of edit mode
+* bpybb.utils.make_active(obj) - Make the passed in object active
+* bpybb.utils.parent(child_obj, parent_obj, keep_transform=False) - Parent one object to another
+* bpybb.utils.duplicate_object(obj=None, linked=False)
+* bpybb.utils.render_animation() - Renders the animation in the currently active scene
+* bpybb.utils.render_image(write_still=False) - Renders the currently active scene
+* bpybb.utils.remove_libraries() - Remove libraries that were linked into the Blend file
+* bpybb.utils.deselect_all_objects() - Similar to bpy.ops.object.select_all(action="DESELECT")
+
+## Color Utilities
+
+* bpybb.color.convert_srgb_to_linear_rgb(srgb_color_component) - Converting from sRGB to Linear RGB based on [sRGB to CIE XYZ](https://en.wikipedia.org/wiki/SRGB#From_sRGB_to_CIE_XYZ)
+* bpybb.color.hex_color_to_rgb(hex_color) - Converting from a color in the form of a [hex triplet string](en.wikipedia.org/wiki/Web_colors#Hex_triplet) to a Linear RGB (Supports: "#RRGGBB" or "RRGGBB")
+* bpybb.color.hex_color_to_rgba(hex_color, alpha=1.0) - Converting from a color in the form of a hex triplet string to a Linear RGB (Supports: "#RRGGBB" or "RRGGBB") with an Alpha value
+
+## Add-on Utilities
+
+* bpybb.addon.enable_addon(addon_module_name) - enables a given addon; Checkout this video explanation with example ["How to enable add-ons with Python in Blender (with examples)"](https://youtu.be/HnrInoBWT6Q)
+* bpybb.addon.enable_animation_animall() - enable [Animall addon](https://docs.blender.org/manual/en/dev/addons/animation/animall.html)
+* bpybb.addon.enable_ant_landscape() - enable [ANT Landscape addon](https://docs.blender.org/manual/en/3.0/addons/add_mesh/ant_landscape.html)
+* bpybb.addon.enable_extra_curves() - enable [Add Curve Extra Objects addon](https://docs.blender.org/manual/en/3.0/addons/add_curve/extra_objects.html)
+* bpybb.addon.enable_extra_meshes() - enable [Add Mesh Extra Objects addon](https://docs.blender.org/manual/en/3.0/addons/add_mesh/mesh_extra_objects.html)
+* bpybb.addon.enable_import_images_as_planes() - enable [Images as Planes addon](https://docs.blender.org/manual/en/3.0/addons/import_export/images_as_planes.html)
+* bpybb.addon.enable_mod_tools() - enable [Modifier Tools addon](https://docs.blender.org/manual/en/3.0/addons/add_mesh/ant_landscape.html)
+* bpybb.addon.enable_pointcache_pc2() - enable [Pointcache (pc2) addon](https://docs.blender.org/manual/en/3.0/addons/import_export/pc2.html)
+
+## Collection Utilities
+
+* bpybb.collection.create_collection(col_name) - creates a [Blender Scene Collection](https://docs.blender.org/manual/en/latest/scene_layout/collections/collections.html)
+* bpybb.collection.create_collection(collection_name: str, location: mathutils.Vector, rotation_euler: Optional[mathutils.Euler] = None, base_collection: Optional[bpy_types.Collection] = None) -> bpy_types.Object - creates an instance of a collection
+
+## HDRI Utilities
+
+* bpybb.hdri.apply_hdri(path_to_image, bg_color, hdri_light_strength, bg_strength) - creates a HDRI setup based on a technique from a [FlippedNormals tutorial](https://www.youtube.com/watch?v=dbAWTNCJVEs)
+
+## Material Utilities
+
+* bpybb.material.apply_material(material) - apply a material to the currently active object.
+* bpybb.material.make_color_ramp_from_color_list(colors, color_ramp_node) - creates new sliders on a Color Ramp Node and applies the list of colors on each slider
+
+## Mesh Utilities
+
+* bpybb.mesh.get_vert_coordinates_list(obj) - get a list of vertex coordinates for a given object
+* bpybb.mesh.subdivide() - subdivide the current active object
+
+## Random Utilities
+
+* bpybb.random.time_seed() - Sets the random seed based on the time and copies the seed into the clipboard
+* bpybb.random.get_random_rotation() - Returns a random Euler rotation on X, Y, Z
+
+## Object Utilities
+
+* bpybb.object.add_empty(name=None) - Add an Empty object into the scene
+* bpybb.object.apply_location() - Applies the location of the current object
+* bpybb.object.rotate_object(axis: int, degrees: float) - Rotate the active object about a given axis
+* bpybb.object.track_empty(obj) - Adds an Empty object and adds a To Track Constraint on the passed in object to track the Empty
+* bpybb.object.add_bezier_circle(radius: float = 1.0, bevel_depth: float = 0.0, resolution_u: int = 12, extrude: float = 0.0) - Adds a Bezier circle curve into the scene.
+* bpybb.object.add_round_cube(radius: float = 1.0) - Adds a Round Cube into the scene.
+* bpybb.object.add_subdivided_round_cube(radius: float = 1.0) - Adds a Round Cube into the scene and applies a Subdivision modifier.
+* join_objects(objects: list[bpy_types.Object]) -> bpy_types.Object - Joins the provided objects into one object
+
+## Animation Utilities
+
+* bpybb.animate.set_fcurve_extrapolation_to_linear(obj=None) - loops over all the fcurves of an action and sets the extrapolation to "LINEAR"
+* bpybb.animate.set_fcurve_interpolation_to_linear(obj=None) - loops over all the fcurve key frame points of an action and sets the interpolation to "LINEAR"
+* bpybb.animate.animate_360_rotation(axis_index, last_frame, obj=None, clockwise=False, linear=True, start_frame=1) - animates the 360 rotation of an object about the given axis
+* bpybb.animate.animate_rotation(angle, axis_index, last_frame, obj=None, clockwise=False, linear=True, start_frame=1) - animates the rotation of an object about the given axis
+* bpybb.animate.create_data_animation_loop(obj, data_path, start_value, mid_value, start_frame, loop_length, linear_extrapolation=True) - make a data property loop
+* bpybb.animate.animate_up_n_down_bob(start_value: mathutils.Vector, mid_value: mathutils.Vector, obj: bpy_types.Object = None, loop_length: int = 90, start_frame: int = random.randint(0, 60)) - animate the up and down bobbing motion of an object
+* bpybb.animate.add_fcruve_cycles_modifier(obj: bpy_types.Object = None) - Apply a cycles modifier to all the fcurve animation data of an object.
+
+## Modifier Utilities
+
+* bpybb.modifier.add_displace_modifier(name: str, texture_type: str, empty_obj: bpy_types.Object = None) - Add a displace modifier and a texture to the currently active object.
+
+## Output Utilities
+
+* bpybb.output.set_1080p_render_res() - Set the resolution of the rendered image to 1080p
+* bpybb.output.set_1080px_square_render_res() - Set the resolution of the rendered image to 1080 by 1080 pixels
+* bpybb.output.set_1440px_square_render_res() - Set the resolution of the rendered image to 1440 by 1440 pixels
+* bpybb.output.set_2048px_square_render_res() - Set the resolution of the rendered image to 2048 by 2048 pixels
+* bpybb.output.set_2k_render_res() - Set the resolution of the rendered image to 2K
+* bpybb.output.set_4096px_square_render_res() - Set the resolution of the rendered image to 4096 by 4096 pixels
+* bpybb.output.set_4k_render_res() - Set the resolution of the rendered image to 4K
+* bpybb.output.set_720px_square_render_res() - Set the resolution of the rendered image to 720 by 720 pixels
+* bpybb.output.set_instagram_portrait_render_res() - Set the resolution of the rendered image to 1080x1350
+* bpybb.output.set_instagram_square_render_res() - Set the resolution of the rendered image to 1080x1080
+* bpybb.output.set_square_render_res(pixels) - Set the resolution of the rendered image to a square
+* bpybb.output.set_twitter_landscape_render_res() - Set the resolution of the rendered image to 1280x720 from Twitter's Media Best Practices ref: https://developer.twitter.com/en/docs/twitter-api/v1/media/upload-media/uploading-media/media-best-practices
+* bpybb.output.set_twitter_square_render_res() - Set the resolution of the rendered image to 720x720 from Twitter's Media Best Practices ref: https://developer.twitter.com/en/docs/twitter-api/v1/media/upload-media/uploading-media/media-best-practices
+* bpybb.output.set_wqhd_render_res() - Set the resolution of the rendered image to 2560x1440 (QHD)
+
+## World Shader Utilities
+
+* bpybb.world_shader.set_up_world_sun_light() - Set up the lighing in a scene using the ShaderNodeTexSky world shader node
```

### Comparing `bpy_building_blocks-0.0.23/src/bpy_building_blocks.egg-info/SOURCES.txt` & `bpy_building_blocks-0.0.24/src/bpy_building_blocks.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 src/bpybb/material.py
 src/bpybb/mesh.py
 src/bpybb/modifier.py
 src/bpybb/object.py
 src/bpybb/output.py
 src/bpybb/random.py
 src/bpybb/utils.py
-src/bpybb/version.py
+src/bpybb/version.py
+src/bpybb/world_shader.py
```

### Comparing `bpy_building_blocks-0.0.23/src/bpybb/addon.py` & `bpy_building_blocks-0.0.24/src/bpybb/addon.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-"""
-This module contains utilities for working with Blender add-ons.
-"""
-
-import addon_utils
-
-
-def enable_addon(addon_module_name):
-    """
-    Checkout this video explanation with example
-
-    "How to enable add-ons with Python in Blender (with examples)"
-    https://youtu.be/HnrInoBWT6Q
-    """
-    loaded_default, loaded_state = addon_utils.check(addon_module_name)
-    if not loaded_state:
-        addon_utils.enable(addon_module_name)
-
-
-def enable_extra_curves():
-    """
-    enable Add Curve Extra Objects addon
-    https://docs.blender.org/manual/en/3.0/addons/add_curve/extra_objects.html
-    """
-    enable_addon(addon_module_name="add_curve_extra_objects")
-
-
-def enable_extra_meshes():
-    """
-    enable Add Mesh Extra Objects addon
-    https://docs.blender.org/manual/en/3.0/addons/add_mesh/mesh_extra_objects.html
-    """
-    enable_addon(addon_module_name="add_mesh_extra_objects")
-
-
-def enable_ant_landscape():
-    """
-    enable ANT Landscape addon
-    https://docs.blender.org/manual/en/3.0/addons/add_mesh/ant_landscape.html
-    """
-    enable_addon(addon_module_name="ant_landscape")
-
-
-def enable_mod_tools():
-    """
-    enable Modifier Tools addon
-    https://docs.blender.org/manual/en/3.0/addons/add_mesh/ant_landscape.html
-    """
-    enable_addon(addon_module_name="space_view3d_modifier_tools")
-
-
-def enable_import_images_as_planes():
-    """
-    enable Images as Planes addon
-    https://docs.blender.org/manual/en/3.0/addons/import_export/images_as_planes.html
-    """
-    enable_addon(addon_module_name="io_import_images_as_planes")
-
-
-def enable_pointcache_pc2():
-    """
-    enable Pointcache (pc2) addon
-    https://docs.blender.org/manual/en/3.0/addons/import_export/pc2.html
-    """
-    enable_addon(addon_module_name="io_export_pc2")
-
-
-def enable_animation_animall():
-    """
-    enable Animall addon
-    https://docs.blender.org/manual/en/dev/addons/animation/animall.html
-    """
-    enable_addon(addon_module_name="animation_animall")
+"""
+This module contains utilities for working with Blender add-ons.
+"""
+
+import addon_utils
+
+
+def enable_addon(addon_module_name):
+    """
+    Checkout this video explanation with example
+
+    "How to enable add-ons with Python in Blender (with examples)"
+    https://youtu.be/HnrInoBWT6Q
+    """
+    loaded_default, loaded_state = addon_utils.check(addon_module_name)
+    if not loaded_state:
+        addon_utils.enable(addon_module_name)
+
+
+def enable_extra_curves():
+    """
+    enable Add Curve Extra Objects addon
+    https://docs.blender.org/manual/en/3.0/addons/add_curve/extra_objects.html
+    """
+    enable_addon(addon_module_name="add_curve_extra_objects")
+
+
+def enable_extra_meshes():
+    """
+    enable Add Mesh Extra Objects addon
+    https://docs.blender.org/manual/en/3.0/addons/add_mesh/mesh_extra_objects.html
+    """
+    enable_addon(addon_module_name="add_mesh_extra_objects")
+
+
+def enable_ant_landscape():
+    """
+    enable ANT Landscape addon
+    https://docs.blender.org/manual/en/3.0/addons/add_mesh/ant_landscape.html
+    """
+    enable_addon(addon_module_name="ant_landscape")
+
+
+def enable_mod_tools():
+    """
+    enable Modifier Tools addon
+    https://docs.blender.org/manual/en/3.0/addons/add_mesh/ant_landscape.html
+    """
+    enable_addon(addon_module_name="space_view3d_modifier_tools")
+
+
+def enable_import_images_as_planes():
+    """
+    enable Images as Planes addon
+    https://docs.blender.org/manual/en/3.0/addons/import_export/images_as_planes.html
+    """
+    enable_addon(addon_module_name="io_import_images_as_planes")
+
+
+def enable_pointcache_pc2():
+    """
+    enable Pointcache (pc2) addon
+    https://docs.blender.org/manual/en/3.0/addons/import_export/pc2.html
+    """
+    enable_addon(addon_module_name="io_export_pc2")
+
+
+def enable_animation_animall():
+    """
+    enable Animall addon
+    https://docs.blender.org/manual/en/dev/addons/animation/animall.html
+    """
+    enable_addon(addon_module_name="animation_animall")
```

### Comparing `bpy_building_blocks-0.0.23/src/bpybb/animate.py` & `bpy_building_blocks-0.0.24/src/bpybb/animate.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-"""
-This module contains utilities for speeding up animation creation.
-"""
-
-import math
-import random
-
-import bpy_types
-import mathutils
-
-from bpybb.utils import active_object
-
-
-def set_fcurve_extrapolation_to_linear(obj: bpy_types.Object = None) -> None:
-    """
-    Loops over all the fcurves of an action
-    and sets the extrapolation to "LINEAR".
-    """
-    if obj is None:
-        obj = active_object()
-
-    for fcurve in obj.animation_data.action.fcurves:
-        fcurve.extrapolation = "LINEAR"
-
-
-def set_fcurve_interpolation_to_linear(obj: bpy_types.Object = None) -> None:
-    """
-    Loops over all the fcurve key frame points of an action
-    and sets the interpolation to "LINEAR".
-    """
-    if obj is None:
-        obj = active_object()
-
-    for fcurve in obj.animation_data.action.fcurves:
-        for keyframe_point in fcurve.keyframe_points:
-            keyframe_point.interpolation = "LINEAR"
-
-
-def add_fcruve_cycles_modifier(obj: bpy_types.Object = None) -> None:
-    """
-    Apply a cycles modifier to all the fcurve animation data of an object.
-    """
-    if obj is None:
-        obj = active_object()
-
-    for fcurve in obj.animation_data.action.fcurves.values():
-        modifier = fcurve.modifiers.new(type="CYCLES")
-        modifier.mode_before = "REPEAT"
-        modifier.mode_after = "REPEAT"
-
-
-def animate_360_rotation(axis_index, last_frame, obj=None, clockwise=False, linear=True, start_frame=1):
-    animate_rotation(360, axis_index, last_frame, obj, clockwise, linear, start_frame)
-
-
-def animate_rotation(angle, axis_index, last_frame, obj=None, clockwise=False, linear=True, start_frame=1):
-    if not obj:
-        obj = active_object()
-    frame = start_frame
-    obj.keyframe_insert("rotation_euler", index=axis_index, frame=frame)
-
-    if clockwise:
-        angle_offset = -angle
-    else:
-        angle_offset = angle
-    frame = last_frame
-    obj.rotation_euler[axis_index] = math.radians(angle_offset) + obj.rotation_euler[axis_index]
-    obj.keyframe_insert("rotation_euler", index=axis_index, frame=frame)
-
-    if linear:
-        set_fcurve_extrapolation_to_linear()
-
-
-def create_data_animation_loop(obj, data_path, start_value, mid_value, start_frame, loop_length, linear_extrapolation=True):
-    """
-    To make a data property loop we need to:
-    1. set the property to an initial value and add a keyframe in the beginning of the loop
-    2. set the property to a middle value and add a keyframe in the middle of the loop
-    3. set the property the initial value and add a keyframe at the end of the loop
-    """
-
-    # set the start value
-    setattr(obj, data_path, start_value)
-    # add a keyframe at the start
-    obj.keyframe_insert(data_path, frame=start_frame)
-
-    # set the middle value
-    setattr(obj, data_path, mid_value)
-    # add a keyframe in the middle
-    mid_frame = start_frame + (loop_length) / 2
-    obj.keyframe_insert(data_path, frame=mid_frame)
-
-    # set the end value
-    setattr(obj, data_path, start_value)
-    # add a keyframe in the end
-    end_frame = start_frame + loop_length
-    obj.keyframe_insert(data_path, frame=end_frame)
-
-    if linear_extrapolation:
-        set_fcurve_extrapolation_to_linear()
-
-
-def animate_up_n_down_bob(
-    start_value: mathutils.Vector, mid_value: mathutils.Vector, obj: bpy_types.Object = None, loop_length: int = 90, start_frame: int = random.randint(0, 60)
-) -> None:
-    """Animate the up and down bobbing motion of an object. Apply a fcurve cycles modifier to make it seamless."""
-    if obj is None:
-        obj = active_object()
-
-    create_data_animation_loop(
-        obj,
-        "location",
-        start_value=start_value,
-        mid_value=mid_value,
-        start_frame=start_frame,
-        loop_length=loop_length,
-        linear_extrapolation=False,
-    )
-
-    add_fcruve_cycles_modifier(obj)
+"""
+This module contains utilities for speeding up animation creation.
+"""
+
+import math
+import random
+
+import bpy_types
+import mathutils
+
+from bpybb.utils import active_object
+
+
+def set_fcurve_extrapolation_to_linear(obj: bpy_types.Object = None) -> None:
+    """
+    Loops over all the fcurves of an action
+    and sets the extrapolation to "LINEAR".
+    """
+    if obj is None:
+        obj = active_object()
+
+    for fcurve in obj.animation_data.action.fcurves:
+        fcurve.extrapolation = "LINEAR"
+
+
+def set_fcurve_interpolation_to_linear(obj: bpy_types.Object = None) -> None:
+    """
+    Loops over all the fcurve key frame points of an action
+    and sets the interpolation to "LINEAR".
+    """
+    if obj is None:
+        obj = active_object()
+
+    for fcurve in obj.animation_data.action.fcurves:
+        for keyframe_point in fcurve.keyframe_points:
+            keyframe_point.interpolation = "LINEAR"
+
+
+def add_fcruve_cycles_modifier(obj: bpy_types.Object = None) -> None:
+    """
+    Apply a cycles modifier to all the fcurve animation data of an object.
+    """
+    if obj is None:
+        obj = active_object()
+
+    for fcurve in obj.animation_data.action.fcurves.values():
+        modifier = fcurve.modifiers.new(type="CYCLES")
+        modifier.mode_before = "REPEAT"
+        modifier.mode_after = "REPEAT"
+
+
+def animate_360_rotation(axis_index, last_frame, obj=None, clockwise=False, linear=True, start_frame=1):
+    animate_rotation(360, axis_index, last_frame, obj, clockwise, linear, start_frame)
+
+
+def animate_rotation(angle, axis_index, last_frame, obj=None, clockwise=False, linear=True, start_frame=1):
+    if not obj:
+        obj = active_object()
+    frame = start_frame
+    obj.keyframe_insert("rotation_euler", index=axis_index, frame=frame)
+
+    if clockwise:
+        angle_offset = -angle
+    else:
+        angle_offset = angle
+    frame = last_frame
+    obj.rotation_euler[axis_index] = math.radians(angle_offset) + obj.rotation_euler[axis_index]
+    obj.keyframe_insert("rotation_euler", index=axis_index, frame=frame)
+
+    if linear:
+        set_fcurve_extrapolation_to_linear()
+
+
+def create_data_animation_loop(obj, data_path, start_value, mid_value, start_frame, loop_length, linear_extrapolation=True):
+    """
+    To make a data property loop we need to:
+    1. set the property to an initial value and add a keyframe in the beginning of the loop
+    2. set the property to a middle value and add a keyframe in the middle of the loop
+    3. set the property the initial value and add a keyframe at the end of the loop
+    """
+
+    # set the start value
+    setattr(obj, data_path, start_value)
+    # add a keyframe at the start
+    obj.keyframe_insert(data_path, frame=start_frame)
+
+    # set the middle value
+    setattr(obj, data_path, mid_value)
+    # add a keyframe in the middle
+    mid_frame = start_frame + (loop_length) / 2
+    obj.keyframe_insert(data_path, frame=mid_frame)
+
+    # set the end value
+    setattr(obj, data_path, start_value)
+    # add a keyframe in the end
+    end_frame = start_frame + loop_length
+    obj.keyframe_insert(data_path, frame=end_frame)
+
+    if linear_extrapolation:
+        set_fcurve_extrapolation_to_linear()
+
+
+def animate_up_n_down_bob(
+    start_value: mathutils.Vector, mid_value: mathutils.Vector, obj: bpy_types.Object = None, loop_length: int = 90, start_frame: int = random.randint(0, 60)
+) -> None:
+    """Animate the up and down bobbing motion of an object. Apply a fcurve cycles modifier to make it seamless."""
+    if obj is None:
+        obj = active_object()
+
+    create_data_animation_loop(
+        obj,
+        "location",
+        start_value=start_value,
+        mid_value=mid_value,
+        start_frame=start_frame,
+        loop_length=loop_length,
+        linear_extrapolation=False,
+    )
+
+    add_fcruve_cycles_modifier(obj)
```

### Comparing `bpy_building_blocks-0.0.23/src/bpybb/color.py` & `bpy_building_blocks-0.0.24/src/bpybb/color.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-"""
-Utility functions for working with color
-"""
-
-from typing import Tuple
-
-import math
-
-
-def hex_color_to_rgb(hex_color: str) -> Tuple[float]:
-    """
-    Converting from a color in the form of a hex triplet string (en.wikipedia.org/wiki/Web_colors#Hex_triplet)
-    to a Linear RGB
-
-    Supports: "#RRGGBB" or "RRGGBB"
-
-    Note: We are converting into Linear RGB since Blender uses a Linear Color Space internally
-    https://docs.blender.org/manual/en/latest/render/color_management.html
-    """
-    # remove the leading '#' symbol if present
-    if hex_color.startswith("#"):
-        hex_color = hex_color[1:]
-
-    assert len(hex_color) == 6, f"RRGGBB is the supported hex color format: {hex_color}"
-
-    # extracting the Red color component - RRxxxx
-    red = int(hex_color[:2], 16)
-    # dividing by 255 to get a number between 0.0 and 1.0
-    srgb_red = red / 255
-    linear_red = convert_srgb_to_linear_rgb(srgb_red)
-
-    # extracting the Green color component - xxGGxx
-    green = int(hex_color[2:4], 16)
-    # dividing by 255 to get a number between 0.0 and 1.0
-    srgb_green = green / 255
-    linear_green = convert_srgb_to_linear_rgb(srgb_green)
-
-    # extracting the Blue color component - xxxxBB
-    blue = int(hex_color[4:6], 16)
-    # dividing by 255 to get a number between 0.0 and 1.0
-    srgb_blue = blue / 255
-    linear_blue = convert_srgb_to_linear_rgb(srgb_blue)
-
-    return tuple([linear_red, linear_green, linear_blue])
-
-
-def hex_color_to_rgba(hex_color: str, alpha: float = 1.0) -> Tuple[float]:
-    """
-    Converting from a color in the form of a hex triplet string (en.wikipedia.org/wiki/Web_colors#Hex_triplet)
-    to a Linear RGB with an Alpha passed as a parameter
-
-    Supports: "#RRGGBB" or "RRGGBB"
-    """
-    linear_red, linear_green, linear_blue = hex_color_to_rgb(hex_color)
-    return tuple([linear_red, linear_green, linear_blue, alpha])
-
-
-def convert_srgb_to_linear_rgb(srgb_color_component: float) -> float:
-    """
-    Converting from sRGB to Linear RGB
-    based on https://en.wikipedia.org/wiki/SRGB#From_sRGB_to_CIE_XYZ
-    """
-    if srgb_color_component <= 0.04045:
-        linear_color_component = srgb_color_component / 12.92
-    else:
-        linear_color_component = math.pow((srgb_color_component + 0.055) / 1.055, 2.4)
-
-    return linear_color_component
+"""
+Utility functions for working with color
+"""
+
+from typing import Tuple
+
+import math
+
+
+def hex_color_to_rgb(hex_color: str) -> Tuple[float]:
+    """
+    Converting from a color in the form of a hex triplet string (en.wikipedia.org/wiki/Web_colors#Hex_triplet)
+    to a Linear RGB
+
+    Supports: "#RRGGBB" or "RRGGBB"
+
+    Note: We are converting into Linear RGB since Blender uses a Linear Color Space internally
+    https://docs.blender.org/manual/en/latest/render/color_management.html
+    """
+    # remove the leading '#' symbol if present
+    if hex_color.startswith("#"):
+        hex_color = hex_color[1:]
+
+    assert len(hex_color) == 6, f"RRGGBB is the supported hex color format: {hex_color}"
+
+    # extracting the Red color component - RRxxxx
+    red = int(hex_color[:2], 16)
+    # dividing by 255 to get a number between 0.0 and 1.0
+    srgb_red = red / 255
+    linear_red = convert_srgb_to_linear_rgb(srgb_red)
+
+    # extracting the Green color component - xxGGxx
+    green = int(hex_color[2:4], 16)
+    # dividing by 255 to get a number between 0.0 and 1.0
+    srgb_green = green / 255
+    linear_green = convert_srgb_to_linear_rgb(srgb_green)
+
+    # extracting the Blue color component - xxxxBB
+    blue = int(hex_color[4:6], 16)
+    # dividing by 255 to get a number between 0.0 and 1.0
+    srgb_blue = blue / 255
+    linear_blue = convert_srgb_to_linear_rgb(srgb_blue)
+
+    return tuple([linear_red, linear_green, linear_blue])
+
+
+def hex_color_to_rgba(hex_color: str, alpha: float = 1.0) -> Tuple[float]:
+    """
+    Converting from a color in the form of a hex triplet string (en.wikipedia.org/wiki/Web_colors#Hex_triplet)
+    to a Linear RGB with an Alpha passed as a parameter
+
+    Supports: "#RRGGBB" or "RRGGBB"
+    """
+    linear_red, linear_green, linear_blue = hex_color_to_rgb(hex_color)
+    return tuple([linear_red, linear_green, linear_blue, alpha])
+
+
+def convert_srgb_to_linear_rgb(srgb_color_component: float) -> float:
+    """
+    Converting from sRGB to Linear RGB
+    based on https://en.wikipedia.org/wiki/SRGB#From_sRGB_to_CIE_XYZ
+    """
+    if srgb_color_component <= 0.04045:
+        linear_color_component = srgb_color_component / 12.92
+    else:
+        linear_color_component = math.pow((srgb_color_component + 0.055) / 1.055, 2.4)
+
+    return linear_color_component
```

### Comparing `bpy_building_blocks-0.0.23/src/bpybb/hdri.py` & `bpy_building_blocks-0.0.24/src/bpybb/hdri.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-"""
-This module contains utilities for working with HDRIs.
-"""
-
-import bpy
-
-
-def apply_hdri(path_to_image, bg_color, hdri_light_strength, bg_strength):
-    """
-    Based on a technique from a FlippedNormals tutorial
-    https://www.youtube.com/watch?v=dbAWTNCJVEs
-    """
-    world_node_tree = bpy.context.scene.world.node_tree
-
-    nodes_to_remove = []
-    for node in world_node_tree.nodes:
-        nodes_to_remove.append(node)
-
-    for node in nodes_to_remove:
-        world_node_tree.nodes.remove(node)
-
-    location_x = 0
-    texture_coordinate_node = world_node_tree.nodes.new(type="ShaderNodeTexCoord")
-    texture_coordinate_node.name = "Texture Coordinate"
-    texture_coordinate_node.location.x = location_x
-    location_x += 200
-
-    mapping_node = world_node_tree.nodes.new(type="ShaderNodeMapping")
-    mapping_node.location.x = location_x
-    location_x += 200
-    mapping_node.name = "Mapping"
-
-    environment_texture_node = world_node_tree.nodes.new(type="ShaderNodeTexEnvironment")
-    environment_texture_node.location.x = location_x
-    location_x += 300
-    environment_texture_node.name = "Environment Texture"
-    environment_texture_node.image = bpy.data.images.load(path_to_image)
-
-    background_node = world_node_tree.nodes.new(type="ShaderNodeBackground")
-    background_node.location.x = location_x
-    background_node.name = "Background"
-    background_node.inputs["Strength"].default_value = hdri_light_strength
-
-    background_node_2 = world_node_tree.nodes.new(type="ShaderNodeBackground")
-    background_node_2.location.x = location_x
-    background_node_2.location.y = -100
-    background_node_2.name = "Background.001"
-    background_node_2.inputs["Color"].default_value = bg_color
-    background_node_2.inputs["Strength"].default_value = bg_strength
-
-    light_path_node = world_node_tree.nodes.new(type="ShaderNodeLightPath")
-    light_path_node.location.x = location_x
-    light_path_node.location.y = 400
-    location_x += 200
-    light_path_node.name = "Light Path"
-
-    mix_shader_node = world_node_tree.nodes.new(type="ShaderNodeMixShader")
-    mix_shader_node.location.x = location_x
-    location_x += 200
-    mix_shader_node.name = "Mix Shader"
-
-    world_output_node = world_node_tree.nodes.new(type="ShaderNodeOutputWorld")
-    world_output_node.location.x = location_x
-    location_x += 200
-
-    # links begin
-    from_node = background_node
-    to_node = mix_shader_node
-    world_node_tree.links.new(from_node.outputs["Background"], to_node.inputs["Shader"])
-
-    from_node = mapping_node
-    to_node = environment_texture_node
-    world_node_tree.links.new(from_node.outputs["Vector"], to_node.inputs["Vector"])
-
-    from_node = texture_coordinate_node
-    to_node = mapping_node
-    world_node_tree.links.new(from_node.outputs["Generated"], to_node.inputs["Vector"])
-
-    from_node = environment_texture_node
-    to_node = background_node
-    world_node_tree.links.new(from_node.outputs["Color"], to_node.inputs["Color"])
-
-    from_node = background_node_2
-    to_node = mix_shader_node
-    world_node_tree.links.new(from_node.outputs["Background"], to_node.inputs[2])
-
-    from_node = light_path_node
-    to_node = mix_shader_node
-    world_node_tree.links.new(from_node.outputs["Is Camera Ray"], to_node.inputs["Fac"])
-
-    from_node = mix_shader_node
-    to_node = world_output_node
-    world_node_tree.links.new(from_node.outputs["Shader"], to_node.inputs["Surface"])
-    # links end
-
-    return world_node_tree
+"""
+This module contains utilities for working with HDRIs.
+"""
+
+import bpy
+
+
+def apply_hdri(path_to_image, bg_color, hdri_light_strength, bg_strength):
+    """
+    Based on a technique from a FlippedNormals tutorial
+    https://www.youtube.com/watch?v=dbAWTNCJVEs
+    """
+    world_node_tree = bpy.context.scene.world.node_tree
+
+    nodes_to_remove = []
+    for node in world_node_tree.nodes:
+        nodes_to_remove.append(node)
+
+    for node in nodes_to_remove:
+        world_node_tree.nodes.remove(node)
+
+    location_x = 0
+    texture_coordinate_node = world_node_tree.nodes.new(type="ShaderNodeTexCoord")
+    texture_coordinate_node.name = "Texture Coordinate"
+    texture_coordinate_node.location.x = location_x
+    location_x += 200
+
+    mapping_node = world_node_tree.nodes.new(type="ShaderNodeMapping")
+    mapping_node.location.x = location_x
+    location_x += 200
+    mapping_node.name = "Mapping"
+
+    environment_texture_node = world_node_tree.nodes.new(type="ShaderNodeTexEnvironment")
+    environment_texture_node.location.x = location_x
+    location_x += 300
+    environment_texture_node.name = "Environment Texture"
+    environment_texture_node.image = bpy.data.images.load(path_to_image)
+
+    background_node = world_node_tree.nodes.new(type="ShaderNodeBackground")
+    background_node.location.x = location_x
+    background_node.name = "Background"
+    background_node.inputs["Strength"].default_value = hdri_light_strength
+
+    background_node_2 = world_node_tree.nodes.new(type="ShaderNodeBackground")
+    background_node_2.location.x = location_x
+    background_node_2.location.y = -100
+    background_node_2.name = "Background.001"
+    background_node_2.inputs["Color"].default_value = bg_color
+    background_node_2.inputs["Strength"].default_value = bg_strength
+
+    light_path_node = world_node_tree.nodes.new(type="ShaderNodeLightPath")
+    light_path_node.location.x = location_x
+    light_path_node.location.y = 400
+    location_x += 200
+    light_path_node.name = "Light Path"
+
+    mix_shader_node = world_node_tree.nodes.new(type="ShaderNodeMixShader")
+    mix_shader_node.location.x = location_x
+    location_x += 200
+    mix_shader_node.name = "Mix Shader"
+
+    world_output_node = world_node_tree.nodes.new(type="ShaderNodeOutputWorld")
+    world_output_node.location.x = location_x
+    location_x += 200
+
+    # links begin
+    from_node = background_node
+    to_node = mix_shader_node
+    world_node_tree.links.new(from_node.outputs["Background"], to_node.inputs["Shader"])
+
+    from_node = mapping_node
+    to_node = environment_texture_node
+    world_node_tree.links.new(from_node.outputs["Vector"], to_node.inputs["Vector"])
+
+    from_node = texture_coordinate_node
+    to_node = mapping_node
+    world_node_tree.links.new(from_node.outputs["Generated"], to_node.inputs["Vector"])
+
+    from_node = environment_texture_node
+    to_node = background_node
+    world_node_tree.links.new(from_node.outputs["Color"], to_node.inputs["Color"])
+
+    from_node = background_node_2
+    to_node = mix_shader_node
+    world_node_tree.links.new(from_node.outputs["Background"], to_node.inputs[2])
+
+    from_node = light_path_node
+    to_node = mix_shader_node
+    world_node_tree.links.new(from_node.outputs["Is Camera Ray"], to_node.inputs["Fac"])
+
+    from_node = mix_shader_node
+    to_node = world_output_node
+    world_node_tree.links.new(from_node.outputs["Shader"], to_node.inputs["Surface"])
+    # links end
+
+    return world_node_tree
```

### Comparing `bpy_building_blocks-0.0.23/src/bpybb/object.py` & `bpy_building_blocks-0.0.24/src/bpybb/object.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,86 +1,105 @@
-"""
-This module contains utilities for working with Blender objects.
-"""
-
-import bpy
-
-import bpy_types
-
-from bpybb.utils import active_object, make_active
-from bpybb.addon import enable_extra_meshes
-
-
-def apply_location():
-    bpy.ops.object.transform_apply(location=True)
-
-
-def add_empty(name=None):
-    bpy.ops.object.empty_add(type="PLAIN_AXES")
-    empty_obj = active_object()
-    if name:
-        empty_obj.name = name
-    else:
-        empty_obj.name = "empty.cntrl"
-    return empty_obj
-
-
-def track_empty(obj):
-    empty_target = add_empty(name="empty.tracker-target")
-
-    make_active(obj)
-    bpy.ops.object.constraint_add(type="TRACK_TO")
-    bpy.context.object.constraints["Track To"].target = empty_target
-
-    return empty_target
-
-
-def add_bezier_circle(radius: float = 1.0, bevel_depth: float = 0.0, resolution_u: int = 12, extrude: float = 0.0) -> bpy_types.Object:
-    """Adds a Bezier circle curve into the scene.
-
-    Args:
-        radius (float, optional): the radius of the circle. Defaults to 1.
-        bevel_depth (float, optional): the size of the bevel (the bevel is off if this is 0). Defaults to 0.
-        resolution_u (int, optional): the number of computed points between two control points. Defaults to 12.
-
-    Returns:
-        bpy_types.Object: a reference to the created Bezier circle curve object
-    """
-    bpy.ops.curve.primitive_bezier_circle_add(radius=radius)
-
-    bezier_circle_obj = active_object()
-
-    bezier_circle_obj.data.bevel_depth = bevel_depth
-    bezier_circle_obj.data.resolution_u = resolution_u
-    bezier_circle_obj.data.extrude = extrude
-
-    return bezier_circle_obj
-
-
-def add_round_cube(radius: float = 1.0) -> bpy_types.Object:
-    """Adds a Round Cube into the scene.
-
-    Args:
-        radius (float, optional): the radios of the Round Cube. Defaults to 1.0.
-
-    Returns:
-        bpy_types.Object: a reference to the created Round Cube curve object
-    """
-    enable_extra_meshes()
-    bpy.ops.mesh.primitive_round_cube_add(radius=radius)
-    return active_object()
-
-
-def add_subdivided_round_cube(radius: float = 1.0) -> tuple[bpy_types.Object, bpy.types.SubsurfModifier]:
-    """Adds a Round Cube into the scene and applies a Subdivision modifier.
-
-    Args:
-        radius (float, optional): the radios of the Round Cube. Defaults to 1.0.
-
-    Returns:
-        bpy_types.Object: a reference to the created Round Cube curve object
-    """
-    round_cube_obj = add_round_cube(radius)
-
-    bpy.ops.object.modifier_add(type="SUBSURF")
-
-    return round_cube_obj, round_cube_obj.modifiers["Subdivision"]
+"""
+This module contains utilities for working with Blender objects.
+"""
+
+import math
+
+import bpy
+
+import bpy_types
+
+from bpybb.utils import active_object, make_active, deselect_all_objects
+from bpybb.addon import enable_extra_meshes
+
+
+def join_objects(objects: list[bpy_types.Object]) -> bpy_types.Object:
+    deselect_all_objects()
+
+    for obj in objects:
+        obj.select_set(True)
+
+    bpy.ops.object.join()
+
+    new_obj = active_object()
+
+    return new_obj
+
+
+def rotate_object(axis: int, degrees: float) -> None:
+    bpy.context.active_object.rotation_euler[axis] = math.radians(degrees)
+
+
+def apply_location():
+    bpy.ops.object.transform_apply(location=True)
+
+
+def add_empty(name=None):
+    bpy.ops.object.empty_add(type="PLAIN_AXES")
+    empty_obj = active_object()
+    if name:
+        empty_obj.name = name
+    else:
+        empty_obj.name = "empty.cntrl"
+    return empty_obj
+
+
+def track_empty(obj):
+    empty_target = add_empty(name="empty.tracker-target")
+
+    make_active(obj)
+    bpy.ops.object.constraint_add(type="TRACK_TO")
+    bpy.context.object.constraints["Track To"].target = empty_target
+
+    return empty_target
+
+
+def add_bezier_circle(radius: float = 1.0, bevel_depth: float = 0.0, resolution_u: int = 12, extrude: float = 0.0) -> bpy_types.Object:
+    """Adds a Bezier circle curve into the scene.
+
+    Args:
+        radius (float, optional): the radius of the circle. Defaults to 1.
+        bevel_depth (float, optional): the size of the bevel (the bevel is off if this is 0). Defaults to 0.
+        resolution_u (int, optional): the number of computed points between two control points. Defaults to 12.
+
+    Returns:
+        bpy_types.Object: a reference to the created Bezier circle curve object
+    """
+    bpy.ops.curve.primitive_bezier_circle_add(radius=radius)
+
+    bezier_circle_obj = active_object()
+
+    bezier_circle_obj.data.bevel_depth = bevel_depth
+    bezier_circle_obj.data.resolution_u = resolution_u
+    bezier_circle_obj.data.extrude = extrude
+
+    return bezier_circle_obj
+
+
+def add_round_cube(radius: float = 1.0) -> bpy_types.Object:
+    """Adds a Round Cube into the scene.
+
+    Args:
+        radius (float, optional): the radios of the Round Cube. Defaults to 1.0.
+
+    Returns:
+        bpy_types.Object: a reference to the created Round Cube curve object
+    """
+    enable_extra_meshes()
+    bpy.ops.mesh.primitive_round_cube_add(radius=radius)
+    return active_object()
+
+
+def add_subdivided_round_cube(radius: float = 1.0) -> tuple[bpy_types.Object, bpy.types.SubsurfModifier]:
+    """Adds a Round Cube into the scene and applies a Subdivision modifier.
+
+    Args:
+        radius (float, optional): the radios of the Round Cube. Defaults to 1.0.
+
+    Returns:
+        bpy_types.Object: a reference to the created Round Cube curve object
+    """
+    round_cube_obj = add_round_cube(radius)
+
+    bpy.ops.object.modifier_add(type="SUBSURF")
+
+    return round_cube_obj, round_cube_obj.modifiers["Subdivision"]
```

### Comparing `bpy_building_blocks-0.0.23/src/bpybb/output.py` & `bpy_building_blocks-0.0.24/src/bpybb/output.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-"""
-This module contains utilities for setting up the render resolution.
-"""
-
-import bpy
-
-
-def set_square_render_res(pixels):
-    """
-    Set the resolution of the rendered image to a square
-    """
-    bpy.context.scene.render.resolution_x = pixels
-    bpy.context.scene.render.resolution_y = pixels
-
-
-def set_720px_square_render_res():
-    """
-    Set the resolution of the rendered image to 720 by 720 pixels
-    """
-    set_square_render_res(pixels=720)
-
-
-def set_1080px_square_render_res():
-    """
-    Set the resolution of the rendered image to 1080 by 1080 pixels
-    """
-    set_square_render_res(pixels=1080)
-
-
-def set_1440px_square_render_res():
-    """
-    Set the resolution of the rendered image to 1440 by 1440 pixels
-    """
-    set_square_render_res(pixels=1440)
-
-
-def set_2048px_square_render_res():
-    """
-    Set the resolution of the rendered image to 2048 by 2048 pixels
-    """
-    set_square_render_res(pixels=2048)
-
-
-def set_4096px_square_render_res():
-    """
-    Set the resolution of the rendered image to 4096 by 4096 pixels
-    """
-    set_square_render_res(pixels=4096)
-
-
-def set_1080p_render_res():
-    """
-    Set the resolution of the rendered image to 1080p
-    """
-    bpy.context.scene.render.resolution_x = 1920
-    bpy.context.scene.render.resolution_y = 1080
-
-
-def set_wqhd_render_res():
-    """
-    Set the resolution of the rendered image to 2560x1440 (QHD)
-    """
-    bpy.context.scene.render.resolution_x = 2560
-    bpy.context.scene.render.resolution_y = 1440
-
-
-def set_2k_render_res():
-    """
-    Set the resolution of the rendered image to 2K
-    """
-    bpy.context.scene.render.resolution_x = 2048
-    bpy.context.scene.render.resolution_y = 1080
-
-
-def set_4k_render_res():
-    """
-    Set the resolution of the rendered image to 4K
-    """
-    bpy.context.scene.render.resolution_x = 4096
-    bpy.context.scene.render.resolution_y = 2160
-
-
-def set_twitter_landscape_render_res():
-    """
-    Set the resolution of the rendered image to 1280x720
-    from Twitter's Media Best Practices
-    ref: https://developer.twitter.com/en/docs/twitter-api/v1/media/upload-media/uploading-media/media-best-practices
-    """
-    bpy.context.scene.render.resolution_x = 1280
-    bpy.context.scene.render.resolution_y = 720
-
-
-def set_twitter_square_render_res():
-    """
-    Set the resolution of the rendered image to 720x720
-    from Twitter's Media Best Practices
-    ref: https://developer.twitter.com/en/docs/twitter-api/v1/media/upload-media/uploading-media/media-best-practices
-    """
-    set_720px_square_render_res()
-
-
-def set_instagram_portrait_render_res():
-    """
-    Set the resolution of the rendered image to 1080x1350
-    """
-    bpy.context.scene.render.resolution_x = 1080
-    bpy.context.scene.render.resolution_y = 1350
-
-
-def set_instagram_square_render_res():
-    """
-    Set the resolution of the rendered image to 1080x1080
-    """
-    set_1080px_square_render_res()
+"""
+This module contains utilities for setting up the render resolution.
+"""
+
+import bpy
+
+
+def set_square_render_res(pixels):
+    """
+    Set the resolution of the rendered image to a square
+    """
+    bpy.context.scene.render.resolution_x = pixels
+    bpy.context.scene.render.resolution_y = pixels
+
+
+def set_720px_square_render_res():
+    """
+    Set the resolution of the rendered image to 720 by 720 pixels
+    """
+    set_square_render_res(pixels=720)
+
+
+def set_1080px_square_render_res():
+    """
+    Set the resolution of the rendered image to 1080 by 1080 pixels
+    """
+    set_square_render_res(pixels=1080)
+
+
+def set_1440px_square_render_res():
+    """
+    Set the resolution of the rendered image to 1440 by 1440 pixels
+    """
+    set_square_render_res(pixels=1440)
+
+
+def set_2048px_square_render_res():
+    """
+    Set the resolution of the rendered image to 2048 by 2048 pixels
+    """
+    set_square_render_res(pixels=2048)
+
+
+def set_4096px_square_render_res():
+    """
+    Set the resolution of the rendered image to 4096 by 4096 pixels
+    """
+    set_square_render_res(pixels=4096)
+
+
+def set_1080p_render_res():
+    """
+    Set the resolution of the rendered image to 1080p
+    """
+    bpy.context.scene.render.resolution_x = 1920
+    bpy.context.scene.render.resolution_y = 1080
+
+
+def set_wqhd_render_res():
+    """
+    Set the resolution of the rendered image to 2560x1440 (QHD)
+    """
+    bpy.context.scene.render.resolution_x = 2560
+    bpy.context.scene.render.resolution_y = 1440
+
+
+def set_2k_render_res():
+    """
+    Set the resolution of the rendered image to 2K
+    """
+    bpy.context.scene.render.resolution_x = 2048
+    bpy.context.scene.render.resolution_y = 1080
+
+
+def set_4k_render_res():
+    """
+    Set the resolution of the rendered image to 4K
+    """
+    bpy.context.scene.render.resolution_x = 4096
+    bpy.context.scene.render.resolution_y = 2160
+
+
+def set_twitter_landscape_render_res():
+    """
+    Set the resolution of the rendered image to 1280x720
+    from Twitter's Media Best Practices
+    ref: https://developer.twitter.com/en/docs/twitter-api/v1/media/upload-media/uploading-media/media-best-practices
+    """
+    bpy.context.scene.render.resolution_x = 1280
+    bpy.context.scene.render.resolution_y = 720
+
+
+def set_twitter_square_render_res():
+    """
+    Set the resolution of the rendered image to 720x720
+    from Twitter's Media Best Practices
+    ref: https://developer.twitter.com/en/docs/twitter-api/v1/media/upload-media/uploading-media/media-best-practices
+    """
+    set_720px_square_render_res()
+
+
+def set_instagram_portrait_render_res():
+    """
+    Set the resolution of the rendered image to 1080x1350
+    """
+    bpy.context.scene.render.resolution_x = 1080
+    bpy.context.scene.render.resolution_y = 1350
+
+
+def set_instagram_square_render_res():
+    """
+    Set the resolution of the rendered image to 1080x1080
+    """
+    set_1080px_square_render_res()
```

### Comparing `bpy_building_blocks-0.0.23/src/bpybb/random.py` & `bpy_building_blocks-0.0.24/src/bpybb/random.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-"""
-This module contains utilities for working with random number generation.
-"""
-
-import math
-import random
-import time
-
-import bpy
-import mathutils
-
-from bpybb.utils import active_object, apply_rotation
-
-
-def time_seed() -> float:
-    """
-    Sets the random seed based on the time
-    and copies the seed into the clipboard
-    """
-    seed = time.time()
-    print(f"seed: {seed}")
-    random.seed(seed)
-
-    bpy.context.window_manager.clipboard = str(seed)
-
-    return seed
-
-
-def get_random_rotation() -> mathutils.Euler:
-    """Returns a random Euler rotation on X, Y, Z"""
-    x = math.radians(random.uniform(0, 360))
-    y = math.radians(random.uniform(0, 360))
-    z = math.radians(random.uniform(0, 360))
-    return mathutils.Euler((x, y, z))
-
-
-def apply_random_rotation() -> None:
-    """
-    Applies a random rotation on X, Y, Z for the currently active object
-    """
-    obj = active_object()
-
-    obj.rotation_euler = get_random_rotation()
-
-    apply_rotation()
+"""
+This module contains utilities for working with random number generation.
+"""
+
+import math
+import random
+import time
+
+import bpy
+import mathutils
+
+from bpybb.utils import active_object, apply_rotation
+
+
+def time_seed() -> float:
+    """
+    Sets the random seed based on the time
+    and copies the seed into the clipboard
+    """
+    seed = time.time()
+    print(f"seed: {seed}")
+    random.seed(seed)
+
+    bpy.context.window_manager.clipboard = str(seed)
+
+    return seed
+
+
+def get_random_rotation() -> mathutils.Euler:
+    """Returns a random Euler rotation on X, Y, Z"""
+    x = math.radians(random.uniform(0, 360))
+    y = math.radians(random.uniform(0, 360))
+    z = math.radians(random.uniform(0, 360))
+    return mathutils.Euler((x, y, z))
+
+
+def apply_random_rotation() -> None:
+    """
+    Applies a random rotation on X, Y, Z for the currently active object
+    """
+    obj = active_object()
+
+    obj.rotation_euler = get_random_rotation()
+
+    apply_rotation()
```

### Comparing `bpy_building_blocks-0.0.23/src/bpybb/utils.py` & `bpy_building_blocks-0.0.24/src/bpybb/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,222 +1,237 @@
-"""
-This module contains common helper utilities.
-"""
-
-import contextlib
-
-import bpy
-
-
-class Axis:
-    """Helper class to make code working with axis more readable."""
-
-    X = 0
-    Y = 1
-    Z = 2
-
-
-def active_object():
-    """
-    returns the currently active object
-    """
-    return bpy.context.active_object
-
-
-def make_active(obj):
-    """
-    Select and make the object active in the scene
-
-    Args:
-        obj: object.
-    """
-    bpy.ops.object.select_all(action="DESELECT")
-    obj.select_set(True)
-    bpy.context.view_layer.objects.active = obj
-
-
-def render_animation():
-    """start rendering the animation
-    same as Menu > Render > Render Animation"""
-    bpy.ops.render.render(animation=True)
-
-
-def app_version_is_or_greater_than(major: int, minor: int = 0, subversion: int = 0) -> bool:
-    """The current version of Blender is equal to or
-    greater than the passed in major.minor.subversion
-    """
-    return bpy.app.version >= (major, minor, subversion)
-
-
-def app_version_less_than(major: int, minor: int = 0, subversion: int = 0) -> bool:
-    """The current version of Blender is less than
-    the passed in major.minor.subversion
-    """
-    return bpy.app.version < (major, minor, subversion)
-
-
-@contextlib.contextmanager
-def edit_mode():
-    """
-    A context manager for toggling the edit_mode
-
-    Usage:
-    with edit_mode():
-        # do mesh editing
-    """
-    # enter edit mode
-    bpy.ops.object.editmode_toggle()
-
-    yield  # return out of the function in edit_mode
-
-    # when leaving the context manager scope - exit edit_mode
-    bpy.ops.object.editmode_toggle()
-
-
-def purge_orphans():
-    """
-    Remove all orphan data blocks
-
-    see this from more info:
-    https://youtu.be/3rNqVPtbhzc?t=149
-    """
-    if bpy.app.version >= (3, 0, 0):
-        # run this only for Blender versions 3.0 and higher
-        bpy.ops.outliner.orphans_purge(do_local_ids=True, do_linked_ids=True, do_recursive=True)
-    else:
-        # run this only for Blender versions lower than 3.0
-        # call purge_orphans() recursively until there are no more orphan data blocks to purge
-        result = bpy.ops.outliner.orphans_purge()
-        if result.pop() != "CANCELLED":
-            purge_orphans()
-
-
-def clean_scene():
-    """
-    Removing all of the objects, collection, materials, particles,
-    textures, images, curves, meshes, actions, nodes, and worlds from the scene
-
-    Checkout this video explanation with example
-
-    "How to clean the scene with Python in Blender (with examples)"
-    https://youtu.be/3rNqVPtbhzc
-    """
-    # make sure the active object is not in Edit Mode
-    if bpy.context.active_object and bpy.context.active_object.mode == "EDIT":
-        bpy.ops.object.editmode_toggle()
-
-    # make sure non of the objects are hidden from the viewport, selection, or disabled
-    for obj in bpy.data.objects:
-        obj.hide_set(False)
-        obj.hide_select = False
-        obj.hide_viewport = False
-
-    # select all the object and delete them (just like pressing A + X + D in the viewport)
-    bpy.ops.object.select_all(action="SELECT")
-    bpy.ops.object.delete()
-
-    # find all the collections and remove them
-    collection_names = [col.name for col in bpy.data.collections]
-    for name in collection_names:
-        bpy.data.collections.remove(bpy.data.collections[name])
-
-    # in the case when you modify the world shader
-    # delete and recreate the world object
-    world_names = [world.name for world in bpy.data.worlds]
-    for name in world_names:
-        bpy.data.worlds.remove(bpy.data.worlds[name])
-    # create a new world data block
-    bpy.ops.world.new()
-    bpy.context.scene.world = bpy.data.worlds["World"]
-
-    purge_orphans()
-
-
-def clean_scene_experimental():
-    """
-    An alternative clean scene function that just deletes
-    the whole scene and creates a new one.
-
-    Note: This might crash Blender! (hence experimental in the name)
-    Proceed at your own risk!
-    """
-
-    # rename the current scene, so the new scene won't have a Scene.001
-    old_scene_name = "to_delete"
-    bpy.context.window.scene.name = old_scene_name
-
-    # create a new scene (the name should be just "Scene")
-    bpy.ops.scene.new()
-
-    # remove the old scene
-    bpy.data.scenes.remove(bpy.data.scenes[old_scene_name])
-
-    # create a new world data block
-    bpy.ops.world.new()
-    bpy.context.scene.world = bpy.data.worlds["World"]
-
-    purge_orphans()
-
-
-def render_animation():
-    """
-    Renders the animation in the currently active scene
-    """
-    bpy.ops.render.render(animation=True)
-
-
-def render_image(write_still=False):
-    """
-    Renders an image in the currently active scene at the current frame
-
-    Args:
-        write_still: write the rendered image to disk. Defaults to False.
-    """
-    bpy.ops.render.render(write_still=write_still)
-
-
-def parent(child_obj, parent_obj, keep_transform=False):
-    """
-    Parent the child object to the parent object
-
-    Args:
-        child_obj: child object that will be parented.
-        parent_obj: parent object that will be parented to.
-        keep_transform: keep the transform of the child object. Defaults to False.
-    """
-    make_active(child_obj)
-    child_obj.parent = parent_obj
-    if keep_transform:
-        child_obj.matrix_parent_inverse = parent_obj.matrix_world.inverted()
-
-
-def duplicate_object(obj=None, linked=False):
-    """
-    Duplicate object
-
-    Args:
-        obj: source object that will be duplicated.
-        linked: link duplicated object to target source.
-    """
-    if obj is None:
-        obj = active_object()
-
-    bpy.ops.object.select_all(action="DESELECT")
-    obj.select_set(True)
-    bpy.context.view_layer.objects.active = obj
-
-    bpy.ops.object.duplicate(linked=linked)
-    duplicate_obj = active_object()
-
-    return duplicate_obj
-
-
-def apply_scale():
-    bpy.ops.object.transform_apply(scale=True)
-
-
-def apply_location():
-    bpy.ops.object.transform_apply(location=True)
-
-
-def apply_rotation():
-    bpy.ops.object.transform_apply(rotation=True)
+"""
+This module contains common helper utilities.
+"""
+
+import contextlib
+
+import bpy
+
+
+class Axis:
+    """Helper class to make code working with axis more readable."""
+
+    X = 0
+    Y = 1
+    Z = 2
+
+
+def active_object():
+    """
+    returns the currently active object
+    """
+    return bpy.context.active_object
+
+
+def make_active(obj):
+    """
+    Select and make the object active in the scene
+
+    Args:
+        obj: object.
+    """
+    deselect_all_objects()
+    obj.select_set(True)
+    bpy.context.view_layer.objects.active = obj
+
+
+def deselect_all_objects():
+    """
+    Similar to bpy.ops.object.select_all(action="DESELECT")
+    """
+    for obj in bpy.data.objects:
+        obj.select_set(False)
+
+
+def render_animation():
+    """start rendering the animation
+    same as Menu > Render > Render Animation"""
+    bpy.ops.render.render(animation=True)
+
+
+def app_version_is_or_greater_than(major: int, minor: int = 0, subversion: int = 0) -> bool:
+    """The current version of Blender is equal to or
+    greater than the passed in major.minor.subversion
+    """
+    return bpy.app.version >= (major, minor, subversion)
+
+
+def app_version_less_than(major: int, minor: int = 0, subversion: int = 0) -> bool:
+    """The current version of Blender is less than
+    the passed in major.minor.subversion
+    """
+    return bpy.app.version < (major, minor, subversion)
+
+
+@contextlib.contextmanager
+def edit_mode():
+    """
+    A context manager for toggling the edit_mode
+
+    Usage:
+    with edit_mode():
+        # do mesh editing
+    """
+    # enter edit mode
+    bpy.ops.object.editmode_toggle()
+
+    yield  # return out of the function in edit_mode
+
+    # when leaving the context manager scope - exit edit_mode
+    bpy.ops.object.editmode_toggle()
+
+
+def purge_orphans():
+    """
+    Remove all orphan data blocks
+
+    see this from more info:
+    https://youtu.be/3rNqVPtbhzc?t=149
+    """
+    if bpy.app.version >= (3, 0, 0):
+        # run this only for Blender versions 3.0 and higher
+        bpy.ops.outliner.orphans_purge(do_local_ids=True, do_linked_ids=True, do_recursive=True)
+    else:
+        # run this only for Blender versions lower than 3.0
+        # call purge_orphans() recursively until there are no more orphan data blocks to purge
+        result = bpy.ops.outliner.orphans_purge()
+        if result.pop() != "CANCELLED":
+            purge_orphans()
+
+
+def clean_scene():
+    """
+    Removing all of the objects, collection, materials, particles,
+    textures, images, curves, meshes, actions, nodes, and worlds from the scene
+
+    Checkout this video explanation with example
+
+    "How to clean the scene with Python in Blender (with examples)"
+    https://youtu.be/3rNqVPtbhzc
+    """
+    # make sure the active object is not in Edit Mode
+    if bpy.context.active_object and bpy.context.active_object.mode == "EDIT":
+        bpy.ops.object.editmode_toggle()
+
+    # make sure non of the objects are hidden from the viewport, selection, or disabled
+    for obj in bpy.data.objects:
+        obj.hide_set(False)
+        obj.hide_select = False
+        obj.hide_viewport = False
+
+    # select all the object and delete them (just like pressing A + X + D in the viewport)
+    bpy.ops.object.select_all(action="SELECT")
+    bpy.ops.object.delete()
+
+    # find all the collections and remove them
+    collection_names = [col.name for col in bpy.data.collections]
+    for name in collection_names:
+        bpy.data.collections.remove(bpy.data.collections[name])
+
+    # in the case when you modify the world shader
+    # delete and recreate the world object
+    world_names = [world.name for world in bpy.data.worlds]
+    for name in world_names:
+        bpy.data.worlds.remove(bpy.data.worlds[name])
+    # create a new world data block
+    bpy.ops.world.new()
+    bpy.context.scene.world = bpy.data.worlds["World"]
+
+    purge_orphans()
+
+
+def clean_scene_experimental():
+    """
+    An alternative clean scene function that just deletes
+    the whole scene and creates a new one.
+
+    Note: This might crash Blender! (hence experimental in the name)
+    Proceed at your own risk!
+    """
+
+    # rename the current scene, so the new scene won't have a Scene.001
+    old_scene_name = "to_delete"
+    bpy.context.window.scene.name = old_scene_name
+
+    # create a new scene (the name should be just "Scene")
+    bpy.ops.scene.new()
+
+    # remove the old scene
+    bpy.data.scenes.remove(bpy.data.scenes[old_scene_name])
+
+    # create a new world data block
+    bpy.ops.world.new()
+    bpy.context.scene.world = bpy.data.worlds["World"]
+
+    purge_orphans()
+
+
+def remove_libraries() -> None:
+    """
+    Remove libraries that were linked into the Blend file
+    """
+    bpy.data.batch_remove(bpy.data.libraries)
+
+
+def render_animation():
+    """
+    Renders the animation in the currently active scene
+    """
+    bpy.ops.render.render(animation=True)
+
+
+def render_image(write_still=False):
+    """
+    Renders an image in the currently active scene at the current frame
+
+    Args:
+        write_still: write the rendered image to disk. Defaults to False.
+    """
+    bpy.ops.render.render(write_still=write_still)
+
+
+def parent(child_obj, parent_obj, keep_transform=False):
+    """
+    Parent the child object to the parent object
+
+    Args:
+        child_obj: child object that will be parented.
+        parent_obj: parent object that will be parented to.
+        keep_transform: keep the transform of the child object. Defaults to False.
+    """
+    make_active(child_obj)
+    child_obj.parent = parent_obj
+    if keep_transform:
+        child_obj.matrix_parent_inverse = parent_obj.matrix_world.inverted()
+
+
+def duplicate_object(obj=None, linked=False):
+    """
+    Duplicate object
+
+    Args:
+        obj: source object that will be duplicated.
+        linked: link duplicated object to target source.
+    """
+    if obj is None:
+        obj = active_object()
+
+    deselect_all_objects()
+    obj.select_set(True)
+    bpy.context.view_layer.objects.active = obj
+
+    bpy.ops.object.duplicate(linked=linked)
+    duplicate_obj = active_object()
+
+    return duplicate_obj
+
+
+def apply_scale():
+    bpy.ops.object.transform_apply(scale=True)
+
+
+def apply_location():
+    bpy.ops.object.transform_apply(location=True)
+
+
+def apply_rotation():
+    bpy.ops.object.transform_apply(rotation=True)
```

