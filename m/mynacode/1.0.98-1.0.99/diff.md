# Comparing `tmp/mynacode-1.0.98-py3-none-any.whl.zip` & `tmp/mynacode-1.0.99-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 8923 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      102 b- defN 22-Sep-11 20:53 mlauto/__init__.py
 -rw-rw-rw-  2.0 fat    13388 b- defN 23-Feb-02 06:52 mlauto/mlauto.py
 -rw-rw-rw-  2.0 fat      111 b- defN 23-Feb-24 03:08 mynacode/__init__.py
 -rw-rw-rw-  2.0 fat     8317 b- defN 23-Mar-20 01:11 mynacode/mynacode - Copy.py
--rw-rw-rw-  2.0 fat     6404 b- defN 23-May-07 22:14 mynacode/mynacode.py
--rw-rw-rw-  2.0 fat      352 b- defN 23-May-07 23:02 mynacode-1.0.98.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-07 23:02 mynacode-1.0.98.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-07 23:02 mynacode-1.0.98.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      689 b- defN 23-May-07 23:02 mynacode-1.0.98.dist-info/RECORD
-9 files, 29464 bytes uncompressed, 7743 bytes compressed:  73.7%
+-rw-rw-rw-  2.0 fat     6408 b- defN 23-May-07 23:05 mynacode/mynacode.py
+-rw-rw-rw-  2.0 fat      352 b- defN 23-May-07 23:05 mynacode-1.0.99.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-07 23:05 mynacode-1.0.99.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-07 23:05 mynacode-1.0.99.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      689 b- defN 23-May-07 23:05 mynacode-1.0.99.dist-info/RECORD
+9 files, 29468 bytes uncompressed, 7743 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: mynacode/mynacode - Copy.py
 Comment: 
 
 Filename: mynacode/mynacode.py
 Comment: 
 
-Filename: mynacode-1.0.98.dist-info/METADATA
+Filename: mynacode-1.0.99.dist-info/METADATA
 Comment: 
 
-Filename: mynacode-1.0.98.dist-info/WHEEL
+Filename: mynacode-1.0.99.dist-info/WHEEL
 Comment: 
 
-Filename: mynacode-1.0.98.dist-info/top_level.txt
+Filename: mynacode-1.0.99.dist-info/top_level.txt
 Comment: 
 
-Filename: mynacode-1.0.98.dist-info/RECORD
+Filename: mynacode-1.0.99.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mynacode/mynacode.py

```diff
@@ -81,15 +81,15 @@
 
   train = np.array(train)
   test = np.array(test)
   val = np.array(val)
 
   data = {'run_id': run_id, 'train_shape' : train.shape, 'test_shape': test.shape, 'val_shape': val.shape,
           'train_mean': np.mean(train), 'test_mean': np.mean(test), 'val_mean': np.mean(val),
-          'train_median': np.median(train), 'test_mean': np.median(test), 'val_mean': np.median(val),
+          'train_median': np.median(train), 'test_median': np.median(test), 'val_median': np.median(val),
           'train_min': np.min(train), 'test_min': np.min(test), 'val_min': np.min(val),
           'train_max': np.max(train), 'test_max': np.max(test), 'val_max': np.max(val),
           'username': username, 'key': key}
   
   response = requests.post(protocol+'://'+IP+'/api/add_datasets', data=data)
   
   if response.text == '0':
```

