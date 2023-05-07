# Comparing `tmp/spatialcsv-0.0.8.tar.gz` & `tmp/spatialcsv-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatialcsv-0.0.8.tar", last modified: Thu Apr 13 23:18:26 2023, max compression
+gzip compressed data, was "spatialcsv-0.0.9.tar", last modified: Tue Apr 18 00:43:22 2023, max compression
```

## Comparing `spatialcsv-0.0.8.tar` & `spatialcsv-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-13 23:18:26.562468 spatialcsv-0.0.8/
--rw-r--r--   0 thomer    (1000) thomer    (1000)     1560 2023-04-02 12:42:12.000000 spatialcsv-0.0.8/LICENSE
--rw-r--r--   0 thomer    (1000) thomer    (1000)      122 2023-04-02 12:42:12.000000 spatialcsv-0.0.8/MANIFEST.in
--rw-r--r--   0 thomer    (1000) thomer    (1000)     1484 2023-04-13 23:18:26.562468 spatialcsv-0.0.8/PKG-INFO
--rw-r--r--   0 thomer    (1000) thomer    (1000)      672 2023-04-12 23:58:14.000000 spatialcsv-0.0.8/README.md
--rw-r--r--   0 thomer    (1000) thomer    (1000)       38 2023-04-13 01:16:34.000000 spatialcsv-0.0.8/requirements.txt
--rw-r--r--   0 thomer    (1000) thomer    (1000)      393 2023-04-13 23:18:26.562468 spatialcsv-0.0.8/setup.cfg
--rw-r--r--   0 thomer    (1000) thomer    (1000)     1908 2023-04-13 23:17:49.000000 spatialcsv-0.0.8/setup.py
-drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-13 23:18:26.562468 spatialcsv-0.0.8/spatialcsv/
--rw-r--r--   0 thomer    (1000) thomer    (1000)      150 2023-04-13 23:17:49.000000 spatialcsv-0.0.8/spatialcsv/__init__.py
--rw-r--r--   0 thomer    (1000) thomer    (1000)      445 2023-04-02 12:42:12.000000 spatialcsv-0.0.8/spatialcsv/cli.py
--rw-r--r--   0 thomer    (1000) thomer    (1000)     8782 2023-04-13 14:55:32.000000 spatialcsv-0.0.8/spatialcsv/spatialcsv.py
--rw-r--r--   0 thomer    (1000) thomer    (1000)      986 2023-04-13 14:20:34.000000 spatialcsv-0.0.8/spatialcsv/spatialfolium.py
-drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-13 23:18:26.562468 spatialcsv-0.0.8/spatialcsv.egg-info/
--rw-r--r--   0 thomer    (1000) thomer    (1000)     1484 2023-04-13 23:18:26.000000 spatialcsv-0.0.8/spatialcsv.egg-info/PKG-INFO
--rw-r--r--   0 thomer    (1000) thomer    (1000)      423 2023-04-13 23:18:26.000000 spatialcsv-0.0.8/spatialcsv.egg-info/SOURCES.txt
--rw-r--r--   0 thomer    (1000) thomer    (1000)       39 2023-04-13 23:18:26.000000 spatialcsv-0.0.8/spatialcsv.egg-info/dependency_links.txt
--rw-r--r--   0 thomer    (1000) thomer    (1000)       51 2023-04-13 23:18:26.000000 spatialcsv-0.0.8/spatialcsv.egg-info/entry_points.txt
--rw-r--r--   0 thomer    (1000) thomer    (1000)        1 2023-04-02 12:46:06.000000 spatialcsv-0.0.8/spatialcsv.egg-info/not-zip-safe
--rw-r--r--   0 thomer    (1000) thomer    (1000)       38 2023-04-13 23:18:26.000000 spatialcsv-0.0.8/spatialcsv.egg-info/requires.txt
--rw-r--r--   0 thomer    (1000) thomer    (1000)       11 2023-04-13 23:18:26.000000 spatialcsv-0.0.8/spatialcsv.egg-info/top_level.txt
-drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-13 23:18:26.562468 spatialcsv-0.0.8/tests/
--rw-r--r--   0 thomer    (1000) thomer    (1000)      402 2023-04-02 12:42:12.000000 spatialcsv-0.0.8/tests/test_spatialcsv.py
+drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-18 00:43:22.563402 spatialcsv-0.0.9/
+-rw-r--r--   0 thomer    (1000) thomer    (1000)     1560 2023-04-02 12:42:12.000000 spatialcsv-0.0.9/LICENSE
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      122 2023-04-02 12:42:12.000000 spatialcsv-0.0.9/MANIFEST.in
+-rw-r--r--   0 thomer    (1000) thomer    (1000)     1484 2023-04-18 00:43:22.563402 spatialcsv-0.0.9/PKG-INFO
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      672 2023-04-12 23:58:14.000000 spatialcsv-0.0.9/README.md
+-rw-r--r--   0 thomer    (1000) thomer    (1000)       55 2023-04-18 00:42:22.000000 spatialcsv-0.0.9/requirements.txt
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      393 2023-04-18 00:43:22.563402 spatialcsv-0.0.9/setup.cfg
+-rw-r--r--   0 thomer    (1000) thomer    (1000)     1908 2023-04-18 00:43:02.000000 spatialcsv-0.0.9/setup.py
+drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-18 00:43:22.563402 spatialcsv-0.0.9/spatialcsv/
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      150 2023-04-18 00:43:02.000000 spatialcsv-0.0.9/spatialcsv/__init__.py
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      445 2023-04-02 12:42:12.000000 spatialcsv-0.0.9/spatialcsv/cli.py
+-rw-r--r--   0 thomer    (1000) thomer    (1000)     9642 2023-04-18 00:41:26.000000 spatialcsv-0.0.9/spatialcsv/spatialcsv.py
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      986 2023-04-13 14:20:34.000000 spatialcsv-0.0.9/spatialcsv/spatialfolium.py
+drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-18 00:43:22.563402 spatialcsv-0.0.9/spatialcsv.egg-info/
+-rw-r--r--   0 thomer    (1000) thomer    (1000)     1484 2023-04-18 00:43:22.000000 spatialcsv-0.0.9/spatialcsv.egg-info/PKG-INFO
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      423 2023-04-18 00:43:22.000000 spatialcsv-0.0.9/spatialcsv.egg-info/SOURCES.txt
+-rw-r--r--   0 thomer    (1000) thomer    (1000)       56 2023-04-18 00:43:22.000000 spatialcsv-0.0.9/spatialcsv.egg-info/dependency_links.txt
+-rw-r--r--   0 thomer    (1000) thomer    (1000)       51 2023-04-18 00:43:22.000000 spatialcsv-0.0.9/spatialcsv.egg-info/entry_points.txt
+-rw-r--r--   0 thomer    (1000) thomer    (1000)        1 2023-04-02 12:46:06.000000 spatialcsv-0.0.9/spatialcsv.egg-info/not-zip-safe
+-rw-r--r--   0 thomer    (1000) thomer    (1000)       55 2023-04-18 00:43:22.000000 spatialcsv-0.0.9/spatialcsv.egg-info/requires.txt
+-rw-r--r--   0 thomer    (1000) thomer    (1000)       11 2023-04-18 00:43:22.000000 spatialcsv-0.0.9/spatialcsv.egg-info/top_level.txt
+drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-18 00:43:22.563402 spatialcsv-0.0.9/tests/
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      402 2023-04-02 12:42:12.000000 spatialcsv-0.0.9/tests/test_spatialcsv.py
```

### Comparing `spatialcsv-0.0.8/LICENSE` & `spatialcsv-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialcsv-0.0.8/PKG-INFO` & `spatialcsv-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialcsv
-Version: 0.0.8
+Version: 0.0.9
 Summary: Easily add location points to a map from a csv
 Home-page: https://github.com/TJHomer/spatialcsv
 Author: Tracy Homer
 Author-email: thomer@mac.com
 License: GNU General Public License v3
 Keywords: spatialcsv
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `spatialcsv-0.0.8/README.md` & `spatialcsv-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `spatialcsv-0.0.8/setup.py` & `spatialcsv-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,10 +54,10 @@
     keywords='spatialcsv',
     name='spatialcsv',
     packages=find_packages(include=['spatialcsv', 'spatialcsv.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/TJHomer/spatialcsv',
-    version='0.0.8',
+    version='0.0.9',
     zip_safe=False,
 )
```

### Comparing `spatialcsv-0.0.8/spatialcsv/spatialcsv.py` & `spatialcsv-0.0.9/spatialcsv/spatialcsv.py`

 * *Files 18% similar despite different names*

```diff
@@ -72,16 +72,14 @@
         with open(self.csv) as csvfile:
             reader = csv.DictReader(csvfile)
             header = reader.fieldnames
             return header
 
 
 
-l = Locations('/home/thomer/School/Software_Design_GEOG422/Repo/spatialcsv/spatialcsv/us-state-capitals.csv', 'latitude', 'longitude')
-l.check_lat_long()
 
 class Map(ipyleaflet.Map):
     
     def __init__(self, center=[20, 0], zoom=2, **kwargs) -> None:
 
         if "scroll_wheel_zoom" not in kwargs:
             kwargs["scroll_wheel_zoom"] = True
@@ -240,15 +238,15 @@
         """
         import geopandas as gpd
         gdf = gpd.read_file(data)
         geojson = gdf.__geo_interface__
         self.add_geojson(geojson, name=name, **kwargs)
 
 
-    def add_geodf(self, data, name='GeoDataFrame', **kwargs)
+    def add_geodf(self, data, name='GeoDataFrame', **kwargs):
         """Adds a GeoDataFrame to the map
         
         Args:
             data: geodataframe instance
         """
         geodf = ipyleaflet.GeoData(data=data, name=name, **kwargs)
         self.add_layer(geodf)
@@ -268,13 +266,43 @@
         elif name == "Shapefile":
             self.add_shp(self, data, name, **kwargs)
         elif name == "GeoDataFrame":
             self.add_geodf(self, data, name, **kwargs)
         else:
             print("This type of vector is not supported yet.")
         
+    def add_raster(self, url, name='Raster', fit_bounds=True, **kwargs):
+        """Adds a raster layer to the map.
+        Args:
+            url (str): The URL of the raster layer.
+            name (str, optional): The name of the raster layer. Defaults to 'Raster'.
+            fit_bounds (bool, optional): Whether to fit the map bounds to the raster layer. Defaults to True.
+        """
+        import httpx
+
+        titiler_endpoint = "https://titiler.xyz"
+
+        r = httpx.get(
+            f"{titiler_endpoint}/cog/info",
+            params = {
+                "url": url,
+            }
+        ).json()
+
+        bounds = r["bounds"]
 
+        r = httpx.get(
+            f"{titiler_endpoint}/cog/tilejson.json",
+            params = {
+                "url": url,
+            }
+        ).json()
 
+        tile = r["tiles"][0]
 
+        self.add_tile_layer(url=tile, name=name, **kwargs)
 
+        if fit_bounds:
+            bbox = [[bounds[1], bounds[0]], [bounds[3], bounds[2]]]
+            self.fit_bounds(bbox)
 
-    
+
```

### Comparing `spatialcsv-0.0.8/spatialcsv/spatialfolium.py` & `spatialcsv-0.0.9/spatialcsv/spatialfolium.py`

 * *Files identical despite different names*

### Comparing `spatialcsv-0.0.8/spatialcsv.egg-info/PKG-INFO` & `spatialcsv-0.0.9/spatialcsv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialcsv
-Version: 0.0.8
+Version: 0.0.9
 Summary: Easily add location points to a map from a csv
 Home-page: https://github.com/TJHomer/spatialcsv
 Author: Tracy Homer
 Author-email: thomer@mac.com
 License: GNU General Public License v3
 Keywords: spatialcsv
 Classifier: Development Status :: 2 - Pre-Alpha
```

