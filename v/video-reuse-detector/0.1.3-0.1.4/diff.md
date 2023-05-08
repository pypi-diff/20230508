# Comparing `tmp/video_reuse_detector-0.1.3.tar.gz` & `tmp/video_reuse_detector-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video_reuse_detector-0.1.3.tar", max compression
+gzip compressed data, was "video_reuse_detector-0.1.4.tar", max compression
```

## Comparing `video_reuse_detector-0.1.3.tar` & `video_reuse_detector-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0      473 2023-03-16 11:59:24.538884 video_reuse_detector-0.1.3/README.md
--rw-r--r--   0        0        0      557 2023-04-26 13:27:56.653126 video_reuse_detector-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.3/vrd/__init__.py
--rw-r--r--   0        0        0     7108 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.3/vrd/annotation_matcher.py
--rw-r--r--   0        0        0     8582 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.3/vrd/dbhandler.py
--rw-r--r--   0        0        0    10226 2023-03-16 12:02:09.580704 video_reuse_detector-0.1.3/vrd/faiss_helper.py
--rw-r--r--   0        0        0     9168 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.3/vrd/frame_extractor.py
--rw-r--r--   0        0        0     4528 2023-03-16 11:59:49.747162 video_reuse_detector-0.1.3/vrd/image_preprocessing.py
--rw-r--r--   0        0        0     3939 2023-03-16 12:04:47.942450 video_reuse_detector-0.1.3/vrd/keras_layer_helper.py
--rw-r--r--   0        0        0    35384 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.3/vrd/neighbours.py
--rw-r--r--   0        0        0     1853 2023-03-16 12:02:09.504703 video_reuse_detector-0.1.3/vrd/neural_networks.py
--rw-r--r--   0        0        0    28571 2023-03-16 12:02:09.740706 video_reuse_detector-0.1.3/vrd/notebook_helper.py
--rw-r--r--   0        0        0    30541 2023-03-16 10:48:57.684639 video_reuse_detector-0.1.3/vrd/overlap_calculator.py
--rw-r--r--   0        0        0    21750 2023-04-26 13:10:06.029443 video_reuse_detector-0.1.3/vrd/sequence_finder.py
--rw-r--r--   0        0        0    13450 2023-03-16 12:02:09.604704 video_reuse_detector-0.1.3/vrd/vrd_project.py
--rw-r--r--   0        0        0        0 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.3/vrd/widgets/__init__.py
--rw-r--r--   0        0        0     5045 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.3/vrd/widgets/manual_image_preview.py
--rw-r--r--   0        0        0     4145 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.3/vrd/widgets/sequences_w_lowest_distance_by_duration.py
--rw-r--r--   0        0        0     4572 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.3/vrd/widgets/sequences_w_lowest_distances.py
--rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 video_reuse_detector-0.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0      473 2023-03-16 11:59:24.538884 video_reuse_detector-0.1.4/README.md
+-rw-r--r--   0        0        0      557 2023-05-08 09:42:06.385735 video_reuse_detector-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.4/vrd/__init__.py
+-rw-r--r--   0        0        0     7108 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.4/vrd/annotation_matcher.py
+-rw-r--r--   0        0        0     8582 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.4/vrd/dbhandler.py
+-rw-r--r--   0        0        0    10226 2023-03-16 12:02:09.580704 video_reuse_detector-0.1.4/vrd/faiss_helper.py
+-rw-r--r--   0        0        0     9168 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.4/vrd/frame_extractor.py
+-rw-r--r--   0        0        0     4528 2023-03-16 11:59:49.747162 video_reuse_detector-0.1.4/vrd/image_preprocessing.py
+-rw-r--r--   0        0        0     3939 2023-03-16 12:04:47.942450 video_reuse_detector-0.1.4/vrd/keras_layer_helper.py
+-rw-r--r--   0        0        0    35384 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.4/vrd/neighbours.py
+-rw-r--r--   0        0        0     1853 2023-03-16 12:02:09.504703 video_reuse_detector-0.1.4/vrd/neural_networks.py
+-rw-r--r--   0        0        0    28571 2023-03-16 12:02:09.740706 video_reuse_detector-0.1.4/vrd/notebook_helper.py
+-rw-r--r--   0        0        0    30541 2023-03-16 10:48:57.684639 video_reuse_detector-0.1.4/vrd/overlap_calculator.py
+-rw-r--r--   0        0        0    22766 2023-05-08 08:48:46.431032 video_reuse_detector-0.1.4/vrd/sequence_finder.py
+-rw-r--r--   0        0        0    13450 2023-03-16 12:02:09.604704 video_reuse_detector-0.1.4/vrd/vrd_project.py
+-rw-r--r--   0        0        0        0 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.4/vrd/widgets/__init__.py
+-rw-r--r--   0        0        0     5045 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.4/vrd/widgets/manual_image_preview.py
+-rw-r--r--   0        0        0     4145 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.4/vrd/widgets/sequences_w_lowest_distance_by_duration.py
+-rw-r--r--   0        0        0     4572 2023-03-10 13:15:34.586534 video_reuse_detector-0.1.4/vrd/widgets/sequences_w_lowest_distances.py
+-rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 video_reuse_detector-0.1.4/PKG-INFO
```

### Comparing `video_reuse_detector-0.1.3/pyproject.toml` & `video_reuse_detector-0.1.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "video-reuse-detector"
-version = "0.1.3"
+version = "0.1.4"
 description = "The video reuse detector"
 authors = ["TomasSkotare <tomas.skotare@umu.se>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "vrd"}]
 
 [tool.poetry.dependencies]
```

### Comparing `video_reuse_detector-0.1.3/vrd/annotation_matcher.py` & `video_reuse_detector-0.1.4/vrd/annotation_matcher.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.3/vrd/dbhandler.py` & `video_reuse_detector-0.1.4/vrd/dbhandler.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.3/vrd/faiss_helper.py` & `video_reuse_detector-0.1.4/vrd/faiss_helper.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.3/vrd/frame_extractor.py` & `video_reuse_detector-0.1.4/vrd/frame_extractor.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.3/vrd/image_preprocessing.py` & `video_reuse_detector-0.1.4/vrd/image_preprocessing.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.3/vrd/keras_layer_helper.py` & `video_reuse_detector-0.1.4/vrd/keras_layer_helper.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.3/vrd/neighbours.py` & `video_reuse_detector-0.1.4/vrd/neighbours.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.3/vrd/neural_networks.py` & `video_reuse_detector-0.1.4/vrd/neural_networks.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.3/vrd/notebook_helper.py` & `video_reuse_detector-0.1.4/vrd/notebook_helper.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.3/vrd/overlap_calculator.py` & `video_reuse_detector-0.1.4/vrd/overlap_calculator.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.3/vrd/sequence_finder.py` & `video_reuse_detector-0.1.4/vrd/sequence_finder.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,26 +32,32 @@
     """Finds sequences (frames matching second-per-second) from a given neighbours class."""
 
     sequence_lil_matrix: lil_matrix
     shortest_allowed_sequence: int
     max_distance: int
     neigh: neighbours.Neighbours
     pandas_background: str
+    image_max_width: int
+    add_frame_numbering: bool
 
     def __init__(
         self,
         neigh: neighbours.Neighbours,
         max_distance=30000,
         shortest_allowed_sequence=3,
         pandas_background=None,
+        image_max_width=None,
+        image_frame_text=False
     ) -> None:
         self.neigh = neigh
         self.max_distance = max_distance
         self.shortest_allowed_sequence = shortest_allowed_sequence
         self.pandas_background = pandas_background
+        self.image_max_width = image_max_width
+        self.add_frame_numbering = image_frame_text
 
         matrix = self._calculate_sequence_matrix(max_distance=max_distance)
         # Make upper triangular
         matrix = triu(matrix + matrix.T)
         self.sequence_lil_matrix_distance = matrix.tolil()
         self.sequence_lil_matrix = self.sequence_lil_matrix_distance.astype(np.bool8)
 
@@ -346,30 +352,40 @@
         sequences,
         show_limit: int = None,
         show_shift=False,
         frame_resize=(30, 30),
         sort_order: callable = None,
         convert_format=None,
         pandas_background=None,
+        image_max_width: int = None,
+        add_frame_numbering: bool = None
     ):
         """Displays longest-to-shortest sequences in a notebook
 
         Args:
             sequences (list): The sequence list of tuples (start1, start2, duration)
             show_limit (int, optional): The maximum number of sequences to show (Default: all)
             show_shift (bool, optional): Show statistics for "shifting", i.e. moving the matches one or 
                 several seconds forward or backwards.
             frame_resize (tuple, optional): Size of the thumbnails of each frame
             sort_order (callable): A handler that can sort or filter the sequence list.
             convert_format: The image format to return, for example "jpeg" to save space.
             pandas_background: Override background color of pandas to this value
+            image_max_width (int): If not none, wraps longer sequences into multiple rows according this threshold
+                of maximum width 
+            add_frame_numbering (bool): Whether to add text describing the frame # or not when wrapping
         """
         frames = self.neigh.frames
         if pandas_background is None:
             pandas_background = self.pandas_background
+        if image_max_width is None:
+            image_max_width = self.image_max_width
+        if add_frame_numbering is None:
+            add_frame_numbering = self.add_frame_numbering
+                
 
         if sort_order is None:
             # Default: Sort by duration
             sequences = sorted(sequences, key=lambda x: x[2], reverse=True)
         else:
             sequences = sort_order(sequences)
 
@@ -415,15 +431,15 @@
                     "props": f"background-color: {pandas_background};",
                 }
                 df = df.set_properties(**{"background-color": pandas_background})
                 df = df.set_table_styles([headers])
             display(df)
 
             img = self.show_sequence(
-                start1, start2, duration, frames, frame_resize=frame_resize
+                start1, start2, duration, frames, frame_resize=frame_resize, row_max_width=image_max_width, add_frame_numbering=add_frame_numbering
             )
             if convert_format:
                 img_bytes = BytesIO()
                 try:
                     img.save(img_bytes, format=convert_format)
                 except Exception as e: # This should be OSError only, but that didn't work
                     # Likely can't handle transparency, try again
@@ -510,36 +526,38 @@
         start2: int,
         duration: int,
         frames,
         frame_resize=(90, 70),
         row_max_width=700,
         row_spacing=10,
         background_opacity=0,
+        add_frame_numbering=False
     ):
         """Generates a comparison image for a given sequence
 
         Args:
             start1 (int): Start time 1 (as related to the Frame)
             start2 (int): _description_
             duration (int): _description_
             frames (FrameExtractor): _description_
             frame_resize (tuple, optional): Size of each resulting image in the sequence. Defaults to (200, 200).
             row_max_width: The maximum number of pixels allowed for one row. If this value is exceeded 
                 (i.e. width * # frames), the rows are broken up into several rows
             row_spacing: The number of pixels between each row (if any)
             background_opacity: The opacity of the unused pixels (if any)
+            add_frame_numbering: If true, adds a text in the row spacing describing which frames are shown
 
         Returns:
             A PIL image with the whole sequence
         """
 
         images = frames.all_images
         width, height = frame_resize
         max_width = width * duration
-        if max_width > row_max_width:
+        if row_max_width is not None and max_width > row_max_width:
             per_row = np.floor(row_max_width / width).astype(int)
             no_rows = np.ceil(duration / per_row).astype(int)
         else:
             per_row = duration
             no_rows = 1
         row_spacing_pixels = row_spacing * (no_rows - 1)
 
@@ -564,15 +582,15 @@
             merged.paste(
                 img2,
                 (
                     width * image_column,
                     current_row * row_spacing + current_row * 2 * height + height,
                 ),
             )
-            if i > 0 and image_column == 0:
+            if add_frame_numbering and i > 0 and image_column == 0:
                 y_loc = current_row * height * 2 + (current_row - 1) * row_spacing
                 draw.text(
                     (10, y_loc),
                     f"Frames {i+1}-{i + np.min([duration-i, per_row])}",
                     fill=(0, 0, 0),
                 )
         return merged
```

### Comparing `video_reuse_detector-0.1.3/vrd/vrd_project.py` & `video_reuse_detector-0.1.4/vrd/vrd_project.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.3/vrd/widgets/manual_image_preview.py` & `video_reuse_detector-0.1.4/vrd/widgets/manual_image_preview.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.3/vrd/widgets/sequences_w_lowest_distance_by_duration.py` & `video_reuse_detector-0.1.4/vrd/widgets/sequences_w_lowest_distance_by_duration.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.3/vrd/widgets/sequences_w_lowest_distances.py` & `video_reuse_detector-0.1.4/vrd/widgets/sequences_w_lowest_distances.py`

 * *Files identical despite different names*

### Comparing `video_reuse_detector-0.1.3/PKG-INFO` & `video_reuse_detector-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video-reuse-detector
-Version: 0.1.3
+Version: 0.1.4
 Summary: The video reuse detector
 License: MIT
 Author: TomasSkotare
 Author-email: tomas.skotare@umu.se
 Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

