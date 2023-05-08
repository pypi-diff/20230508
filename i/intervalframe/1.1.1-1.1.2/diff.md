# Comparing `tmp/intervalframe-1.1.1.tar.gz` & `tmp/intervalframe-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intervalframe-1.1.1.tar", max compression
+gzip compressed data, was "intervalframe-1.1.2.tar", max compression
```

## Comparing `intervalframe-1.1.1.tar` & `intervalframe-1.1.2.tar`

### file list

```diff
@@ -1,43 +1,24 @@
--rwxr-xr-x   0        0        0    17895 2019-08-12 18:05:36.000000 intervalframe-1.1.1/LICENSE.md
--rwxr-xr-x   0        0        0     1017 2022-01-03 18:58:56.000000 intervalframe-1.1.1/README.md
--rw-r--r--   0        0        0     6148 2023-05-06 21:49:29.742968 intervalframe-1.1.1/intervalframe/.DS_Store
--rw-r--r--   0        0        0      444 2023-05-07 12:06:17.723328 intervalframe-1.1.1/intervalframe/__init__.py
--rw-r--r--   0        0        0     6148 2023-02-02 16:32:30.612368 intervalframe-1.1.1/intervalframe/core/.DS_Store
--rw-r--r--   0        0        0    35644 2023-04-20 03:11:01.689833 intervalframe-1.1.1/intervalframe/core/IntervalFrame.py
--rw-r--r--   0        0        0    17962 2023-05-06 21:51:36.202476 intervalframe-1.1.1/intervalframe/core/IntervalSeries.py
--rw-r--r--   0        0        0    13847 2021-02-11 01:00:19.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/IntervalFrame.cpython-36.pyc
--rw-r--r--   0        0        0     2412 2020-06-20 18:07:35.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/IntervalFrame.cpython-37.pyc
--rw-r--r--   0        0        0    14936 2020-08-07 02:06:35.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/IntervalFrame.cpython-38.pyc
--rw-r--r--   0        0        0    17497 2022-01-10 22:35:33.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/IntervalFrame.cpython-39.pyc
--rw-r--r--   0        0        0    16411 2020-08-12 17:39:28.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/IntervalFrame2.cpython-36.pyc
--rw-r--r--   0        0        0    15354 2020-08-07 16:54:53.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/IntervalFrame2.cpython-38.pyc
--rw-r--r--   0        0        0    14341 2021-09-21 15:04:53.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/IntervalSeries.cpython-39.pyc
--rw-r--r--   0        0        0     1668 2020-06-30 16:23:11.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/groupby.cpython-36.pyc
--rw-r--r--   0        0        0     1705 2020-07-23 15:49:38.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/groupby.cpython-38.pyc
--rw-r--r--   0        0        0    13606 2020-08-05 01:16:10.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/indexing.cpython-36.pyc
--rw-r--r--   0        0        0    13148 2020-08-03 18:50:48.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/indexing.cpython-38.pyc
--rw-r--r--   0        0        0     6239 2020-08-12 17:39:28.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/indexing2.cpython-36.pyc
--rw-r--r--   0        0        0     6207 2020-08-07 14:44:23.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/indexing2.cpython-38.pyc
--rw-r--r--   0        0        0    20091 2020-08-05 01:16:10.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/multi_indexing.cpython-36.pyc
--rw-r--r--   0        0        0    19570 2020-08-07 02:07:14.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/multi_indexing.cpython-38.pyc
--rw-r--r--   0        0        0    11416 2020-08-12 18:16:35.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/multi_indexing2.cpython-36.pyc
--rw-r--r--   0        0        0     9820 2020-08-07 16:58:33.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/multi_indexing2.cpython-38.pyc
--rw-r--r--   0        0        0      611 2020-07-04 18:32:05.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/utilities.cpython-36.pyc
--rw-r--r--   0        0        0      636 2020-07-23 15:49:38.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/utilities.cpython-38.pyc
--rw-r--r--   0        0        0     1244 2020-06-30 16:23:05.000000 intervalframe-1.1.1/intervalframe/core/groupby.py
--rw-r--r--   0        0        0     4299 2022-01-10 22:35:34.000000 intervalframe-1.1.1/intervalframe/core/index/__pycache__/indexers.cpython-39.pyc
--rw-r--r--   0        0        0     6980 2023-02-02 17:51:34.367876 intervalframe-1.1.1/intervalframe/core/index/indexers.py
--rw-r--r--   0        0        0     2473 2021-09-21 15:04:53.000000 intervalframe-1.1.1/intervalframe/read/__pycache__/read_h5.cpython-39.pyc
--rw-r--r--   0        0        0     1191 2022-01-10 22:35:34.000000 intervalframe-1.1.1/intervalframe/read/__pycache__/read_text.cpython-39.pyc
--rw-r--r--   0        0        0    20974 2021-02-11 01:01:08.000000 intervalframe-1.1.1/intervalframe/read/h5_utilities.py
--rw-r--r--   0        0        0     6848 2023-03-25 17:26:19.423023 intervalframe-1.1.1/intervalframe/read/read_h5.py
--rw-r--r--   0        0        0      815 2023-01-26 17:56:39.789523 intervalframe-1.1.1/intervalframe/read/read_parquet.py
--rw-r--r--   0        0        0     2453 2023-01-26 20:00:28.520286 intervalframe-1.1.1/intervalframe/read/read_text.py
--rw-r--r--   0        0        0    20967 2020-07-10 01:08:55.000000 intervalframe-1.1.1/intervalframe/utilities/h5_utilities.py
--rw-r--r--   0        0        0     2856 2021-09-21 15:04:53.000000 intervalframe-1.1.1/intervalframe/write/__pycache__/write_h5.cpython-39.pyc
--rw-r--r--   0        0        0    20967 2020-07-10 01:08:55.000000 intervalframe-1.1.1/intervalframe/write/h5_utilities.py
--rw-r--r--   0        0        0     7192 2023-03-25 13:52:13.113838 intervalframe-1.1.1/intervalframe/write/write_h5.py
--rw-r--r--   0        0        0      736 2023-01-30 21:43:29.435395 intervalframe-1.1.1/intervalframe/write/write_parquet.py
--rw-r--r--   0        0        0        0 2020-07-22 20:58:51.000000 intervalframe-1.1.1/intervalframe/write/write_text.py
--rw-r--r--   0        0        0     1992 2023-05-07 12:06:29.926871 intervalframe-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2787 1970-01-01 00:00:00.000000 intervalframe-1.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0    17895 2019-08-12 18:05:36.000000 intervalframe-1.1.2/LICENSE.md
+-rwxr-xr-x   0        0        0     1017 2022-01-03 18:58:56.000000 intervalframe-1.1.2/README.md
+-rw-r--r--   0        0        0     6148 2023-05-08 14:50:48.246993 intervalframe-1.1.2/intervalframe/.DS_Store
+-rw-r--r--   0        0        0      444 2023-05-08 14:58:49.487881 intervalframe-1.1.2/intervalframe/__init__.py
+-rw-r--r--   0        0        0     6148 2023-02-02 16:32:30.612368 intervalframe-1.1.2/intervalframe/core/.DS_Store
+-rw-r--r--   0        0        0    36691 2023-05-08 14:56:39.086479 intervalframe-1.1.2/intervalframe/core/IntervalFrame.py
+-rw-r--r--   0        0        0    18564 2023-05-08 14:58:21.201049 intervalframe-1.1.2/intervalframe/core/IntervalSeries.py
+-rw-r--r--   0        0        0     1244 2020-06-30 16:23:05.000000 intervalframe-1.1.2/intervalframe/core/groupby.py
+-rw-r--r--   0        0        0     4299 2022-01-10 22:35:34.000000 intervalframe-1.1.2/intervalframe/core/index/__pycache__/indexers.cpython-39.pyc
+-rw-r--r--   0        0        0     6980 2023-02-02 17:51:34.367876 intervalframe-1.1.2/intervalframe/core/index/indexers.py
+-rw-r--r--   0        0        0     2473 2021-09-21 15:04:53.000000 intervalframe-1.1.2/intervalframe/read/__pycache__/read_h5.cpython-39.pyc
+-rw-r--r--   0        0        0     1191 2022-01-10 22:35:34.000000 intervalframe-1.1.2/intervalframe/read/__pycache__/read_text.cpython-39.pyc
+-rw-r--r--   0        0        0    20974 2021-02-11 01:01:08.000000 intervalframe-1.1.2/intervalframe/read/h5_utilities.py
+-rw-r--r--   0        0        0     6848 2023-03-25 17:26:19.423023 intervalframe-1.1.2/intervalframe/read/read_h5.py
+-rw-r--r--   0        0        0      815 2023-01-26 17:56:39.789523 intervalframe-1.1.2/intervalframe/read/read_parquet.py
+-rw-r--r--   0        0        0     2453 2023-01-26 20:00:28.520286 intervalframe-1.1.2/intervalframe/read/read_text.py
+-rw-r--r--   0        0        0    20967 2020-07-10 01:08:55.000000 intervalframe-1.1.2/intervalframe/utilities/h5_utilities.py
+-rw-r--r--   0        0        0     2856 2021-09-21 15:04:53.000000 intervalframe-1.1.2/intervalframe/write/__pycache__/write_h5.cpython-39.pyc
+-rw-r--r--   0        0        0    20967 2020-07-10 01:08:55.000000 intervalframe-1.1.2/intervalframe/write/h5_utilities.py
+-rw-r--r--   0        0        0     7192 2023-03-25 13:52:13.113838 intervalframe-1.1.2/intervalframe/write/write_h5.py
+-rw-r--r--   0        0        0      736 2023-01-30 21:43:29.435395 intervalframe-1.1.2/intervalframe/write/write_parquet.py
+-rw-r--r--   0        0        0        0 2020-07-22 20:58:51.000000 intervalframe-1.1.2/intervalframe/write/write_text.py
+-rw-r--r--   0        0        0     2008 2023-05-08 14:58:59.689426 intervalframe-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2824 1970-01-01 00:00:00.000000 intervalframe-1.1.2/PKG-INFO
```

### Comparing `intervalframe-1.1.1/LICENSE.md` & `intervalframe-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.1/README.md` & `intervalframe-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.1/intervalframe/.DS_Store` & `intervalframe-1.1.2/intervalframe/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 00000420: 0000 00b8 6270 6c69 7374 3030 d601 0203  ....bplist00....
 00000430: 0405 0607 0807 080b 085d 5368 6f77 5374  .........]ShowSt
 00000440: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
 00000450: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 00000460: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
 00000470: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
 00000480: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00000490: 0908 095f 1018 7b7b 3434 332c 2033 3937  ..._..{{443, 397
+00000490: 0908 095f 1018 7b7b 3434 332c 2033 3938  ..._..{{443, 398
 000004a0: 7d2c 207b 3932 302c 2034 3336 7d7d 0908  }, {920, 436}}..
 000004b0: 1523 2f3b 525f 6b6c 6d6e 6f8a 0000 0000  .#/;R_klmno.....
 000004c0: 0000 0101 0000 0000 0000 000d 0000 0000  ................
 000004d0: 0000 0000 0000 0000 0000 008b 0000 0004  ................
 000004e0: 0063 006f 0072 0065 7653 726e 6c6f 6e67  .c.o.r.evSrnlong
 000004f0: 0000 0001 0000 0004 0072 0065 0061 0064  .........r.e.a.d
 00000500: 6277 7370 626c 6f62 0000 00b8 6270 6c69  bwspblob....bpli
@@ -96,16 +96,16 @@
 000005f0: 6f62 0000 00b8 6270 6c69 7374 3030 d601  ob....bplist00..
 00000600: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
 00000610: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
 00000620: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 00000630: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 00000640: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
 00000650: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00000660: 7208 0908 095f 1018 7b7b 3130 362c 2034  r...._..{{106, 4
-00000670: 3338 7d2c 207b 3932 302c 2034 3336 7d7d  38}, {920, 436}}
+00000660: 7208 0908 095f 1018 7b7b 3434 332c 2033  r...._..{{443, 3
+00000670: 3937 7d2c 207b 3932 302c 2034 3336 7d7d  97}, {920, 436}}
 00000680: 0908 1523 2f3b 525f 6b6c 6d6e 6f8a 0000  ...#/;R_klmno...
 00000690: 0000 0000 0101 0000 0000 0000 000d 0000  ................
 000006a0: 0000 0000 0000 0000 0000 0000 008b 0000  ................
 000006b0: 0005 0077 0072 0069 0074 0065 7653 726e  ...w.r.i.t.evSrn
 000006c0: 6c6f 6e67 0000 0001 0000 0000 0000 0000  long............
 000006d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `intervalframe-1.1.1/intervalframe/core/.DS_Store` & `intervalframe-1.1.2/intervalframe/core/.DS_Store`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.1/intervalframe/core/IntervalFrame.py` & `intervalframe-1.1.2/intervalframe/core/IntervalFrame.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,62 +154,83 @@
 
         return repr_string
 
     
     @property
     def shape(self):
         """
+        Dimensions of IntervalFrame
         """
         
         return self.df.shape
 
 
     @property
     def iloc(self):
         """
+        Position locator for IntervalFrame
         """
 
         # If index is None
         if self.index is None:
             return None
 
         return iLocator(self)
 
     
     @property
     def loc(self):
         """
+        Label locator for IntervalFrame
         """
 
         # If index is None
         if self.index is None:
             return None
 
         return Locator(self)
         
     
     @property
     def values(self):
         """
+        NumPy representation of IntervalFrame
         """
 
         return self.df.values
 
     
     @property
     def columns(self):
         """
+        Columns of IntervalFrame
         """
 
         return self.df.columns
 
     
     @staticmethod
-    def from_array(starts, ends, labels=None):
+    def from_array(starts: np.ndarray,
+                   ends: np.ndarray,
+                   labels: np.ndarray = None):
         """
+        Create IntervalFrame from array
+
+        Parameters
+        ----------
+            starts : np.ndarray
+                Starts of intervals
+            ends : np.ndarray
+                Ends of intervals
+            labels : np.ndarray
+                Labels for hierarchical indexing
+
+        Returns
+        -------
+            iframe : IntervalFrame
         """
 
         # Add intervals
         if labels is None:
             index = IntervalArray()
             index.add(starts, ends)
         else:
@@ -219,16 +240,29 @@
         # Create IntervalFrame
         iframe = IntervalFrame(index)
         
         return iframe
     
 
     @staticmethod
-    def from_dict_range(dict_range, bin_size=10000):
+    def from_dict_range(dict_range: Dict[str,int],
+                        bin_size: int = 10000):
         """
+        Construct IntervalFrame from dictionary of ranges
+
+        Parameters
+        ----------
+            dict_range : Dict[str,int]
+                Dictionary of ranges
+            bin_size : int
+                Size of bins
+
+        Returns
+        -------
+            iframe : IntervalFrame
         """
 
         # Add intervals
         index = LabeledIntervalArray.create_bin(dict_range, bin_size)
 
         # Create IntervalFrame
         iframe = IntervalFrame(index)
@@ -319,31 +353,35 @@
         from ..read.read_parquet import read_parquet
 
         # Read bed
         iframe = read_parquet(filename)
 
         return iframe
 
-                
+    
+    @property
     def starts(self):
         """
+        Starts of intervals
         """
 
         # If index is None
         if self.index is None:
             return None
         
         # Extract starts in intervals
         starts = self.index.starts
         
         return starts
         
     
+    @property
     def ends(self):
         """
+        Ends of intervals
         """
 
         # If index is None
         if self.index is None:
             return None
         
         # Extract ends in intervals
```

### Comparing `intervalframe-1.1.1/intervalframe/core/IntervalSeries.py` & `intervalframe-1.1.2/intervalframe/core/IntervalSeries.py`

 * *Files 8% similar despite different names*

```diff
@@ -117,46 +117,66 @@
 
         return repr_string
 
     
     @property
     def shape(self):
         """
+        Dimensions of IntervalFrame
         """
         
         return self.series.shape
 
 
     @property
     def iloc(self):
         """
+        Positional indexer
         """
 
         return indexers.iLocator(self)
 
     
     @property
     def loc(self):
         """
+        Label indexer
         """
 
         return indexers.Locator(self)
         
     
     @property
     def values(self):
         """
+        Numpy array of values
         """
         
         return self.series.values
 
     
     @staticmethod
-    def from_array(starts, ends, labels=None):
-        """
+    def from_array(starts: np.ndarray,
+                   ends: np.ndarray,
+                   labels: np.ndarray = None):
+        """
+        Create IntervalSeries from arrays
+
+        Parameters
+        ----------
+            starts : np.ndarray
+                Starts of intervals
+            ends : np.ndarray
+                Ends of intervals
+            labels : np.ndarray
+                Labels of intervals
+
+        Returns
+        -------
+            iseries : IntervalSeries
         """
 
         # Add intervals
         if labels is None:
             index = IntervalArray()
             index.from_array(starts, ends)
         else:
@@ -164,27 +184,29 @@
             index.from_array(starts, ends, labels)
             
         # Create IntervalSeries
         iseries = IntervalSeries(index)
         
         return iseries
                 
-                
+    @property
     def starts(self):
         """
+        Starts of intervals
         """
         
         # Extract starts in intervals
         starts = self.index.extract_starts()
         
         return starts
         
-    
+    @property
     def ends(self):
         """
+        Ends of intervals
         """
         
         # Extract ends in intervals
         ends = self.index.extract_ends()
         
         return ends
```

### Comparing `intervalframe-1.1.1/intervalframe/core/groupby.py` & `intervalframe-1.1.2/intervalframe/core/groupby.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.1/intervalframe/core/index/__pycache__/indexers.cpython-39.pyc` & `intervalframe-1.1.2/intervalframe/core/index/__pycache__/indexers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.1/intervalframe/core/index/indexers.py` & `intervalframe-1.1.2/intervalframe/core/index/indexers.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.1/intervalframe/read/__pycache__/read_h5.cpython-39.pyc` & `intervalframe-1.1.2/intervalframe/read/__pycache__/read_h5.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.1/intervalframe/read/__pycache__/read_text.cpython-39.pyc` & `intervalframe-1.1.2/intervalframe/read/__pycache__/read_text.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.1/intervalframe/read/h5_utilities.py` & `intervalframe-1.1.2/intervalframe/read/h5_utilities.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.1/intervalframe/read/read_h5.py` & `intervalframe-1.1.2/intervalframe/read/read_h5.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.1/intervalframe/read/read_parquet.py` & `intervalframe-1.1.2/intervalframe/read/read_parquet.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.1/intervalframe/read/read_text.py` & `intervalframe-1.1.2/intervalframe/read/read_text.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.1/intervalframe/utilities/h5_utilities.py` & `intervalframe-1.1.2/intervalframe/utilities/h5_utilities.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.1/intervalframe/write/__pycache__/write_h5.cpython-39.pyc` & `intervalframe-1.1.2/intervalframe/write/__pycache__/write_h5.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.1/intervalframe/write/h5_utilities.py` & `intervalframe-1.1.2/intervalframe/write/h5_utilities.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.1/intervalframe/write/write_h5.py` & `intervalframe-1.1.2/intervalframe/write/write_h5.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.1/intervalframe/write/write_parquet.py` & `intervalframe-1.1.2/intervalframe/write/write_parquet.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.1/pyproject.toml` & `intervalframe-1.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "intervalframe"
-version = "1.1.1"
+version = "1.1.2"
 description = "Python package for interval manipulation"
 authors = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 maintainers = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 repository = "https://github.com/kylessmith/intervalframe"
 documentation = "https://www.biosciencestack.com/static/intervalframe/docs/index.html"
 keywords = ["cython", "interval", "ailist", "frame"]
 readme = 'README.md'
@@ -30,14 +30,15 @@
 python = "^3.10"
 numpy = "^1.23.5"
 cython = "^0.29.32"
 pandas = "^1.5.2"
 ailist = "^2.1.0"
 tabulate = "^0.9.0"
 linear_segment = "^1.0.0"
+h5py = "^3.8.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0",
             "cython>=0.29.32",
```

### Comparing `intervalframe-1.1.1/PKG-INFO` & `intervalframe-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intervalframe
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python package for interval manipulation
 Home-page: https://github.com/kylessmith/intervalframe
 License: GPL-2.0-or-later
 Keywords: cython,interval,ailist,frame
 Author: Kyle S. Smith
 Author-email: kyle.smith@stjude.org
 Maintainer: Kyle S. Smith
@@ -26,14 +26,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: ailist (>=2.1.0,<3.0.0)
 Requires-Dist: cython (>=0.29.32,<0.30.0)
+Requires-Dist: h5py (>=3.8.0,<4.0.0)
 Requires-Dist: linear_segment (>=1.0.0,<2.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Documentation, https://www.biosciencestack.com/static/intervalframe/docs/index.html
 Project-URL: Repository, https://github.com/kylessmith/intervalframe
 Description-Content-Type: text/markdown
```

