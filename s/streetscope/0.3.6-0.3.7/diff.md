# Comparing `tmp/streetscope-0.3.6.tar.gz` & `tmp/streetscope-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streetscope-0.3.6.tar", max compression
+gzip compressed data, was "streetscope-0.3.7.tar", max compression
```

## Comparing `streetscope-0.3.6.tar` & `streetscope-0.3.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0     1072 2023-04-28 01:06:03.496785 streetscope-0.3.6/LICENSE
--rw-r--r--   0        0        0      689 2023-04-28 01:06:03.507513 streetscope-0.3.6/README.md
--rw-r--r--   0        0        0      672 2023-05-07 06:22:50.025105 streetscope-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      141 2023-04-28 01:35:32.382729 streetscope-0.3.6/src/streetscope/__init__.py
--rw-r--r--   0        0        0       27 2023-04-28 01:36:07.601106 streetscope-0.3.6/src/streetscope/cv/__init__.py
--rw-r--r--   0        0        0       27 2023-04-28 10:12:41.686471 streetscope-0.3.6/src/streetscope/cv/segmentation/__init__.py
--rw-r--r--   0        0        0    39101 2023-05-05 01:28:21.346862 streetscope-0.3.6/src/streetscope/cv/segmentation/segmentation.py
--rw-r--r--   0        0        0       55 2023-04-13 03:44:34.089983 streetscope-0.3.6/src/streetscope/download/__init__.py
--rw-r--r--   0        0        0    11847 2023-05-07 06:18:13.579525 streetscope-0.3.6/src/streetscope/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-04-12 01:36:02.614098 streetscope-0.3.6/src/streetscope/download/utils/UserAgent.csv
--rw-r--r--   0        0        0        0 2023-04-12 07:50:41.918376 streetscope-0.3.6/src/streetscope/download/utils/__init__.py
--rw-r--r--   0        0        0     8527 2023-05-07 06:21:09.842314 streetscope-0.3.6/src/streetscope/download/utils/geoprocess.py
--rw-r--r--   0        0        0     1730 2023-05-07 06:09:51.861103 streetscope-0.3.6/src/streetscope/download/utils/get_pids.py
--rw-r--r--   0        0        0     8108 2023-05-05 23:52:21.840224 streetscope-0.3.6/src/streetscope/download/utils/imtool.py
--rw-r--r--   0        0        0        0 2023-04-28 01:06:03.540992 streetscope-0.3.6/src/streetscope/streetscope.py
--rw-r--r--   0        0        0       30 2023-05-03 02:17:38.864664 streetscope-0.3.6/src/streetscope/transform/__init__.py
--rw-r--r--   0        0        0     6768 2023-04-28 09:51:23.730858 streetscope-0.3.6/src/streetscope/transform/transform_image.py
--rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 streetscope-0.3.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-04-28 01:06:03.496785 streetscope-0.3.7/LICENSE
+-rw-r--r--   0        0        0      689 2023-04-28 01:06:03.507513 streetscope-0.3.7/README.md
+-rw-r--r--   0        0        0      655 2023-05-07 07:14:37.251435 streetscope-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      141 2023-04-28 01:35:32.382729 streetscope-0.3.7/src/streetscope/__init__.py
+-rw-r--r--   0        0        0       27 2023-04-28 01:36:07.601106 streetscope-0.3.7/src/streetscope/cv/__init__.py
+-rw-r--r--   0        0        0       27 2023-04-28 10:12:41.686471 streetscope-0.3.7/src/streetscope/cv/segmentation/__init__.py
+-rw-r--r--   0        0        0    39101 2023-05-05 01:28:21.346862 streetscope-0.3.7/src/streetscope/cv/segmentation/segmentation.py
+-rw-r--r--   0        0        0       55 2023-04-13 03:44:34.089983 streetscope-0.3.7/src/streetscope/download/__init__.py
+-rw-r--r--   0        0        0    11712 2023-05-07 06:44:22.707808 streetscope-0.3.7/src/streetscope/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-04-12 01:36:02.614098 streetscope-0.3.7/src/streetscope/download/utils/UserAgent.csv
+-rw-r--r--   0        0        0        0 2023-04-12 07:50:41.918376 streetscope-0.3.7/src/streetscope/download/utils/__init__.py
+-rw-r--r--   0        0        0     8527 2023-05-07 06:28:47.875496 streetscope-0.3.7/src/streetscope/download/utils/geoprocess.py
+-rw-r--r--   0        0        0     1730 2023-05-07 06:09:51.861103 streetscope-0.3.7/src/streetscope/download/utils/get_pids.py
+-rw-r--r--   0        0        0     8108 2023-05-05 23:52:21.840224 streetscope-0.3.7/src/streetscope/download/utils/imtool.py
+-rw-r--r--   0        0        0        0 2023-04-28 01:06:03.540992 streetscope-0.3.7/src/streetscope/streetscope.py
+-rw-r--r--   0        0        0       30 2023-05-03 02:17:38.864664 streetscope-0.3.7/src/streetscope/transform/__init__.py
+-rw-r--r--   0        0        0     6768 2023-04-28 09:51:23.730858 streetscope-0.3.7/src/streetscope/transform/transform_image.py
+-rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 streetscope-0.3.7/PKG-INFO
```

### Comparing `streetscope-0.3.6/LICENSE` & `streetscope-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.6/README.md` & `streetscope-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.6/pyproject.toml` & `streetscope-0.3.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [tool.poetry]
 name = "streetscope"
-version = "0.3.6"
+version = "0.3.7"
 description = "This package handles downloading, cleaning, analyzing street view imagery"
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-aiohttp="^3.8.4"
 Pillow = ">=8.3.2,<9.6"
 geopandas = "^0.9.0"
 geopy = "^2.2.0"
 numpy = "^1.21.2"
 opencv_python = "^4.5.3"
 osmnx = "^1.1.1"
 pandas = "^1.3.3"
```

### Comparing `streetscope-0.3.6/src/streetscope/cv/segmentation/segmentation.py` & `streetscope-0.3.7/src/streetscope/cv/segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.6/src/streetscope/download/streetview_downloader.py` & `streetscope-0.3.7/src/streetscope/download/streetview_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,16 +139,16 @@
 
         def worker(index, row):
             panoid = row['panoid']
             year_month = get_year_month(panoid)
             return index, year_month
         
         with ThreadPoolExecutor() as executor:
-            futures = {executor.submit(worker, i, row): i for i, row in tqdm(df.iterrows(), total = len(df), desc="Preparing to augment metadata", ncols=100)}
-            for future in tqdm(as_completed(futures), total=len(futures), desc="Augmenting timestamp metadata", ncols=100):
+            futures = {executor.submit(worker, i, row): i for i, row in tqdm(df.iterrows(), total = len(df), desc="Preparing to augment metadata")}
+            for future in tqdm(as_completed(futures), total=len(futures), desc="Augmenting timestamp metadata"):
                 row_index, year_month = future.result()
                 df.at[row_index, 'year'] = year_month['year']
                 df.at[row_index, 'month'] = year_month['month']
         return df
                     
     def _get_pids_from_csv(self, input_csv_file, closest=False, disp=False):
         def get_street_view_info(longitude, latitude):
@@ -173,29 +173,28 @@
                     df.rename(columns={col: 'latitude'}, inplace=True)
 
             return df
         df = standardize_column_names(df)
         results = []
 
         with ThreadPoolExecutor() as executor:
-            futures = {executor.submit(worker, row): (row['longitude'], row['latitude']) for _, row in tqdm(df.iterrows(), total = len(df), desc="Preparing to get pids", ncols=100)}
-            for future in tqdm(as_completed(futures), total=len(futures), desc="Getting pids", ncols=100):
+            futures = {executor.submit(worker, row): (row['longitude'], row['latitude']) for _, row in tqdm(df.iterrows(), total = len(df), desc="Preparing to get pids")}
+            for future in tqdm(as_completed(futures), total=len(futures), desc="Getting pids"):
                 (input_longitude, input_latitude), row_results = future.result()
                 for result in row_results:
                     result['input_longitude'] = input_longitude
                     result['input_latitude'] = input_latitude
                     results.append(result)
 
         results_df = pd.DataFrame(results)
         return results_df
     
     def _get_pids_from_shp(self, input_shp_file, closest=False, disp=False):  
         def get_street_view_info(longitude, latitude):
-            with requests.Session() as session:
-                results = panoids(latitude, longitude, closest=closest, disp=disp, session=session)
+            results = panoids(latitude, longitude, closest=closest, disp=disp)
             return results
 
         def worker(row):
             input_longitude = row['longitude']
             input_latitude = row['latitude']
             results = get_street_view_info(input_longitude, input_latitude)
             return (input_longitude, input_latitude), results
@@ -203,16 +202,16 @@
         # read shapefile
         gdf = gpd.read_file(input_shp_file)
         gp = GeoProcessor(gdf, distance=self.distance, grid=self.grid, grid_size=self.grid_size)
         df = gp.get_lat_lon()
         results = []
 
         with ThreadPoolExecutor() as executor:
-            futures = {executor.submit(worker, row): (row['longitude'], row['latitude']) for _, row in tqdm(df.iterrows(), total = len(df), desc="Preparing to get pids", ncols=100)}
-            for future in tqdm(as_completed(futures), total=len(futures), desc="Getting pids", ncols=100):
+            futures = {executor.submit(worker, row): (row['longitude'], row['latitude']) for _, row in tqdm(df.iterrows(), total = len(df), desc="Preparing to get pids")}
+            for future in tqdm(as_completed(futures), total=len(futures), desc="Getting pids"):
                 (input_longitude, input_latitude), row_results = future.result()
                 for result in row_results:
                     result['input_longitude'] = input_longitude
                     result['input_latitude'] = input_latitude
                     results.append(result)
 
         results_df = pd.DataFrame(results)
```

### Comparing `streetscope-0.3.6/src/streetscope/download/utils/UserAgent.csv` & `streetscope-0.3.7/src/streetscope/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.6/src/streetscope/download/utils/geoprocess.py` & `streetscope-0.3.7/src/streetscope/download/utils/geoprocess.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.6/src/streetscope/download/utils/get_pids.py` & `streetscope-0.3.7/src/streetscope/download/utils/get_pids.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.6/src/streetscope/download/utils/imtool.py` & `streetscope-0.3.7/src/streetscope/download/utils/imtool.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.6/src/streetscope/transform/transform_image.py` & `streetscope-0.3.7/src/streetscope/transform/transform_image.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.6/PKG-INFO` & `streetscope-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: streetscope
-Version: 0.3.6
+Version: 0.3.7
 Summary: This package handles downloading, cleaning, analyzing street view imagery
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=8.3.2,<9.6)
 Requires-Dist: Shapely (>=1.7.1,<2.0.0)
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: geopandas (>=0.9.0,<0.10.0)
 Requires-Dist: geopy (>=2.2.0,<3.0.0)
 Requires-Dist: numpy (>=1.21.2,<2.0.0)
 Requires-Dist: opencv_python (>=4.5.3,<5.0.0)
 Requires-Dist: osmnx (>=1.1.1,<2.0.0)
 Requires-Dist: pandas (>=1.3.3,<2.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
```

