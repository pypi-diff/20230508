# Comparing `tmp/polymesh-0.0.8.tar.gz` & `tmp/polymesh-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polymesh-0.0.8.tar", last modified: Wed Nov  2 20:39:34 2022, max compression
+gzip compressed data, was "polymesh-0.0.9.tar", last modified: Thu Dec  1 09:26:34 2022, max compression
```

## Comparing `polymesh-0.0.8.tar` & `polymesh-0.0.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2022-11-02 20:39:34.216666 polymesh-0.0.8/
--rw-rw-rw-   0        0        0     1086 2021-11-30 20:14:54.000000 polymesh-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      151 2022-08-15 22:35:16.000000 polymesh-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3401 2022-11-02 20:39:34.215679 polymesh-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2164 2022-10-11 09:12:23.000000 polymesh-0.0.8/README.md
--rw-rw-rw-   0        0        0      110 2021-11-30 20:14:54.000000 polymesh-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       49 2022-10-20 10:39:41.000000 polymesh-0.0.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-11-02 20:39:34.217664 polymesh-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2213 2022-10-11 06:30:01.000000 polymesh-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-02 20:39:34.114663 polymesh-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-11-02 20:39:34.150662 polymesh-0.0.8/src/polymesh/
--rw-rw-rw-   0        0        0      395 2022-11-02 20:39:05.000000 polymesh-0.0.8/src/polymesh/__init__.py
--rw-rw-rw-   0        0        0     1193 2022-10-28 20:33:57.000000 polymesh-0.0.8/src/polymesh/abc.py
--rw-rw-rw-   0        0        0     4287 2022-10-14 16:41:06.000000 polymesh-0.0.8/src/polymesh/akwrap.py
--rw-rw-rw-   0        0        0     2281 2022-08-11 20:00:29.000000 polymesh-0.0.8/src/polymesh/base.py
--rw-rw-rw-   0        0        0    15909 2022-10-31 09:50:09.000000 polymesh-0.0.8/src/polymesh/cell.py
--rw-rw-rw-   0        0        0    10603 2022-11-02 15:41:02.000000 polymesh-0.0.8/src/polymesh/celldata.py
-drwxrwxrwx   0        0        0        0 2022-11-02 20:39:34.176662 polymesh-0.0.8/src/polymesh/cells/
--rw-rw-rw-   0        0        0      417 2022-07-29 19:44:35.000000 polymesh-0.0.8/src/polymesh/cells/__init__.py
--rw-rw-rw-   0        0        0    19413 2022-10-27 15:46:47.000000 polymesh-0.0.8/src/polymesh/cells/h27.py
--rw-rw-rw-   0        0        0     7171 2022-10-27 15:45:43.000000 polymesh-0.0.8/src/polymesh/cells/h8.py
--rw-rw-rw-   0        0        0     3742 2022-10-28 20:17:32.000000 polymesh-0.0.8/src/polymesh/cells/l2.py
--rw-rw-rw-   0        0        0     1597 2022-10-28 20:26:06.000000 polymesh-0.0.8/src/polymesh/cells/l3.py
--rw-rw-rw-   0        0        0     4263 2022-10-28 20:34:33.000000 polymesh-0.0.8/src/polymesh/cells/q4.py
--rw-rw-rw-   0        0        0     5715 2022-10-28 20:34:58.000000 polymesh-0.0.8/src/polymesh/cells/q9.py
--rw-rw-rw-   0        0        0     3939 2022-10-28 20:48:42.000000 polymesh-0.0.8/src/polymesh/cells/t3.py
--rw-rw-rw-   0        0        0     5641 2022-10-28 20:50:07.000000 polymesh-0.0.8/src/polymesh/cells/t6.py
--rw-rw-rw-   0        0        0     2264 2022-10-28 20:52:11.000000 polymesh-0.0.8/src/polymesh/cells/tet10.py
--rw-rw-rw-   0        0        0     2079 2022-10-28 20:51:18.000000 polymesh-0.0.8/src/polymesh/cells/tet4.py
--rw-rw-rw-   0        0        0     1227 2022-08-27 14:37:46.000000 polymesh-0.0.8/src/polymesh/config.py
--rw-rw-rw-   0        0        0      484 2022-10-11 09:14:45.000000 polymesh-0.0.8/src/polymesh/examples.py
--rw-rw-rw-   0        0        0     1510 2022-07-12 17:34:24.000000 polymesh-0.0.8/src/polymesh/extrude.py
--rw-rw-rw-   0        0        0    18714 2022-10-27 15:33:12.000000 polymesh-0.0.8/src/polymesh/grid.py
--rw-rw-rw-   0        0        0     1578 2022-09-29 17:49:07.000000 polymesh-0.0.8/src/polymesh/line.py
--rw-rw-rw-   0        0        0     2989 2022-10-04 06:36:34.000000 polymesh-0.0.8/src/polymesh/linedata.py
--rw-rw-rw-   0        0        0     1806 2022-08-11 20:01:27.000000 polymesh-0.0.8/src/polymesh/mesh1d.py
--rw-rw-rw-   0        0        0     4668 2022-11-02 12:49:49.000000 polymesh-0.0.8/src/polymesh/pointdata.py
--rw-rw-rw-   0        0        0    54105 2022-11-02 12:26:40.000000 polymesh-0.0.8/src/polymesh/polydata.py
--rw-rw-rw-   0        0        0     2552 2022-09-29 17:49:07.000000 polymesh-0.0.8/src/polymesh/polygon.py
--rw-rw-rw-   0        0        0     1967 2022-09-29 17:49:07.000000 polymesh-0.0.8/src/polymesh/polyhedron.py
--rw-rw-rw-   0        0        0     1113 2022-08-11 20:02:20.000000 polymesh-0.0.8/src/polymesh/pop.py
-drwxrwxrwx   0        0        0        0 2022-11-02 20:39:34.178662 polymesh-0.0.8/src/polymesh/recipes/
--rw-rw-rw-   0        0        0       47 2022-08-26 13:50:59.000000 polymesh-0.0.8/src/polymesh/recipes/__init__.py
--rw-rw-rw-   0        0        0     6796 2022-10-10 19:17:37.000000 polymesh-0.0.8/src/polymesh/recipes/recipes.py
-drwxrwxrwx   0        0        0        0 2022-11-02 20:39:34.184663 polymesh-0.0.8/src/polymesh/space/
--rw-rw-rw-   0        0        0      218 2022-07-29 19:43:16.000000 polymesh-0.0.8/src/polymesh/space/__init__.py
--rw-rw-rw-   0        0        0    15552 2022-10-30 17:44:57.000000 polymesh-0.0.8/src/polymesh/space/coordarray.py
--rw-rw-rw-   0        0        0     7122 2022-11-01 09:06:03.000000 polymesh-0.0.8/src/polymesh/space/frame.py
--rw-rw-rw-   0        0        0     2121 2022-08-15 17:01:57.000000 polymesh-0.0.8/src/polymesh/space/point.py
--rw-rw-rw-   0        0        0     9502 2022-08-14 21:21:37.000000 polymesh-0.0.8/src/polymesh/space/utils.py
-drwxrwxrwx   0        0        0        0 2022-11-02 20:39:34.187687 polymesh-0.0.8/src/polymesh/tet/
--rw-rw-rw-   0        0        0       48 2022-08-15 20:10:29.000000 polymesh-0.0.8/src/polymesh/tet/__init__.py
--rw-rw-rw-   0        0        0      875 2022-08-15 20:01:52.000000 polymesh-0.0.8/src/polymesh/tet/tetmesh.py
--rw-rw-rw-   0        0        0      509 2022-08-15 20:06:45.000000 polymesh-0.0.8/src/polymesh/tet/tetutils.py
--rw-rw-rw-   0        0        0     2396 2022-08-11 20:02:28.000000 polymesh-0.0.8/src/polymesh/tile.py
-drwxrwxrwx   0        0        0        0 2022-11-02 20:39:34.203709 polymesh-0.0.8/src/polymesh/topo/
--rw-rw-rw-   0        0        0       45 2022-06-20 19:19:52.000000 polymesh-0.0.8/src/polymesh/topo/__init__.py
--rw-rw-rw-   0        0        0    28178 2022-11-02 12:31:08.000000 polymesh-0.0.8/src/polymesh/topo/topo.py
--rw-rw-rw-   0        0        0     7454 2022-08-14 21:21:59.000000 polymesh-0.0.8/src/polymesh/topo/topoarray.py
--rw-rw-rw-   0        0        0     3314 2022-07-31 23:37:40.000000 polymesh-0.0.8/src/polymesh/topo/topodata.py
--rw-rw-rw-   0        0        0    12269 2022-10-30 19:01:53.000000 polymesh-0.0.8/src/polymesh/topo/tr.py
-drwxrwxrwx   0        0        0        0 2022-11-02 20:39:34.213666 polymesh-0.0.8/src/polymesh/tri/
--rw-rw-rw-   0        0        0       21 2022-08-16 19:33:25.000000 polymesh-0.0.8/src/polymesh/tri/__init__.py
--rw-rw-rw-   0        0        0     8689 2022-06-24 16:09:47.000000 polymesh-0.0.8/src/polymesh/tri/triang.py
--rw-rw-rw-   0        0        0     6739 2022-10-27 15:33:12.000000 polymesh-0.0.8/src/polymesh/tri/trimesh.py
--rw-rw-rw-   0        0        0    15226 2022-10-27 15:33:12.000000 polymesh-0.0.8/src/polymesh/tri/triutils.py
--rw-rw-rw-   0        0        0    27408 2022-11-02 15:40:43.000000 polymesh-0.0.8/src/polymesh/utils.py
--rw-rw-rw-   0        0        0     1108 2022-07-13 07:52:14.000000 polymesh-0.0.8/src/polymesh/voxelize.py
--rw-rw-rw-   0        0        0     3265 2022-02-11 21:32:01.000000 polymesh-0.0.8/src/polymesh/vtkcelltypes.py
--rw-rw-rw-   0        0        0     1951 2022-08-11 20:02:44.000000 polymesh-0.0.8/src/polymesh/vtkutils.py
-drwxrwxrwx   0        0        0        0 2022-11-02 20:39:34.164662 polymesh-0.0.8/src/polymesh.egg-info/
--rw-rw-rw-   0        0        0     3401 2022-11-02 20:39:34.000000 polymesh-0.0.8/src/polymesh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1687 2022-11-02 20:39:34.000000 polymesh-0.0.8/src/polymesh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-02 20:39:34.000000 polymesh-0.0.8/src/polymesh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-08-15 19:43:24.000000 polymesh-0.0.8/src/polymesh.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       47 2022-11-02 20:39:34.000000 polymesh-0.0.8/src/polymesh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-02 20:39:34.000000 polymesh-0.0.8/src/polymesh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       50 2022-10-27 15:33:12.000000 polymesh-0.0.8/test-requirements.txt
+drwxrwxrwx   0        0        0        0 2022-12-01 09:26:34.911609 polymesh-0.0.9/
+-rw-rw-rw-   0        0        0     1086 2022-09-19 20:52:09.000000 polymesh-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      151 2022-09-19 20:52:09.000000 polymesh-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3401 2022-12-01 09:26:34.910967 polymesh-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2164 2022-10-11 12:57:54.000000 polymesh-0.0.9/README.md
+-rw-rw-rw-   0        0        0      110 2022-09-19 20:52:09.000000 polymesh-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       71 2022-12-01 09:17:38.000000 polymesh-0.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2022-12-01 09:26:34.912150 polymesh-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2213 2022-09-19 20:52:09.000000 polymesh-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-01 09:26:34.846650 polymesh-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-12-01 09:26:34.871854 polymesh-0.0.9/src/polymesh/
+-rw-rw-rw-   0        0        0      395 2022-12-01 09:09:20.000000 polymesh-0.0.9/src/polymesh/__init__.py
+-rw-rw-rw-   0        0        0     1211 2022-11-24 15:40:06.000000 polymesh-0.0.9/src/polymesh/abc.py
+-rw-rw-rw-   0        0        0     4287 2022-10-12 18:15:56.000000 polymesh-0.0.9/src/polymesh/akwrap.py
+-rw-rw-rw-   0        0        0     2281 2022-11-29 18:43:50.000000 polymesh-0.0.9/src/polymesh/base.py
+-rw-rw-rw-   0        0        0    15884 2022-11-07 20:12:38.000000 polymesh-0.0.9/src/polymesh/cell.py
+-rw-rw-rw-   0        0        0    11437 2022-11-28 18:47:10.000000 polymesh-0.0.9/src/polymesh/celldata.py
+drwxrwxrwx   0        0        0        0 2022-12-01 09:26:34.896805 polymesh-0.0.9/src/polymesh/cells/
+-rw-rw-rw-   0        0        0      417 2022-09-19 20:52:09.000000 polymesh-0.0.9/src/polymesh/cells/__init__.py
+-rw-rw-rw-   0        0        0    19413 2022-11-02 21:12:44.000000 polymesh-0.0.9/src/polymesh/cells/h27.py
+-rw-rw-rw-   0        0        0     7171 2022-11-02 21:12:44.000000 polymesh-0.0.9/src/polymesh/cells/h8.py
+-rw-rw-rw-   0        0        0     3742 2022-11-02 21:12:45.000000 polymesh-0.0.9/src/polymesh/cells/l2.py
+-rw-rw-rw-   0        0        0     1597 2022-11-02 21:12:45.000000 polymesh-0.0.9/src/polymesh/cells/l3.py
+-rw-rw-rw-   0        0        0     4263 2022-11-02 21:12:45.000000 polymesh-0.0.9/src/polymesh/cells/q4.py
+-rw-rw-rw-   0        0        0     5715 2022-11-02 21:12:45.000000 polymesh-0.0.9/src/polymesh/cells/q9.py
+-rw-rw-rw-   0        0        0     3939 2022-11-02 21:12:45.000000 polymesh-0.0.9/src/polymesh/cells/t3.py
+-rw-rw-rw-   0        0        0     5641 2022-11-02 21:12:45.000000 polymesh-0.0.9/src/polymesh/cells/t6.py
+-rw-rw-rw-   0        0        0     2264 2022-11-02 21:12:45.000000 polymesh-0.0.9/src/polymesh/cells/tet10.py
+-rw-rw-rw-   0        0        0     2079 2022-11-02 21:12:45.000000 polymesh-0.0.9/src/polymesh/cells/tet4.py
+-rw-rw-rw-   0        0        0     1227 2022-09-19 20:52:09.000000 polymesh-0.0.9/src/polymesh/config.py
+-rw-rw-rw-   0        0        0      484 2022-09-26 08:10:28.000000 polymesh-0.0.9/src/polymesh/examples.py
+-rw-rw-rw-   0        0        0     1510 2022-09-19 20:52:09.000000 polymesh-0.0.9/src/polymesh/extrude.py
+-rw-rw-rw-   0        0        0    18714 2022-10-27 07:03:56.000000 polymesh-0.0.9/src/polymesh/grid.py
+-rw-rw-rw-   0        0        0     1578 2022-09-23 21:22:09.000000 polymesh-0.0.9/src/polymesh/line.py
+-rw-rw-rw-   0        0        0     2989 2022-09-26 08:36:27.000000 polymesh-0.0.9/src/polymesh/linedata.py
+-rw-rw-rw-   0        0        0     1806 2022-09-19 20:52:09.000000 polymesh-0.0.9/src/polymesh/mesh1d.py
+-rw-rw-rw-   0        0        0     4670 2022-11-30 06:57:57.000000 polymesh-0.0.9/src/polymesh/pointdata.py
+-rw-rw-rw-   0        0        0    57535 2022-11-29 20:09:50.000000 polymesh-0.0.9/src/polymesh/polydata.py
+-rw-rw-rw-   0        0        0     2552 2022-09-23 20:36:40.000000 polymesh-0.0.9/src/polymesh/polygon.py
+-rw-rw-rw-   0        0        0     1967 2022-09-23 21:19:18.000000 polymesh-0.0.9/src/polymesh/polyhedron.py
+-rw-rw-rw-   0        0        0     1113 2022-09-19 20:52:09.000000 polymesh-0.0.9/src/polymesh/pop.py
+drwxrwxrwx   0        0        0        0 2022-12-01 09:26:34.898573 polymesh-0.0.9/src/polymesh/recipes/
+-rw-rw-rw-   0        0        0       47 2022-09-19 20:52:09.000000 polymesh-0.0.9/src/polymesh/recipes/__init__.py
+-rw-rw-rw-   0        0        0     6796 2022-10-11 12:57:54.000000 polymesh-0.0.9/src/polymesh/recipes/recipes.py
+drwxrwxrwx   0        0        0        0 2022-12-01 09:26:34.901763 polymesh-0.0.9/src/polymesh/space/
+-rw-rw-rw-   0        0        0      218 2022-09-19 20:52:09.000000 polymesh-0.0.9/src/polymesh/space/__init__.py
+-rw-rw-rw-   0        0        0    17470 2022-11-24 19:35:58.000000 polymesh-0.0.9/src/polymesh/space/coordarray.py
+-rw-rw-rw-   0        0        0     7122 2022-11-02 21:12:46.000000 polymesh-0.0.9/src/polymesh/space/frame.py
+-rw-rw-rw-   0        0        0     2121 2022-09-19 20:52:09.000000 polymesh-0.0.9/src/polymesh/space/point.py
+-rw-rw-rw-   0        0        0    11598 2022-11-24 19:28:29.000000 polymesh-0.0.9/src/polymesh/space/utils.py
+drwxrwxrwx   0        0        0        0 2022-12-01 09:26:34.903771 polymesh-0.0.9/src/polymesh/tet/
+-rw-rw-rw-   0        0        0       48 2022-09-19 20:52:09.000000 polymesh-0.0.9/src/polymesh/tet/__init__.py
+-rw-rw-rw-   0        0        0      875 2022-09-19 20:52:09.000000 polymesh-0.0.9/src/polymesh/tet/tetmesh.py
+-rw-rw-rw-   0        0        0      509 2022-09-19 20:52:09.000000 polymesh-0.0.9/src/polymesh/tet/tetutils.py
+-rw-rw-rw-   0        0        0     2396 2022-09-19 20:52:09.000000 polymesh-0.0.9/src/polymesh/tile.py
+drwxrwxrwx   0        0        0        0 2022-12-01 09:26:34.907398 polymesh-0.0.9/src/polymesh/topo/
+-rw-rw-rw-   0        0        0       45 2022-09-19 20:52:09.000000 polymesh-0.0.9/src/polymesh/topo/__init__.py
+-rw-rw-rw-   0        0        0    28178 2022-11-29 12:58:58.000000 polymesh-0.0.9/src/polymesh/topo/topo.py
+-rw-rw-rw-   0        0        0     7454 2022-09-19 20:52:09.000000 polymesh-0.0.9/src/polymesh/topo/topoarray.py
+-rw-rw-rw-   0        0        0     3314 2022-09-19 20:52:09.000000 polymesh-0.0.9/src/polymesh/topo/topodata.py
+-rw-rw-rw-   0        0        0    12269 2022-11-02 21:12:46.000000 polymesh-0.0.9/src/polymesh/topo/tr.py
+drwxrwxrwx   0        0        0        0 2022-12-01 09:26:34.909979 polymesh-0.0.9/src/polymesh/tri/
+-rw-rw-rw-   0        0        0       21 2022-09-19 20:52:09.000000 polymesh-0.0.9/src/polymesh/tri/__init__.py
+-rw-rw-rw-   0        0        0     8689 2022-09-19 20:52:09.000000 polymesh-0.0.9/src/polymesh/tri/triang.py
+-rw-rw-rw-   0        0        0     6739 2022-10-27 07:05:36.000000 polymesh-0.0.9/src/polymesh/tri/trimesh.py
+-rw-rw-rw-   0        0        0    15226 2022-10-27 07:09:22.000000 polymesh-0.0.9/src/polymesh/tri/triutils.py
+-rw-rw-rw-   0        0        0    27293 2022-11-24 19:23:05.000000 polymesh-0.0.9/src/polymesh/utils.py
+-rw-rw-rw-   0        0        0     1108 2022-09-19 20:52:09.000000 polymesh-0.0.9/src/polymesh/voxelize.py
+-rw-rw-rw-   0        0        0     3265 2022-09-19 20:52:09.000000 polymesh-0.0.9/src/polymesh/vtkcelltypes.py
+-rw-rw-rw-   0        0        0     1951 2022-09-19 20:52:09.000000 polymesh-0.0.9/src/polymesh/vtkutils.py
+drwxrwxrwx   0        0        0        0 2022-12-01 09:26:34.887858 polymesh-0.0.9/src/polymesh.egg-info/
+-rw-rw-rw-   0        0        0     3401 2022-12-01 09:26:34.000000 polymesh-0.0.9/src/polymesh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1687 2022-12-01 09:26:34.000000 polymesh-0.0.9/src/polymesh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-01 09:26:34.000000 polymesh-0.0.9/src/polymesh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-23 18:24:23.000000 polymesh-0.0.9/src/polymesh.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       69 2022-12-01 09:26:34.000000 polymesh-0.0.9/src/polymesh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2022-12-01 09:26:34.000000 polymesh-0.0.9/src/polymesh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       50 2022-10-27 07:52:55.000000 polymesh-0.0.9/test-requirements.txt
```

### Comparing `polymesh-0.0.8/LICENSE` & `polymesh-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/PKG-INFO` & `polymesh-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: polymesh
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package to build, manipulate and analyze polygonal meshes.
 Home-page: https://github.com/dewloosh/PolyMesh
 Author: dewloosh
 Author-email: dewloosh@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/dewloosh/PolyMesh/archive/refs/tags/0.0.8.zip
+Download-URL: https://github.com/dewloosh/PolyMesh/archive/refs/tags/0.0.9.zip
 Description: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dewloosh/PolyMesh/main?labpath=notebooks%5Cgrid.ipynb)
         [![CircleCI](https://circleci.com/gh/dewloosh/PolyMesh.svg?style=shield)](https://circleci.com/gh/dewloosh/PolyMesh) 
         [![Documentation Status](https://readthedocs.org/projects/polymesh/badge/?version=latest)](https://polymesh.readthedocs.io/en/latest/?badge=latest) 
         [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
         [![PyPI](https://badge.fury.io/py/PolyMesh.svg)](https://pypi.org/project/PolyMesh) 
         
         # **PolyMesh** - A Python Library for Compound Meshes with Jagged Topology
```

### Comparing `polymesh-0.0.8/README.md` & `polymesh-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/setup.py` & `polymesh-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/abc.py` & `polymesh-0.0.9/src/polymesh/abc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-from typing import Callable
 from dewloosh.core.meta import ABCMeta_Weak
 
 
 class ABCMeta_MeshData(ABCMeta_Weak):
     """
     Meta class for PointData and CellData classes.
     
@@ -23,15 +22,16 @@
         for base in bases:
             _attr_map_.update(base.__dict__.get('_attr_map_', {}))
         cls._attr_map_ = _attr_map_
         
         # generate shape functions
         shpfnc = namespace.get('shpfnc', None)
         if shpfnc is None:
-            cls.pina=True
+            # shape functions should be generated here
+            pass
         return cls
     
     
 class ABC_MeshData(metaclass=ABCMeta_MeshData):
     """Helper class that provides a standard way to create an ABC using
     inheritance.
     """
```

### Comparing `polymesh-0.0.8/src/polymesh/akwrap.py` & `polymesh-0.0.9/src/polymesh/akwrap.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/base.py` & `polymesh-0.0.9/src/polymesh/base.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/cell.py` & `polymesh-0.0.9/src/polymesh/cell.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Tuple, List, Callable
 
 import numpy as np
 from numpy import ndarray
 from sympy import Matrix, lambdify
 
 from neumann.array import atleast1d, ascont
-from neumann.utils import to_range
+from neumann.utils import to_range_1d
 
 from .celldata import CellData
 from .utils import (jacobian_matrix_bulk, points_of_cells,
                     pcoords_to_coords_1d, cells_coords)
 from .tri.triutils import area_tri_bulk
 from .tet.tetutils import tet_vol_bulk
 from .vtkutils import mesh_to_UnstructuredGrid as mesh_to_vtk
@@ -174,15 +174,15 @@
     def jacobian_matrix(self, *args, dshp=None, ecoords=None, topo=None, **kwargs):
         """
         Returns the jacobian matrix.
 
         Parameters
         ----------
         dshp : numpy.ndarray
-            2d array of shape function derivatives for the master cell.
+            3d array of shape function derivatives for the master cell.
 
         ecoords : numpy.ndarray, Optional
             3d array of nodal coordinates for all cells. 
             Either 'ecoords' or 'topo' must be provided.
 
         topo : numpy.ndarray, Optional
             2d integer topology array.
@@ -211,15 +211,15 @@
             Forwarded to :func:`jacobian_matrix` if the jacobian
             is not provided by the parameter 'jac'.
 
         Returns
         -------
         float or numpy.ndarray
             Value of the Jacobian for one or more cells.
-            
+
         See Also
         --------
         :func:`jacobian_matrix`
 
         """
         if jac is None:
             jac = self.jacobian_matrix(**kwargs)
@@ -357,16 +357,16 @@
 
         if points is None:
             points = np.array(self.lcoords()).flatten()
             rng = [-1, 1]
         else:
             rng = np.array([0, 1]) if rng is None else np.array(rng)
 
-        points, rng = to_range(points, source=rng, target=[
-                               0, 1]).flatten(), [0, 1]
+        points, rng = to_range_1d(points, source=rng, target=[
+            0, 1]).flatten(), [0, 1]
         datacoords = pcoords_to_coords_1d(points, ecoords)  # (nE * nP, nD)
 
         if not flatten:
             nE = ecoords.shape[0]
             nP = points.shape[0]
             datacoords = datacoords.reshape(
                 nE, nP, datacoords.shape[-1])  # (nE, nP, nD)
```

### Comparing `polymesh-0.0.8/src/polymesh/celldata.py` & `polymesh-0.0.9/src/polymesh/celldata.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 import numpy as np
 from numpy import ndarray
 
+from dewloosh.core import classproperty
 from neumann.array import atleast2d, atleast3d, repeat
 
 from .base import PointDataBase, CellDataBase, PolyDataBase as PolyData
 from .utils import (avg_cell_data, distribute_nodal_data_bulk,
                     homogenize_nodal_values)
 
 
@@ -27,15 +28,15 @@
         'ndf': 'ndf',  # nodal distribution factors
         'id': 'id',  # global indices of the cells
         'areas': 'areas',  # areas of 1d cells
         't': 't',  # thicknesses for 2d cells
         'activity': 'activity',  # activity of the cells
         'ndf': 'ndf',  # nodal distribution factors
     }
-
+    
     def __init__(self, *args, pointdata=None, celldata=None,
                  wrap=None, topo=None, fields=None, frames=None,
                  db=None, activity=None, container: PolyData = None, **kwargs):
         amap = self.__class__._attr_map_
         fields = {} if fields is None else fields
         assert isinstance(fields, dict)
 
@@ -66,15 +67,43 @@
         self.pointdata = pointdata
         self._container = container
 
         if self.db is not None:
             if isinstance(frames, ndarray):
                 # this handles possible repetition of a single frame
                 self.frames = frames
-
+    
+    @classproperty
+    def _dbkey_nodes_(cls) -> str:
+        return cls._attr_map_['nodes']
+    
+    @classproperty
+    def _dbkey_frames_(cls) -> str:
+        return cls._attr_map_['frames']
+    
+    @classproperty
+    def _dbkey_areas_(cls) -> str:
+        return cls._attr_map_['areas']
+    
+    @classproperty
+    def _dbkey_thickness_(cls) -> str:
+        return cls._attr_map_['t']
+    
+    @classproperty
+    def _dbkey_activity_(cls) -> str:
+        return cls._attr_map_['activity']
+    
+    @classproperty
+    def _dbkey_ndf_(cls) -> str:
+        return cls._attr_map_['ndf']
+    
+    @classproperty
+    def _dbkey_id_(cls) -> str:
+        return cls._attr_map_['id']
+    
     @property
     def pd(self) -> PointDataBase:
         """
         Returns the attached point database. This is what
         the topology of the cells are referring to.
         """
         return self.pointdata
@@ -110,32 +139,35 @@
         return None if c is None else c.root()
 
     def source(self) -> PolyData:
         c = self.container
         return None if c is None else c.source()
 
     def __getattr__(self, attr):
+        """
+        Modified for being able to fetch data from pointcloud.
+        """
         if attr in self.__dict__:
             return getattr(self, attr)
         try:
             return getattr(self._wrapped, attr)
         except AttributeError:
             try:
                 if self.pointdata is not None:
                     if attr in self.pointdata.fields:
                         data = self.pointdata[attr].to_numpy()
                         topo = self.nodes
                         return avg_cell_data(data, topo)
             except:
                 pass
-            raise AttributeError("'{}' object has no attribute \
-                called {}".format(self.__class__.__name__, attr))
+            name = self.__class__.__name__
+            raise AttributeError(f"'{name}' object has no attribute called {attr}")
         except Exception:
-            raise AttributeError("'{}' object has no attribute \
-                called {}".format(self.__class__.__name__, attr))
+            name = self.__class__.__name__
+            raise AttributeError(f"'{name}' object has no attribute called {attr}")
 
     def set_nodal_distribution_factors(self, factors: ndarray, key: str = None):
         """
         Sets nodal distribution factors.
 
         Parameters
         ----------
@@ -269,15 +301,15 @@
         value : numpy.ndarray
             A 3d float array.
 
         """
         assert isinstance(value, ndarray)
         value = atleast3d(value)
         if len(value) == 1:
-            value = repeat(value[0], len(self.celldata._wrapped))
+            value = repeat(value[0], len(self._wrapped))
         else:
             assert len(value) == len(self._wrapped)
         self._wrapped[self.__class__._attr_map_['frames']] = value
 
     @property
     def id(self) -> ndarray:
         """
```

### Comparing `polymesh-0.0.8/src/polymesh/cells/h27.py` & `polymesh-0.0.9/src/polymesh/cells/h27.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/cells/h8.py` & `polymesh-0.0.9/src/polymesh/cells/h8.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/cells/l2.py` & `polymesh-0.0.9/src/polymesh/cells/l2.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/cells/l3.py` & `polymesh-0.0.9/src/polymesh/cells/l3.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/cells/q4.py` & `polymesh-0.0.9/src/polymesh/cells/q4.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/cells/q9.py` & `polymesh-0.0.9/src/polymesh/cells/q9.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/cells/t3.py` & `polymesh-0.0.9/src/polymesh/cells/t3.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/cells/t6.py` & `polymesh-0.0.9/src/polymesh/cells/t6.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/cells/tet10.py` & `polymesh-0.0.9/src/polymesh/cells/tet10.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/cells/tet4.py` & `polymesh-0.0.9/src/polymesh/cells/tet4.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/config.py` & `polymesh-0.0.9/src/polymesh/config.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/extrude.py` & `polymesh-0.0.9/src/polymesh/extrude.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/grid.py` & `polymesh-0.0.9/src/polymesh/grid.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/line.py` & `polymesh-0.0.9/src/polymesh/line.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/linedata.py` & `polymesh-0.0.9/src/polymesh/linedata.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/mesh1d.py` & `polymesh-0.0.9/src/polymesh/mesh1d.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/pointdata.py` & `polymesh-0.0.9/src/polymesh/pointdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 import numpy as np
 from numpy import ndarray
 
 from neumann.linalg import ReferenceFrame as FrameLike
-from neumann.array import isboolarray
+from neumann.logical import isboolarray
 
 from .space import CartesianFrame, PointCloud
 from .base import PointDataBase
 
 
 def gen_frame(coords): return CartesianFrame(dim=coords.shape[1])
```

### Comparing `polymesh-0.0.8/src/polymesh/polydata.py` & `polymesh-0.0.9/src/polymesh/polydata.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 from copy import copy, deepcopy
 from typing import Union, Hashable, Collection, Iterable, Tuple
 from numpy import ndarray
 import numpy as np
 import awkward as ak
 from awkward import Array as akarray
 import functools
+import warnings
 
+from dewloosh.core.warning import PerformanceWarning
 from linkeddeepdict import DeepDict
 from neumann.linalg.sparse import JaggedArray
 from neumann.linalg import Vector, ReferenceFrame as FrameLike
 from neumann.linalg.vector import VectorBase
-from neumann.array import atleastnd, minmax
+from neumann.array import atleast1d, atleastnd, minmax
 
 from .akwrap import AkWrapper
 from .topo.topo import inds_to_invmap_as_dict, remap_topo_1d
 from .space import CartesianFrame, PointCloud
 from .utils import cells_coords, cells_around, cell_centers_bulk
 from .utils import k_nearest_neighbours as KNN
 from .vtkutils import mesh_to_UnstructuredGrid as mesh_to_vtk, PolyData_to_mesh
@@ -61,15 +63,15 @@
 __all__ = ['PolyData']
 
 
 class PolyData(PolyDataBase):
     """
     A class to handle complex polygonal meshes.
 
-    The `PolyData` class is arguably the most important class in the library 
+    The `PolyData` class is the most important class in the library 
     and a backbone of all mesh classes. 
 
     The implementation is based on the `awkward` library, which provides 
     memory-efficient, numba-jittable data classes to deal with dense, sparse, 
     complete or incomplete data. These data structures are managed in pure
     Python by the `DeepDict` class.
 
@@ -81,21 +83,14 @@
     ----------
     pd : PolyData or CellData, Optional
         A PolyData or a CellData instance. Dafault is None.
 
     cd : CellData, Optional
         A CellData instance, if the first argument is provided. Dafault is None.
 
-    coords : ndarray, Optional.
-        2d numpy array of floats, describing a pointcloud. Default is None.
-
-    topo : ndarray, Optional.
-        2d numpy array of integers, describing the topology of a polygonal mesh. 
-        Default is None.
-
     celltype : int, Optional.
         An integer spcifying a valid celltype.
 
     Examples
     --------
     >>> from polymesh import PolyData, PointData
     >>> from polymesh.grid import grid
@@ -145,14 +140,16 @@
                  point_fields: dict = None, parent: 'PolyData' = None, **kwargs):
         self._reset_point_data()
         self._reset_cell_data()
         self._frame = frame
         self._newaxis = newaxis
         self._parent = parent
         self._config = DeepDict()
+        self._cid2bid = None  # maps cell indices to block indices
+        self._bid2b = None  # maps block indices to block addresses
         self._init_config_()
 
         self.point_index_manager = IndexManager()
         self.cell_index_manager = IndexManager()
 
         if isinstance(pd, PointData):
             self.pointdata = pd
@@ -303,26 +300,111 @@
                         b[k] = v
 
         result.__dict__.update(self.__dict__)
         return result
 
     @property
     def pd(self) -> PointData:
-        """Returns the attached pointdata."""
+        """
+        Returns the attached pointdata.
+        """
         return self.pointdata
 
     @property
     def cd(self) -> PolyCell:
-        """Returns the attached celldata."""
+        """
+        Returns the attached celldata.
+        """
         return self.celldata
+    
+    def lock(self, create_mappers:bool=False) -> 'PolyData':
+        """
+        Locks the layout. If a `PolyData` instance is locked,
+        missing keys are handled the same way as they would've been handled
+        if it was a ´dict´. Also, setting or deleting items in a locked
+        dictionary and not possible and you will experience an error upon trying.
+        
+        The object is returned for continuation.
+        
+        Parameters
+        ----------
+        create_mappers : bool, Optional
+            If True, some mappers are generated to speed up certain types of
+            searches, like finding a block containing cells based on their indices.
+            
+            .. versionadded:: 0.0.9
+                            
+        """
+        if not self._locked and create_mappers:
+            bid2b, cid2bid = self._create_mappers_()
+            self._cid2bid = cid2bid  # maps cell indices to block indices
+            self._bid2b = bid2b  # maps block indices to block addresses
+        self._locked = True
+        return self
 
-    def simplify(self, inplace=True):
-        # generalization of triangulation
-        # cells should be broken into simplest representations
-        raise NotImplementedError
+    def unlock(self) -> 'PolyData':
+        """
+        Releases the layout. If a `PolyMesh` instance is not locked,
+        a missing key creates a new level in the layout, also setting and deleting
+        items becomes an option. Additionally, mappers created with the call
+        `generate_cell_mappers` are deleted.
+        
+        The object is returned for continuation.
+        
+        """
+        self._locked = False
+        self._cid2bid = None  # maps cell indices to block indices
+        self._bid2b = None  # maps block indices to block addresses
+        return self
+        
+    def blocks_of_cells(self, i : Union[int, Iterable]=None) -> dict:
+        """
+        Returns a dictionary that maps cell indices to blocks or 
+        block addresses.
+        
+        .. versionadded:: 0.0.9
+        
+        """
+        assert self.is_root(), "This must be called on the root object."
+        if self._cid2bid is None:
+            warnings.warn(
+                "Calling 'obj.lock(create_mappers=True)' creates additional"
+                " mappers that make lookups like this much more efficient. "
+                "See the doc of the PolyMesh library for more details.", 
+                PerformanceWarning)
+            bid2b, cid2bid = self._create_mappers_()
+        else:
+            cid2bid = self._cid2bid
+            bid2b = self._bid2b
+        if i is None:
+            return {cid : bid2b[bid] for cid, bid in cid2bid.items()}
+        cids = atleast1d(i)
+        bids = [cid2bid[cid] for cid in cids]
+        cid2b = {cid : bid2b[bid] for cid, bid in zip(cids, bids)}
+        return cid2b
+               
+    def _create_mappers_(self) -> Tuple[dict, dict]:
+        """
+        Generates mappers between cells and blocks to speed up some
+        queries. This can only be called on the root object.
+        The object is returned for continuation.
+        """
+        assert self.is_root(), "This must be called on the root object."
+        bid2b = {}  # block index to block address
+        cids = []  # cell indices
+        bids = []  # block infices of cells
+        for bid, b in enumerate(self.cellblocks(inclusive=True)):
+            b.id = bid
+            bid2b[bid] = b
+            cids.append(b.cd.id)
+            bids.append(np.full(len(b.cd), bid))
+        cids = np.concatenate(cids)
+        bids = np.concatenate(bids)
+        cid2bid = {cid : bid for cid, bid in zip(cids, bids)}
+        return bid2b, cid2bid
 
     def __deepcopy__(self, memo):
         return self.__copy__(memo)
 
     @classmethod
     def read(cls, *args, **kwargs) -> 'PolyData':
         """Reads from a file using PyVista."""
@@ -379,14 +461,15 @@
     def from_dict(cls, d_in: dict) -> Tuple[dict, 'PolyData']:
         """
         Reads a mesh form a dictionary. Returns a decorated version
         of the input dictionary and a `PolyData` instance.
 
         It must be implemented in subclasses. An example is 
         :class:`sigmaepsilon.solid.fem.linemesh.BernoulliFrame`
+        
         """
         raise NotImplementedError
 
     def to_pandas(self, *args, fields: Iterable[str] = None, **kwargs):
         """
         Returns the data contained within the mesh to pandas dataframes.
 
@@ -932,15 +1015,15 @@
                 assert cd is not None
                 pd[addr[l0:]] = PolyData(None, cd)
                 assert pd[addr[l0:]].celldata is not None
         if nummrg:
             pd.nummrg()
         return pd
 
-    def nummrg(self, store_indices=True):
+    def nummrg(self, store_indices:bool=True):
         """
         Merges node numbering.
         """
         if not self.is_root():
             self.root().nummrg()
             return self
         topo = self.topology()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `polymesh-0.0.8/src/polymesh/polygon.py` & `polymesh-0.0.9/src/polymesh/polygon.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/polyhedron.py` & `polymesh-0.0.9/src/polymesh/polyhedron.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/pop.py` & `polymesh-0.0.9/src/polymesh/pop.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/recipes/recipes.py` & `polymesh-0.0.9/src/polymesh/recipes/recipes.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/space/coordarray.py` & `polymesh-0.0.9/src/polymesh/space/coordarray.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from numba.core import types as nbtypes, cgutils
-from numba.extending import typeof_impl, models, \
-    make_attribute_wrapper, register_model, box, \
-    unbox, NativeValue, type_callable, lower_builtin,\
-    overload, overload_attribute
+from numba.extending import (typeof_impl, models,
+                             make_attribute_wrapper, register_model, box,
+                             unbox, NativeValue, type_callable, lower_builtin,
+                             overload, overload_attribute)
 import operator
 from typing import Union
 from numpy import ndarray
 import numpy as np
 from numba import njit, prange
 from typing import Union
 
@@ -15,15 +15,15 @@
 
 from neumann.array import minmax
 from neumann.linalg.vector import VectorBase, Vector
 from neumann.linalg.frame import ReferenceFrame as FrameLike
 
 from .frame import CartesianFrame
 from .point import Point
-from .utils import index_of_closest_point
+from .utils import index_of_closest_point, index_of_furthest_point
 
 __cache = True
 
 
 __all__ = ['PointCloud']
 
 
@@ -64,14 +64,15 @@
     inds : numpy.ndarray, Optional
         An 1d integer array specifying point indices. Default is None.
 
     Examples
     --------
     Collect the points of a simple triangulation and get the center:
 
+    >>> from polymesh.space import PointCloud
     >>> from polymesh.tri import triangulate
     >>> coords, *_ = triangulate(size=(800, 600), shape=(10, 10))
     >>> coords = PointCloud(coords)
     >>> coords.center()
         array([400., 300.,   0.])
 
     Centralize and get center again:
@@ -109,23 +110,23 @@
     (-400., 400.)
 
     The object keeps track of indices after slicing, always
     referring to the top level array:
 
     >>> coords[10:50][[1, 2, 10]].inds
     array([11, 12, 20])
-    
+
     The instances are available in numba-jitted functions:
-    
+
     >>> from numba import njit
-    
+
     >>> @njit
     >>> def foo(arr): 
     >>>     return arr.inds
-    
+
     >>> c = np.array([[0, 0, 0], [0, 0, 1.], [0, 0, 0]])
     >>> COORD = PointCloud(c, inds=np.array([0, 1, 2, 3]))
     >>> foo(COORD)
 
     """
 
     _array_cls_ = VectorBase
@@ -223,57 +224,81 @@
         ----------
 
         target : ReferenceFrame, Optional
             A frame of reference. Default is None.
 
         Returns
         -------
-        :class:`VectorBase`
+        VectorBase
             A numpy array.
 
         """
         arr = self.show(target)
         def foo(i): return np.mean(arr[:, i])
         return np.array(list(map(foo, range(self.shape[1]))))
 
     def id_of_closest(self, p: VectorLike, frame: FrameLike = None):
         """
         Returns the index of the point being closest to `p`.
 
         Parameters
         ----------
         p : Vector or Array, Optional
-            An array of a vector. If provided as an array, the `frame`
-            argument can be used to specify the parent frame in which the
-            motion is tp be understood.
+            Vectors or coordinates of one or more points. If provided as 
+            an array, the `frame` argument can be used to specify the 
+            parent frame in which the coordinates are to be understood.
 
         frame : ReferenceFrame, Optional
             A frame in which the input is defined if it is not a Vector.
             Default is None.
 
         Returns
         -------
         int
 
         """
         if not isinstance(p, Vector):
             p = Vector(p, frame=frame)
         return index_of_closest_point(self.show(), p.show())
+    
+    def id_of_furthest(self, p: VectorLike, frame: FrameLike = None):
+        """
+        Returns the index of the point being furthest from `p`.
+
+        Parameters
+        ----------
+        p : Vector or Array, Optional
+            Vectors or coordinates of one or more points. If provided as 
+            an array, the `frame` argument can be used to specify the 
+            parent frame in which the coordinates are to be understood.
+
+        frame : ReferenceFrame, Optional
+            A frame in which the input is defined if it is not a Vector.
+            Default is None.
+
+        Returns
+        -------
+        int
+
+        """
+        if not isinstance(p, Vector):
+            p = Vector(p, frame=frame)
+        return index_of_furthest_point(self.show(), p.show())
 
     def closest(self, p: VectorLike, frame: FrameLike = None) -> Point:
         """
         Returns the point being closest to `p`.
 
         Parameters
         ----------
 
         p : Vector or Array, Optional
-            An array of a vector. If provided as an array, the `frame`
-            argument can be used to specify the parent frame in which the
-            motion is tp be understood.
+            Vectors or coordinates of one or more points. If provided as 
+            an array, the `frame` argument can be used to specify the 
+            parent frame in which the coordinates are to be understood.
 
         frame : ReferenceFrame, Optional
             A frame in which the input is defined if it is not a Vector.
             Default is None.
 
         Returns
         -------
@@ -282,15 +307,50 @@
         """
         id = self.id_of_closest(p, frame)
         arr = self._array[id, :]
         if isinstance(self.inds, np.ndarray):
             gid = self.inds[id]
         else:
             gid = id
-        return Point(arr, frame=self.frame, id=id, gid=gid)
+        if isinstance(id, int):      
+            return Point(arr, frame=self.frame, id=id, gid=gid)
+        else:
+            return PointCloud(arr, frame=self.frame, inds=id)
+        
+    def furthest(self, p: VectorLike, frame: FrameLike = None) -> Point:
+        """
+        Returns the point being closest to `p`.
+
+        Parameters
+        ----------
+
+        p : Vector or Array, Optional
+            Vectors or coordinates of one or more points. If provided as 
+            an array, the `frame` argument can be used to specify the 
+            parent frame in which the coordinates are to be understood.
+
+        frame : ReferenceFrame, Optional
+            A frame in which the input is defined if it is not a Vector.
+            Default is None.
+
+        Returns
+        -------
+        Point
+
+        """
+        id = self.id_of_furthest(p, frame)
+        arr = self._array[id, :]
+        if isinstance(self.inds, np.ndarray):
+            gid = self.inds[id]
+        else:
+            gid = id
+        if isinstance(id, int):      
+            return Point(arr, frame=self.frame, id=id, gid=gid)
+        else:
+            return PointCloud(arr, frame=self.frame, inds=id)
 
     def show(self, target: FrameLike = None):
         """
         Returns the coordinates of the points in a specified frame, 
         or the root frame if there is no target provided.
 
         Parameters
@@ -509,18 +569,7 @@
         c.pyapi.serialize_object(PointCloud))
     data_obj = c.box(typ.data, native_obj.data)
     inds_obj = c.box(typ.inds, native_obj.inds)
     python_obj = c.pyapi.call_function_objargs(class_obj, (data_obj, inds_obj))
     c.pyapi.decref(data_obj)
     c.pyapi.decref(inds_obj)
     return python_obj
-
-
-if __name__ == '__main__':
-    from numba import njit
-
-    @njit
-    def foo(arr): return arr.inds
-
-    c = np.array([[0, 0, 0], [0, 0, 1.], [0, 0, 0]])
-    COORD = PointCloud(c, inds=np.array([0, 1, 2, 3]))
-    foo(COORD)
```

### Comparing `polymesh-0.0.8/src/polymesh/space/frame.py` & `polymesh-0.0.9/src/polymesh/space/frame.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/space/point.py` & `polymesh-0.0.9/src/polymesh/space/point.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/space/utils.py` & `polymesh-0.0.9/src/polymesh/space/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # -*- coding: utf-8 -*-
 import numpy as np
 from numpy import ndarray
+from numpy.linalg import norm
 from numba import njit, prange
 
 from neumann import squeeze
 from neumann.linalg import normalize, normalize2d, norm2d
 from neumann.array import atleast2d
 
 from ..utils import center_of_points, cell_center, cell_coords
-    
+
 __cache = True
 
 
 @njit(nogil=True, cache=__cache)
 def frame_of_plane(coords: ndarray):
     """
     Returns the frame of a planar surface. It needs
     at least 3 pointds to work properly (len(coords>=3)).
-    
+
     It takes the center, the first point and a point from
     the middle to form the coordinate axes.
-    
+
     Parameters
     ----------
     coords : numpy.ndarray
         2d coordinate array
 
     Returns
     -------        
     numpy.ndarray
         3x3 global -> local DCM matrix 
-        
+
     """
     tr = np.zeros((3, 3), dtype=coords.dtype)
     center = center_of_points(coords)
     tr[:, 0] = normalize(coords[0] - center)
     tr[:, 1] = normalize(coords[np.int(len(coords)/2)] - center)
     tr[:, 2] = normalize(np.cross(tr[:, 0], tr[:, 1]))
     tr[:, 1] = np.cross(tr[:, 2], tr[:, 0])
@@ -55,15 +56,15 @@
     topo : numpy.ndarray
         2d point-based topology array
 
     Returns
     -------       
     numpy.ndarray
         3d array of 3x3 transformation matrices
-        
+
     """
     nE, nNE = topo.shape
     nNE -= 1
     tr = np.zeros((nE, 3, 3), dtype=coords.dtype)
     for iE in prange(nE):
         tr[iE, 0, :] = normalize(coords[topo[iE, 1]] - coords[topo[iE, 0]])
         tr[iE, 1, :] = normalize(coords[topo[iE, nNE]] - coords[topo[iE, 0]])
@@ -94,15 +95,15 @@
         2d coordinate array of local coordinates
 
     numpy.ndarray
         2d array of cell centers
 
     numpy.ndarray
         3d array of 3x3 transformation matrices
-        
+
     """
     nE, nNE = topo.shape
     tr = np.zeros((nE, 3, 3), dtype=coords.dtype)
     res = np.zeros((nE, nNE, 2), dtype=coords.dtype)
     centers = np.zeros((nE, 3), dtype=coords.dtype)
     for iE in prange(nE):
         centers[iE] = cell_center(cell_coords(coords, topo[iE]))
@@ -124,15 +125,15 @@
     ijk = np.eye(3)
     tr = np.zeros((nE, 3, 3), dtype=coords.dtype)
     for iE in prange(nE):
         tr[iE, 0, :] = normalize(coords[topo[iE, nNE]] - coords[topo[iE, 0]])
         _dot = ijk @ tr[iE, 0, :]
         i2 = np.argmin(np.absolute(_dot))
         _dot = np.dot(ijk[i2], tr[iE, 0, :])
-        tr[iE, 2, :] = normalize(ijk[i2] - tr[iE, 0, :] * _dot)            
+        tr[iE, 2, :] = normalize(ijk[i2] - tr[iE, 0, :] * _dot)
         tr[iE, 1, :] = np.cross(tr[iE, 2, :], tr[iE, 0, :])
     return tr
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
 def _frames_of_lines_ref(coords: ndarray, topo: ndarray, refZ: ndarray):
     nE, nNE = topo.shape
@@ -143,66 +144,66 @@
         k = refZ[iE] - coords[topo[iE, 0]]
         tr[iE, 2, :] = normalize(k - tr[iE, 0, :] * np.dot(tr[iE, 0, :], k))
         tr[iE, 1, :] = np.cross(tr[iE, 2, :], tr[iE, 0, :])
     return tr
 
 
 @squeeze(True)
-def frames_of_lines(coords: ndarray, topo: ndarray, refZ: ndarray=None):
+def frames_of_lines(coords: ndarray, topo: ndarray, refZ: ndarray = None):
     """
     Returns coordinate frames of line elements defined by a coordinate array
     and a topology array. The cross-sections of the line elements are
     in the local y-z plane. The direction of the local z axis can be set by 
     providing reference points in the local x-z planes of the lines. If there
     are no references provided, local z axes lean towards global z. 
     Other properties are determined in a way, so that x-y-z form a 
     right-handed orthonormal basis.
-    
+
     Parameters
     ----------
     coords : numpy.ndarray
         2d coordinate array
 
     topo : numpy.ndarray
         2d point-based topology array
-        
+
     refZ : numpy.ndarray, Optional
         1d or 2d float array of reference points. If it is 2d, it must
         contain values for all lines defined by `topo`. 
         Default is None.
 
     Returns
     -------      
     numpy.ndarray
         3d array of 3x3 transformation matrices
-        
+
     """
     topo = atleast2d(topo)
     if isinstance(refZ, ndarray):
         if len(topo.shape) == 2 and len(refZ.shape) == 1:
             _refZ = np.zeros((topo.shape[0], 3))
             _refZ[:] = refZ
         else:
             _refZ = refZ
         return _frames_of_lines_ref(coords, topo, _refZ)
     else:
         return _frames_of_lines_auto(coords, topo)
-    
+
 
 @njit(nogil=True, parallel=True, cache=__cache)
-def is_planar_surface(normals: ndarray, tol=1e-8):
+def is_planar_surface(normals: ndarray, tol: float = 1e-8) -> bool:
     """
     Returns true if all the normals point in the same direction.
     The provided normal vectors are assumed to be normalized.
-    
+
     Parameters
     ----------
     normals : numpy.ndarray
         2d float array of surface normals
-        
+
     tol : float
         Floating point tolerance as maximum deviation.
 
     Returns
     -------       
     Bool
         True if the surfaces whose normal vectors are provided form
@@ -212,78 +213,148 @@
     diffs = np.zeros(nE, dtype=normals.dtype)
     for i in prange(1, nE):
         diffs[i] = np.abs(normals[i] @ normals[0] - 1)
     return diffs.max() <= tol
 
 
 @njit(nogil=True, cache=__cache)
-def distances_from_point(coords: ndarray, p: ndarray, normalize=False):
+def distances_from_point(coords: ndarray, p: ndarray,
+                         normalize: bool = False) -> ndarray:
     if normalize:
         return norm2d(normalize2d(coords - p))
     else:
         return norm2d(coords - p)
 
 
-@njit(nogil=True, cache=__cache)
-def index_of_furthest_point(coords: ndarray, p: ndarray):
-    return np.argmax(distances_from_point(coords, p))
+@njit(nogil=True, parallel=True, cache=__cache)
+def distance_matrix(x: ndarray, y: ndarray) -> ndarray:
+    N = x.shape[0]
+    M = y.shape[0]
+    res = np.zeros((N, M), dtype=x.dtype)
+    for n in prange(N):
+        for m in prange(M):
+            res[n, m] = np.linalg.norm(x[n] - y[m])
+    return res
+
+
+def index_of_closest_point(coords: ndarray, target: ndarray) -> int:
+    """
+    Returs the index of the point in 'coords', being closest to
+    one or more targets.
+
+    Parameters
+    ----------
+    coords : numpy.ndarray
+        2d float array of vertex coordinates.
+
+    target : numpy.ndarray
+        1d or 2d coordinate array of the target point(s).
+
+    Returns
+    -------
+    int or Iterable[int]
+        One or more indices of 'coords', for which the distance from
+        one or more points described by 'target' is minimal.
+
+    """
+    if len(target.shape) == 1:
+        assert coords.shape[1] == target.shape[0], \
+            "The dimensions of `coords` and `target` are not compatible."
+        return _index_of_closest_point(coords, target)
+    else:
+        d = distance_matrix(target, coords)
+        return np.argmin(d, axis=1)
+
+
+def index_of_furthest_point(coords: ndarray, target: ndarray) -> int:
+    """
+    Returs the index of the point in 'coords', being furthest from
+    one or more targets.
+
+    Parameters
+    ----------
+    coords : numpy.ndarray
+        2d float array of vertex coordinates.
+
+    target : numpy.ndarray
+        1d or 2d coordinate array of the target point(s).
+
+    Returns
+    -------
+    int or Iterable[int]
+        One or more indices of 'coords', for which the distance from
+        one or more points described by 'target' is maximal.
+
+    """
+    if len(target.shape) == 1:
+        assert coords.shape[1] == target.shape[0], \
+            "The dimensions of `coords` and `target` are not compatible."
+        return _index_of_furthest_point(coords, target)
+    else:
+        d = distance_matrix(target, coords)
+        return np.argmax(d, axis=1)
 
 
 @njit(nogil=True, cache=__cache)
-def index_of_closest_point(coords: ndarray, p: ndarray):
+def _index_of_closest_point(coords: ndarray, p: ndarray) -> int:
     return np.argmin(distances_from_point(coords, p))
 
 
+@njit(nogil=True, cache=__cache)
+def _index_of_furthest_point(coords: ndarray, p: ndarray) -> int:
+    return np.argmax(distances_from_point(coords, p))
+
+
 @njit(nogil=True, parallel=True, cache=__cache)
-def is_line(coords: ndarray, tol=1e-8):
+def is_line(coords: ndarray, tol=1e-8) -> bool:
     """
     Returns true if all the normals point in the same direction.
     The provided normal vectors are assumed to be normalized.
-    
+
     Parameters
     ----------
     coords : numpy.ndarray
         2d float array of point coordinates
-        
+
     tol : float
         Floating point tolerance as maximum deviation.
 
     Returns
     -------        
     Bool
         True if all absolute deviations from the line between the first 
         and the last point is smaller than 'tol'.
-        
+
     """
     nP = coords.shape[0]
     c = normalize2d(move_points(coords, -coords[0]))
     d = c[-1] - c[0]
     diffs = np.zeros(nP, dtype=coords.dtype)
     for i in prange(1, nP):
         diffs[i] = np.abs(c[i] @ d)
     return diffs.max() <= tol
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
-def is_planar(coords: ndarray, tol=1e-8):
+def is_planar(coords: ndarray, tol: float = 1e-8) -> bool:
     """
     Returns true if all the points fit on a planar surface.
-    
+
     Parameters
     ----------
     coords : numpy.ndarray
         2d float array of point coordinates
-        
+
     tol : float
         Floating point tolerance as maximum deviation.
 
     Returns
     -------        
     Bool
-                
+
     """
     nP = coords.shape[0]
     dA = distances_from_point(coords, coords[0])
     iB = np.argmax(dA)
     dB = distances_from_point(coords, coords[iB])
     iC = np.argmax(dA + dB)
     inds = np.array([0, iB, iC])
@@ -292,12 +363,12 @@
     diffs = np.zeros(nP, dtype=coords.dtype)
     for i in prange(1, nP):
         diffs[i] = np.abs(coords[i] @ d)
     return diffs.max() <= tol
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
-def move_points(coords: ndarray, p: ndarray):
+def move_points(coords: ndarray, p: ndarray) -> ndarray:
     res = np.zeros_like(coords)
     for i in prange(coords.shape[0]):
         res[i] = coords[i] + p
-    return res
+    return res
```

### Comparing `polymesh-0.0.8/src/polymesh/tet/tetmesh.py` & `polymesh-0.0.9/src/polymesh/tet/tetmesh.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/tile.py` & `polymesh-0.0.9/src/polymesh/tile.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/topo/topo.py` & `polymesh-0.0.9/src/polymesh/topo/topo.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/topo/topoarray.py` & `polymesh-0.0.9/src/polymesh/topo/topoarray.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/topo/topodata.py` & `polymesh-0.0.9/src/polymesh/topo/topodata.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/topo/tr.py` & `polymesh-0.0.9/src/polymesh/topo/tr.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/tri/triang.py` & `polymesh-0.0.9/src/polymesh/tri/triang.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/tri/trimesh.py` & `polymesh-0.0.9/src/polymesh/tri/trimesh.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/tri/triutils.py` & `polymesh-0.0.9/src/polymesh/tri/triutils.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/utils.py` & `polymesh-0.0.9/src/polymesh/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,122 +24,123 @@
 __cache = True
 
 nbint64 = nbtypes.int64
 nbint64A = nbint64[:]
 nbfloat64A = nbtypes.float64[:]
 
 
-def k_nearest_neighbours(X: ndarray, Y: ndarray=None, *args, backend='scipy', 
-                         k=1, workers=-1, tree_kwargs=None, query_kwargs=None, 
-                         leaf_size=30, return_distance=False, 
+def k_nearest_neighbours(X: ndarray, Y: ndarray = None, *args, backend='scipy',
+                         k=1, workers=-1, tree_kwargs=None, query_kwargs=None,
+                         leaf_size=30, return_distance=False,
                          max_distance=None, **kwargs):
     """
     Returns the k nearest neighbours (KNN) of a KDTree for a pointcloud using `scipy`
     or `sklearn`. The function acts as a uniform interface for similar functionality
     of `scipy` and `sklearn`. The most important parameters are highlighted, for the 
     complete list of arguments, see the corresponding docs:
-    
+
     https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.KDTree.html#scipy.spatial.KDTree
-        
+
     https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KDTree.html  
-    
+
     To learn more about nearest neighbour searches in general:
-    
+
     https://scikit-learn.org/stable/modules/neighbors.html
-    
+
     Parameters
     ----------
     X : numpy.ndarray
         An array of points to build the tree.
-        
+
     Y : numpy.ndarray, Optional
         An array of sampling points to query the tree. If None it is the
         same as the points used to build the tree. Default is None. 
-        
+
     k : int or Sequence[int], Optional
         Either the number of nearest neighbors to return, 
         or a list of the k-th nearest neighbors to return, starting from 1.
-    
+
     leaf_size : positive int, Optional
         The number of points at which the algorithm switches over to brute-force.
         Default is 10.
-    
+
     workers : int, Optional
         Only if backend is 'scipy'.
         Number of workers to use for parallel processing. If -1 is given all 
         CPU threads are used. Default: -1.
-        
+
         New in 'scipy' version 1.6.0.
-        
+
     max_distance : float, Optional
         Return only neighbors within this distance. It can be a single value, or 
         an array of values of shape matching the input, while a None value
         translates to an infinite upper bound.
         Default is None.
-        
+
     tree_kwargs : dict, Optional
         Extra keyword arguments passed to the KDTree creator of the selected
         backend. Default is None.
-                  
+
     Returns
     -------
     d : float or array of floats
         The distances to the nearest neighbors. Only returned if
         `return_distance==True`.
-        
+
     i : integer or array of integers
         The index of each neighbor.
-    
+
     Raises
     ------
     ImportError
         In the abscence of a usable backend.
-     
+
     Examples
     --------
     >>> from sigmaepsilon.mesh.grid import Grid
     >>> from sigmaepsilon.mesh import KNN
     >>> size = 80, 60, 20
     >>> shape = 10, 8, 4
     >>> grid = Grid(size=size, shape=shape, eshape='H8')
     >>> X = grid.centers()
     >>> i = KNN(X, X, k=3, max_distance=10.0)
-       
+
     """
     tree_kwargs = {} if tree_kwargs is None else tree_kwargs
     query_kwargs = {} if query_kwargs is None else query_kwargs
-    if backend=='scipy':
+    if backend == 'scipy':
         from scipy.spatial import KDTree
         tree = KDTree(X, leafsize=leaf_size, **tree_kwargs)
         max_distance = np.inf if max_distance is None else max_distance
         query_kwargs['distance_upper_bound'] = max_distance
         if version.parse(__scipy_version__) < version.parse("1.6.0"):
-            warnings.warn("Multithreaded execution of a KNN search is " + \
-                "running on a single thread in scipy<1.6.0. Install a newer" + \
-                "version or use `backend=sklearn` if scikit is installed.")
+            warnings.warn("Multithreaded execution of a KNN search is " +
+                          "running on a single thread in scipy<1.6.0. Install a newer" +
+                          "version or use `backend=sklearn` if scikit is installed.")
             d, i = tree.query(Y, k=k, **query_kwargs)
         else:
             d, i = tree.query(Y, k=k, workers=workers)
-    elif backend=='sklearn':
+    elif backend == 'sklearn':
         if not __has_sklearn__:
             raise ImportError("'sklearn' must be installed for this!")
         from sklearn.neighbors import KDTree
         tree = KDTree(X, leaf_size=leaf_size, **tree_kwargs)
         if max_distance is None:
             d, i = tree.query(Y, k=k, **query_kwargs)
         else:
             r = max_distance
             d, i = tree.query_radius(Y, r, k=k, **query_kwargs)
     else:
-        raise ImportError("Either `sklearn` or `scipy` must be present for this!")
+        raise ImportError(
+            "Either `sklearn` or `scipy` must be present for this!")
     return (d, i) if return_distance else i
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
-def knn_to_lines(inds : ndarray):
+def knn_to_lines(inds: ndarray):
     nN, nK = inds.shape
     res = np.zeros((nN, nK, 2), dtype=inds.dtype)
     for i in prange(nN):
         for j in prange(nK):
             res[i, j, 0] = i
             res[i, j, 1] = inds[i, j]
     return res
@@ -149,59 +150,59 @@
     """
     Alias for :func:`points_around`.
     """
     return points_around(*args, **kwargs)
 
 
 def points_around(points: np.ndarray, r_max: float, *args,
-                  frmt:str='dict', MT:bool=True, n_max:int=10, **kwargs):
+                  frmt: str = 'dict', MT: bool = True, n_max: int = 10, **kwargs):
     """
     Returns neighbouring points for each entry in `points` that are
     closer than the distance `r_max`. The results are returned in
     diffent formats, depending on the format specifier argument `frmt`.
-    
+
     Parameters
     ----------
     points : numpy.ndarray
         Coordinates of several points as a 2d float numpy array.
-        
+
     r_max : float
         Maximum distance.
-    
+
     n_max: int, Optional
         Maximum number of neighbours. Default is 10.
-        
+
     frmt : str
         A string specifying the output format. Valid options are
         'jagged', 'csr' and 'dict'. 
         See below for the details on the returned object.
-        
+
     Returns
     -------
     if frmt = 'csr' : dewloosh.math.linalg.sparse.csr.csr_matrix
         A numba-jittable sparse matrix format.                      
-    
+
     frmt = 'dict' : numba Dict(int : int[:])
-    
+
     frmt = 'jagged' : dewloosh.math.linalg.sparse.JaggedArray
         A subclass of `awkward.Array`
-   
+
     """
     if MT:
-        data, widths = _cells_around_MT_(points, r_max, n_max)    
+        data, widths = _cells_around_MT_(points, r_max, n_max)
     else:
         raise NotImplementedError
     if frmt == 'dict':
         return _cells_data_to_dict(data, widths)
     elif frmt == 'jagged':
         return _cells_data_to_jagged(data, widths)
     elif frmt == 'csr':
         d = _cells_data_to_dict(data, widths)
         data, inds, indptr, shp = _dict_to_spdata(d, widths)
-        return csr_matrix(data=data, indices=inds, 
+        return csr_matrix(data=data, indices=inds,
                           indptr=indptr, shape=shp)
     raise RuntimeError("Unhandled case!")
 
 
 @njit(nogil=True, cache=__cache)
 def _dict_to_spdata(d: dict, widths: np.ndarray):
     N = int(np.sum(widths))
@@ -257,15 +258,15 @@
 @njit(nogil=True, parallel=True, cache=__cache)
 def _flatten_jagged_data(data, widths) -> ndarray:
     nE = len(widths)
     inds = np.zeros(nE + 1, dtype=widths.dtype)
     inds[1:] = np.cumsum(widths)
     res = np.zeros(np.sum(widths))
     for i in prange(nE):
-        res[inds[i] : inds[i+1]] = data[i, :widths[i]]
+        res[inds[i]: inds[i+1]] = data[i, :widths[i]]
     return res
 
 
 def _cells_data_to_jagged(data, widths):
     data = _flatten_jagged_data(data, widths)
     return JaggedArray(data, cuts=widths)
 
@@ -283,138 +284,144 @@
         normsbuf[:] = norms(centers - centers[iE])
         res[iE] = np.where(normsbuf <= r_max)[0]
         widths[iE] = len(res[iE])
     return res, widths
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
-def _cells_around_MT_(centers: np.ndarray, r_max: float, n_max: int=10):
+def _cells_around_MT_(centers: np.ndarray, r_max: float, n_max: int = 10):
     nE = len(centers)
     res = np.zeros((nE, n_max), dtype=np.int64)
     widths = np.zeros(nE, dtype=np.int64)
     for iE in prange(nE):
         inds = np.where(norms(centers - centers[iE]) <= r_max)[0]
         if inds.shape[0] <= n_max:
             res[iE, :inds.shape[0]] = inds
         else:
             res[iE, :] = inds[:n_max]
         widths[iE] = len(res[iE])
     return res, widths
 
 
+# !FIXME : this is duplicated in polymesh.space.utils
 def index_of_closest_point(coords: ndarray, target: ndarray) -> int:
     """
     Returs the index of the closes point to a target location.
-    
+
     Parameters
     ----------
     coords : numpy.ndarray
         2d float array of (nP, nD) of vertex coordinates.
-        
+
         nP : number of points
-        
+
         nD : number of dimensions of the model space
-            
+
     target : numpy.ndarray
         Coordinate array of the target point.
 
     Returns
     -------
     int
         The index of 'coords', for which the distance from
         'target' is minimal.
-    
+
     """
+    warnings.warn("This is deprecated, use polymesh.space.index_of_closest_point instaead.",
+                  warnings.DeprecationWarning)
     assert coords.shape[1] == target.shape[0], \
         "The dimensions of `coords` and `target` are not compatible."
     return np.argmin(norm(coords - target, axis=1))
 
 
+# !FIXME : this is duplicated in polymesh.space.utils
 def index_of_furthest_point(coords: ndarray, target: ndarray) -> int:
     """
     Returs the index of the furthest point to a target location.
-    
+
     Parameters
     ----------
     coords : numpy.ndarray
         2d float array of (nP, nD) of vertex coordinates.
-        
+
         nP : number of points
-        
+
         nD : number of dimensions of the model space
-            
+
     target : numpy.ndarray
         Coordinate array of the target point.
 
     Returns
     -------
     int
         The index of 'coords', for which the distance from
         'target' is maximal.
-    
+
     """
+    warnings.warn("This is deprecated, use polymesh.space.index_of_furthest_point instaead.",
+                  warnings.DeprecationWarning)
     assert coords.shape[1] == target.shape[0], \
         "The dimensions of `coords` and `target` are not compatible."
     return np.argmax(norm(coords - target, axis=1))
 
 
-def points_of_cells(coords: ndarray, topo: ndarray, *args, 
-                    local_axes:ndarray=None, centralize:bool=True, 
+def points_of_cells(coords: ndarray, topo: ndarray, *args,
+                    local_axes: ndarray = None, centralize: bool = True,
                     **kwargs) -> ndarray:
     """
     Returns an explicit representation of coordinates of the cells from a 
     pointset and a topology. If coordinate frames are provided, the coorindates 
     are returned with  respect to those frames.
-    
+
     Parameters
     ----------
     coords : numpy.ndarray
         2d float array of shape (nP, nD) of vertex coordinates.
-               
+
         nP : number of points
-            
+
         nD : number of dimensions of the model space
-            
+
     topo : numpy.ndarray
         A 2D array of shape (nE, nNE) of vertex indices. The i-th row contains the 
         vertex indices of the i-th element.
-        
+
         nE : number of elements
-        
+
         nNE : number of nodes per element
-            
+
     local_axes : numpy.ndarray
         Reference frames as a3d array of shape (..., 3, 3). A single 3x3 numpy array 
         or matrices for all elements in 'topo' must be provided.
-            
+
     centralize : bool, Optional
         If True, and 'frame' is not None, the local coordinates are returned
         with respect to the geometric center of each element.
-        
+
     Returns
     -------
     numpy.ndarray
         3d float array of coordinates
-    
+
     Notes
     -----
     It is assumed that all entries in 'coords' are coordinates of
     points in the same frame.
-    
+
     """
     if local_axes is not None:
-        return cells_coords_tr(cells_coords(coords, topo), 
+        return cells_coords_tr(cells_coords(coords, topo),
                                local_axes, centralize=centralize)
     else:
         return cells_coords(coords, topo)
-    
-    
+
+
 @njit(nogil=True, parallel=True, cache=__cache)
-def cells_coords_tr(ecoords: ndarray, local_axes: ndarray, 
-                    centralize:bool=True) -> ndarray:
+def cells_coords_tr(ecoords: ndarray, local_axes: ndarray,
+                    centralize: bool = True) -> ndarray:
     nE, nNE, _ = ecoords.shape
     res = np.zeros_like(ecoords)
     for i in prange(nE):
         if centralize:
             cc = cell_center(ecoords[i])
             ecoords[i, :, 0] -= cc[0]
             ecoords[i, :, 1] -= cc[1]
@@ -431,38 +438,38 @@
     Returns coordinates of cells from a coordinate base array and
     a topology array.
 
     Parameters
     ----------
     coords : numpy.ndarray
         2d float array of shape (nP, nD) of vertex coordinates.
-        
+
         nP : number of points
-        
+
         nD : number of dimensions of the model space
-            
+
     topo : numpy.ndarray
         A 2D array of shape (nE, nNE) of vertex indices. The i-th row contains 
         the vertex indices of the i-th element.
-        
+
         nE : number of elements
-        
+
         nNE : number of nodes per element
 
     Returns
     -------
     numpy.ndarray
         A 3d array of shape (nE, nNE, nD) that contains coordinates for all nodes 
         of all cells according to the argument 'topo'.
 
     Notes
     -----
     The array 'coords' must be fully populated up to the maximum index
     in 'topo'. (len(coords) >= (topo.max() + 1))
-    
+
     """
     nE, nNE = topo.shape
     res = np.zeros((nE, nNE, coords.shape[1]), dtype=coords.dtype)
     for iE in prange(nE):
         for iNE in prange(nNE):
             res[iE, iNE] = coords[topo[iE, iNE]]
     return res
@@ -474,22 +481,22 @@
     Returns coordinates of a single cell from a coordinate 
     array and a topology array.
 
     Parameters
     ----------
     coords : numpy.ndarray
         2d array of shape (nP, nD) of vertex coordinates.
-            
+
         nP : number of points
-            
+
         nD : number of dimensions of the model space
-    
+
     topo : (nNE) numpy.ndarray
         1D array of vertex indices.
-            
+
         nNE : number of nodes per element
 
     Returns
     -------
     (nNE, nD) numpy.ndarray
         Coordinates for all nodes of all cells according to the
         argument 'topo'.
@@ -518,15 +525,15 @@
         2d coordinate array of the element. The array has as many rows,
         as the number of nodes of the cell, and two columns.
 
     Returns
     -------
     numpy.ndarray
         1d coordinate array.
-        
+
     """
     return np.array([np.mean(ecoords[:, 0]), np.mean(ecoords[:, 1])],
                     dtype=ecoords.dtype)
 
 
 @njit(nogil=True, cache=__cache)
 def cell_center(coords: np.ndarray):
@@ -539,15 +546,15 @@
         2d coordinate array of the element. The array has as many rows,
         as the number of nodes of the cell, and three columns.
 
     Returns
     -------
     numpy.ndarray
         1d coordinate array.
-        
+
     """
     return np.array([np.mean(coords[:, 0]), np.mean(coords[:, 1]),
                      np.mean(coords[:, 2])], dtype=coords.dtype)
 
 
 def cell_centers_bulk(coords: ndarray, topo: ndarray) -> ndarray:
     """
@@ -561,15 +568,15 @@
     topo : numpy.ndarray
         2d point-based topology array.
 
     Returns
     -------
     numpy.ndarray
         2d coordinate array.
-        
+
     """
     return np.mean(cells_coords(coords, topo), axis=1)
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
 def nodal_distribution_factors(topo: ndarray, volumes: ndarray):
     """
@@ -587,32 +594,32 @@
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
 def distribute_nodal_data_bulk(data: ndarray, topo: ndarray, ndf: ndarray):
     """
     Distributes nodal data to the cells. The parameter 'ndf' controls
     the behaviour of the distribution.
-    
+
     Parameters
     ----------
     data : numpy.ndarray
         2d array of shape (nP, nX), the data defined on points.
-    
+
     topo : numpy.ndarray
         2d integer array of shape (nE, nNE), describing the topology.
-    
+
     ndf : numpy.ndarray, Optional
         2d float array of shape (nE, nNE), describing the distribution
         of cells to the nodes.
-        
+
     Returns
     -------
     numpy.ndarray
         A 3d float array of shape (nE, nNE, nX).
-    
+
     """
     nE, nNE = topo.shape
     res = np.zeros((nE, nNE, data.shape[1]))
     for iE in prange(nE):
         for jNE in prange(nNE):
             res[iE, jNE] = data[topo[iE, jNE]] * ndf[iE, jNE]
     return res
@@ -701,15 +708,15 @@
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
 def jacobian_matrix_bulk(dshp: ndarray, ecoords: ndarray):
     """
     Returns Jacobian matrices of local to global transformation 
     for several cells.
-    
+
     dshp (nG, nN, nD)
     ecoords  (nE, nNE, nD)
     ---
     (nE, nG, nD, nD)
     """
     nE = ecoords.shape[0]
     nG, _, nD = dshp.shape
@@ -733,20 +740,20 @@
 @njit(nogil=True, parallel=True, cache=__cache)
 def jacobian_matrix_bulk_1d(dshp: ndarray, ecoords: ndarray):
     """
     Returns the Jacobian matrix for multiple cells (nE), evaluated at
     multiple (nP) points.
     ---
     (nE, nP, 1, 1)
-    
+
     Notes
     -----
     As long as the line is straight, it is a constant metric element,
     and 'dshp' is only required here to provide an output with a correct shape.
-    
+
     """
     lengths = lengths_of_lines2(ecoords)
     nE = ecoords.shape[0]
     if len(dshp.shape) > 4:
         # variable metric element -> dshp (nE, nP, nNE, nDOF, ...)
         nP = dshp.shape[1]
     else:
@@ -755,23 +762,23 @@
     res = np.zeros((nE, nP, 1, 1), dtype=dshp.dtype)
     for iE in prange(nE):
         res[iE, :, 0, 0] = lengths[iE] / 2
     return res
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
-def center_of_points(coords : ndarray):
+def center_of_points(coords: ndarray):
     res = np.zeros(coords.shape[1], dtype=coords.dtype)
     for i in prange(res.shape[0]):
         res[i] = np.mean(coords[:, i])
     return res
 
 
 @njit(nogil=True, cache=__cache)
-def centralize(coords : ndarray):
+def centralize(coords: ndarray):
     nD = coords.shape[1]
     center = center_of_points(coords)
     coords[:, 0] -= center[0]
     coords[:, 1] -= center[1]
     if nD > 2:
         coords[:, 2] -= center[2]
     return coords
@@ -796,59 +803,59 @@
     return res
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
 def distances_of_points(coords: ndarray):
     """
     Calculates distances between a series of points.
-    
+
     Parameters
     ----------
     coords : numpy.ndarray
         2d float array of shape (N, ...).
-        
+
     Returns
     -------
     numpy.ndarray
         1d float array of shape (nP,).
-        
+
     """
     nP = coords.shape[0]
     res = np.zeros(nP, dtype=coords.dtype)
     for i in prange(1, nP):
         res[i] = norm(coords[i] - coords[i-1])
     return res
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
 def pcoords_to_coords_1d(pcoords: ndarray, ecoords: ndarray):
     """
     Returns a flattened array of points, evaluated at multiple
     points and cells. 
-    
+
     Only for 1d cells.
-    
+
     Parameters
     ----------
     pcoords : numpy.ndarray
         1d float array of length nP, coordinates in the range [-1 , 1].
-        
+
     ecoords : numpy.ndarray
         3d float array of shape (nE, 2+, nD) of cell coordinates.
-    
+
     Notes
     -----
     It works for arbitrary topologies, but handles every cell as a line
     going from the firts to the last node of the cell.
-    
+
     Returns
     -------
     numpy.ndarray
         2d float array of shape (nE * nP, nD). 
-        
+
     """
     nP = pcoords.shape[0]
     nE = ecoords.shape[0]
     nX = nE * nP
     res = np.zeros((nX, ecoords.shape[2]), dtype=ecoords.dtype)
     for iE in prange(nE):
         for jP in prange(nP):
@@ -858,25 +865,25 @@
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
 def norms(a: ndarray):
     """
     Returns the Euclidean norms for the input data, calculated
     along axis 1.
-    
+
     Parameters
     ----------
     a : numpy.ndarray
         2d array of data of shape (N, ...).
-        
+
     Returns
     -------
     numpy.ndarray
         1d float array of shape (N, ).
-    
+
     """
     nI = len(a)
     res = np.zeros(nI)
     for iI in prange(len(a)):
         res[iI] = np.dot(a[iI], a[iI])
     return np.sqrt(res)
 
@@ -884,8 +891,8 @@
 @njit(nogil=True, parallel=True, cache=__cache)
 def homogenize_nodal_values(data: ndarray, measure: ndarray):
     nE, _, nDATA = data.shape  # nE, nNE, nDATA
     res = np.zeros((nE, nDATA), dtype=data.dtype)
     for i in prange(nE):
         for j in prange(nDATA):
             res[i, j] = np.sum(data[i, :, j]) / measure[i]
-    return res
+    return res
```

### Comparing `polymesh-0.0.8/src/polymesh/voxelize.py` & `polymesh-0.0.9/src/polymesh/voxelize.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/vtkcelltypes.py` & `polymesh-0.0.9/src/polymesh/vtkcelltypes.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh/vtkutils.py` & `polymesh-0.0.9/src/polymesh/vtkutils.py`

 * *Files identical despite different names*

### Comparing `polymesh-0.0.8/src/polymesh.egg-info/PKG-INFO` & `polymesh-0.0.9/src/polymesh.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: polymesh
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package to build, manipulate and analyze polygonal meshes.
 Home-page: https://github.com/dewloosh/PolyMesh
 Author: dewloosh
 Author-email: dewloosh@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/dewloosh/PolyMesh/archive/refs/tags/0.0.8.zip
+Download-URL: https://github.com/dewloosh/PolyMesh/archive/refs/tags/0.0.9.zip
 Description: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dewloosh/PolyMesh/main?labpath=notebooks%5Cgrid.ipynb)
         [![CircleCI](https://circleci.com/gh/dewloosh/PolyMesh.svg?style=shield)](https://circleci.com/gh/dewloosh/PolyMesh) 
         [![Documentation Status](https://readthedocs.org/projects/polymesh/badge/?version=latest)](https://polymesh.readthedocs.io/en/latest/?badge=latest) 
         [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
         [![PyPI](https://badge.fury.io/py/PolyMesh.svg)](https://pypi.org/project/PolyMesh) 
         
         # **PolyMesh** - A Python Library for Compound Meshes with Jagged Topology
```

### Comparing `polymesh-0.0.8/src/polymesh.egg-info/SOURCES.txt` & `polymesh-0.0.9/src/polymesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

