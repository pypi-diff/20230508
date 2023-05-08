# Comparing `tmp/sliderule-3.1.0.tar.gz` & `tmp/sliderule-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliderule-3.1.0.tar", last modified: Thu Apr 27 14:09:53 2023, max compression
+gzip compressed data, was "sliderule-3.2.0.tar", last modified: Mon May  8 12:42:08 2023, max compression
```

## Comparing `sliderule-3.1.0.tar` & `sliderule-3.2.0.tar`

### file list

```diff
@@ -1,51 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 14:09:53.818036 sliderule-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-04-27 14:09:41.000000 sliderule-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-04-27 14:09:41.000000 sliderule-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-04-27 14:09:53.818036 sliderule-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-04-27 14:09:41.000000 sliderule-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-27 14:09:41.000000 sliderule-3.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-27 14:09:53.818036 sliderule-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-04-27 14:09:41.000000 sliderule-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 14:09:53.818036 sliderule-3.1.0/sliderule/
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/arcticdem.py
--rw-r--r--   0 runner    (1001) docker     (122)    24752 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/earthdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    16811 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/gedi.py
--rw-r--r--   0 runner    (1001) docker     (122)     9833 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/h5.py
--rw-r--r--   0 runner    (1001) docker     (122)    36102 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/icesat2.py
--rw-r--r--   0 runner    (1001) docker     (122)    38844 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/ipxapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    85029 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/ipysliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)    44220 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/sliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-04-27 14:09:41.000000 sliderule-3.1.0/sliderule/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 14:09:53.818036 sliderule-3.1.0/sliderule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-04-27 14:09:53.000000 sliderule-3.1.0/sliderule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      998 2023-04-27 14:09:53.000000 sliderule-3.1.0/sliderule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 14:09:53.000000 sliderule-3.1.0/sliderule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-27 14:09:53.000000 sliderule-3.1.0/sliderule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-27 14:09:53.000000 sliderule-3.1.0/sliderule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 14:09:53.818036 sliderule-3.1.0/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     4151 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/_landsat.py
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/big_query.py
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/build_arctic_dem_mosaics_index.py
--rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/build_arctic_dem_mosaics_vrt_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/build_arctic_dem_strips_vrt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/extract_h5_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     7509 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/hls.py
--rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/icepyx_region.py
--rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/landsat.py
--rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/lpdaac_download.py
--rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/query_cmr.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/query_elevations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/query_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/query_photons.py
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/query_stac.py
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/query_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/region_of_interest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/results_to_s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/stac.py
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/stream_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/tail_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-04-27 14:09:41.000000 sliderule-3.1.0/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-27 14:09:41.000000 sliderule-3.1.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:42:08.882824 sliderule-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-05-08 12:41:56.000000 sliderule-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-08 12:41:56.000000 sliderule-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-05-08 12:42:08.882824 sliderule-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-05-08 12:41:56.000000 sliderule-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-05-08 12:41:56.000000 sliderule-3.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-08 12:42:08.882824 sliderule-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-05-08 12:41:56.000000 sliderule-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:42:08.878824 sliderule-3.2.0/sliderule/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/arcticdem.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24752 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/earthdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18906 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/gedi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9833 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/h5.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36209 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/icesat2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38844 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/ipxapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    85029 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/ipysliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44386 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/sliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:42:08.878824 sliderule-3.2.0/sliderule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-05-08 12:42:08.000000 sliderule-3.2.0/sliderule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      950 2023-05-08 12:42:08.000000 sliderule-3.2.0/sliderule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 12:42:08.000000 sliderule-3.2.0/sliderule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-08 12:42:08.000000 sliderule-3.2.0/sliderule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-08 12:42:08.000000 sliderule-3.2.0/sliderule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:42:08.882824 sliderule-3.2.0/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/big_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/build_arctic_dem_mosaics_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/build_arctic_dem_mosaics_vrt_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/build_arctic_dem_strips_vrt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/extract_h5_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/icepyx_region.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/lpdaac_download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/query_cmr.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/query_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/query_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/query_photons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/query_stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/query_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/region_of_interest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/results_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/stream_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/tail_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-08 12:41:56.000000 sliderule-3.2.0/version.txt
```

### Comparing `sliderule-3.1.0/LICENSE` & `sliderule-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/PKG-INFO` & `sliderule-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.1.0
+Version: 3.2.0
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule-python/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.1.0/README.md` & `sliderule-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/setup.py` & `sliderule-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/sliderule/arcticdem.py` & `sliderule-3.2.0/sliderule/arcticdem.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/sliderule/earthdata.py` & `sliderule-3.2.0/sliderule/earthdata.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/sliderule/gedi.py` & `sliderule-3.2.0/sliderule/gedi.py`

 * *Files 12% similar despite different names*

```diff
@@ -119,20 +119,51 @@
         profiles["flatten"] = time.perf_counter() - tstart_flatten
         return gdf
 
     # Flatten Records
     columns = {}
     records = []
     num_records = 0
+    field_dictionary = {} # [<field_name>] = {"shot_number": [], <field_name>: []}
+    file_dictionary = {} # [id] = "filename"
     if len(rsps) > 0:
         # Sort Records
         for rsp in rsps:
             if rectype in rsp['__rectype']:
                 records += rsp,
                 num_records += len(rsp[batch_column])
+            elif 'rsrec' == rsp['__rectype'] or 'zsrec' == rsp['__rectype']:
+                if rsp["num_samples"] <= 0:
+                    continue
+                # Get field names and set
+                sample = rsp["samples"][0]
+                field_names = list(sample.keys())
+                field_names.remove("__rectype")
+                field_set = rsp['key']
+                as_numpy_array = False
+                if rsp["num_samples"] > 1:
+                    as_numpy_array = True
+                # On first time, build empty dictionary for field set associated with raster
+                if field_set not in field_dictionary:
+                    field_dictionary[field_set] = {'shot_number': []}
+                    for field in field_names:
+                        field_dictionary[field_set][field_set + "." + field] = []
+                # Populate dictionary for field set
+                field_dictionary[field_set]['shot_number'] += numpy.uint64(rsp['index']),
+                for field in field_names:
+                    if as_numpy_array:
+                        data = []
+                        for s in rsp["samples"]:
+                            data += s[field],
+                        field_dictionary[field_set][field_set + "." + field] += numpy.array(data),
+                    else:
+                        field_dictionary[field_set][field_set + "." + field] += sample[field],
+            elif 'fileidrec' == rsp['__rectype']:
+                file_dictionary[rsp["file_id"]] = rsp["file_name"]
+
         # Build Columns
         if num_records > 0:
             # Initialize Columns
             sample_record = records[0][batch_column][0]
             for field in sample_record.keys():
                 fielddef = sliderule.get_definition(sample_record['__rectype'], field)
                 if len(fielddef) > 0:
@@ -149,18 +180,29 @@
                     cnt += 1
     else:
         logger.debug("No response returned")
 
     # Build Initial GeoDataFrame
     gdf = __todataframe(columns)
 
-    # Delete Extent ID Column
+    # Merge Ancillary Fields
+    tstart_merge = time.perf_counter()
+    for field_set in field_dictionary:
+        df = geopandas.pd.DataFrame(field_dictionary[field_set])
+        gdf = geopandas.pd.merge(gdf, df, how='left', on='shot_number').set_axis(gdf.index)
+    profiles["merge"] = time.perf_counter() - tstart_merge
+
+    # Delete Shot Number Column
     if len(gdf) > 0 and not keep_id:
         del gdf["shot_number"]
 
+    # Attach Metadata
+    if len(file_dictionary) > 0:
+        gdf.attrs['file_directory'] = file_dictionary
+
     # Return GeoDataFrame
     profiles["flatten"] = time.perf_counter() - tstart_flatten
     return gdf
 
 #
 #  Query Resources from CMR
 #
```

### Comparing `sliderule-3.1.0/sliderule/h5.py` & `sliderule-3.2.0/sliderule/h5.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/sliderule/icesat2.py` & `sliderule-3.2.0/sliderule/icesat2.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,19 +314,14 @@
 
     # Latch Start Time
     tstart = time.perf_counter()
 
     # Submission Arguments for CMR
     kwargs.setdefault('return_metadata', False)
 
-    # Check Parameters are Valid
-    if ("poly" not in parm) and ("t0" not in parm) and ("t1" not in parm):
-        logger.error("Must supply some bounding parameters with request (poly, t0, t1)")
-        return []
-
     # Pull Out Polygon
     if "clusters" in parm and parm["clusters"] and len(parm["clusters"]) > 0:
         kwargs['polygon'] = parm["clusters"]
     elif "poly" in parm and parm["poly"] and len(parm["poly"]) > 0:
         kwargs['polygon'] = parm["poly"]
 
     # Pull Out Time Period
@@ -334,28 +329,33 @@
         kwargs['time_start'] = parm["t0"]
     if "t1" in parm:
         kwargs['time_end'] = parm["t1"]
 
     # Build Filters
     name_filter_enabled = False
     rgt_filter = '????'
-    if "rgt" in parm:
+    if "rgt" in parm and parm["rgt"] != None:
         rgt_filter = f'{parm["rgt"]}'.zfill(4)
         name_filter_enabled = True
     cycle_filter = '??'
-    if "cycle" in parm:
+    if "cycle" in parm and parm["cycle"] != None:
         cycle_filter = f'{parm["cycle"]}'.zfill(2)
         name_filter_enabled = True
     region_filter = '??'
-    if "region" in parm:
+    if "region" in parm and parm["region"] != None:
         region_filter = f'{parm["region"]}'.zfill(2)
         name_filter_enabled = True
     if name_filter_enabled:
         kwargs['name_filter'] = '*_' + rgt_filter + cycle_filter + region_filter + '_*'
 
+    # Check Parameters are Valid
+    if (not name_filter_enabled) and ("poly" not in parm) and ("t0" not in parm) and ("t1" not in parm):
+        logger.error("Must supply some bounding parameters with request (poly, t0, t1)")
+        return []
+
     # Make CMR Request
     if kwargs['return_metadata']:
         resources,metadata = earthdata.cmr(short_name='ATL03', version=version, **kwargs)
     else:
         resources = earthdata.cmr(short_name='ATL03', version=version, **kwargs)
 
     # Check Resources are Under Limit
```

### Comparing `sliderule-3.1.0/sliderule/io.py` & `sliderule-3.2.0/sliderule/io.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/sliderule/ipxapi.py` & `sliderule-3.2.0/sliderule/ipxapi.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/sliderule/ipysliderule.py` & `sliderule-3.2.0/sliderule/ipysliderule.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/sliderule/sliderule.py` & `sliderule-3.2.0/sliderule/sliderule.py`

 * *Files 1% similar despite different names*

```diff
@@ -802,28 +802,31 @@
 
     Examples
     --------
         >>> import sliderule
         >>> num_servers, max_workers = sliderule.update_available_servers(10)
     '''
     global service_url, service_org, request_timeout
+    requested_nodes = 0
 
     # Update number of nodes
     if type(desired_nodes) == int:
         rsps_body = {}
         requested_nodes = desired_nodes
         headers = __build_auth_header()
 
         # Get boundaries of cluster and calculate nodes to request
         try:
             host = "https://ps." + service_url + "/api/org_num_nodes/" + service_org + "/"
             rsps = session.get(host, headers=headers, timeout=request_timeout)
             rsps_body = rsps.json()
             rsps.raise_for_status()
             requested_nodes = max(min(desired_nodes, rsps_body["max_nodes"]), rsps_body["min_nodes"])
+            if requested_nodes != desired_nodes:
+                logger.info("Provisioning system desired nodes truncated to {}".format(requested_nodes))
         except requests.exceptions.HTTPError as e:
             logger.info('{}'.format(e))
             logger.info('Provisioning system status request returned error => {}'.format(rsps_body["error_msg"]))
 
         # Request number of nodes in cluster
         try:
             if type(time_to_live) == int:
@@ -840,15 +843,16 @@
     
     # Get number of nodes currently registered
     try:
         rsps = source("status", parm={"service":"sliderule"}, path="/discovery", silence=True)
         available_servers = rsps["nodes"]
     except FatalError:
         available_servers = 0
-    return available_servers, available_servers
+    
+    return available_servers, requested_nodes
 
 #
 # scaleout
 #
 def scaleout(desired_nodes, time_to_live, bypass_dns):
     '''
     Scale the cluster and wait for cluster to reach desired state
@@ -872,20 +876,19 @@
     if desired_nodes < 0:
         raise FatalError("Number of desired nodes must be greater than zero ({})".format(desired_nodes))
     # Initialize DNS
     __initdns() # clear cache of DNS lookups for clusters
     if bypass_dns:
         __jamdns() # use ip address for cluster
     # Send Initial Request for Desired Cluster State
-    update_available_servers(desired_nodes=desired_nodes, time_to_live=time_to_live)
     start = time.time()
-    available_nodes,_ = update_available_servers()
+    available_nodes,requested_nodes = update_available_servers(desired_nodes=desired_nodes, time_to_live=time_to_live)
     scale_up_needed = False
     # Wait for Cluster to Reach Desired State
-    while available_nodes < desired_nodes:
+    while available_nodes < requested_nodes:
         scale_up_needed = True
         logger.info("Waiting while cluster scales to desired capacity (currently at {} nodes, desired is {} nodes)... {} seconds".format(available_nodes, desired_nodes, int(time.time() - start)))
         time.sleep(10.0)
         available_nodes,_ = update_available_servers()
         # Override DNS if Cluster is Starting
         if available_nodes == 0 and not __dnsoverridden():
             __jamdns()
```

### Comparing `sliderule-3.1.0/sliderule.egg-info/PKG-INFO` & `sliderule-3.2.0/sliderule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.1.0
+Version: 3.2.0
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule-python/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.1.0/sliderule.egg-info/SOURCES.txt` & `sliderule-3.2.0/sliderule.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -16,23 +16,20 @@
 sliderule/sliderule.py
 sliderule/version.py
 sliderule.egg-info/PKG-INFO
 sliderule.egg-info/SOURCES.txt
 sliderule.egg-info/dependency_links.txt
 sliderule.egg-info/requires.txt
 sliderule.egg-info/top_level.txt
-utils/_landsat.py
 utils/big_query.py
 utils/build_arctic_dem_mosaics_index.py
 utils/build_arctic_dem_mosaics_vrt_list.py
 utils/build_arctic_dem_strips_vrt.py
 utils/extract_h5_dataset.py
-utils/hls.py
 utils/icepyx_region.py
-utils/landsat.py
 utils/lpdaac_download.py
 utils/monitor.py
 utils/query_cmr.py
 utils/query_elevations.py
 utils/query_metrics.py
 utils/query_photons.py
 utils/query_stac.py
```

### Comparing `sliderule-3.1.0/utils/big_query.py` & `sliderule-3.2.0/utils/big_query.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/utils/build_arctic_dem_mosaics_index.py` & `sliderule-3.2.0/utils/build_arctic_dem_mosaics_index.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/utils/build_arctic_dem_mosaics_vrt_list.py` & `sliderule-3.2.0/utils/build_arctic_dem_mosaics_vrt_list.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/utils/build_arctic_dem_strips_vrt.py` & `sliderule-3.2.0/utils/build_arctic_dem_strips_vrt.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/utils/extract_h5_dataset.py` & `sliderule-3.2.0/utils/extract_h5_dataset.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/utils/icepyx_region.py` & `sliderule-3.2.0/utils/icepyx_region.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/utils/lpdaac_download.py` & `sliderule-3.2.0/utils/lpdaac_download.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/utils/monitor.py` & `sliderule-3.2.0/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/utils/query_cmr.py` & `sliderule-3.2.0/utils/query_cmr.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/utils/query_elevations.py` & `sliderule-3.2.0/utils/query_elevations.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/utils/query_metrics.py` & `sliderule-3.2.0/utils/query_metrics.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/utils/query_photons.py` & `sliderule-3.2.0/utils/query_photons.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/utils/query_stac.py` & `sliderule-3.2.0/utils/query_stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/utils/query_version.py` & `sliderule-3.2.0/utils/query_version.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/utils/region_of_interest.py` & `sliderule-3.2.0/utils/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/utils/results_to_s3.py` & `sliderule-3.2.0/utils/results_to_s3.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/utils/stac.py` & `sliderule-3.2.0/utils/stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/utils/stream_events.py` & `sliderule-3.2.0/utils/stream_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/utils/tail_events.py` & `sliderule-3.2.0/utils/tail_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.1.0/utils/utils.py` & `sliderule-3.2.0/utils/utils.py`

 * *Files identical despite different names*

