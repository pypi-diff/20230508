# Comparing `tmp/dissect.util-3.7.dev1.tar.gz` & `tmp/dissect.util-3.8.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.util-3.7.dev1.tar", last modified: Thu Mar 16 13:05:22 2023, max compression
+gzip compressed data, was "dissect.util-3.8.dev1.tar", last modified: Mon May  8 09:34:41 2023, max compression
```

## Comparing `dissect.util-3.7.dev1.tar` & `dissect.util-3.8.dev1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:22.161786 dissect.util-3.7.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-03-16 13:05:22.161786 dissect.util-3.7.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:22.141785 dissect.util-3.7.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:22.153785 dissect.util-3.7.dev1/dissect/util/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/dissect/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:22.153785 dissect.util-3.7.dev1/dissect/util/compression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:59.000000 dissect.util-3.7.dev1/dissect/util/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/dissect/util/compression/lz4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/dissect/util/compression/lznt1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/dissect/util/compression/lzo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/dissect/util/compression/lzxpress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/dissect/util/compression/lzxpress_huffman.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/dissect/util/compression/sevenbit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/dissect/util/cpio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:22.157786 dissect.util-3.7.dev1/dissect/util/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:59.000000 dissect.util-3.7.dev1/dissect/util/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/dissect/util/encoding/surrogateescape.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/dissect/util/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/dissect/util/plist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/dissect/util/sid.py
--rw-r--r--   0 runner    (1001) docker     (123)    18497 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/dissect/util/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:22.157786 dissect.util-3.7.dev1/dissect/util/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:59.000000 dissect.util-3.7.dev1/dissect/util/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/dissect/util/tools/dump_nskeyedarchiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/dissect/util/ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/dissect/util/xmemoryview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:22.153785 dissect.util-3.7.dev1/dissect.util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-03-16 13:05:22.000000 dissect.util-3.7.dev1/dissect.util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-16 13:05:22.000000 dissect.util-3.7.dev1/dissect.util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 13:05:22.000000 dissect.util-3.7.dev1/dissect.util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-16 13:05:22.000000 dissect.util-3.7.dev1/dissect.util.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 13:05:22.000000 dissect.util-3.7.dev1/dissect.util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-16 13:05:07.000000 dissect.util-3.7.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 13:05:22.161786 dissect.util-3.7.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:22.157786 dissect.util-3.7.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:59.000000 dissect.util-3.7.dev1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:22.161786 dissect.util-3.7.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/tests/data/bin.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/tests/data/crc.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/tests/data/hpbin.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/tests/data/hpodc.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/tests/data/newc.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/tests/data/odc.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/tests/test_cpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/tests/test_plist.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/tests/test_sid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/tests/test_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/tests/test_xmemoryview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-16 13:04:58.000000 dissect.util-3.7.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:34:41.112528 dissect.util-3.8.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-08 09:34:41.112528 dissect.util-3.8.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:34:41.104528 dissect.util-3.8.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:34:41.108528 dissect.util-3.8.dev1/dissect/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/dissect/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:34:41.108528 dissect.util-3.8.dev1/dissect/util/compression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/dissect/util/compression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/dissect/util/compression/lz4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/dissect/util/compression/lznt1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/dissect/util/compression/lzo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/dissect/util/compression/lzxpress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/dissect/util/compression/lzxpress_huffman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/dissect/util/compression/sevenbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/dissect/util/cpio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:34:41.108528 dissect.util-3.8.dev1/dissect/util/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/dissect/util/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/dissect/util/encoding/surrogateescape.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/dissect/util/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/dissect/util/plist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/dissect/util/sid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18781 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/dissect/util/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:34:41.108528 dissect.util-3.8.dev1/dissect/util/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/dissect/util/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/dissect/util/tools/dump_nskeyedarchiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/dissect/util/ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/dissect/util/xmemoryview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:34:41.108528 dissect.util-3.8.dev1/dissect.util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-08 09:34:41.000000 dissect.util-3.8.dev1/dissect.util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-08 09:34:41.000000 dissect.util-3.8.dev1/dissect.util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:34:41.000000 dissect.util-3.8.dev1/dissect.util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-08 09:34:41.000000 dissect.util-3.8.dev1/dissect.util.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 09:34:41.000000 dissect.util-3.8.dev1/dissect.util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-08 09:34:31.000000 dissect.util-3.8.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 09:34:41.112528 dissect.util-3.8.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:34:41.108528 dissect.util-3.8.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:34:41.112528 dissect.util-3.8.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/tests/data/bin.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/tests/data/crc.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/tests/data/hpbin.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/tests/data/hpodc.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/tests/data/newc.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/tests/data/odc.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/tests/test_cpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/tests/test_plist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/tests/test_sid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/tests/test_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/tests/test_xmemoryview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-08 09:34:26.000000 dissect.util-3.8.dev1/tox.ini
```

### Comparing `dissect.util-3.7.dev1/LICENSE` & `dissect.util-3.8.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/PKG-INFO` & `dissect.util-3.8.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.util
-Version: 3.7.dev1
+Version: 3.8.dev1
 Summary: A Dissect module implementing various utility functions for the other Dissect modules
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.util
 Project-URL: repository, https://github.com/fox-it/dissect.util
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.util-3.7.dev1/README.md` & `dissect.util-3.8.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/dissect/util/compression/lz4.py` & `dissect.util-3.8.dev1/dissect/util/compression/lz4.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/dissect/util/compression/lznt1.py` & `dissect.util-3.8.dev1/dissect/util/compression/lznt1.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/dissect/util/compression/lzo.py` & `dissect.util-3.8.dev1/dissect/util/compression/lzo.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/dissect/util/compression/lzxpress.py` & `dissect.util-3.8.dev1/dissect/util/compression/lzxpress.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/dissect/util/compression/lzxpress_huffman.py` & `dissect.util-3.8.dev1/dissect/util/compression/lzxpress_huffman.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/dissect/util/compression/sevenbit.py` & `dissect.util-3.8.dev1/dissect/util/compression/sevenbit.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/dissect/util/cpio.py` & `dissect.util-3.8.dev1/dissect/util/cpio.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/dissect/util/plist.py` & `dissect.util-3.8.dev1/dissect/util/plist.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/dissect/util/sid.py` & `dissect.util-3.8.dev1/dissect/util/sid.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/dissect/util/stream.py` & `dissect.util-3.8.dev1/dissect/util/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import io
 import os
 from bisect import bisect_left, bisect_right
+from threading import Lock
 from typing import BinaryIO, Optional, Union
 
 STREAM_BUFFER_SIZE = int(os.getenv("DISSECT_STREAM_BUFFER_SIZE", io.DEFAULT_BUFFER_SIZE))
 
 
 class AlignedStream(io.RawIOBase):
     """Basic buffered stream that provides easy aligned reads.
@@ -30,14 +31,15 @@
         self.size = size
         self.align = align
 
         self._pos = 0
         self._pos_align = 0
 
         self._buf = None
+        self._seek_lock = Lock()
 
     def _set_pos(self, pos: int) -> None:
         """Update the position and aligned position within the stream."""
         new_pos_align = pos - (pos % self.align)
 
         if self._pos_align != new_pos_align:
             self._pos_align = new_pos_align
@@ -65,83 +67,85 @@
         else:
             raise IOError("invalid whence value")
 
         return pos
 
     def seek(self, pos: int, whence: int = io.SEEK_SET) -> int:
         """Seek the stream to the specified position."""
-        pos = self._seek(pos, whence)
-        self._set_pos(pos)
+        with self._seek_lock:
+            pos = self._seek(pos, whence)
+            self._set_pos(pos)
 
-        return pos
+            return pos
 
     def read(self, n: int = -1) -> bytes:
         """Read and return up to n bytes, or read to the end of the stream if n is -1.
 
         Returns an empty bytes object on EOF.
         """
         if n is not None and n < -1:
             raise ValueError("invalid number of bytes to read")
 
         r = []
         size = self.size
         align = self.align
 
-        if size is None and n == -1:
-            r = []
-            if self._buf:
-                buffer_pos = self._pos - self._pos_align
-                r.append(self._buf[buffer_pos:])
-
-            r.append(self._read(self._pos_align + align, -1))
-
-            buf = b"".join(r)
-            self._set_pos(self._pos + len(buf))
-            return buf
-
-        if size is not None:
-            remaining = size - self._pos
+        with self._seek_lock:
+            if size is None and n == -1:
+                r = []
+                if self._buf:
+                    buffer_pos = self._pos - self._pos_align
+                    r.append(self._buf[buffer_pos:])
+
+                r.append(self._read(self._pos_align + align, -1))
+
+                buf = b"".join(r)
+                self._set_pos(self._pos + len(buf))
+                return buf
+
+            if size is not None:
+                remaining = size - self._pos
+
+                if n == -1:
+                    n = remaining
+                else:
+                    n = min(n, remaining)
+
+            if n == 0 or size is not None and size <= self._pos:
+                return b""
+
+            # Read misaligned start from buffer
+            if self._pos != self._pos_align:
+                self._fill_buf()
 
-            if n == -1:
-                n = remaining
-            else:
-                n = min(n, remaining)
-
-        if n == 0 or size is not None and size <= self._pos:
-            return b""
-
-        # Read misaligned start from buffer
-        if self._pos != self._pos_align:
-            self._fill_buf()
-
-            buffer_pos = self._pos - self._pos_align
-            remaining = align - buffer_pos
-            buffer_len = min(n, remaining)
+                buffer_pos = self._pos - self._pos_align
+                remaining = align - buffer_pos
+                buffer_len = min(n, remaining)
 
-            r.append(self._buf[buffer_pos : buffer_pos + buffer_len])
+                r.append(self._buf[buffer_pos : buffer_pos + buffer_len])
 
-            n -= buffer_len
-            self._set_pos(self._pos + buffer_len)
+                n -= buffer_len
+                self._set_pos(self._pos + buffer_len)
 
-        # Aligned blocks
-        if n >= align:
-            count, n = divmod(n, align)
+            # Aligned blocks
+            if n >= align:
+                count, n = divmod(n, align)
 
-            read_len = count * align
-            r.append(self._read(self._pos, read_len))
+                read_len = count * align
+                r.append(self._read(self._pos, read_len))
 
-            self._set_pos(self._pos + read_len)
+                self._set_pos(self._pos + read_len)
 
-        # Misaligned end
-        if n > 0:
-            self._fill_buf()
-            r.append(self._buf[:n])
-            self._set_pos(self._pos + n)
+            # Misaligned end
+            if n > 0:
+                self._fill_buf()
+                r.append(self._buf[:n])
+                self._set_pos(self._pos + n)
 
-        return b"".join(r)
+            return b"".join(r)
 
     def readinto(self, b: bytearray) -> int:
         """Read bytes into a pre-allocated bytes-like object b.
 
         Returns an int representing the number of bytes read (0 for EOF).
         """
         buf = self.read(len(b))
```

### Comparing `dissect.util-3.7.dev1/dissect/util/tools/dump_nskeyedarchiver.py` & `dissect.util-3.8.dev1/dissect/util/tools/dump_nskeyedarchiver.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/dissect/util/ts.py` & `dissect.util-3.8.dev1/dissect/util/ts.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/dissect/util/xmemoryview.py` & `dissect.util-3.8.dev1/dissect/util/xmemoryview.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/dissect.util.egg-info/PKG-INFO` & `dissect.util-3.8.dev1/dissect.util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.util
-Version: 3.7.dev1
+Version: 3.8.dev1
 Summary: A Dissect module implementing various utility functions for the other Dissect modules
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.util
 Project-URL: repository, https://github.com/fox-it/dissect.util
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.util-3.7.dev1/dissect.util.egg-info/SOURCES.txt` & `dissect.util-3.8.dev1/dissect.util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/pyproject.toml` & `dissect.util-3.8.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/tests/data/bin.cpio.gz` & `dissect.util-3.8.dev1/tests/data/bin.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/tests/data/crc.cpio.gz` & `dissect.util-3.8.dev1/tests/data/crc.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/tests/data/hpbin.cpio.gz` & `dissect.util-3.8.dev1/tests/data/hpbin.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/tests/data/hpodc.cpio.gz` & `dissect.util-3.8.dev1/tests/data/hpodc.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/tests/data/newc.cpio.gz` & `dissect.util-3.8.dev1/tests/data/newc.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/tests/data/odc.cpio.gz` & `dissect.util-3.8.dev1/tests/data/odc.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/tests/test_compression.py` & `dissect.util-3.8.dev1/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/tests/test_cpio.py` & `dissect.util-3.8.dev1/tests/test_cpio.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/tests/test_plist.py` & `dissect.util-3.8.dev1/tests/test_plist.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/tests/test_sid.py` & `dissect.util-3.8.dev1/tests/test_sid.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/tests/test_stream.py` & `dissect.util-3.8.dev1/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/tests/test_ts.py` & `dissect.util-3.8.dev1/tests/test_ts.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/tests/test_xmemoryview.py` & `dissect.util-3.8.dev1/tests/test_xmemoryview.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.7.dev1/tox.ini` & `dissect.util-3.8.dev1/tox.ini`

 * *Files identical despite different names*

