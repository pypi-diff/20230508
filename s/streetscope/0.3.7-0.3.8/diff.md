# Comparing `tmp/streetscope-0.3.7.tar.gz` & `tmp/streetscope-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streetscope-0.3.7.tar", max compression
+gzip compressed data, was "streetscope-0.3.8.tar", max compression
```

## Comparing `streetscope-0.3.7.tar` & `streetscope-0.3.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0     1072 2023-04-28 01:06:03.496785 streetscope-0.3.7/LICENSE
--rw-r--r--   0        0        0      689 2023-04-28 01:06:03.507513 streetscope-0.3.7/README.md
--rw-r--r--   0        0        0      655 2023-05-07 07:14:37.251435 streetscope-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      141 2023-04-28 01:35:32.382729 streetscope-0.3.7/src/streetscope/__init__.py
--rw-r--r--   0        0        0       27 2023-04-28 01:36:07.601106 streetscope-0.3.7/src/streetscope/cv/__init__.py
--rw-r--r--   0        0        0       27 2023-04-28 10:12:41.686471 streetscope-0.3.7/src/streetscope/cv/segmentation/__init__.py
--rw-r--r--   0        0        0    39101 2023-05-05 01:28:21.346862 streetscope-0.3.7/src/streetscope/cv/segmentation/segmentation.py
--rw-r--r--   0        0        0       55 2023-04-13 03:44:34.089983 streetscope-0.3.7/src/streetscope/download/__init__.py
--rw-r--r--   0        0        0    11712 2023-05-07 06:44:22.707808 streetscope-0.3.7/src/streetscope/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-04-12 01:36:02.614098 streetscope-0.3.7/src/streetscope/download/utils/UserAgent.csv
--rw-r--r--   0        0        0        0 2023-04-12 07:50:41.918376 streetscope-0.3.7/src/streetscope/download/utils/__init__.py
--rw-r--r--   0        0        0     8527 2023-05-07 06:28:47.875496 streetscope-0.3.7/src/streetscope/download/utils/geoprocess.py
--rw-r--r--   0        0        0     1730 2023-05-07 06:09:51.861103 streetscope-0.3.7/src/streetscope/download/utils/get_pids.py
--rw-r--r--   0        0        0     8108 2023-05-05 23:52:21.840224 streetscope-0.3.7/src/streetscope/download/utils/imtool.py
--rw-r--r--   0        0        0        0 2023-04-28 01:06:03.540992 streetscope-0.3.7/src/streetscope/streetscope.py
--rw-r--r--   0        0        0       30 2023-05-03 02:17:38.864664 streetscope-0.3.7/src/streetscope/transform/__init__.py
--rw-r--r--   0        0        0     6768 2023-04-28 09:51:23.730858 streetscope-0.3.7/src/streetscope/transform/transform_image.py
--rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 streetscope-0.3.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-04-28 01:06:03.496785 streetscope-0.3.8/LICENSE
+-rw-r--r--   0        0        0      689 2023-04-28 01:06:03.507513 streetscope-0.3.8/README.md
+-rw-r--r--   0        0        0      655 2023-05-08 06:44:40.178091 streetscope-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0      141 2023-04-28 01:35:32.382729 streetscope-0.3.8/src/streetscope/__init__.py
+-rw-r--r--   0        0        0       27 2023-04-28 01:36:07.601106 streetscope-0.3.8/src/streetscope/cv/__init__.py
+-rw-r--r--   0        0        0       27 2023-04-28 10:12:41.686471 streetscope-0.3.8/src/streetscope/cv/segmentation/__init__.py
+-rw-r--r--   0        0        0    38123 2023-05-08 06:40:15.055721 streetscope-0.3.8/src/streetscope/cv/segmentation/segmentation.py
+-rw-r--r--   0        0        0       55 2023-04-13 03:44:34.089983 streetscope-0.3.8/src/streetscope/download/__init__.py
+-rw-r--r--   0        0        0    10879 2023-05-08 06:39:30.199613 streetscope-0.3.8/src/streetscope/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-04-12 01:36:02.614098 streetscope-0.3.8/src/streetscope/download/utils/UserAgent.csv
+-rw-r--r--   0        0        0        0 2023-04-12 07:50:41.918376 streetscope-0.3.8/src/streetscope/download/utils/__init__.py
+-rw-r--r--   0        0        0     8218 2023-05-08 06:39:41.173631 streetscope-0.3.8/src/streetscope/download/utils/geoprocess.py
+-rw-r--r--   0        0        0     1730 2023-05-07 06:09:51.861103 streetscope-0.3.8/src/streetscope/download/utils/get_pids.py
+-rw-r--r--   0        0        0     8108 2023-05-05 23:52:21.840224 streetscope-0.3.8/src/streetscope/download/utils/imtool.py
+-rw-r--r--   0        0        0        0 2023-04-28 01:06:03.540992 streetscope-0.3.8/src/streetscope/streetscope.py
+-rw-r--r--   0        0        0       30 2023-05-03 02:17:38.864664 streetscope-0.3.8/src/streetscope/transform/__init__.py
+-rw-r--r--   0        0        0     6500 2023-05-08 06:40:31.590915 streetscope-0.3.8/src/streetscope/transform/transform_image.py
+-rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 streetscope-0.3.8/PKG-INFO
```

### Comparing `streetscope-0.3.7/LICENSE` & `streetscope-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.7/README.md` & `streetscope-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.7/pyproject.toml` & `streetscope-0.3.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streetscope"
-version = "0.3.7"
+version = "0.3.8"
 description = "This package handles downloading, cleaning, analyzing street view imagery"
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `streetscope-0.3.7/src/streetscope/cv/segmentation/segmentation.py` & `streetscope-0.3.8/src/streetscope/cv/segmentation/segmentation.py`

 * *Files 3% similar despite different names*

```diff
@@ -681,18 +681,8 @@
             nested_dict = results_to_nested_dict(results)
             with open(json_output_file, 'w') as f:
                 json.dump(nested_dict, f, indent=2) 
                 
         if "csv" in pixel_ratio_save_format:
             csv_output_file = Path(dir_output) / 'pixel_ratio.csv'
             df = results_to_dataframe(results)
-            df.to_csv(csv_output_file)
-    
-if __name__ == "__main__":
-    segmentation = Segmenter()
-    # segmentation.segment("/Users/koichiito/Downloads/Delft/panorama", 
-    #                     "/Users/koichiito/Downloads/Delft/panorama_segmented", 
-    #                     dir_pixel_ratio_output = "/Users/koichiito/Downloads/Delft",
-    #                     batch_size=1, num_workers=1, save_image_options = ["segmented_image"], pixel_ratio_save_format=[])
-    segmentation.calculate_pixel_ratio_post_process("/Users/koichiito/Downloads/Delft/panorama_segmented", "/Users/koichiito/Downloads/Delft", pixel_ratio_save_format=["json", "csv"])
-    # segmentation = Segmenter(model_name="facebook/mask2former-swin-large-mapillary-vistas-semantic", dataset="mapillary")
-    # segmentation.segment("/Users/koichiito/Desktop/test2/panorama", "/Users/koichiito/Desktop/test2/panorama_segmented", batch_size=5, num_workers=5, save_image_options = ["segmented_image", "blend_image"], pixel_ratio_save_format="csv")
+            df.to_csv(csv_output_file)
```

### Comparing `streetscope-0.3.7/src/streetscope/download/streetview_downloader.py` & `streetscope-0.3.8/src/streetscope/download/streetview_downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -264,19 +264,8 @@
         panoids = self._read_pids(path_pid)
         panoids_rest = self._check_already(panoids)
 
         panoids = self._read_pids(path_pid)
         panoids_rest = self._check_already(panoids)
 
         UAs = random.choices(self.user_agent, k = len(panoids_rest))
-        ImageTool.dwl_multiple(panoids_rest, zoom, v_tiles, h_tiles, panorama_output, UAs, cropped, full, log_path=self.log_path)
-
-if __name__ == "__main__":
-    sv_downloader = StreetViewDownloader(gsv_api_key="AIzaSyCPHEaGhci712SM9UsB8f-Mdpl1lsA6VH0", 
-                                        log_path = "/Volumes/exfat_archi/streetscope_test/delft",
-                                        distance=1
-                                        # grid = True, grid_size = 0.1
-                                        )
-    sv_downloader.download_gsv("/Volumes/exfat_archi/streetscope_test/delft/images", 
-                            # path_pid = "/Volumes/exfat_archi/streetscope_test/delft/images/pids.csv",
-                            input_shp_file = "/Volumes/exfat_archi/streetscope_test/delft/Delft/Delft.shp", augment_metadata=True)
-    # sv_downloader.download_gsv("/Users/koichiito/Downloads/Delft", lat = 52.004400, lng = 4.342597, augment_metadata=True)
+        ImageTool.dwl_multiple(panoids_rest, zoom, v_tiles, h_tiles, panorama_output, UAs, cropped, full, log_path=self.log_path)
```

### Comparing `streetscope-0.3.7/src/streetscope/download/utils/UserAgent.csv` & `streetscope-0.3.8/src/streetscope/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.7/src/streetscope/download/utils/geoprocess.py` & `streetscope-0.3.8/src/streetscope/download/utils/geoprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,16 +163,8 @@
         gdf['geometry'] = gpd.GeoSeries(gdf['street_points'], crs=self.utm_crs)
         gdf = gdf.to_crs("EPSG:4326")
         
         # Extract longitude and latitude
         gdf['longitude'] = gdf.geometry.x
         gdf['latitude'] = gdf.geometry.y
         
-        return gdf[['longitude', 'latitude']]
-    
-if __name__ == "__main__":
-    # Example usage:
-    gdf = gpd.read_file('/Users/koichiito/Downloads/Delft/Delft.shp')
-    processor = GeoProcessor(gdf, distance=1)
-    result_gdf = processor.get_lat_lon()
-    # save as csv
-    result_gdf.to_csv('/Users/koichiito/Downloads/Delft/Delft.csv', index=False)
+        return gdf[['longitude', 'latitude']]
```

### Comparing `streetscope-0.3.7/src/streetscope/download/utils/get_pids.py` & `streetscope-0.3.8/src/streetscope/download/utils/get_pids.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.7/src/streetscope/download/utils/imtool.py` & `streetscope-0.3.8/src/streetscope/download/utils/imtool.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.7/src/streetscope/transform/transform_image.py` & `streetscope-0.3.8/src/streetscope/transform/transform_image.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,12 +171,8 @@
             dir_output = Path(self.dir_output) / current_style
             dir_output.mkdir(parents=True, exist_ok=True)
 
             with ThreadPoolExecutor() as executor:
                 futures = [executor.submit(run, *process_image(self.dir_input, dir_output, name, show_size, current_style)) \
                     for name in self.dir_input.rglob('*') if name.suffix.lower() in image_extensions]
                 for future in tqdm(as_completed(futures), total=len(futures), desc=f"Converting to {current_style}"):
-                    future.result()
-
-if __name__ == "__main__":
-    image_transformer = ImageTransformer(dir_input="/Users/koichiito/Desktop/test/panorama_segmented", dir_output="/Users/koichiito/Desktop/test")
-    image_transformer.transform_images(style_list=["perspective", "fisheye"], show_size=100)
+                    future.result()
```

### Comparing `streetscope-0.3.7/PKG-INFO` & `streetscope-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streetscope
-Version: 0.3.7
+Version: 0.3.8
 Summary: This package handles downloading, cleaning, analyzing street view imagery
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

