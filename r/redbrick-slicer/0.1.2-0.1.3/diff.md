# Comparing `tmp/redbrick-slicer-0.1.2.tar.gz` & `tmp/redbrick-slicer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbrick-slicer-0.1.2.tar", last modified: Thu May  4 10:16:11 2023, max compression
+gzip compressed data, was "redbrick-slicer-0.1.3.tar", last modified: Mon May  8 06:48:38 2023, max compression
```

## Comparing `redbrick-slicer-0.1.2.tar` & `redbrick-slicer-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:16:11.731998 redbrick-slicer-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-04 10:16:11.731998 redbrick-slicer-0.1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:16:11.727998 redbrick-slicer-0.1.2/redbrick_slicer/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:16:11.731998 redbrick-slicer-0.1.2/redbrick_slicer/common/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/common/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/common/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/common/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/common/labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/common/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:16:11.731998 redbrick-slicer-0.1.2/redbrick_slicer/export/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/export/public.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:16:11.731998 redbrick-slicer-0.1.2/redbrick_slicer/labeling/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/labeling/public.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:16:11.731998 redbrick-slicer-0.1.2/redbrick_slicer/repo/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/repo/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/repo/labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/repo/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/slicer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:16:11.731998 redbrick-slicer-0.1.2/redbrick_slicer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/utils/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/utils/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:16:11.731998 redbrick-slicer-0.1.2/redbrick_slicer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-04 10:16:11.000000 redbrick-slicer-0.1.2/redbrick_slicer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-04 10:16:11.000000 redbrick-slicer-0.1.2/redbrick_slicer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:16:11.000000 redbrick-slicer-0.1.2/redbrick_slicer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-04 10:16:11.000000 redbrick-slicer-0.1.2/redbrick_slicer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 10:16:11.000000 redbrick-slicer-0.1.2/redbrick_slicer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-04 10:16:11.731998 redbrick-slicer-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:48:38.389729 redbrick-slicer-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-08 06:48:38.393729 redbrick-slicer-0.1.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:48:38.381729 redbrick-slicer-0.1.3/redbrick_slicer/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:48:38.385729 redbrick-slicer-0.1.3/redbrick_slicer/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/common/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/common/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/common/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/common/labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/common/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:48:38.389729 redbrick-slicer-0.1.3/redbrick_slicer/export/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/export/public.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:48:38.389729 redbrick-slicer-0.1.3/redbrick_slicer/labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/labeling/public.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:48:38.389729 redbrick-slicer-0.1.3/redbrick_slicer/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/repo/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/repo/labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/repo/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16912 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/slicer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:48:38.389729 redbrick-slicer-0.1.3/redbrick_slicer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/utils/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/redbrick_slicer/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:48:38.385729 redbrick-slicer-0.1.3/redbrick_slicer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-08 06:48:38.000000 redbrick-slicer-0.1.3/redbrick_slicer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-08 06:48:38.000000 redbrick-slicer-0.1.3/redbrick_slicer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 06:48:38.000000 redbrick-slicer-0.1.3/redbrick_slicer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-08 06:48:38.000000 redbrick-slicer-0.1.3/redbrick_slicer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 06:48:38.000000 redbrick-slicer-0.1.3/redbrick_slicer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-08 06:48:38.393729 redbrick-slicer-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-08 06:48:24.000000 redbrick-slicer-0.1.3/setup.py
```

### Comparing `redbrick-slicer-0.1.2/redbrick_slicer/__init__.py` & `redbrick-slicer-0.1.3/redbrick_slicer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """RedBrick Slicer Integration Package."""
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 
 def get_task(
     url: str, token: str, endpoint: str = "https://api.redbrickai.com"
 ) -> None:
     """Interact with a RedBrick task in 3D Slicer application.
```

### Comparing `redbrick-slicer-0.1.2/redbrick_slicer/common/client.py` & `redbrick-slicer-0.1.3/redbrick_slicer/common/client.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.2/redbrick_slicer/common/context.py` & `redbrick-slicer-0.1.3/redbrick_slicer/common/context.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.2/redbrick_slicer/common/export.py` & `redbrick-slicer-0.1.3/redbrick_slicer/common/export.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.2/redbrick_slicer/common/labeling.py` & `redbrick-slicer-0.1.3/redbrick_slicer/common/labeling.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.2/redbrick_slicer/export/public.py` & `redbrick-slicer-0.1.3/redbrick_slicer/export/public.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.2/redbrick_slicer/labeling/public.py` & `redbrick-slicer-0.1.3/redbrick_slicer/labeling/public.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.2/redbrick_slicer/project.py` & `redbrick-slicer-0.1.3/redbrick_slicer/project.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.2/redbrick_slicer/repo/export.py` & `redbrick-slicer-0.1.3/redbrick_slicer/repo/export.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.2/redbrick_slicer/repo/labeling.py` & `redbrick-slicer-0.1.3/redbrick_slicer/repo/labeling.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.2/redbrick_slicer/repo/project.py` & `redbrick-slicer-0.1.3/redbrick_slicer/repo/project.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.2/redbrick_slicer/slicer.py` & `redbrick-slicer-0.1.3/redbrick_slicer/slicer.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,20 +117,24 @@
                 for child in parent_cat[0]["children"]:
                     self.segments += RBSlicer._get_categories(child)
 
         if not self.segments:
             print("Unsupported taxonomy")
             return
 
+        taxName = re.sub(r"[^a-zA-Z]", "", taxonomy["name"])
+        is_tax_v2 = bool(taxonomy.get("isNew"))
+
+        print("Taxonomy:", taxName)
         print("Available categories:", self.segments)
+        print("Task ID:", self.task_id)
+        print("Please use corresponding segmentation and source volumes")
 
         slicer.mrmlScene.Clear(0)
 
-        taxName = re.sub(r"[^a-zA-Z]", "", taxonomy["name"])
-
         term_json_file = os.path.join(self.project_dir, "terminologies.json")
         term_json = {
             "SegmentationCategoryTypeContextName": taxName,
             "@schema": "https://raw.githubusercontent.com/qiicr/dcmqi/master/doc/segment-context-schema.json#",
             "SegmentationCodes": {
                 "Category": [
                     {
@@ -147,15 +151,15 @@
                                     for obj_type in taxonomy["objectTypes"]
                                     if obj_type["labelType"] == "SEGMENTATION"
                                     and not obj_type.get("archived")
                                     and obj_type["category"] == cat
                                 ][0],
                                 idx + 1,
                             )
-                            if taxonomy.get("isNew")
+                            if is_tax_v2
                             else self._cat2cat(cat, idx + 1, taxonomy["colorMap"])
                             for idx, cat in enumerate(self.segments)
                         ],
                     }
                 ],
             },
         }
@@ -172,15 +176,18 @@
             "Segmentations/DefaultTerminologyEntry", defaultCat
         )
 
         loop = asyncio.get_event_loop()
         if len(task["items"]) == 1 and ".nii" in task["items"][0]:
             path = os.path.join(
                 self.data_dir,
-                "volume.nii" + (".gz" if ".nii.gz" in task["items"][0] else ""),
+                "vol_"
+                + str(self.task_id)
+                + ".nii"
+                + (".gz" if ".nii.gz" in task["items"][0] else ""),
             )
             if not os.path.isfile(path):
                 loop.run_until_complete(
                     download_files([(task["itemsPresigned"][0], path)])
                 )
             slicer.util.loadVolume(path)
         else:
@@ -195,15 +202,17 @@
             with DICOMUtils.TemporaryDICOMDatabase() as db:
                 DICOMUtils.importDicom(self.data_dir, db)
                 patientUIDs = db.patients()
                 assert len(patientUIDs) == 1, "Failed to load data"
                 DICOMUtils.loadPatientByUID(patientUIDs[0])
 
         if task["labelsPath"]:
-            labels_path = os.path.join(self.task_dir, "labels.nii")
+            labels_path = os.path.join(
+                self.task_dir, "seg_" + str(self.task_id) + ".nii"
+            )
             if os.path.isfile(labels_path):
                 os.remove(labels_path)
             loop.run_until_complete(download_files([(task["labelsPath"], labels_path)]))
 
             slicer.util.loadSegmentation(labels_path)
             segmentationNode = slicer.mrmlScene.GetFirstNodeByClass(
                 "vtkMRMLSegmentationNode"
@@ -237,16 +246,16 @@
         }
 
         label_rb_map = {}
         for label in labels:
             label["dicom"]["slicer:segmentid"] = all_segments_map[
                 label["dicom"]["instanceid"]
             ]
-            label_rb_map[label["dicom"]["instanceid"]] = "::".join(
-                label["category"][0][1:]
+            label_rb_map[label["dicom"]["instanceid"]] = (
+                label["category"] if is_tax_v2 else "::".join(label["category"][0][1:])
             )
         for label in labels:
             if label["dicom"].get("groupids"):
                 for groupid in label["dicom"]["groupids"]:
                     label_rb_map[groupid] = label_rb_map.get(groupid, "")
                     label_rb_map[groupid] += (
                         ("+" if label_rb_map[groupid] else "")
@@ -347,15 +356,15 @@
 
         segmentationNode = scene.GetFirstNodeByClass("vtkMRMLSegmentationNode")
         rb_segmentation = segmentationNode.GetSegmentation()
         labels = {}
         for num in range(rb_segmentation.GetNumberOfSegments()):
             seg = rb_segmentation.GetNthSegment(num)
             name = seg.GetName()
-            if name not in self.segments:
+            if name not in self.segments and "+" not in name:
                 print(f"Category: `{name}` not found. Skipping")
                 continue
             val = num + 1  # seg.GetLabelValue()
             labels[name + "#" + str(val)] = {
                 "category": [["object"] + name.split("::")],
                 "attributes": [],
                 "labelid": str(uuid4()),
```

### Comparing `redbrick-slicer-0.1.2/redbrick_slicer/utils/async_utils.py` & `redbrick-slicer-0.1.3/redbrick_slicer/utils/async_utils.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.2/redbrick_slicer/utils/files.py` & `redbrick-slicer-0.1.3/redbrick_slicer/utils/files.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.2/redbrick_slicer/utils/url.py` & `redbrick-slicer-0.1.3/redbrick_slicer/utils/url.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.2/redbrick_slicer.egg-info/SOURCES.txt` & `redbrick-slicer-0.1.3/redbrick_slicer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.2/setup.cfg` & `redbrick-slicer-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.2/setup.py` & `redbrick-slicer-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 setup(
     name="redbrick-slicer",
     version=version,
     url="https://github.com/redbrick-ai/redbrick-slicer",
     description="RedBrick platform 3D Slicer Integration!",
     py_modules=["redbrick_slicer"],
-    python_requires=">=3.6, <3.10",
+    python_requires=">=3.6",
     packages=find_packages(),
     long_description_content_type="text/markdown",
     include_package_data=True,
     install_requires=install_requires,
     extras_require={
         "dev": [
             "twine==3.1.1",
```

