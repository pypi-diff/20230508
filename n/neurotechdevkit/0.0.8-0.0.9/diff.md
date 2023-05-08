# Comparing `tmp/neurotechdevkit-0.0.8.tar.gz` & `tmp/neurotechdevkit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurotechdevkit-0.0.8.tar", max compression
+gzip compressed data, was "neurotechdevkit-0.0.9.tar", max compression
```

## Comparing `neurotechdevkit-0.0.8.tar` & `neurotechdevkit-0.0.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    11339 2023-05-02 20:07:20.054177 neurotechdevkit-0.0.8/LICENSE
--rw-r--r--   0        0        0     2679 2023-05-02 20:07:20.054177 neurotechdevkit-0.0.8/README.md
--rw-r--r--   0        0        0     1932 2023-05-02 20:07:34.875093 neurotechdevkit-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2043 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/__init__.py
--rw-r--r--   0        0        0     1138 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/__init__.py
--rw-r--r--   0        0        0     4661 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/_animations.py
--rw-r--r--   0        0        0     2236 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/_formatting.py
--rw-r--r--   0        0        0     8947 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/_source.py
--rw-r--r--   0        0        0     3444 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/_target.py
--rw-r--r--   0        0        0    49812 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/colormaps.py
--rw-r--r--   0        0        0     2307 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=10°.png
--rw-r--r--   0        0        0    30101 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=120°.png
--rw-r--r--   0        0        0    50607 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=150°.png
--rw-r--r--   0        0        0    61496 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=180°.png
--rw-r--r--   0        0        0     4467 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=20°.png
--rw-r--r--   0        0        0      715 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=2°.png
--rw-r--r--   0        0        0     8691 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=40°.png
--rw-r--r--   0        0        0     1147 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=5°.png
--rw-r--r--   0        0        0    12673 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=60°.png
--rw-r--r--   0        0        0    20015 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=90°.png
--rw-r--r--   0        0        0     2753 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=Flat.png
--rw-r--r--   0        0        0     3377 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/target-dark.png
--rw-r--r--   0        0        0     3598 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/target-light.png
--rw-r--r--   0        0        0      674 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/font.py
--rw-r--r--   0        0        0    96364 2023-05-02 20:07:20.174184 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/fonts/Manrope-Bold.ttf
--rw-r--r--   0        0        0    97116 2023-05-02 20:07:20.178185 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/fonts/Manrope-ExtraBold.ttf
--rw-r--r--   0        0        0    96304 2023-05-02 20:07:20.178185 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/fonts/Manrope-ExtraLight.ttf
--rw-r--r--   0        0        0    96312 2023-05-02 20:07:20.178185 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/fonts/Manrope-Light.ttf
--rw-r--r--   0        0        0    96492 2023-05-02 20:07:20.178185 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/fonts/Manrope-Medium.ttf
--rw-r--r--   0        0        0    96412 2023-05-02 20:07:20.178185 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/fonts/Manrope-Regular.ttf
--rw-r--r--   0        0        0    96528 2023-05-02 20:07:20.178185 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/fonts/Manrope-SemiBold.ttf
--rw-r--r--   0        0        0     4243 2023-05-02 20:07:20.178185 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/layers.py
--rw-r--r--   0        0        0     5325 2023-05-02 20:07:20.178185 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/layout.py
--rw-r--r--   0        0        0     5996 2023-05-02 20:07:20.178185 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/legends.py
--rw-r--r--   0        0        0     7467 2023-05-02 20:07:20.178185 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/napari.py
--rw-r--r--   0        0        0     8647 2023-05-02 20:07:20.178185 neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/simulations.py
--rw-r--r--   0        0        0      898 2023-05-02 20:07:20.178185 neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/__init__.py
--rw-r--r--   0        0        0    42314 2023-05-02 20:07:20.182185 neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/_base.py
--rw-r--r--   0        0        0    12924 2023-05-02 20:07:20.182185 neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/_metrics.py
--rw-r--r--   0        0        0     6060 2023-05-02 20:07:20.182185 neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/_resources.py
--rw-r--r--   0        0        0    50222 2023-05-02 20:07:20.182185 neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/_results.py
--rw-r--r--   0        0        0     4524 2023-05-02 20:07:20.182185 neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/_scenario_0.py
--rw-r--r--   0        0        0     8319 2023-05-02 20:07:20.182185 neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/_scenario_1.py
--rw-r--r--   0        0        0    11280 2023-05-02 20:07:20.182185 neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/_scenario_2.py
--rw-r--r--   0        0        0     7305 2023-05-02 20:07:20.182185 neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/_shots.py
--rw-r--r--   0        0        0     4456 2023-05-02 20:07:20.182185 neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/_time.py
--rw-r--r--   0        0        0    11292 2023-05-02 20:07:20.182185 neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/_utils.py
--rw-r--r--   0        0        0  2195183 2023-05-02 20:07:20.194186 neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/data/skull_mask_bm8_dx_0.5mm.mat
--rw-r--r--   0        0        0      885 2023-05-02 20:07:20.194186 neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/materials.py
--rw-r--r--   0        0        0    57468 2023-05-02 20:07:20.194186 neurotechdevkit-0.0.8/src/neurotechdevkit/sources.py
--rw-r--r--   0        0        0     3964 1970-01-01 00:00:00.000000 neurotechdevkit-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-05-02 20:12:45.238385 neurotechdevkit-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2067 2023-05-02 20:12:45.238385 neurotechdevkit-0.0.9/README.md
+-rw-r--r--   0        0        0     1932 2023-05-02 20:12:57.898483 neurotechdevkit-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2043 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/__init__.py
+-rw-r--r--   0        0        0     1138 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/__init__.py
+-rw-r--r--   0        0        0     4661 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/_animations.py
+-rw-r--r--   0        0        0     2236 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/_formatting.py
+-rw-r--r--   0        0        0     8947 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/_source.py
+-rw-r--r--   0        0        0     3444 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/_target.py
+-rw-r--r--   0        0        0    49812 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/colormaps.py
+-rw-r--r--   0        0        0     2307 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=10°.png
+-rw-r--r--   0        0        0    30101 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=120°.png
+-rw-r--r--   0        0        0    50607 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=150°.png
+-rw-r--r--   0        0        0    61496 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=180°.png
+-rw-r--r--   0        0        0     4467 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=20°.png
+-rw-r--r--   0        0        0      715 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=2°.png
+-rw-r--r--   0        0        0     8691 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=40°.png
+-rw-r--r--   0        0        0     1147 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=5°.png
+-rw-r--r--   0        0        0    12673 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=60°.png
+-rw-r--r--   0        0        0    20015 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=90°.png
+-rw-r--r--   0        0        0     2753 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=Flat.png
+-rw-r--r--   0        0        0     3377 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/target-dark.png
+-rw-r--r--   0        0        0     3598 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/target-light.png
+-rw-r--r--   0        0        0      674 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/font.py
+-rw-r--r--   0        0        0    96364 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/fonts/Manrope-Bold.ttf
+-rw-r--r--   0        0        0    97116 2023-05-02 20:12:45.338386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/fonts/Manrope-ExtraBold.ttf
+-rw-r--r--   0        0        0    96304 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/fonts/Manrope-ExtraLight.ttf
+-rw-r--r--   0        0        0    96312 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/fonts/Manrope-Light.ttf
+-rw-r--r--   0        0        0    96492 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/fonts/Manrope-Medium.ttf
+-rw-r--r--   0        0        0    96412 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/fonts/Manrope-Regular.ttf
+-rw-r--r--   0        0        0    96528 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/fonts/Manrope-SemiBold.ttf
+-rw-r--r--   0        0        0     4243 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/layers.py
+-rw-r--r--   0        0        0     5325 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/layout.py
+-rw-r--r--   0        0        0     5996 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/legends.py
+-rw-r--r--   0        0        0     7467 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/napari.py
+-rw-r--r--   0        0        0     8647 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/simulations.py
+-rw-r--r--   0        0        0      898 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/__init__.py
+-rw-r--r--   0        0        0    42314 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/_base.py
+-rw-r--r--   0        0        0    12924 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/_metrics.py
+-rw-r--r--   0        0        0     6060 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/_resources.py
+-rw-r--r--   0        0        0    50222 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/_results.py
+-rw-r--r--   0        0        0     4524 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/_scenario_0.py
+-rw-r--r--   0        0        0     8319 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/_scenario_1.py
+-rw-r--r--   0        0        0    11280 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/_scenario_2.py
+-rw-r--r--   0        0        0     7305 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/_shots.py
+-rw-r--r--   0        0        0     4456 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/_time.py
+-rw-r--r--   0        0        0    11292 2023-05-02 20:12:45.342386 neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/_utils.py
+-rw-r--r--   0        0        0  2195183 2023-05-02 20:12:45.354386 neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/data/skull_mask_bm8_dx_0.5mm.mat
+-rw-r--r--   0        0        0      885 2023-05-02 20:12:45.354386 neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/materials.py
+-rw-r--r--   0        0        0    57468 2023-05-02 20:12:45.354386 neurotechdevkit-0.0.9/src/neurotechdevkit/sources.py
+-rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 neurotechdevkit-0.0.9/PKG-INFO
```

### Comparing `neurotechdevkit-0.0.8/LICENSE` & `neurotechdevkit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/pyproject.toml` & `neurotechdevkit-0.0.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neurotechdevkit"
-version = "v0.0.8"
+version = "v0.0.9"
 description = "A research repo for the NDK (Neurotech Development Kit) project"
 authors = ["AE Studio <bci@ae.studio>"]
 maintainers = ["AE Studio <bci@ae.studio>"]
 packages = [{include = "neurotechdevkit", from = "src" }]
 
 readme = "README.md"
 license = "Apache-2.0"
```

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/__init__.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/__init__.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/__init__.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/__init__.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/_animations.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/_animations.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/_formatting.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/_formatting.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/_source.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/_source.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/_target.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/_target.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/colormaps.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/colormaps.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=10°.png` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=10°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=120°.png` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=120°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=150°.png` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=150°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=180°.png` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=180°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=20°.png` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=20°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=2°.png` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=2°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=40°.png` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=40°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=5°.png` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=5°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=60°.png` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=60°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=90°.png` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=90°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/Angle=Flat.png` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/Angle=Flat.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/target-dark.png` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/target-dark.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/components/target-light.png` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/components/target-light.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/font.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/font.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/fonts/Manrope-Bold.ttf` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/fonts/Manrope-Bold.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/fonts/Manrope-ExtraBold.ttf` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/fonts/Manrope-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/fonts/Manrope-ExtraLight.ttf` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/fonts/Manrope-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/fonts/Manrope-Light.ttf` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/fonts/Manrope-Light.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/fonts/Manrope-Medium.ttf` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/fonts/Manrope-Medium.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/fonts/Manrope-Regular.ttf` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/fonts/Manrope-Regular.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/fonts/Manrope-SemiBold.ttf` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/fonts/Manrope-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/layers.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/layers.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/layout.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/layout.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/legends.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/legends.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/napari.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/napari.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/rendering/simulations.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/rendering/simulations.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/__init__.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/__init__.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/_base.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/_base.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/_metrics.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/_metrics.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/_resources.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/_resources.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/_results.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/_results.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/_scenario_0.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/_scenario_0.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/_scenario_1.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/_scenario_1.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/_scenario_2.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/_scenario_2.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/_shots.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/_shots.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/_time.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/_time.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/_utils.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/_utils.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/data/skull_mask_bm8_dx_0.5mm.mat` & `neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/data/skull_mask_bm8_dx_0.5mm.mat`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/scenarios/materials.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/scenarios/materials.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.0.8/src/neurotechdevkit/sources.py` & `neurotechdevkit-0.0.9/src/neurotechdevkit/sources.py`

 * *Files identical despite different names*

