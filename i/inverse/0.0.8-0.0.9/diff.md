# Comparing `tmp/inverse-0.0.8-py3-none-any.whl.zip` & `tmp/inverse-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 286904 bytes, number of entries: 104
+Zip file size: 286892 bytes, number of entries: 104
 -rw-r--r--  2.0 unx      330 b- defN 80-Jan-01 00:00 inverse/__init__.py
 -rw-r--r--  2.0 unx        9 b- defN 80-Jan-01 00:00 inverse/__version__.py
 -rw-r--r--  2.0 unx     1281 b- defN 80-Jan-01 00:00 inverse/c_ext/vector_ops.c
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/__init__.py
 -rw-r--r--  2.0 unx     1380 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/cdeneme.py
 -rw-r--r--  2.0 unx    16728 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/clib
 -rw-r--r--  2.0 unx      216 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/clib.c
@@ -49,15 +49,15 @@
 -rw-r--r--  2.0 unx      790 b- defN 80-Jan-01 00:00 inverse/src/engine/algos/benchmarks/vector_ops_bench.py
 -rw-r--r--  2.0 unx     1315 b- defN 80-Jan-01 00:00 inverse/src/engine/algos_save/_save_base.py
 -rw-r--r--  2.0 unx     4534 b- defN 80-Jan-01 00:00 inverse/src/engine/algos_save/_save_sparse.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/src/engine/base_classes/__init__.py
 -rw-r--r--  2.0 unx      367 b- defN 80-Jan-01 00:00 inverse/src/engine/base_classes/big_matrix_base.py
 -rw-r--r--  2.0 unx     1884 b- defN 80-Jan-01 00:00 inverse/src/engine/main.py
 -rw-r--r--  2.0 unx     2677 b- defN 80-Jan-01 00:00 inverse/src/engine/main_funcs_to_load.py
--rw-r--r--  2.0 unx     4380 b- defN 80-Jan-01 00:00 inverse/src/engine/matrix_converters.py
+-rw-r--r--  2.0 unx     4360 b- defN 80-Jan-01 00:00 inverse/src/engine/matrix_converters.py
 -rw-r--r--  2.0 unx     2763 b- defN 80-Jan-01 00:00 inverse/src/engine/nontest_test.py
 -rw-r--r--  2.0 unx     3357 b- defN 80-Jan-01 00:00 inverse/src/engine/sp_matrix_ops.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/src/large_data/__init__.py
 -rw-r--r--  2.0 unx      467 b- defN 80-Jan-01 00:00 inverse/src/large_data/data_converters.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/src/loggers/__init__.py
 -rw-r--r--  2.0 unx      790 b- defN 80-Jan-01 00:00 inverse/src/loggers/_logger.py
 -rw-r--r--  2.0 unx     2087 b- defN 80-Jan-01 00:00 inverse/src/loggers/_logger3.py
@@ -95,12 +95,12 @@
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/tests/test_inverse_matrices/__init__.py
 -rw-r--r--  2.0 unx     1300 b- defN 80-Jan-01 00:00 inverse/tests/test_inverse_matrices/test_some.py
 -rw-r--r--  2.0 unx      715 b- defN 80-Jan-01 00:00 inverse/tests/test_inverse_matrices/test_sparse_inverse.py
 -rw-r--r--  2.0 unx      421 b- defN 80-Jan-01 00:00 inverse/tests/test_main.py
 -rw-r--r--  2.0 unx     1443 b- defN 80-Jan-01 00:00 inverse/tests/test_matrix_op_main.py
 -rw-r--r--  2.0 unx     3630 b- defN 80-Jan-01 00:00 inverse/tests/test_mini_tests.py
 -rw-r--r--  2.0 unx     1548 b- defN 80-Jan-01 00:00 inverse/tests/tests.py
--rw-r--r--  2.0 unx     1069 b- defN 80-Jan-01 00:00 inverse-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     2327 b- defN 80-Jan-01 00:00 inverse-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 inverse-0.0.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx     9388 b- defN 16-Jan-01 00:00 inverse-0.0.8.dist-info/RECORD
-104 files, 772432 bytes uncompressed, 271786 bytes compressed:  64.8%
+-rw-r--r--  2.0 unx     1069 b- defN 80-Jan-01 00:00 inverse-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2327 b- defN 80-Jan-01 00:00 inverse-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 inverse-0.0.9.dist-info/WHEEL
+?rw-r--r--  2.0 unx     9388 b- defN 16-Jan-01 00:00 inverse-0.0.9.dist-info/RECORD
+104 files, 772412 bytes uncompressed, 271774 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -294,20 +294,20 @@
 
 Filename: inverse/tests/test_mini_tests.py
 Comment: 
 
 Filename: inverse/tests/tests.py
 Comment: 
 
-Filename: inverse-0.0.8.dist-info/LICENSE
+Filename: inverse-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: inverse-0.0.8.dist-info/METADATA
+Filename: inverse-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: inverse-0.0.8.dist-info/WHEEL
+Filename: inverse-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: inverse-0.0.8.dist-info/RECORD
+Filename: inverse-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inverse/src/engine/matrix_converters.py

```diff
@@ -128,8 +128,8 @@
     # sonuc2 = np.matmul(matrix, inverse_mat2)
     sonuc3 = np.matmul(matrix, matrix_check)
 
     eps = 0.0001
     kontrol = close_identity(matrix=sonuc1, eps=eps)
     # kontrol2 = close_identity(matrix=sonuc2, eps=eps)
     kontrol2 = close_identity(matrix=sonuc3, eps=eps)
-    print(CallStack)
+
```

## Comparing `inverse-0.0.8.dist-info/LICENSE` & `inverse-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `inverse-0.0.8.dist-info/METADATA` & `inverse-0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inverse
-Version: 0.0.8
+Version: 0.0.9
 Summary: large matrix operations
 Home-page: https://github.com/SermetPekin/inverse-repo
 License: MIT
 Author: Sermet Pekin
 Author-email: sermet.pekin@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `inverse-0.0.8.dist-info/RECORD` & `inverse-0.0.9.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 inverse/src/engine/algos/benchmarks/vector_ops_bench.py,sha256=JzWriBPL-bA10k7U4ITzGef4Kp0-uL3sXSpPzgTl-zE,790
 inverse/src/engine/algos_save/_save_base.py,sha256=lUr48MvFEODhZJ9Oc6-QZI2y_Q_RtBcZLb6qZxfnBN4,1315
 inverse/src/engine/algos_save/_save_sparse.py,sha256=TQRViJD33oWw84BJSCKlq96TURP33_rf9PJQFcbc0Ks,4534
 inverse/src/engine/base_classes/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inverse/src/engine/base_classes/big_matrix_base.py,sha256=OKOmkAOAvfJviuQsqa13FP0L2X2gnFieNmqUaEgVdsg,367
 inverse/src/engine/main.py,sha256=sQ4cTO5FCvG3r6kY6UgLhHlRZlGuyFO0nshkpEXn4T8,1884
 inverse/src/engine/main_funcs_to_load.py,sha256=UPL-AP9zxJSiDXfMhF9Kf9lCuW5IWoSw9SRrfIshe_E,2677
-inverse/src/engine/matrix_converters.py,sha256=O5Qa02oS10QstApONSZFS7_9Ezhi8nq6THf5HjvFz3E,4380
+inverse/src/engine/matrix_converters.py,sha256=1MswCHF6ruZ5Tqtl3PMbAUdhZqB1FFhCUfJcPGj5uHM,4360
 inverse/src/engine/nontest_test.py,sha256=Rpu9W3f9mRMEN31tO4wEuq9R6J3D60kCGk6j29rJroY,2763
 inverse/src/engine/sp_matrix_ops.py,sha256=_8L-OYJTLVfa6u3kiMG3qKOSgsV2niinMTxJY1s0lqw,3357
 inverse/src/large_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inverse/src/large_data/data_converters.py,sha256=yGlEge3y7bzQnIXWEHOz-c0ldOvZYtEWPpiaCMICeDY,467
 inverse/src/loggers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inverse/src/loggers/_logger.py,sha256=IglHV2MkswZEM5Ok6awmmMpPKOfSRN1SuTL6lsDpP2E,790
 inverse/src/loggers/_logger3.py,sha256=V9QftNCW8v1PldB31iIe39Iihvw5m9tSoHR0UCISvDA,2087
@@ -94,11 +94,11 @@
 inverse/tests/test_inverse_matrices/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inverse/tests/test_inverse_matrices/test_some.py,sha256=8rGE5qC9Sapy3nK6B8ikjWC8HL-NRnDsqJtXIdYJWNs,1300
 inverse/tests/test_inverse_matrices/test_sparse_inverse.py,sha256=DkLIE5Zpn2OQU9bVAgpzNYh8QCcI7r231VMdlE6GZzw,715
 inverse/tests/test_main.py,sha256=F3q6UOEIB90I_g5CYhIDlhiXhxnPUspfUaHnzQETTNI,421
 inverse/tests/test_matrix_op_main.py,sha256=ZiR4oAXV27kmZhimNhs4Xfyru4a6zMf633u5uSs9SXg,1443
 inverse/tests/test_mini_tests.py,sha256=FTES-jBIJ2QH5APyMCsKLhAG2DbbwrQjfmmQdhcOcHQ,3630
 inverse/tests/tests.py,sha256=QV1Gv33kfsqCxGlAAIMVucTopTnAu6fj8lQw8wfw9is,1548
-inverse-0.0.8.dist-info/LICENSE,sha256=HfUG_pNgR_KESlLAy_oG9ttnqf9XDmCmIHrtkXICRlE,1069
-inverse-0.0.8.dist-info/METADATA,sha256=nhgnPo00VVe9vhU8lZ3HXkAHxbphj2wV141T_2PPzHo,2327
-inverse-0.0.8.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-inverse-0.0.8.dist-info/RECORD,,
+inverse-0.0.9.dist-info/LICENSE,sha256=HfUG_pNgR_KESlLAy_oG9ttnqf9XDmCmIHrtkXICRlE,1069
+inverse-0.0.9.dist-info/METADATA,sha256=UZkNAYyWBdh-HAclou83O2QEYwTCGM-Cla5DPQgTr2M,2327
+inverse-0.0.9.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+inverse-0.0.9.dist-info/RECORD,,
```

