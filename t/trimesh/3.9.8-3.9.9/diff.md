# Comparing `tmp/trimesh-3.9.8.tar.gz` & `tmp/trimesh-3.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trimesh-3.9.8.tar", last modified: Fri Feb 26 00:55:19 2021, max compression
+gzip compressed data, was "trimesh-3.9.9.tar", last modified: Mon Mar 15 03:11:30 2021, max compression
```

## Comparing `trimesh-3.9.8.tar` & `trimesh-3.9.9.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-26 00:55:19.669364 trimesh-3.9.8/
--rw-r--r--   0 runner    (1001) docker     (116)     1090 2021-02-26 00:55:07.000000 trimesh-3.9.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (116)       63 2021-02-26 00:55:07.000000 trimesh-3.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    17033 2021-02-26 00:55:19.669364 trimesh-3.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    14243 2021-02-26 00:55:07.000000 trimesh-3.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       69 2021-02-26 00:55:19.669364 trimesh-3.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     5262 2021-02-26 00:55:07.000000 trimesh-3.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-26 00:55:19.661364 trimesh-3.9.8/trimesh/
--rw-r--r--   0 runner    (1001) docker     (116)     1534 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    92000 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     2535 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/boolean.py
--rw-r--r--   0 runner    (1001) docker     (116)    16290 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/bounds.py
--rw-r--r--   0 runner    (1001) docker     (116)    20650 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/caching.py
--rw-r--r--   0 runner    (1001) docker     (116)    21851 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/collision.py
--rw-r--r--   0 runner    (1001) docker     (116)     7657 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/comparison.py
--rw-r--r--   0 runner    (1001) docker     (116)     5152 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/constants.py
--rw-r--r--   0 runner    (1001) docker     (116)     6812 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/convex.py
--rw-r--r--   0 runner    (1001) docker     (116)    40606 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/creation.py
--rw-r--r--   0 runner    (1001) docker     (116)     5397 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/curvature.py
--rw-r--r--   0 runner    (1001) docker     (116)      617 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/decomposition.py
--rw-r--r--   0 runner    (1001) docker     (116)     1232 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-26 00:55:19.661364 trimesh-3.9.8/trimesh/exchange/
--rw-r--r--   0 runner    (1001) docker     (116)      295 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/exchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7572 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/exchange/assimp.py
--rw-r--r--   0 runner    (1001) docker     (116)    17922 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/exchange/binvox.py
--rw-r--r--   0 runner    (1001) docker     (116)    13256 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/exchange/dae.py
--rw-r--r--   0 runner    (1001) docker     (116)     8441 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/exchange/export.py
--rw-r--r--   0 runner    (1001) docker     (116)    53265 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/exchange/gltf.py
--rw-r--r--   0 runner    (1001) docker     (116)    20881 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/exchange/load.py
--rw-r--r--   0 runner    (1001) docker     (116)     4482 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/exchange/misc.py
--rw-r--r--   0 runner    (1001) docker     (116)    31940 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/exchange/obj.py
--rw-r--r--   0 runner    (1001) docker     (116)     2767 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/exchange/off.py
--rw-r--r--   0 runner    (1001) docker     (116)     5647 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/exchange/openctm.py
--rw-r--r--   0 runner    (1001) docker     (116)    30692 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/exchange/ply.py
--rw-r--r--   0 runner    (1001) docker     (116)     8708 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/exchange/stl.py
--rw-r--r--   0 runner    (1001) docker     (116)     8477 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/exchange/threemf.py
--rw-r--r--   0 runner    (1001) docker     (116)     5811 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/exchange/urdf.py
--rw-r--r--   0 runner    (1001) docker     (116)    17204 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/exchange/xml_based.py
--rw-r--r--   0 runner    (1001) docker     (116)     3029 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/exchange/xyz.py
--rw-r--r--   0 runner    (1001) docker     (116)    14316 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/geometry.py
--rw-r--r--   0 runner    (1001) docker     (116)    30218 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/graph.py
--rw-r--r--   0 runner    (1001) docker     (116)    25347 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/grouping.py
--rw-r--r--   0 runner    (1001) docker     (116)     6049 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/inertia.py
--rw-r--r--   0 runner    (1001) docker     (116)     3682 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/integrate.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-26 00:55:19.661364 trimesh-3.9.8/trimesh/interfaces/
--rw-r--r--   0 runner    (1001) docker     (116)      159 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3080 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/interfaces/blender.py
--rw-r--r--   0 runner    (1001) docker     (116)     3616 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/interfaces/generic.py
--rw-r--r--   0 runner    (1001) docker     (116)     7258 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/interfaces/gmsh.py
--rw-r--r--   0 runner    (1001) docker     (116)     2455 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/interfaces/scad.py
--rw-r--r--   0 runner    (1001) docker     (116)     1906 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/interfaces/vhacd.py
--rw-r--r--   0 runner    (1001) docker     (116)    27831 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/intersections.py
--rw-r--r--   0 runner    (1001) docker     (116)     3443 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/interval.py
--rw-r--r--   0 runner    (1001) docker     (116)     6130 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/nsphere.py
--rw-r--r--   0 runner    (1001) docker     (116)     7775 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/parent.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-26 00:55:19.665364 trimesh-3.9.8/trimesh/path/
--rw-r--r--   0 runner    (1001) docker     (116)      223 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7781 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/arc.py
--rw-r--r--   0 runner    (1001) docker     (116)     9199 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/creation.py
--rw-r--r--   0 runner    (1001) docker     (116)     3749 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/curve.py
--rw-r--r--   0 runner    (1001) docker     (116)    19584 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/entities.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-26 00:55:19.665364 trimesh-3.9.8/trimesh/path/exchange/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/exchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    37951 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/exchange/dxf.py
--rw-r--r--   0 runner    (1001) docker     (116)     1935 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/exchange/export.py
--rw-r--r--   0 runner    (1001) docker     (116)     2477 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/exchange/load.py
--rw-r--r--   0 runner    (1001) docker     (116)     6097 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/exchange/misc.py
--rw-r--r--   0 runner    (1001) docker     (116)    16214 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/exchange/svg_io.py
--rw-r--r--   0 runner    (1001) docker     (116)     2325 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/intersections.py
--rw-r--r--   0 runner    (1001) docker     (116)    13152 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/packing.py
--rw-r--r--   0 runner    (1001) docker     (116)    46093 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/path.py
--rw-r--r--   0 runner    (1001) docker     (116)    25364 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/polygons.py
--rw-r--r--   0 runner    (1001) docker     (116)     3199 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/raster.py
--rw-r--r--   0 runner    (1001) docker     (116)     3637 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/repair.py
--rw-r--r--   0 runner    (1001) docker     (116)    17037 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/segments.py
--rw-r--r--   0 runner    (1001) docker     (116)    12959 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/simplify.py
--rw-r--r--   0 runner    (1001) docker     (116)    14549 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/traversal.py
--rw-r--r--   0 runner    (1001) docker     (116)     1405 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/path/util.py
--rw-r--r--   0 runner    (1001) docker     (116)     4602 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/permutate.py
--rw-r--r--   0 runner    (1001) docker     (116)    17476 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/points.py
--rw-r--r--   0 runner    (1001) docker     (116)    10162 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/poses.py
--rw-r--r--   0 runner    (1001) docker     (116)    25573 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/primitives.py
--rw-r--r--   0 runner    (1001) docker     (116)    19400 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/proximity.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-26 00:55:19.665364 trimesh-3.9.8/trimesh/ray/
--rw-r--r--   0 runner    (1001) docker     (116)      342 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11359 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/ray/ray_pyembree.py
--rw-r--r--   0 runner    (1001) docker     (116)    13444 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/ray/ray_triangle.py
--rw-r--r--   0 runner    (1001) docker     (116)     4583 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/ray/ray_util.py
--rw-r--r--   0 runner    (1001) docker     (116)    10799 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/registration.py
--rw-r--r--   0 runner    (1001) docker     (116)     5853 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/remesh.py
--rw-r--r--   0 runner    (1001) docker     (116)    12643 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/rendering.py
--rw-r--r--   0 runner    (1001) docker     (116)    11672 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/repair.py
--rw-r--r--   0 runner    (1001) docker     (116)     7170 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-26 00:55:19.665364 trimesh-3.9.8/trimesh/resources/
--rw-r--r--   0 runner    (1001) docker     (116)     1227 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1947 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/resources/blender_boolean.py.template
--rw-r--r--   0 runner    (1001) docker     (116)     1147 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/resources/blender_unwrap.py.template
--rw-r--r--   0 runner    (1001) docker     (116)    11077 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/resources/dxf.json.template
--rw-r--r--   0 runner    (1001) docker     (116)    24687 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/resources/gltf_2_schema.zip
--rw-r--r--   0 runner    (1001) docker     (116)      487 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/resources/ply.template
--rw-r--r--   0 runner    (1001) docker     (116)      190 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/resources/svg.base.template
--rw-r--r--   0 runner    (1001) docker     (116)       37 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/resources/svg.path.template
--rw-r--r--   0 runner    (1001) docker     (116)     1261 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/resources/units_to_inches.json
--rw-r--r--   0 runner    (1001) docker     (116)   167999 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/resources/viewer.template.zip
--rw-r--r--   0 runner    (1001) docker     (116)     5726 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-26 00:55:19.665364 trimesh-3.9.8/trimesh/scene/
--rw-r--r--   0 runner    (1001) docker     (116)      142 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/scene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12423 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/scene/cameras.py
--rw-r--r--   0 runner    (1001) docker     (116)     8996 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/scene/lighting.py
--rw-r--r--   0 runner    (1001) docker     (116)    38189 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/scene/scene.py
--rw-r--r--   0 runner    (1001) docker     (116)    18540 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/scene/transforms.py
--rw-r--r--   0 runner    (1001) docker     (116)     1286 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/schemas.py
--rw-r--r--   0 runner    (1001) docker     (116)    11346 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/smoothing.py
--rw-r--r--   0 runner    (1001) docker     (116)    73000 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/transformations.py
--rw-r--r--   0 runner    (1001) docker     (116)    21445 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/triangles.py
--rw-r--r--   0 runner    (1001) docker     (116)     3735 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/units.py
--rw-r--r--   0 runner    (1001) docker     (116)      990 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/unwrap.py
--rw-r--r--   0 runner    (1001) docker     (116)    67133 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/util.py
--rw-r--r--   0 runner    (1001) docker     (116)       22 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-26 00:55:19.665364 trimesh-3.9.8/trimesh/viewer/
--rw-r--r--   0 runner    (1001) docker     (116)      989 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3042 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/viewer/notebook.py
--rw-r--r--   0 runner    (1001) docker     (116)     8057 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/viewer/trackball.py
--rw-r--r--   0 runner    (1001) docker     (116)     9274 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/viewer/widget.py
--rw-r--r--   0 runner    (1001) docker     (116)    31143 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/viewer/windowed.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-26 00:55:19.665364 trimesh-3.9.8/trimesh/visual/
--rw-r--r--   0 runner    (1001) docker     (116)      925 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/visual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      984 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/visual/base.py
--rw-r--r--   0 runner    (1001) docker     (116)    25592 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/visual/color.py
--rw-r--r--   0 runner    (1001) docker     (116)    13083 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/visual/material.py
--rw-r--r--   0 runner    (1001) docker     (116)     2555 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/visual/objects.py
--rw-r--r--   0 runner    (1001) docker     (116)    10242 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/visual/texture.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-26 00:55:19.669364 trimesh-3.9.8/trimesh/voxel/
--rw-r--r--   0 runner    (1001) docker     (116)       60 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/voxel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11907 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/voxel/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     9681 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/voxel/creation.py
--rw-r--r--   0 runner    (1001) docker     (116)    27518 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/voxel/encoding.py
--rw-r--r--   0 runner    (1001) docker     (116)     5543 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/voxel/morphology.py
--rw-r--r--   0 runner    (1001) docker     (116)    12268 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/voxel/ops.py
--rw-r--r--   0 runner    (1001) docker     (116)    19944 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/voxel/runlength.py
--rw-r--r--   0 runner    (1001) docker     (116)     5337 2021-02-26 00:55:07.000000 trimesh-3.9.8/trimesh/voxel/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-26 00:55:19.661364 trimesh-3.9.8/trimesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    17033 2021-02-26 00:55:19.000000 trimesh-3.9.8/trimesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3279 2021-02-26 00:55:19.000000 trimesh-3.9.8/trimesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-26 00:55:19.000000 trimesh-3.9.8/trimesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      421 2021-02-26 00:55:19.000000 trimesh-3.9.8/trimesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2021-02-26 00:55:19.000000 trimesh-3.9.8/trimesh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 03:11:30.323855 trimesh-3.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1090 2021-03-15 03:11:18.000000 trimesh-3.9.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2021-03-15 03:11:18.000000 trimesh-3.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    17033 2021-03-15 03:11:30.323855 trimesh-3.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    14243 2021-03-15 03:11:18.000000 trimesh-3.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-03-15 03:11:30.323855 trimesh-3.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     5262 2021-03-15 03:11:18.000000 trimesh-3.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 03:11:30.307855 trimesh-3.9.9/trimesh/
+-rw-r--r--   0 runner    (1001) docker     (121)     1534 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    92000 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16290 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20650 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/caching.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21851 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/collision.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7657 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5152 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6812 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/convex.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40606 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/creation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5397 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/curvature.py
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 03:11:30.311855 trimesh-3.9.9/trimesh/exchange/
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7572 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/exchange/assimp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17922 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/exchange/binvox.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13256 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/exchange/dae.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8441 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/exchange/export.py
+-rw-r--r--   0 runner    (1001) docker     (121)    53522 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/exchange/gltf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20881 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/exchange/load.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4482 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/exchange/misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31940 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/exchange/obj.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2767 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/exchange/off.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5647 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/exchange/openctm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30692 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/exchange/ply.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8708 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/exchange/stl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8477 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/exchange/threemf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5811 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/exchange/urdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17204 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/exchange/xml_based.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3029 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/exchange/xyz.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14316 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30218 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25347 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/grouping.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6049 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/inertia.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3682 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/integrate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 03:11:30.311855 trimesh-3.9.9/trimesh/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3080 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/interfaces/blender.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3831 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/interfaces/generic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7258 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/interfaces/gmsh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2455 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/interfaces/scad.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1906 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/interfaces/vhacd.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27831 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/intersections.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3443 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/interval.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6130 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/nsphere.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7775 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/parent.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 03:11:30.311855 trimesh-3.9.9/trimesh/path/
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7781 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/arc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9199 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/creation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3749 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/curve.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19584 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/entities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 03:11:30.315855 trimesh-3.9.9/trimesh/path/exchange/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37951 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/exchange/dxf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1935 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/exchange/export.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2477 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/exchange/load.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6097 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/exchange/misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16214 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/exchange/svg_io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2325 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/intersections.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13152 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/packing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46093 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/path.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25364 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/polygons.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3199 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/raster.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3637 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/repair.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17037 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/segments.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12959 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14549 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/traversal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1405 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/path/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4602 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/permutate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17476 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/points.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10162 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/poses.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25573 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19400 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/proximity.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 03:11:30.315855 trimesh-3.9.9/trimesh/ray/
+-rw-r--r--   0 runner    (1001) docker     (121)      342 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11359 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/ray/ray_pyembree.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13444 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/ray/ray_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4583 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/ray/ray_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10799 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/registration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5853 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/remesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12643 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/rendering.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11672 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/repair.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7170 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 03:11:30.319855 trimesh-3.9.9/trimesh/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)     1227 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1947 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/resources/blender_boolean.py.template
+-rw-r--r--   0 runner    (1001) docker     (121)     1147 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/resources/blender_unwrap.py.template
+-rw-r--r--   0 runner    (1001) docker     (121)    11077 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/resources/dxf.json.template
+-rw-r--r--   0 runner    (1001) docker     (121)    24687 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/resources/gltf_2_schema.zip
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/resources/ply.template
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/resources/svg.base.template
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/resources/svg.path.template
+-rw-r--r--   0 runner    (1001) docker     (121)     1261 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/resources/units_to_inches.json
+-rw-r--r--   0 runner    (1001) docker     (121)   167999 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/resources/viewer.template.zip
+-rw-r--r--   0 runner    (1001) docker     (121)     5726 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 03:11:30.319855 trimesh-3.9.9/trimesh/scene/
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/scene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12423 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/scene/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8996 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/scene/lighting.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38458 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/scene/scene.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18957 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/scene/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1286 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11346 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    73000 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21445 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/triangles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3735 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/units.py
+-rw-r--r--   0 runner    (1001) docker     (121)      990 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/unwrap.py
+-rw-r--r--   0 runner    (1001) docker     (121)    67133 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 03:11:30.319855 trimesh-3.9.9/trimesh/viewer/
+-rw-r--r--   0 runner    (1001) docker     (121)      989 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3042 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/viewer/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8057 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/viewer/trackball.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9274 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/viewer/widget.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31143 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/viewer/windowed.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 03:11:30.323855 trimesh-3.9.9/trimesh/visual/
+-rw-r--r--   0 runner    (1001) docker     (121)      925 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/visual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      984 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/visual/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25592 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/visual/color.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13083 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/visual/material.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2555 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/visual/objects.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10242 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/visual/texture.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 03:11:30.323855 trimesh-3.9.9/trimesh/voxel/
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/voxel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11907 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/voxel/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9681 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/voxel/creation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27518 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/voxel/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5543 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/voxel/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12268 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/voxel/ops.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19944 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/voxel/runlength.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5337 2021-03-15 03:11:18.000000 trimesh-3.9.9/trimesh/voxel/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 03:11:30.307855 trimesh-3.9.9/trimesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    17033 2021-03-15 03:11:29.000000 trimesh-3.9.9/trimesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3279 2021-03-15 03:11:30.000000 trimesh-3.9.9/trimesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-15 03:11:29.000000 trimesh-3.9.9/trimesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      421 2021-03-15 03:11:29.000000 trimesh-3.9.9/trimesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-03-15 03:11:29.000000 trimesh-3.9.9/trimesh.egg-info/top_level.txt
```

### Comparing `trimesh-3.9.8/LICENSE.md` & `trimesh-3.9.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/PKG-INFO` & `trimesh-3.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trimesh
-Version: 3.9.8
+Version: 3.9.9
 Summary: Import, export, process, analyze and view triangular meshes.
 Home-page: https://github.com/mikedh/trimesh
 Author: Michael Dawson-Haggerty
 Author-email: mikedh@kerfed.com
 License: MIT
 Description: [![trimesh](https://trimsh.org/images/logotype-a.svg)](http://trimsh.org)
```

### Comparing `trimesh-3.9.8/README.md` & `trimesh-3.9.9/README.md`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/setup.py` & `trimesh-3.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/__init__.py` & `trimesh-3.9.9/trimesh/__init__.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/base.py` & `trimesh-3.9.9/trimesh/base.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/boolean.py` & `trimesh-3.9.9/trimesh/boolean.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/bounds.py` & `trimesh-3.9.9/trimesh/bounds.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/caching.py` & `trimesh-3.9.9/trimesh/caching.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/collision.py` & `trimesh-3.9.9/trimesh/collision.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/comparison.py` & `trimesh-3.9.9/trimesh/comparison.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/constants.py` & `trimesh-3.9.9/trimesh/constants.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/convex.py` & `trimesh-3.9.9/trimesh/convex.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/creation.py` & `trimesh-3.9.9/trimesh/creation.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/curvature.py` & `trimesh-3.9.9/trimesh/curvature.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/decomposition.py` & `trimesh-3.9.9/trimesh/decomposition.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/exceptions.py` & `trimesh-3.9.9/trimesh/exceptions.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/exchange/assimp.py` & `trimesh-3.9.9/trimesh/exchange/assimp.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/exchange/binvox.py` & `trimesh-3.9.9/trimesh/exchange/binvox.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/exchange/dae.py` & `trimesh-3.9.9/trimesh/exchange/dae.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/exchange/export.py` & `trimesh-3.9.9/trimesh/exchange/export.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/exchange/gltf.py` & `trimesh-3.9.9/trimesh/exchange/gltf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1067,14 +1067,20 @@
             try:
                 # try loading units from the GLTF extra
                 metadata['units'] = str(m["extras"]["units"])
             except BaseException:
                 # GLTF spec indicates the default units are meters
                 metadata['units'] = 'meters'
 
+            try:
+                # load extras metadata if available
+                metadata['extras'] = str(m["extras"])
+            except BaseException:
+                pass
+
             for j, p in enumerate(m["primitives"]):
                 # if we don't have a triangular mesh continue
                 # if not specified assume it is a mesh
                 if "mode" in p and p["mode"] != 4:
                     log.warning('skipping primitive with mode {}!'.format(p['mode']))
                     continue
 
@@ -1270,14 +1276,17 @@
                 kwargs["matrix"], transformations.quaternion_matrix(quat))
         if "scale" in child:
             # add scale to the matrix
             kwargs["matrix"] = np.dot(
                 kwargs["matrix"],
                 np.diag(np.concatenate((child['scale'], [1.0]))))
 
+        if "extras" in child:
+            kwargs["extras"] = child["extras"]
+
         if "mesh" in child:
             geometries = mesh_prim[child["mesh"]]
             # if the node has a mesh associated with it
             if len(geometries) > 1:
                 # append root node
                 graph.append(kwargs.copy())
                 # put primitives as children
```

### Comparing `trimesh-3.9.8/trimesh/exchange/load.py` & `trimesh-3.9.9/trimesh/exchange/load.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/exchange/misc.py` & `trimesh-3.9.9/trimesh/exchange/misc.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/exchange/obj.py` & `trimesh-3.9.9/trimesh/exchange/obj.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/exchange/off.py` & `trimesh-3.9.9/trimesh/exchange/off.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/exchange/openctm.py` & `trimesh-3.9.9/trimesh/exchange/openctm.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/exchange/ply.py` & `trimesh-3.9.9/trimesh/exchange/ply.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/exchange/stl.py` & `trimesh-3.9.9/trimesh/exchange/stl.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/exchange/threemf.py` & `trimesh-3.9.9/trimesh/exchange/threemf.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/exchange/urdf.py` & `trimesh-3.9.9/trimesh/exchange/urdf.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/exchange/xml_based.py` & `trimesh-3.9.9/trimesh/exchange/xml_based.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/exchange/xyz.py` & `trimesh-3.9.9/trimesh/exchange/xyz.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/geometry.py` & `trimesh-3.9.9/trimesh/geometry.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/graph.py` & `trimesh-3.9.9/trimesh/graph.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/grouping.py` & `trimesh-3.9.9/trimesh/grouping.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/inertia.py` & `trimesh-3.9.9/trimesh/inertia.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/integrate.py` & `trimesh-3.9.9/trimesh/integrate.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/interfaces/blender.py` & `trimesh-3.9.9/trimesh/interfaces/blender.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/interfaces/generic.py` & `trimesh-3.9.9/trimesh/interfaces/generic.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,22 +23,25 @@
         self.kwargs = kwargs
         self.meshes = meshes
         self.script = script
         self.exchange = exchange
 
     def __enter__(self):
         # windows has problems with multiple programs using open files so we close
-        # them at the end of the enter call, and delete them ourselves at the
-        # exit
+        # them at the end of the enter call, and delete them ourselves at exit
+        # Blender sorts its objects alphabetically
+        # so prefix the mesh number on the file name
+        digit_count = len(str(len(self.meshes)))
         self.mesh_pre = [
             NamedTemporaryFile(
                 suffix='.{}'.format(
                     self.exchange),
+                prefix='{}_'.format(str(i).zfill(digit_count)),
                 mode='wb',
-                delete=False) for i in self.meshes]
+                delete=False) for i in range(len(self.meshes))]
         self.mesh_post = NamedTemporaryFile(
             suffix='.{}'.format(
                 self.exchange),
             mode='rb',
             delete=False)
         self.script_out = NamedTemporaryFile(
             mode='wb', delete=False)
```

### Comparing `trimesh-3.9.8/trimesh/interfaces/gmsh.py` & `trimesh-3.9.9/trimesh/interfaces/gmsh.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/interfaces/scad.py` & `trimesh-3.9.9/trimesh/interfaces/scad.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/interfaces/vhacd.py` & `trimesh-3.9.9/trimesh/interfaces/vhacd.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/intersections.py` & `trimesh-3.9.9/trimesh/intersections.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/interval.py` & `trimesh-3.9.9/trimesh/interval.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/nsphere.py` & `trimesh-3.9.9/trimesh/nsphere.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/parent.py` & `trimesh-3.9.9/trimesh/parent.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/path/arc.py` & `trimesh-3.9.9/trimesh/path/arc.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/path/creation.py` & `trimesh-3.9.9/trimesh/path/creation.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/path/curve.py` & `trimesh-3.9.9/trimesh/path/curve.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/path/entities.py` & `trimesh-3.9.9/trimesh/path/entities.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/path/exchange/dxf.py` & `trimesh-3.9.9/trimesh/path/exchange/dxf.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/path/exchange/export.py` & `trimesh-3.9.9/trimesh/path/exchange/export.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/path/exchange/load.py` & `trimesh-3.9.9/trimesh/path/exchange/load.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/path/exchange/misc.py` & `trimesh-3.9.9/trimesh/path/exchange/misc.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/path/exchange/svg_io.py` & `trimesh-3.9.9/trimesh/path/exchange/svg_io.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/path/intersections.py` & `trimesh-3.9.9/trimesh/path/intersections.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/path/packing.py` & `trimesh-3.9.9/trimesh/path/packing.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/path/path.py` & `trimesh-3.9.9/trimesh/path/path.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/path/polygons.py` & `trimesh-3.9.9/trimesh/path/polygons.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/path/raster.py` & `trimesh-3.9.9/trimesh/path/raster.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/path/repair.py` & `trimesh-3.9.9/trimesh/path/repair.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/path/segments.py` & `trimesh-3.9.9/trimesh/path/segments.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/path/simplify.py` & `trimesh-3.9.9/trimesh/path/simplify.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/path/traversal.py` & `trimesh-3.9.9/trimesh/path/traversal.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/path/util.py` & `trimesh-3.9.9/trimesh/path/util.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/permutate.py` & `trimesh-3.9.9/trimesh/permutate.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/points.py` & `trimesh-3.9.9/trimesh/points.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/poses.py` & `trimesh-3.9.9/trimesh/poses.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/primitives.py` & `trimesh-3.9.9/trimesh/primitives.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/proximity.py` & `trimesh-3.9.9/trimesh/proximity.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/ray/ray_pyembree.py` & `trimesh-3.9.9/trimesh/ray/ray_pyembree.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/ray/ray_triangle.py` & `trimesh-3.9.9/trimesh/ray/ray_triangle.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/ray/ray_util.py` & `trimesh-3.9.9/trimesh/ray/ray_util.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/registration.py` & `trimesh-3.9.9/trimesh/registration.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/remesh.py` & `trimesh-3.9.9/trimesh/remesh.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/rendering.py` & `trimesh-3.9.9/trimesh/rendering.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/repair.py` & `trimesh-3.9.9/trimesh/repair.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/resolvers.py` & `trimesh-3.9.9/trimesh/resolvers.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/resources/__init__.py` & `trimesh-3.9.9/trimesh/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/resources/blender_boolean.py.template` & `trimesh-3.9.9/trimesh/resources/blender_boolean.py.template`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/resources/blender_unwrap.py.template` & `trimesh-3.9.9/trimesh/resources/blender_unwrap.py.template`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/resources/dxf.json.template` & `trimesh-3.9.9/trimesh/resources/dxf.json.template`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/resources/gltf_2_schema.zip` & `trimesh-3.9.9/trimesh/resources/gltf_2_schema.zip`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/resources/units_to_inches.json` & `trimesh-3.9.9/trimesh/resources/units_to_inches.json`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/resources/viewer.template.zip` & `trimesh-3.9.9/trimesh/resources/viewer.template.zip`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/sample.py` & `trimesh-3.9.9/trimesh/sample.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/scene/cameras.py` & `trimesh-3.9.9/trimesh/scene/cameras.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/scene/lighting.py` & `trimesh-3.9.9/trimesh/scene/lighting.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/scene/scene.py` & `trimesh-3.9.9/trimesh/scene/scene.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,54 +92,56 @@
             geometry.apply_transform(transform)
 
     def add_geometry(self,
                      geometry,
                      node_name=None,
                      geom_name=None,
                      parent_node_name=None,
-                     transform=None):
+                     transform=None,
+                     extras=None):
         """
         Add a geometry to the scene.
 
         If the mesh has multiple transforms defined in its
         metadata, they will all be copied into the
         TransformForest of the current scene automatically.
 
         Parameters
         ----------
         geometry : Trimesh, Path2D, Path3D PointCloud or list
           Geometry to initially add to the scene
-        base_frame : str or hashable
-          Name of base frame
-        metadata : dict
-          Any metadata about the scene
-        graph : TransformForest or None
-          A passed transform graph to use
+        node_name: Name of the added node.
+        geom_name: Name of the added geometry.
+        parent_node_name: Name of the parent node in the graph.
+        transform: Transform that applies to the added node.
+        extras: Optional metadata for the node.
 
         Returns
         ----------
         node_name : str
-          Name of node in self.graph
+          Name of single node in self.graph (passed in) or None if
+          node was not added (eg. geometry was null or a Scene).
         """
 
         if geometry is None:
             return
         # PointCloud objects will look like a sequence
         elif util.is_sequence(geometry):
             # if passed a sequence add all elements
             return [self.add_geometry(
                 geometry=value,
                 node_name=node_name,
                 geom_name=geom_name,
                 parent_node_name=parent_node_name,
-                transform=transform) for value in geometry]
+                transform=transform,
+                extras=extras) for value in geometry]
         elif isinstance(geometry, dict):
             # if someone passed us a dict of geometry
             for key, value in geometry.items():
-                self.add_geometry(value, geom_name=key)
+                self.add_geometry(value, geom_name=key, extras=extras)
             return
         elif isinstance(geometry, Scene):
             # concatenate current scene with passed scene
             concat = self + geometry
             # replace geometry in-place
             self.geometry.clear()
             self.geometry.update(concat.geometry)
@@ -186,15 +188,17 @@
             # create an identity transform from parent_node
             transform = np.eye(4)
 
         self.graph.update(frame_to=node_name,
                           frame_from=parent_node_name,
                           matrix=transform,
                           geometry=name,
-                          geometry_flags={'visible': True})
+                          geometry_flags={'visible': True},
+                          extras=extras)
+
         return node_name
 
     def delete_geometry(self, names):
         """
         Delete one more multiple geometries from the scene and also
         remove any node in the transform graph which references it.
```

### Comparing `trimesh-3.9.8/trimesh/scene/transforms.py` & `trimesh-3.9.9/trimesh/scene/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,17 @@
           Axis of rotation
         angle :  float
           Angle of rotation, in radians
         translation : (3,) float
           Distance to translate
         geometry : hashable
           Geometry object name, e.g. 'mesh_0'
+        extras: dictionary
+          Optional metadata attached to the new frame
+          (expors to glTF node 'extras').
         """
 
         self._updated = str(np.random.random())
         self._cache.clear()
 
         # if no frame specified, use base frame
         if frame_from is None:
@@ -68,24 +71,28 @@
 
         # create the edge attributes
         attr = {'matrix': matrix, 'time': time.time()}
         # pass through geometry to edge attribute
         if 'geometry' in kwargs:
             attr['geometry'] = kwargs['geometry']
 
+        if 'extras' in kwargs:
+            attr['extras'] = kwargs['extras']
+
         # add the edges
         changed = self.transforms.add_edge(frame_from,
                                            frame_to,
                                            **attr)
         # set the node attribute with the geometry information
         if 'geometry' in kwargs:
             nx.set_node_attributes(
                 self.transforms,
                 name='geometry',
                 values={frame_to: kwargs['geometry']})
+
         # if the edge update changed our structure
         # dump our cache of shortest paths
         if changed:
             self._paths = {}
 
     def md5(self):
         return self._updated
@@ -167,25 +174,34 @@
                 info['children'] = children
             # if we have a mesh store by index
             if 'geometry' in node_data[node]:
                 info['mesh'] = mesh_index[node_data[node]['geometry']]
             # check to see if we have camera node
             if node == scene.camera.name:
                 info['camera'] = 0
+
             try:
                 # try to ignore KeyError and StopIteration
                 # parent-child transform is stored in child
                 parent = next(iter(graph.predecessors(node)))
                 # get the (4, 4) homogeneous transform
                 matrix = graph.get_edge_data(parent, node)['matrix']
                 # only include matrix if it is not an identity matrix
                 if np.abs(matrix - np.eye(4)).max() > 1e-5:
                     info['matrix'] = matrix.T.reshape(-1).tolist()
             except BaseException:
                 continue
+
+            try:
+                extras = graph.get_edge_data(parent, node)['extras']
+                if extras:
+                    info['extras'] = extras
+            except BaseException:
+                pass
+
         return {'nodes': result}
 
     def to_edgelist(self):
         """
         Export the current transforms as a list of
         edge tuples, with each tuple having the format:
         (node_a, node_b, {metadata})
```

### Comparing `trimesh-3.9.8/trimesh/schemas.py` & `trimesh-3.9.9/trimesh/schemas.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/smoothing.py` & `trimesh-3.9.9/trimesh/smoothing.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/transformations.py` & `trimesh-3.9.9/trimesh/transformations.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/triangles.py` & `trimesh-3.9.9/trimesh/triangles.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/units.py` & `trimesh-3.9.9/trimesh/units.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/unwrap.py` & `trimesh-3.9.9/trimesh/unwrap.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/util.py` & `trimesh-3.9.9/trimesh/util.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/viewer/__init__.py` & `trimesh-3.9.9/trimesh/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/viewer/notebook.py` & `trimesh-3.9.9/trimesh/viewer/notebook.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/viewer/trackball.py` & `trimesh-3.9.9/trimesh/viewer/trackball.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/viewer/widget.py` & `trimesh-3.9.9/trimesh/viewer/widget.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/viewer/windowed.py` & `trimesh-3.9.9/trimesh/viewer/windowed.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/visual/__init__.py` & `trimesh-3.9.9/trimesh/visual/__init__.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/visual/base.py` & `trimesh-3.9.9/trimesh/visual/base.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/visual/color.py` & `trimesh-3.9.9/trimesh/visual/color.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/visual/material.py` & `trimesh-3.9.9/trimesh/visual/material.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/visual/objects.py` & `trimesh-3.9.9/trimesh/visual/objects.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/visual/texture.py` & `trimesh-3.9.9/trimesh/visual/texture.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/voxel/base.py` & `trimesh-3.9.9/trimesh/voxel/base.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/voxel/creation.py` & `trimesh-3.9.9/trimesh/voxel/creation.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/voxel/encoding.py` & `trimesh-3.9.9/trimesh/voxel/encoding.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/voxel/morphology.py` & `trimesh-3.9.9/trimesh/voxel/morphology.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/voxel/ops.py` & `trimesh-3.9.9/trimesh/voxel/ops.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/voxel/runlength.py` & `trimesh-3.9.9/trimesh/voxel/runlength.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh/voxel/transforms.py` & `trimesh-3.9.9/trimesh/voxel/transforms.py`

 * *Files identical despite different names*

### Comparing `trimesh-3.9.8/trimesh.egg-info/PKG-INFO` & `trimesh-3.9.9/trimesh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trimesh
-Version: 3.9.8
+Version: 3.9.9
 Summary: Import, export, process, analyze and view triangular meshes.
 Home-page: https://github.com/mikedh/trimesh
 Author: Michael Dawson-Haggerty
 Author-email: mikedh@kerfed.com
 License: MIT
 Description: [![trimesh](https://trimsh.org/images/logotype-a.svg)](http://trimsh.org)
```

### Comparing `trimesh-3.9.8/trimesh.egg-info/SOURCES.txt` & `trimesh-3.9.9/trimesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

