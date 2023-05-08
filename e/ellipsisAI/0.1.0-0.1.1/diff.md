# Comparing `tmp/ellipsisAI-0.1.0.tar.gz` & `tmp/ellipsisAI-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellipsisAI-0.1.0.tar", last modified: Thu Nov 17 19:11:09 2022, max compression
+gzip compressed data, was "ellipsisAI-0.1.1.tar", last modified: Mon May  8 16:27:03 2023, max compression
```

## Comparing `ellipsisAI-0.1.0.tar` & `ellipsisAI-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2022-11-17 19:11:09.556591 ellipsisAI-0.1.0/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1074 2022-11-17 11:43:37.000000 ellipsisAI-0.1.0/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5162 2022-11-17 19:11:09.556591 ellipsisAI-0.1.0/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4653 2022-11-17 11:43:37.000000 ellipsisAI-0.1.0/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2022-11-17 19:11:09.556591 ellipsisAI-0.1.0/ellipsisAI/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    13484 2022-11-17 15:50:28.000000 ellipsisAI-0.1.0/ellipsisAI/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2022-11-17 19:11:09.556591 ellipsisAI-0.1.0/ellipsisAI.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5162 2022-11-17 19:11:09.000000 ellipsisAI-0.1.0/ellipsisAI.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      233 2022-11-17 19:11:09.000000 ellipsisAI-0.1.0/ellipsisAI.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2022-11-17 19:11:09.000000 ellipsisAI-0.1.0/ellipsisAI.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       74 2022-11-17 19:11:09.000000 ellipsisAI-0.1.0/ellipsisAI.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       11 2022-11-17 19:11:09.000000 ellipsisAI-0.1.0/ellipsisAI.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       90 2022-11-17 11:43:37.000000 ellipsisAI-0.1.0/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2022-11-17 19:11:09.560591 ellipsisAI-0.1.0/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      887 2022-11-17 19:10:55.000000 ellipsisAI-0.1.0/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-08 16:27:03.060128 ellipsisAI-0.1.1/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1074 2022-11-17 11:43:37.000000 ellipsisAI-0.1.1/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4217 2023-05-08 16:27:03.060128 ellipsisAI-0.1.1/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3745 2023-05-08 16:26:52.000000 ellipsisAI-0.1.1/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-08 16:27:03.060128 ellipsisAI-0.1.1/ellipsisAI/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    11267 2023-05-08 16:26:18.000000 ellipsisAI-0.1.1/ellipsisAI/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-08 16:27:03.060128 ellipsisAI-0.1.1/ellipsisAI.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4217 2023-05-08 16:27:02.000000 ellipsisAI-0.1.1/ellipsisAI.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      233 2023-05-08 16:27:02.000000 ellipsisAI-0.1.1/ellipsisAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-05-08 16:27:02.000000 ellipsisAI-0.1.1/ellipsisAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       74 2023-05-08 16:27:02.000000 ellipsisAI-0.1.1/ellipsisAI.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       11 2023-05-08 16:27:02.000000 ellipsisAI-0.1.1/ellipsisAI.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       90 2022-11-17 11:43:37.000000 ellipsisAI-0.1.1/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-05-08 16:27:03.060128 ellipsisAI-0.1.1/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      887 2023-05-08 16:18:10.000000 ellipsisAI-0.1.1/setup.py
```

### Comparing `ellipsisAI-0.1.0/LICENSE` & `ellipsisAI-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ellipsisAI-0.1.0/PKG-INFO` & `ellipsisAI-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: ellipsisAI
-Version: 0.1.0
+Version: 0.1.1
 Summary: Package to use Ellipsis Drive for AI
 Home-page: https://github.com/ellipsis-drive-internal/python-package-AI
 Author: Daniel van der Maas
 Author-email: daniel@ellipsis-drive.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -23,119 +21,106 @@
 ```
 
 ### Example
 ```python
 import ellipsisAI as ai
 import ellipsis as el
 
-blockId = '170aadad-8eaa-4509-9c0e-c1536d58a1fe'
-captureId = "633b4b9f-d939-4c4a-8d90-0e9fceb64b83"
-targetBlockId = "066458f4-f018-4f49-a1f0-dedfa71b3368"
-temp_folder = 'YOUR_PATH'
+pathId = '170aadad-8eaa-4509-9c0e-c1536d58a1fe'
+timestampId = "633b4b9f-d939-4c4a-8d90-0e9fceb64b83"
+targetPathId = "066458f4-f018-4f49-a1f0-dedfa71b3368"
+tempFolder = 'YOUR_PATH'
 
 #login to get a authentication token
-token = el.logIn('YOUR_USERNAME','YOUR_PASSWORD')
+token = el.account.logIn('YOUR_USERNAME','YOUR_PASSWORD')
 
 #retrieve the zoom and bounds of the capture you wish to classify
-classificationZoom = ai.getZoom(blockId, captureId, token)
-bounds = ai.getBounds(blockId, captureId, token)
+classificationZoom = ai.getReccomendedClassificationZoom(pathId = pathId, timestampId = timestampId, token = token)
+bounds = el.path.raster.timestamp.getBounds(pathId, timestampId, token)
 
 
 #we create a dummy model. We use the identity function mapping an image to itself. We use the getTleData function to retirve the image for the given input tile ofthe model.
 def model(tile):
-    image = ai.getTileData(blockId, captureId, tile, token)
-    return(image)
+    result = ai.getTileData(pathId = pathId, timestampId = timestampId, tile = tile, token  = token)
+    if result['status'] == 204:
+        output =  np.zeros((1,256,256))
+    else:
+        r = result['result']
+
+        output = r[0:1,:,:] * 2
+    return(output)
+
 
 #apply the model on the given bounds on the given zoomlevel
-ai.applyModel(model, bounds, targetBlockId, classificationZoom, token, temp_folder)
+ai.applyModel(model, bounds, targetPathId, classificationZoom, token, tempFolder)
 ```
 
 
 ### Functions
 
-#### getZoom
+#### applyModel
 
 ```python
-getZoom(blockId, captureId, token)
+applyModel(model, bounds, targetPathId, classificationZoom, token, tempFolder, modelNoDataValue = -1, targetFromDate = None, targetToDate = None)
 ```
 
-This function retrieves the max zoomlevel of the specified capture. The result can be used as classificationgZoom argument in the applyModel or getTiles function.
+This function applies the given model on all tiles of zoomlevel classificationZoom withing the specified bounds. The results will be written in a new capture of the specified target block.
 
 | Name        | Description |
 | ----------- | -----------|
-| blockId     | The id of the block the capture is in |
-| captureId     | The id of the capture |
+| model        | A function mapping given bounds to a 3D numpy array. |
+| bounds        | A shapely polygon or multipolygon indicating the region you wish to classify |
+| targetPathId        | The id of the path to write the result to |
+| classificationZoom        | The zoomlevel of the tiles you wish to use for the model input as integer. |
 | token        | Your token|
+| tempFolder        | A path where temporary files can be written|
+| modelNoDataValue        | Which number of the model output to interpret as transparent|
+| targetDate        | Dictionary with keys from and to, both must be of type datetime. Defaults to current date|
 
 
-#### getBounds
-
-```python
-getBounds(blockId, captureId, token)
-```
 
-This function retrieves the bounds of the specified capture. The result can be used as bounds argument in the applyModel function.
-
-| Name        | Description |
-| ----------- | -----------|
-| blockId     | The id of the block the capture is in |
-| captureId     | The id of the capture |
-| token        | Your token|
-
-
-#### applyModel
+#### getTiles
 
 ```python
-applyModel(model, bounds, targetBlockId, classificationZoom, token, temp_folder, visualizationId = None, targetNoDataValue = 0, targetStartDate = None, targetEndDate = None)
+getTiles(bounds, classificationZoom)
 ```
 
-This function applies the given model on all tiles of zoomlevel classificationZoom withing the specified bounds. The results will be written in a new capture of the specified target block.
+This function covers a given bounds with tiles of the given zoomlevel. You can use the result to get tile arguments for the getTileData function
 
 | Name        | Description |
 | ----------- | -----------|
-| model        | A function mapping mapping a tile object to a 3 dimensional numpy array. The dimensions of the numpy array should be independent of the tile id. A tile object is a dictionary with keys 'tileX', 'tileY' and 'zoom' as integers. |
-| bounds        | A shapely polygon or multipolygon indicating the region you wish to classify |
-| targetBlockId        | The id of the block to write the result to |
-| classificationZoom        | The zoomlevel of the tiles you wish to use for the model input as integer. |
-| token        | Your token|
-| temp_folder        | A path where temporary files can be written|
-| visualizationId        | visualization to use as input, if not given original raster is used|
-| targetNoDataValue        | Which number of the model output to interpret as transparent|
-| targetStartDate        | datetime object with date to use for the capture to which the results will be written. Defaults to current date|
-| targetEndDate        | datetime object with date to use for the capture to which the results will be written. Defaults to targetStartDate|
+| bounds     | A shapely polygon or multipolygon |
+| classificationZoom        | The zoomlevel of the tiles to cover with as int |
 
 
 
 #### getTileData
 
 ```python
-getTileData(blockId, captureId, tile, token, visualizationId = None, downsampleFactor = 1 )
+getTileData(pathId, timestampId, tile, token = None )
 ```
 
-This function retrieves data for the given tile as numpy array. This function can be used within your model function te retireve relevant data for the given tile.
+This function retrieves raster data for a certain tile.
 
 | Name        | Description |
 | ----------- | -----------|
-| blockId     | the id of the block to get data from |
-| captureId     | the id of the capture to get data from |
-| tile     | A dictionary with keys tileX, tileY and zoom as int |
-| token        | Your token|
-| visualizationId        | The id of the visualization you wish to retrieve. If not given raw data is used|
-| downsampleFactor        | A factor with which to downsample the data. Default 1 (no downsampling)|
-
+| PathId     | Id of the layer to retrieve the raster for |
+| timestampId        | Id of the timestamp to retrieve the raster for |
+| tile        | A dictionary with tileX, tileY and zoom as integers |
+| token        | Your token (optional) |
 
-#### getTiles
+#### getReccomendedClassificationZoom
 
 ```python
-getTiles(bounds, classificationZoom)
+getReccomendedClassificationZoom(pathId, timestampId, token = None)
 ```
 
-This function covers a given bounds with tiles of the given zoomlevel. You can use the result to get tile arguments for the getTileData function
+This function retrieves raster data for a certain tile.
 
 | Name        | Description |
 | ----------- | -----------|
-| bounds     | A shapely polygon or multipolygon |
-| classificationZoom        | The zoomlevel of the tiles to cover with as int |
-
+| PathId     | Id of the layer to retrieve the raster for |
+| timestampId        | Id of the timestamp to retrieve the raster for |
+| token        | Your token (optional) |
```

### Comparing `ellipsisAI-0.1.0/README.md` & `ellipsisAI-0.1.1/ellipsisAI.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,123 +1,126 @@
+Metadata-Version: 2.1
+Name: ellipsisAI
+Version: 0.1.1
+Summary: Package to use Ellipsis Drive for AI
+Home-page: https://github.com/ellipsis-drive-internal/python-package-AI
+Author: Daniel van der Maas
+Author-email: daniel@ellipsis-drive.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 This package is meant to help you run models on Ellipsis Drive content. It should be used in combination with the ellipsis package.
 
 
 ### Install
 ```python
 pip install ellipsisAI
 ```
 
 ### Example
 ```python
 import ellipsisAI as ai
 import ellipsis as el
 
-blockId = '170aadad-8eaa-4509-9c0e-c1536d58a1fe'
-captureId = "633b4b9f-d939-4c4a-8d90-0e9fceb64b83"
-targetBlockId = "066458f4-f018-4f49-a1f0-dedfa71b3368"
-temp_folder = 'YOUR_PATH'
+pathId = '170aadad-8eaa-4509-9c0e-c1536d58a1fe'
+timestampId = "633b4b9f-d939-4c4a-8d90-0e9fceb64b83"
+targetPathId = "066458f4-f018-4f49-a1f0-dedfa71b3368"
+tempFolder = 'YOUR_PATH'
 
 #login to get a authentication token
-token = el.logIn('YOUR_USERNAME','YOUR_PASSWORD')
+token = el.account.logIn('YOUR_USERNAME','YOUR_PASSWORD')
 
 #retrieve the zoom and bounds of the capture you wish to classify
-classificationZoom = ai.getZoom(blockId, captureId, token)
-bounds = ai.getBounds(blockId, captureId, token)
+classificationZoom = ai.getReccomendedClassificationZoom(pathId = pathId, timestampId = timestampId, token = token)
+bounds = el.path.raster.timestamp.getBounds(pathId, timestampId, token)
 
 
 #we create a dummy model. We use the identity function mapping an image to itself. We use the getTleData function to retirve the image for the given input tile ofthe model.
 def model(tile):
-    image = ai.getTileData(blockId, captureId, tile, token)
-    return(image)
+    result = ai.getTileData(pathId = pathId, timestampId = timestampId, tile = tile, token  = token)
+    if result['status'] == 204:
+        output =  np.zeros((1,256,256))
+    else:
+        r = result['result']
+
+        output = r[0:1,:,:] * 2
+    return(output)
+
 
 #apply the model on the given bounds on the given zoomlevel
-ai.applyModel(model, bounds, targetBlockId, classificationZoom, token, temp_folder)
+ai.applyModel(model, bounds, targetPathId, classificationZoom, token, tempFolder)
 ```
 
 
 ### Functions
 
-#### getZoom
+#### applyModel
 
 ```python
-getZoom(blockId, captureId, token)
+applyModel(model, bounds, targetPathId, classificationZoom, token, tempFolder, modelNoDataValue = -1, targetFromDate = None, targetToDate = None)
 ```
 
-This function retrieves the max zoomlevel of the specified capture. The result can be used as classificationgZoom argument in the applyModel or getTiles function.
+This function applies the given model on all tiles of zoomlevel classificationZoom withing the specified bounds. The results will be written in a new capture of the specified target block.
 
 | Name        | Description |
 | ----------- | -----------|
-| blockId     | The id of the block the capture is in |
-| captureId     | The id of the capture |
+| model        | A function mapping given bounds to a 3D numpy array. |
+| bounds        | A shapely polygon or multipolygon indicating the region you wish to classify |
+| targetPathId        | The id of the path to write the result to |
+| classificationZoom        | The zoomlevel of the tiles you wish to use for the model input as integer. |
 | token        | Your token|
+| tempFolder        | A path where temporary files can be written|
+| modelNoDataValue        | Which number of the model output to interpret as transparent|
+| targetDate        | Dictionary with keys from and to, both must be of type datetime. Defaults to current date|
 
 
-#### getBounds
 
-```python
-getBounds(blockId, captureId, token)
-```
-
-This function retrieves the bounds of the specified capture. The result can be used as bounds argument in the applyModel function.
-
-| Name        | Description |
-| ----------- | -----------|
-| blockId     | The id of the block the capture is in |
-| captureId     | The id of the capture |
-| token        | Your token|
-
-
-#### applyModel
+#### getTiles
 
 ```python
-applyModel(model, bounds, targetBlockId, classificationZoom, token, temp_folder, visualizationId = None, targetNoDataValue = 0, targetStartDate = None, targetEndDate = None)
+getTiles(bounds, classificationZoom)
 ```
 
-This function applies the given model on all tiles of zoomlevel classificationZoom withing the specified bounds. The results will be written in a new capture of the specified target block.
+This function covers a given bounds with tiles of the given zoomlevel. You can use the result to get tile arguments for the getTileData function
 
 | Name        | Description |
 | ----------- | -----------|
-| model        | A function mapping mapping a tile object to a 3 dimensional numpy array. The dimensions of the numpy array should be independent of the tile id. A tile object is a dictionary with keys 'tileX', 'tileY' and 'zoom' as integers. |
-| bounds        | A shapely polygon or multipolygon indicating the region you wish to classify |
-| targetBlockId        | The id of the block to write the result to |
-| classificationZoom        | The zoomlevel of the tiles you wish to use for the model input as integer. |
-| token        | Your token|
-| temp_folder        | A path where temporary files can be written|
-| visualizationId        | visualization to use as input, if not given original raster is used|
-| targetNoDataValue        | Which number of the model output to interpret as transparent|
-| targetStartDate        | datetime object with date to use for the capture to which the results will be written. Defaults to current date|
-| targetEndDate        | datetime object with date to use for the capture to which the results will be written. Defaults to targetStartDate|
+| bounds     | A shapely polygon or multipolygon |
+| classificationZoom        | The zoomlevel of the tiles to cover with as int |
 
 
 
 #### getTileData
 
 ```python
-getTileData(blockId, captureId, tile, token, visualizationId = None, downsampleFactor = 1 )
+getTileData(pathId, timestampId, tile, token = None )
 ```
 
-This function retrieves data for the given tile as numpy array. This function can be used within your model function te retireve relevant data for the given tile.
+This function retrieves raster data for a certain tile.
 
 | Name        | Description |
 | ----------- | -----------|
-| blockId     | the id of the block to get data from |
-| captureId     | the id of the capture to get data from |
-| tile     | A dictionary with keys tileX, tileY and zoom as int |
-| token        | Your token|
-| visualizationId        | The id of the visualization you wish to retrieve. If not given raw data is used|
-| downsampleFactor        | A factor with which to downsample the data. Default 1 (no downsampling)|
-
+| PathId     | Id of the layer to retrieve the raster for |
+| timestampId        | Id of the timestamp to retrieve the raster for |
+| tile        | A dictionary with tileX, tileY and zoom as integers |
+| token        | Your token (optional) |
 
-#### getTiles
+#### getReccomendedClassificationZoom
 
 ```python
-getTiles(bounds, classificationZoom)
+getReccomendedClassificationZoom(pathId, timestampId, token = None)
 ```
 
-This function covers a given bounds with tiles of the given zoomlevel. You can use the result to get tile arguments for the getTileData function
+This function retrieves raster data for a certain tile.
 
 | Name        | Description |
 | ----------- | -----------|
-| bounds     | A shapely polygon or multipolygon |
-| classificationZoom        | The zoomlevel of the tiles to cover with as int |
+| PathId     | Id of the layer to retrieve the raster for |
+| timestampId        | Id of the timestamp to retrieve the raster for |
+| token        | Your token (optional) |
+
```

### Comparing `ellipsisAI-0.1.0/ellipsisAI/__init__.py` & `ellipsisAI-0.1.1/ellipsisAI/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,131 +9,112 @@
 from io import BytesIO
 import requests
 import os
 import rasterio
 import geopandas as gpd
 from shapely import geometry
 import pandas as pd
-from PIL import Image
 
-__version__ = '0.1.0'
-url = 'https://api.ellipsis-drive.com/v1'
+__version__ = '0.1.1'
+url = 'https://api.ellipsis-drive.com/v3'
 
 s = requests.Session()
 
 cacheZoom = {}
 cacheBands = {}
 
+    
 
-def getZoom(pathId, timestampId, token):
+def getReccomendedClassificationZoom(pathId, timestampId, token = None):
+    
+    pathId = el.sanitize.validUuid('pathId', pathId, True)
+    timestampId = el.sanitize.validUuid('timestampId', timestampId, True)
+    token = el.sanitize.validString('token', token, False)    
+    
     blockId = pathId
     captureId = timestampId
     
     key = blockId + '_' + captureId
     if key in cacheZoom.keys():
         return(cacheZoom[key])
 
-    metadata = el.path.get(blockId, token)
+    metadata = el.path.get(pathId = blockId, token = token)
     
     if metadata['type'] != 'raster':
         raise ValueError('pathId is of type vector but must be of type raster')
     
     captures = [c for c in metadata['raster']['timestamps'] if c['id'] == captureId]
     
     if len(captures) == 0:
-        raise ValueError('given captureId does not exist')
+        raise ValueError('given timestampId does not exist')
 
     zoom = captures[0]['zoom']
     
     
     cacheZoom[key] = zoom
     return(zoom)
 
 
-def getNumBands(pathId, timestampId, token):
-    
-    blockId = pathId
-    captureId = timestampId
-    
-    key = blockId + '_' + captureId
-    if key in cacheBands.keys():
-        return(cacheBands[key])
 
-    metadata = el.path.get(blockId, token)
-    
-    if metadata['type'] != 'raster':
-        raise ValueError('pathId is of type vector but must be of type raster')
-    
 
-    numBands = len(metadata['raster']['bands'])
-        
-    cacheBands[key] = numBands
-    return(numBands)
+def applyModel(model, bounds, targetPathId, classificationZoom, token, tempFolder, modelNoDataValue = -1, targetDate = None):
+    def f():
+        return
 
+    if type(targetDate) == type(None):
+        targetStartDate = datetime.now()
+        targetEndDate = targetStartDate
 
 
-def getBounds(pathId, timestampId, token):
-    blockId = pathId
-    captureId = timestampId
-    metadata = el.path.get(blockId, token)
-    if metadata['type'] == 'folder':
-        raise ValueError('pathId is of type folder must be of type raster or vector')
-
-
-    captures = [c for c in metadata['raster']['timestamps'] if c['id'] == captureId]
-    
-    if len(captures) == 0:
-        raise ValueError('given captureId does not exist')
 
-    timestamp = captures[0]['id']
-    
-    bounds = el.path.raster.timestamp.getBounds(pathId = blockId, timestampId = timestamp, token = token )
-    
-    return(bounds)
+    if(type(model) != type(f)):
+        raise ValueError('model must be a function')
+        
+    targetPathId = el.sanitize.validUuid('targetPathId', targetPathId, True)
+    bounds = el.sanitize.validShapely('bounds', bounds, True)
+    classificationZoom = el.sanitize.validInt('classificationZoom', classificationZoom, True)
+    token = el.sanitize.validString('token', token, False)
+    tempFolder = el.sanitize.validString('tempFolder', tempFolder, True)
+    modelNoDataValue = el.sanitize.validFloat('modelNoDataValue', modelNoDataValue,  True)
+    targetDate = el.sanitize.validDateRange('targetDate', targetDate, False)
 
-def applyModel(model, bounds, targetPathId, classificationZoom, token, temp_folder, modelNoDataValue = -1, targetStartDate = None, targetEndDate = None):
-    targetBlockId = targetPathId
-    if type(targetStartDate) == type(None):
-        targetStartDate = datetime.now()
-    if type(targetEndDate) == type(None):
-        targetEndDate = targetStartDate
 
 
     targetNoDataValue = modelNoDataValue
     
     if not 'float' in str(type(targetNoDataValue)) and not 'int' in str(type(targetNoDataValue)) :
         raise ValueError('targetNoDataValue must be of type float')
         
         
     print('creating a capture to write in')
 
-    targetCaptureId = el.path.raster.timestamp.add(pathId = targetBlockId, date= {'from':targetStartDate, 'to':targetEndDate}, token=token)['id']
+    targetCaptureId = el.path.raster.timestamp.add(pathId = targetPathId, date= {'from':targetStartDate, 'to':targetEndDate}, token=token)['id']
     print('writing to capture ' + targetCaptureId)
     if  str(type(bounds)) != "<class 'shapely.geometry.polygon.Polygon'>" and str(type(bounds)) != "<class 'shapely.geometry.multipolygon.MultiPolygon'>":
         raise ValueError('Bounds must be a shapely polygon or multipolygon')
         
     if str(type(bounds)) == "<class 'shapely.geometry.polygon.Polygon'>":
         bounds = [bounds]
     else:
         bounds = [b for b in bounds]
 
     output = model({'tileX':0, 'tileY':0, 'zoom':classificationZoom})
 
     if str(type(output)) != "<class 'numpy.ndarray'>":
-        raise ValueError('Output of model funciton must be a 3 dimensional numpy array')
+        raise ValueError('Output of model funciton must be a 3 dimensional numpy array, with the band number in the first dimension')
         
-    if output.shape[0] != output.shape[1]:
-        raise ValueError('First and second dimension of the resutling numpy array of model should have equal length.')
+    if output.shape[1] != output.shape[2]:
+        raise ValueError('Second and third dimension of the resutling numpy array of model should have equal length.')
     if len(output.shape) != 3:
-        raise ValueError('Output of model funciton mus ba a 3 dimensional numpy array')
-    outputWidth = output.shape[0]
-    bands_out = output.shape[2]    
+        raise ValueError('Output of model function mus ba a 3 dimensional numpy array, with the band number in the first dimension')
+    outputWidth = output.shape[1]
+    bands_out = output.shape[0]    
     
     if outputWidth >2048 or bands_out > 40:
-        raise ValueError("output width of model may not exceed 2048 by 2048 by 40.")
+        raise ValueError("output of model may not exceed 40 by 2048 by 2048.")
 
 
     bound = bounds[0]        
     for bound in bounds:
         print('applying model to a connected component of the bounds')
         x1, y1, x2, y2  = bound.bounds
         x1_osm =  math.floor((x1 +180 ) * 2**classificationZoom / 360 )
@@ -144,88 +125,63 @@
         y2_osm = min(2**classificationZoom-1,y2_osm)
         x1_osm = max(0,x1_osm)
         x2_osm = min(2**classificationZoom-1,x2_osm)
         
         total = (x2_osm - x1_osm+1 + (10 - (x2_osm - x1_osm+1)%10 ) ) * (y2_osm-y1_osm +1 + (10 - (y2_osm-y1_osm +1) % 10) )
         frac = 0
         
-        metadata = el.path.get(targetBlockId, token)
+        metadata = el.path.get(targetPathId, token)
         if metadata['type'] != 'raster':
             raise ValueError('pathId is of type folder must be of type raster or vector')
         
         x = x1_osm
         while x < x2_osm:
             y=y1_osm
             while y < y2_osm:
-                r_out = np.zeros(( 10*outputWidth, 10*outputWidth, bands_out+1))
+                r_out = np.zeros(( bands_out, 10*outputWidth, 10*outputWidth))
 
                 N = 0
                 for N in np.arange(10):
                     M=0
                     for M in np.arange(10):
                         frac = frac+1
                         el.util.loadingBar( frac, total)
-                        tile = {'zoom':classificationZoom, 'tileX':x+N, 'tileY':y+M}
-                        r_out[M*outputWidth:(M+1)*outputWidth, N*outputWidth:(N+1)*outputWidth, 0:bands_out] = model( TileToBounds(tile))
+                        tile = {'zoom': int(classificationZoom), 'tileX': float(x+N), 'tileY': float(y+M)}
+                        r_out[:,M*outputWidth:(M+1)*outputWidth, N*outputWidth:(N+1)*outputWidth] = model( tile)
+
 
 
-                r_out[r_out[:,:,-2] !=targetNoDataValue,-1] = 1
-                r_out = np.transpose(r_out, [2,0,1])
-                r_out = r_out.astype('float32')
                 xMin = x/2**classificationZoom *2* 2.003751e+07 - 2.003751e+07
                 xMax = (x + 10)/2**classificationZoom *2* 2.003751e+07 - 2.003751e+07
                 yMin = (2**classificationZoom - y-10)/2**classificationZoom * 2 * 2.003751e+07 - 2.003751e+07
                 yMax = (2**classificationZoom - y )/2**classificationZoom * 2*2.003751e+07 - 2.003751e+07
                 trans = rasterio.transform.from_bounds(xMin, yMin, xMax, yMax, r_out.shape[2], r_out.shape[1])
                 crs = "EPSG:3857"
-                file = temp_folder + '/' + str(frac) + ".tif"
-
+                file = tempFolder + '/' + str(frac) + ".tif"
+                dtype = r_out.dtype
                 
-                with rasterio.open( file, 'w', compress="lzw", tiled=True, blockxsize=256, blockysize=256, count = bands_out+1, width=10*outputWidth, height=10*outputWidth, dtype = 'float32', transform=trans, crs=crs) as dataset:
+                with rasterio.open( file, 'w', compress="lzw", tiled=True, blockxsize=256, blockysize=256, count = bands_out, width=10*outputWidth, height=10*outputWidth, dtype = dtype, transform=trans, crs=crs) as dataset:
                     dataset.write(r_out)
-                el.path.raster.timestamp.upload.add(pathId = targetBlockId, timestampId = targetCaptureId, filePath = file, token = token, fileFormat='tif')
+                el.path.raster.timestamp.file.add(pathId = targetPathId, timestampId = targetCaptureId, filePath = file, token = token, fileFormat='tif', noDataValue =  targetNoDataValue)
                 os.remove(file)
                 
                 y = y+10                
             x = x+10
 
-        captures = [c for c in metadata['raster']['timestamps'] if c['status'] == 'active']
-        if len(captures) ==0:
-            r = s.patch(url + '/path/' + targetBlockId + '/raster' , headers = {"Authorization":token},
-                             json = {'includesTransparent':True})
-            if int(str(r).split('[')[1].split(']')[0]) != 200:
-                raise ValueError(r.text)
 
         print('activating capture')
-        el.activateTimestamp(mapId = targetBlockId, timestampId=targetCaptureId, active = True, token = token)
+        el.path.raster.timestamp.activate(pathId = targetPathId, timestampId=targetCaptureId, token = token)
         print('capture activated result will be available soon')
 
 
-def TileToBounds(tile):
-    LEN = 2.003751e+07
-    x1_osm = tile['tileX']
-    y1_osm = tile['tileY']
-    readZoom  = tile['zoom']
-    
-    xMin = x1_osm * (2*LEN)/2**readZoom -LEN
-    xMax = (x1_osm + 1) * (2*LEN)/2**readZoom -LEN
-    yMax = -(y1_osm * (2*LEN)/2**readZoom -LEN)
-    yMin = -((y1_osm + 1) * (2*LEN)/2**readZoom -LEN)    
-    
-    p = geometry.Polygon( [(xMin, yMin), (xMin, yMax),(xMax, yMax),(xMax, yMin)] )
-    
-    sh = gpd.GeoDataFrame({'geometry':[p]})
-    sh.crs = 'EPSG:3857'
-    sh = sh.to_crs('EPSG:4326')
-    return sh['geometry'].values[0]
 
 def getTiles(bounds, classificationZoom):
     
-    if  str(type(bounds)) != "<class 'shapely.geometry.polygon.Polygon'>" and str(type(bounds)) != "<class 'shapely.geometry.multiPolygon.MultiPolygon'>":
-        raise ValueError('Bounds must be a shapely polygon or multipolygon')
+    bounds = el.sanitize.validShapely('bounds', bounds, True)
+    classificationZoom = el.sanitize.validInt('classificationZoom', classificationZoom, True)    
 
     
     if str(type(bounds)) == "<class 'shapely.geometry.polygon.Polygon'>":
         bounds = [bounds]
     else:
         bounds = [b for b in bounds]
 
@@ -281,78 +237,47 @@
     covering['tileZoom'] = classificationZoom
 
     return(covering)
     
     
     
 
-def getTileData(pathId, timestampId, tile, token, visualizationId = None, downsampleFactor = 1 ):
-    blockId = pathId
-    captureId = timestampId
+def getTileData(pathId, timestampId, tile, token = None ):
+    
+    pathId = el.sanitize.validUuid('pathId', pathId, True)
+    timestampId = el.sanitize.validUuid('timestampId', timestampId, True)
+    tile = el.sanitize.validObject('tile', tile, True)
+    token = el.sanitize.validString('token', token, False)
+    if not 'tileX' in tile.keys() or not 'tileY' in tile.keys() or not 'zoom' in tile.keys():
+        raise ValueError('tile parameter must contain keys, tileX, tileY and zoom, and must be float')
+    if type(tile['tileX']) != type(2.5) and type(tile['tileX']) != type(2) :
+        raise ValueError('tileX key in tile must be of type float')
+    if type(tile['tileY']) != type(2.5) and type(tile['tileY']) != type(2) :
+        raise ValueError('tileY key in tile must be of type float')
+    if type(tile['zoom']) != type(2) :
+        raise ValueError('zoom key in tile must be of type int')
     
     tileX = tile['tileX']
     tileY = tile['tileY']
-    tileZoom = tile['zoom']
-    
-    def getTile(token_inurl, blockId, captureId, visualizationId,x,y,zoom, num_bands ):
-        url_req = url + '/tileService/' + blockId + '/' + str(captureId) + '/' + visualizationId + '/' + str(zoom) + '/' + str(x) + '/' + str(y) + token_inurl
-        r = s.get(url_req , timeout = 10 )
-        if int(str(r).split('[')[1].split(']')[0]) == 403:
-                raise ValueError('Insufficient permission for block ' + blockId)
-        elif int(str(r).split('[')[1].split(']')[0]) != 200:
-                r = np.zeros((256,256,num_bands))
-        elif visualizationId == 'data':
-            r = np.transpose(tifffile.imread(BytesIO(r.content)), [1,2,0] )      
-        else:
-           r = np.array(Image.open(BytesIO(r.content)), dtype = 'uint8')
-        return(r)
-        
-
-    if type(token) != type('x'):
-        raise ValueError('token must be of type string')
-
-    token_inurl = '?token=' + token.replace('Bearer ', '')
-
-    if type(visualizationId) == type(None):
-        visualizationId = 'data'
+    zoom = tile['zoom']
     
+    if( type(token) != type(None) and 'Bearer' in token):
+        token = token.replace('Bearer', '')
+        token = token.replace(' ', '')
+    url_req = url + '/path/' + pathId + '/raster/timestamp/' + timestampId + '/tile/' + str(zoom) + '/' + str(tileX) + '/' + str(tileY)
+    
+    if (token != None):
+       url_req = url_req + '?token=' +  token
+       
+       
+    r = s.get(url_req , timeout = 10 )
+    if int(str(r).split('[')[1].split(']')[0]) == 403:
+            raise ValueError('Insufficient permission for layer ' + pathId)
+    elif r.status_code == 204:
+            return {'status':204, 'result':'no data'}
+    elif r.status_code != 200:
+            raise ValueError(r.text)            
     
-    
-    zoom = getZoom(blockId, captureId, token)
-    num_bands = getNumBands(blockId, captureId, token)
-
-    if not downsampleFactor in np.arange(1,zoom+1):
-        raise ValueError('downsampleFactor must be in ' + str(np.arange(1,zoom+1)))
-    
-    
-    nativeZoom = zoom - downsampleFactor + 1
-
-    if nativeZoom >= tileZoom:
-        factor = 2**(nativeZoom - tileZoom)            
-        r_total = np.zeros((256*factor , 256*factor, num_bands))
-        for x in np.arange(factor):
-            for y in np.arange(factor):
-                r = getTile(token_inurl, blockId, captureId, visualizationId, tileX*factor + x, tileY*factor+y,nativeZoom, num_bands )
-                r_total[ y*256: (y*256 + 256), x*256: (x*256 + 256) ,:] = r
-
-    else:
-        factor = 2**(tileZoom-nativeZoom)
-
-        x = math.floor(tileX/factor)
-        y = math.floor(tileY/factor)
-        r = getTile(token_inurl, blockId, captureId, visualizationId, x, y,nativeZoom )                
-      
-        starty =   (tileY - y*factor) * 256/factor
-        endy = (tileY - y*factor + 1) * 256/factor
-        startx =   (tileX - x*factor) * 256/factor
-        endx = (tileX - x*factor + 1) * 256/factor
+    r = tifffile.imread(BytesIO(r.content))
 
-        endy = math.floor(max(endy, starty+1))
-        endx = math.floor(max(endx, startx+1))
-        
-        r_total = r[starty:endy,startx:endx,:]
-        
 
-    return(r_total)
-    
-    
-    
+    return({'status':200, 'result':r})
```

### Comparing `ellipsisAI-0.1.0/setup.py` & `ellipsisAI-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ellipsisAI",
-    version="0.1.0",
+    version="0.1.1",
     author="Daniel van der Maas",
     author_email="daniel@ellipsis-drive.com",
     description="Package to use Ellipsis Drive for AI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ellipsis-drive-internal/python-package-AI",
     classifiers=[
```

