# Comparing `tmp/uintel-0.3.8.tar.gz` & `tmp/uintel-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uintel-0.3.8.tar", last modified: Wed Feb 15 20:40:30 2023, max compression
+gzip compressed data, was "uintel-0.3.9.tar", last modified: Wed Feb 15 21:55:52 2023, max compression
```

## Comparing `uintel-0.3.8.tar` & `uintel-0.3.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 20:40:30.010417 uintel-0.3.8/
--rw-rw-rw-   0        0        0     1096 2023-01-18 03:00:37.000000 uintel-0.3.8/LICENSE
--rw-rw-rw-   0        0        0     4118 2023-02-15 20:40:30.004419 uintel-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     3336 2023-02-10 03:40:36.000000 uintel-0.3.8/README.md
--rw-rw-rw-   0        0        0       97 2023-01-18 03:00:38.000000 uintel-0.3.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-15 20:40:30.011425 uintel-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1591 2023-02-15 20:39:57.000000 uintel-0.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-15 20:40:29.796398 uintel-0.3.8/src/
-drwxrwxrwx   0        0        0        0 2023-02-15 20:40:29.918475 uintel-0.3.8/src/uintel/
--rw-rw-rw-   0        0        0     3122 2023-02-15 03:54:11.000000 uintel-0.3.8/src/uintel/__init__.py
--rw-rw-rw-   0        0        0     8130 2023-01-26 03:30:11.000000 uintel-0.3.8/src/uintel/aws.py
--rw-rw-rw-   0        0        0     4751 2023-02-15 04:36:27.000000 uintel-0.3.8/src/uintel/colours.py
--rw-rw-rw-   0        0        0    10291 2023-02-15 20:39:52.000000 uintel-0.3.8/src/uintel/esri.py
-drwxrwxrwx   0        0        0        0 2023-02-15 20:40:29.982428 uintel-0.3.8/src/uintel/fonts/
--rw-rw-rw-   0        0        0    94884 2023-01-18 03:00:38.000000 uintel-0.3.8/src/uintel/fonts/Myriad Pro (TrueType).ttf
--rw-rw-rw-   0        0        0   208636 2023-01-18 03:00:38.000000 uintel-0.3.8/src/uintel/fonts/Rubik (TrueType).ttf
--rw-rw-rw-   0        0        0   202424 2023-01-18 03:00:38.000000 uintel-0.3.8/src/uintel/fonts/Rubik Italic (TrueType).ttf
--rw-rw-rw-   0        0        0    20653 2023-02-12 21:37:30.000000 uintel-0.3.8/src/uintel/geometry.py
--rw-rw-rw-   0        0        0    23622 2023-02-15 00:53:18.000000 uintel-0.3.8/src/uintel/install.py
--rw-rw-rw-   0        0        0     2353 2023-01-30 21:31:25.000000 uintel-0.3.8/src/uintel/ogc.py
--rw-rw-rw-   0        0        0     3869 2023-02-10 05:41:23.000000 uintel-0.3.8/src/uintel/query.py
--rw-rw-rw-   0        0        0     8139 2023-01-23 22:19:34.000000 uintel-0.3.8/src/uintel/server.py
--rw-rw-rw-   0        0        0    14891 2023-01-23 21:02:38.000000 uintel-0.3.8/src/uintel/slack.py
--rw-rw-rw-   0        0        0     3222 2023-01-23 21:00:27.000000 uintel-0.3.8/src/uintel/sql.py
-drwxrwxrwx   0        0        0        0 2023-02-15 20:40:29.991877 uintel-0.3.8/src/uintel/styles/
--rw-rw-rw-   0        0        0     1096 2023-01-18 03:00:38.000000 uintel-0.3.8/src/uintel/styles/ui.mplstyle
-drwxrwxrwx   0        0        0        0 2023-02-15 20:40:29.959878 uintel-0.3.8/src/uintel.egg-info/
--rw-rw-rw-   0        0        0     4118 2023-02-15 20:40:29.000000 uintel-0.3.8/src/uintel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      590 2023-02-15 20:40:29.000000 uintel-0.3.8/src/uintel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 20:40:29.000000 uintel-0.3.8/src/uintel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2023-02-15 20:40:29.000000 uintel-0.3.8/src/uintel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-15 20:40:29.000000 uintel-0.3.8/src/uintel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-02-15 21:55:52.340139 uintel-0.3.9/
+-rw-rw-rw-   0        0        0     1096 2023-01-18 03:00:37.000000 uintel-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0     4118 2023-02-15 21:55:52.333917 uintel-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3336 2023-02-10 03:40:36.000000 uintel-0.3.9/README.md
+-rw-rw-rw-   0        0        0       97 2023-01-18 03:00:38.000000 uintel-0.3.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-02-15 21:55:52.341108 uintel-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1591 2023-02-15 21:55:25.000000 uintel-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-15 21:55:52.127353 uintel-0.3.9/src/
+drwxrwxrwx   0        0        0        0 2023-02-15 21:55:52.251396 uintel-0.3.9/src/uintel/
+-rw-rw-rw-   0        0        0     3122 2023-02-15 03:54:11.000000 uintel-0.3.9/src/uintel/__init__.py
+-rw-rw-rw-   0        0        0     8130 2023-01-26 03:30:11.000000 uintel-0.3.9/src/uintel/aws.py
+-rw-rw-rw-   0        0        0     4751 2023-02-15 04:36:27.000000 uintel-0.3.9/src/uintel/colours.py
+-rw-rw-rw-   0        0        0    10867 2023-02-15 21:52:53.000000 uintel-0.3.9/src/uintel/esri.py
+drwxrwxrwx   0        0        0        0 2023-02-15 21:55:52.315724 uintel-0.3.9/src/uintel/fonts/
+-rw-rw-rw-   0        0        0    94884 2023-01-18 03:00:38.000000 uintel-0.3.9/src/uintel/fonts/Myriad Pro (TrueType).ttf
+-rw-rw-rw-   0        0        0   208636 2023-01-18 03:00:38.000000 uintel-0.3.9/src/uintel/fonts/Rubik (TrueType).ttf
+-rw-rw-rw-   0        0        0   202424 2023-01-18 03:00:38.000000 uintel-0.3.9/src/uintel/fonts/Rubik Italic (TrueType).ttf
+-rw-rw-rw-   0        0        0    20653 2023-02-12 21:37:30.000000 uintel-0.3.9/src/uintel/geometry.py
+-rw-rw-rw-   0        0        0    23622 2023-02-15 00:53:18.000000 uintel-0.3.9/src/uintel/install.py
+-rw-rw-rw-   0        0        0     2353 2023-01-30 21:31:25.000000 uintel-0.3.9/src/uintel/ogc.py
+-rw-rw-rw-   0        0        0     3869 2023-02-10 05:41:23.000000 uintel-0.3.9/src/uintel/query.py
+-rw-rw-rw-   0        0        0     8139 2023-01-23 22:19:34.000000 uintel-0.3.9/src/uintel/server.py
+-rw-rw-rw-   0        0        0    14891 2023-01-23 21:02:38.000000 uintel-0.3.9/src/uintel/slack.py
+-rw-rw-rw-   0        0        0     3222 2023-01-23 21:00:27.000000 uintel-0.3.9/src/uintel/sql.py
+drwxrwxrwx   0        0        0        0 2023-02-15 21:55:52.323234 uintel-0.3.9/src/uintel/styles/
+-rw-rw-rw-   0        0        0     1096 2023-01-18 03:00:38.000000 uintel-0.3.9/src/uintel/styles/ui.mplstyle
+drwxrwxrwx   0        0        0        0 2023-02-15 21:55:52.291282 uintel-0.3.9/src/uintel.egg-info/
+-rw-rw-rw-   0        0        0     4118 2023-02-15 21:55:52.000000 uintel-0.3.9/src/uintel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      590 2023-02-15 21:55:52.000000 uintel-0.3.9/src/uintel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-15 21:55:52.000000 uintel-0.3.9/src/uintel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      158 2023-02-15 21:55:52.000000 uintel-0.3.9/src/uintel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-02-15 21:55:52.000000 uintel-0.3.9/src/uintel.egg-info/top_level.txt
```

### Comparing `uintel-0.3.8/LICENSE` & `uintel-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `uintel-0.3.8/PKG-INFO` & `uintel-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uintel
-Version: 0.3.8
+Version: 0.3.9
 Summary: Urban Intelligence's unified Python data analysis toolkit
 Home-page: https://uintel.github.io/pyui/
 Author: Sam Archie
 Author-email: sam.archie@urbanintelligence.co.nz
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `uintel-0.3.8/README.md` & `uintel-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `uintel-0.3.8/setup.py` & `uintel-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 setuptools.setup(
     # State the generic information about the package
     name='uintel',
-    version='0.3.8',
+    version='0.3.9',
     author="Sam Archie",
     author_email="sam.archie@urbanintelligence.co.nz",
     description="Urban Intelligence's unified Python data analysis toolkit",
     long_description=open('README.md').read().replace("docs/images/blue_logo.svg", "https://urbanintelligence.co.nz/wp-content/uploads/2022/05/Artboard-1-copy-23.svg"),
     long_description_content_type='text/markdown',
     license="MIT",
     url="https://uintel.github.io/pyui/",
```

### Comparing `uintel-0.3.8/src/uintel/__init__.py` & `uintel-0.3.9/src/uintel/__init__.py`

 * *Files identical despite different names*

### Comparing `uintel-0.3.8/src/uintel/aws.py` & `uintel-0.3.9/src/uintel/aws.py`

 * *Files identical despite different names*

### Comparing `uintel-0.3.8/src/uintel/colours.py` & `uintel-0.3.9/src/uintel/colours.py`

 * *Files identical despite different names*

### Comparing `uintel-0.3.8/src/uintel/esri.py` & `uintel-0.3.9/src/uintel/esri.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,35 +8,36 @@
 import geopandas as gpd, requests, esridump, esridump.errors, yaml
 import typing, subprocess, logging, os
 
 logging.basicConfig(format='%(asctime)s %(levelname)-8s %(message)s', level=logging.INFO, datefmt='%Y-%m-%d %H:%M:%S')
 logger = logging.getLogger(__name__)
 
 
-def get_data(url: str, layer: int = None, projection: int = 2193, verbose: bool = False, assume_data_type: str = "Feature Layer") -> gpd.GeoDataFrame:
+def get_data(url: str, layer: int = None, projection: int = 2193, verbose: bool = False, assume_data_type: str = "Feature Layer", boundary: gpd.GeoDataFrame = None) -> gpd.GeoDataFrame:
     """Query an ESRI service and return data.
     
     The main function to call to return an ESRI REST MapServer, FeatureService or ImageServer. The url is verified to ensure a layer number is within the url, and gathers any query parameters that were added in the url. An automatic attempt is made to see if the Service contains vector or raster geometry, and thhe appropiate downloading methodology is chosen.
     
     Args:
         url: String of the ESRI Service. E.g. https://services7.arcgis.com/NNoivt2IKUC8czGf/arcgis/rest/services/NZTA_One_Road/FeatureServer.
         layer: If the layer number is not provided at the end of the url, this parameter should be the layer number you wish to get.
         projection: Integer of the CRS that the data should be returned in.
         verbose: Display progress of the downloading procedure and assumptions made if verbose=True. Otherwise, logging is kept to errors or above.
         assume_data_type: If the automatic attempt of determining the type of the Service fails, the assume_data_type is used instead. Hence, assume_data_type should either be: "Feature Service" or "Raster Layer".
+        bbox: A tuple of values in the given projection to limit the returned results of the query
 
     Returns:
         For vector Services, a geopandas.GeoDataFrame (for vector data) is returned.
     
     Raises:
         NotImplementedError: Raised if the Service is a MapServer or ImageServer.
     """
     
     # Verify the given endpoint is okay
-    url, query_parameters = _check_url(url, layer)
+    url, query_parameters = _check_url(url, layer, boundary)
     # Check the type of data of the endpoint so we know which method to download as
     response = requests.get(url + '?f=json')
     if response.ok:
         results = response.json()
         data_type = results.get("type", None)
         if not data_type and 'pixelType' in results:
             data_type = "Raster Layer"
@@ -50,15 +51,15 @@
         return _download_vector_endpoint(url, query_parameters, projection, verbose)
 
     elif data_type == "Raster Layer":
         # Return the server as an numpy array?
         return _download_raster_endpoint(url, query_parameters, projection)
 
 
-def _check_url(url: str, layer: int = None) -> typing.Tuple[str, dict]:
+def _check_url(url: str, layer: int = None, boundary: gpd.GeoDataFrame = None) -> typing.Tuple[str, dict]:
     """Ensure the url is valid.
 
     Check to see if the given url was valid by ensuring it is correctly formatted with the layer number if it is a MapServer or FeatureSever.
 
     Args: 
         url: String of the ESRI Service. E.g. https://services7.arcgis.com/NNoivt2IKUC8czGf/arcgis/rest/services/NZTA_One_Road/FeatureServer.
         layer: If the layer number is not provided at the end of the url, this parameter should be the layer number you wish to get.
@@ -80,14 +81,20 @@
         if "f" in query_parameters:
             del query_parameters["f"]
         # Set the url as everything before the query parameters
         url = url[:url.index('query?')]
     else:
         # Set as default query parameters
         query_parameters = {'where': '1=1', 'outFields': '*'}
+        if boundary:
+            minx, miny, maxx, maxy = boundary.bounds.values[0]
+            query_parameters["geometry"] = f"geometryType=esriGeometryEnvelope&geometry={minx},{miny},{maxx},{maxy}"
+            query_parameters["geometryType"] = "esriGeometryEnvelope"
+            query_parameters["inSR"] = boundary.crs.to_wkt()
+            query_parameters["spatialRel"] = "esriSpatialRelIntersects"
     
     if not url.endswith('/'):
         # Map Server URL needs a slash at the end
         url += '/' 
     
     if url.endswith("FeatureServer/") or url.endswith("MapServer/"):
         if layer:
@@ -110,15 +117,15 @@
     try:
         # Try downloading the data and see if we get stopped
         endpoint_data = gpd.GeoDataFrame.from_features(list(esridump.EsriDumper(url=url, outSR=projection, request_geometry=True, extra_query_args=query_parameters, pause_seconds=0, timeout=120)))
         if len(endpoint_data) > 0:
             endpoint_data.set_crs(projection, inplace=True)
         else:
             endpoint_data = gpd.GeoDataFrame(crs=projection)  
-              
+
     except esridump.errors.EsriDownloadError as error:
         if "Token Required" in str(error):
             # Then we have an endpoint that requires authentication. The best way to generate a token is using the Arcpy package that is only available in the arcgispro virtual environment
             arcgis_venv_path = r'C:\Program Files\ArcGIS\Pro\bin\Python\envs\arcgispro-py3\python.exe'
             if not os.path.exists(arcgis_venv_path):
                 raise RuntimeError("Unfortunately, a token is required and you do not have ArcGIS Pro installed on this device. We are unable to generate a token, so please move onto a device that has ArcGIS installed.")
```

### Comparing `uintel-0.3.8/src/uintel/fonts/Myriad Pro (TrueType).ttf` & `uintel-0.3.9/src/uintel/fonts/Myriad Pro (TrueType).ttf`

 * *Files identical despite different names*

### Comparing `uintel-0.3.8/src/uintel/fonts/Rubik (TrueType).ttf` & `uintel-0.3.9/src/uintel/fonts/Rubik (TrueType).ttf`

 * *Files identical despite different names*

### Comparing `uintel-0.3.8/src/uintel/fonts/Rubik Italic (TrueType).ttf` & `uintel-0.3.9/src/uintel/fonts/Rubik Italic (TrueType).ttf`

 * *Files identical despite different names*

### Comparing `uintel-0.3.8/src/uintel/geometry.py` & `uintel-0.3.9/src/uintel/geometry.py`

 * *Files identical despite different names*

### Comparing `uintel-0.3.8/src/uintel/install.py` & `uintel-0.3.9/src/uintel/install.py`

 * *Files identical despite different names*

### Comparing `uintel-0.3.8/src/uintel/ogc.py` & `uintel-0.3.9/src/uintel/ogc.py`

 * *Files identical despite different names*

### Comparing `uintel-0.3.8/src/uintel/query.py` & `uintel-0.3.9/src/uintel/query.py`

 * *Files identical despite different names*

### Comparing `uintel-0.3.8/src/uintel/server.py` & `uintel-0.3.9/src/uintel/server.py`

 * *Files identical despite different names*

### Comparing `uintel-0.3.8/src/uintel/slack.py` & `uintel-0.3.9/src/uintel/slack.py`

 * *Files identical despite different names*

### Comparing `uintel-0.3.8/src/uintel/sql.py` & `uintel-0.3.9/src/uintel/sql.py`

 * *Files identical despite different names*

### Comparing `uintel-0.3.8/src/uintel/styles/ui.mplstyle` & `uintel-0.3.9/src/uintel/styles/ui.mplstyle`

 * *Files identical despite different names*

### Comparing `uintel-0.3.8/src/uintel.egg-info/PKG-INFO` & `uintel-0.3.9/src/uintel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uintel
-Version: 0.3.8
+Version: 0.3.9
 Summary: Urban Intelligence's unified Python data analysis toolkit
 Home-page: https://uintel.github.io/pyui/
 Author: Sam Archie
 Author-email: sam.archie@urbanintelligence.co.nz
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `uintel-0.3.8/src/uintel.egg-info/SOURCES.txt` & `uintel-0.3.9/src/uintel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

