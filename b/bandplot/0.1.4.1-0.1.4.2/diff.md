# Comparing `tmp/bandplot-0.1.4.1-py3-none-any.whl.zip` & `tmp/bandplot-0.1.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9590 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       26 b- defN 23-May-04 03:00 bandplot/__init__.py
--rw-rw-r--  2.0 unx    28110 b- defN 23-May-04 03:00 bandplot/plots.py
--rw-rw-r--  2.0 unx     6111 b- defN 23-May-04 03:00 bandplot/readdata.py
--rw-rw-r--  2.0 unx    15554 b- defN 23-May-04 03:00 bandplot/wrapper.py
--rw-rw-r--  2.0 unx     2901 b- defN 23-May-04 03:00 bandplot-0.1.4.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-04 03:00 bandplot-0.1.4.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       86 b- defN 23-May-04 03:00 bandplot-0.1.4.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-May-04 03:00 bandplot-0.1.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      711 b- defN 23-May-04 03:00 bandplot-0.1.4.1.dist-info/RECORD
-9 files, 53600 bytes uncompressed, 8366 bytes compressed:  84.4%
+Zip file size: 9614 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       26 b- defN 23-May-08 02:39 bandplot/__init__.py
+-rw-rw-r--  2.0 unx    28110 b- defN 23-May-08 02:39 bandplot/plots.py
+-rw-rw-r--  2.0 unx     6111 b- defN 23-May-08 02:39 bandplot/readdata.py
+-rw-rw-r--  2.0 unx    15638 b- defN 23-May-08 02:39 bandplot/wrapper.py
+-rw-rw-r--  2.0 unx     2901 b- defN 23-May-08 02:39 bandplot-0.1.4.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-08 02:39 bandplot-0.1.4.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       86 b- defN 23-May-08 02:39 bandplot-0.1.4.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-08 02:39 bandplot-0.1.4.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      711 b- defN 23-May-08 02:39 bandplot-0.1.4.2.dist-info/RECORD
+9 files, 53684 bytes uncompressed, 8390 bytes compressed:  84.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: bandplot/readdata.py
 Comment: 
 
 Filename: bandplot/wrapper.py
 Comment: 
 
-Filename: bandplot-0.1.4.1.dist-info/METADATA
+Filename: bandplot-0.1.4.2.dist-info/METADATA
 Comment: 
 
-Filename: bandplot-0.1.4.1.dist-info/WHEEL
+Filename: bandplot-0.1.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: bandplot-0.1.4.1.dist-info/entry_points.txt
+Filename: bandplot-0.1.4.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: bandplot-0.1.4.1.dist-info/top_level.txt
+Filename: bandplot-0.1.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: bandplot-0.1.4.1.dist-info/RECORD
+Filename: bandplot-0.1.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bandplot/__init__.py

```diff
@@ -1,3 +1,3 @@
 
-__version__ = "0.1.4.1"
+__version__ = "0.1.4.2"
```

## bandplot/wrapper.py

```diff
@@ -142,14 +142,16 @@
             elif ispin == "Ispin" and not args.divided:
                 plots.IspinWd(arr, bands, ticks, labels, darr, dele, args.fill, index_f, elements, width_ratios, legend, fig_p)
             elif ispin == "Ispin" and args.divided:
                 plots.DispinWd(arr, bands, ticks, labels, darr, dele, args.fill, index_f, elements, width_ratios, legend, fig_p)
 
     else:
         if dosfiles:
+            if fig_p.output == "BAND.png":
+                fig_p.output = "DOS.png"
             darr, dele, s_elements = readdata.dos(dosfiles)
             index_f, labels_elements = readdata.select(s_elements, args.partial)
             if not elements:
                 elements = labels_elements
 
             plots.pdosfiles(darr, dele, args.fill, index_f, elements, legend, args.exchange, fig_p)
         else:
```

## Comparing `bandplot-0.1.4.1.dist-info/METADATA` & `bandplot-0.1.4.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandplot
-Version: 0.1.4.1
+Version: 0.1.4.2
 Summary: Band structure, DOS or phonon band structure plot from vaspkit or phonopy result.
 Home-page: https://github.com/lkccrr/bandplot
 Author: kan
 Author-email: luokan@hrbeu.edu.cn
 License: MIT
 Keywords: DFT VASP DOS band plot Phonon
 Platform: Unix
```

