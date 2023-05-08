# Comparing `tmp/kyeongmo230508AIL-0.0.2-py3-none-any.whl.zip` & `tmp/kyeongmo230508AIL-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1422 bytes, number of entries: 5
--rw-r--r--  2.0 unx      178 b- defN 23-May-08 15:56 myLib/myLib.py
--rw-r--r--  2.0 unx      296 b- defN 23-May-08 16:01 kyeongmo230508AIL-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-08 16:01 kyeongmo230508AIL-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-May-08 16:01 kyeongmo230508AIL-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      406 b- defN 23-May-08 16:01 kyeongmo230508AIL-0.0.2.dist-info/RECORD
-5 files, 978 bytes uncompressed, 656 bytes compressed:  32.9%
+Zip file size: 1427 bytes, number of entries: 5
+-rw-r--r--  2.0 unx      184 b- defN 23-May-08 16:08 myLib/myLib.py
+-rw-r--r--  2.0 unx      296 b- defN 23-May-08 16:09 kyeongmo230508AIL-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-08 16:09 kyeongmo230508AIL-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-08 16:09 kyeongmo230508AIL-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      406 b- defN 23-May-08 16:09 kyeongmo230508AIL-0.0.3.dist-info/RECORD
+5 files, 984 bytes uncompressed, 661 bytes compressed:  32.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: myLib/myLib.py
 Comment: 
 
-Filename: kyeongmo230508AIL-0.0.2.dist-info/METADATA
+Filename: kyeongmo230508AIL-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: kyeongmo230508AIL-0.0.2.dist-info/WHEEL
+Filename: kyeongmo230508AIL-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: kyeongmo230508AIL-0.0.2.dist-info/top_level.txt
+Filename: kyeongmo230508AIL-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: kyeongmo230508AIL-0.0.2.dist-info/RECORD
+Filename: kyeongmo230508AIL-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## myLib/myLib.py

```diff
@@ -1,9 +1,9 @@
 
-import numpy
+import numpy as np
 import pandas
 from sklearn import *
 from tensorflow import *
 import matplotlib
 import scipy
 from keras import *
 import torch
```

