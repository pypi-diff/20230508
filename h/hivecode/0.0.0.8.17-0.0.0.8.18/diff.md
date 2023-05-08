# Comparing `tmp/hivecode-0.0.0.8.17.tar.gz` & `tmp/hivecode-0.0.0.8.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Juan.Mejia\OneDrive - Idata\Escritorio\Code\hivecode\dist\.tmp-ooslpnpb\hivecode-0.0.0.8.17.tar", last modified: Tue Dec 20 22:31:09 2022, max compression
+gzip compressed data, was "hivecode-0.0.0.8.18.tar", last modified: Mon May  8 01:39:15 2023, max compression
```

## Comparing `hivecode-0.0.0.8.17.tar` & `hivecode-0.0.0.8.18.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2022-12-20 22:31:09.501935 hivecode-0.0.0.8.17/
--rw-rw-rw-   0        0        0     1101 2022-12-16 20:43:43.000000 hivecode-0.0.0.8.17/LICENSE
--rw-rw-rw-   0        0        0     1004 2022-12-20 22:31:09.501935 hivecode-0.0.0.8.17/PKG-INFO
--rw-rw-rw-   0        0        0     1462 2022-12-05 06:00:48.000000 hivecode-0.0.0.8.17/README.md
--rw-rw-rw-   0        0        0     1297 2022-12-20 22:30:58.000000 hivecode-0.0.0.8.17/pyproject.toml
--rw-rw-rw-   0        0        0     1307 2022-12-20 22:31:09.502935 hivecode-0.0.0.8.17/setup.cfg
--rw-rw-rw-   0        0        0       71 2022-10-09 21:52:57.000000 hivecode-0.0.0.8.17/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-20 22:31:09.470324 hivecode-0.0.0.8.17/src/
-drwxrwxrwx   0        0        0        0 2022-12-20 22:31:09.480323 hivecode-0.0.0.8.17/src/hiveadb/
--rw-rw-rw-   0        0        0        0 2022-10-11 04:26:52.000000 hivecode-0.0.0.8.17/src/hiveadb/__init__.py
--rw-rw-rw-   0        0        0     8151 2022-11-27 04:17:52.000000 hivecode-0.0.0.8.17/src/hiveadb/function.py
--rw-rw-rw-   0        0        0    37226 2022-11-29 21:54:14.000000 hivecode-0.0.0.8.17/src/hiveadb/io.py
--rw-rw-rw-   0        0        0        0 2022-10-11 04:27:02.000000 hivecode-0.0.0.8.17/src/hiveadb/py.typed
-drwxrwxrwx   0        0        0        0 2022-12-20 22:31:09.487325 hivecode-0.0.0.8.17/src/hivecode.egg-info/
--rw-rw-rw-   0        0        0     1004 2022-12-20 22:31:09.000000 hivecode-0.0.0.8.17/src/hivecode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      703 2022-12-20 22:31:09.000000 hivecode-0.0.0.8.17/src/hivecode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-20 22:31:09.000000 hivecode-0.0.0.8.17/src/hivecode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-10-09 21:32:42.000000 hivecode-0.0.0.8.17/src/hivecode.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      276 2022-12-20 22:31:09.000000 hivecode-0.0.0.8.17/src/hivecode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2022-12-20 22:31:09.000000 hivecode-0.0.0.8.17/src/hivecode.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-12-20 22:31:09.492325 hivecode-0.0.0.8.17/src/hivecore/
--rw-rw-rw-   0        0        0        0 2022-10-09 06:18:31.000000 hivecode-0.0.0.8.17/src/hivecore/__init__.py
--rw-rw-rw-   0        0        0     1326 2022-11-07 03:40:04.000000 hivecode-0.0.0.8.17/src/hivecore/constant.py
--rw-rw-rw-   0        0        0     3379 2022-10-29 21:48:02.000000 hivecode-0.0.0.8.17/src/hivecore/decorator.py
--rw-rw-rw-   0        0        0      829 2022-11-27 20:16:13.000000 hivecode-0.0.0.8.17/src/hivecore/function.py
--rw-rw-rw-   0        0        0     1508 2022-11-27 04:21:20.000000 hivecode-0.0.0.8.17/src/hivecore/pattern.py
--rw-rw-rw-   0        0        0        0 2022-10-09 20:42:03.000000 hivecode-0.0.0.8.17/src/hivecore/py.typed
-drwxrwxrwx   0        0        0        0 2022-12-20 22:31:09.494325 hivecode-0.0.0.8.17/src/hiveform/
--rw-rw-rw-   0        0        0        0 2022-11-29 21:56:14.000000 hivecode-0.0.0.8.17/src/hiveform/__init__.py
--rw-rw-rw-   0        0        0    24974 2022-12-04 03:12:04.000000 hivecode-0.0.0.8.17/src/hiveform/preprocess.py
-drwxrwxrwx   0        0        0        0 2022-12-20 22:31:09.500927 hivecode-0.0.0.8.17/src/hivesignal/
--rw-rw-rw-   0        0        0        0 2022-11-27 04:28:23.000000 hivecode-0.0.0.8.17/src/hivesignal/__init__.py
--rw-rw-rw-   0        0        0     1684 2022-11-28 13:47:59.000000 hivecode-0.0.0.8.17/src/hivesignal/analysis.py
--rw-rw-rw-   0        0        0     2410 2022-11-28 17:41:57.000000 hivecode-0.0.0.8.17/src/hivesignal/io.py
--rw-rw-rw-   0        0        0        0 2022-11-27 04:28:09.000000 hivecode-0.0.0.8.17/src/hivesignal/py.typed
--rw-rw-rw-   0        0        0     2126 2022-12-20 22:30:48.000000 hivecode-0.0.0.8.17/src/hivesignal/transform.py
--rw-rw-rw-   0        0        0      350 2022-11-28 16:11:05.000000 hivecode-0.0.0.8.17/src/hivesignal/visual.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:39:15.060758 hivecode-0.0.0.8.18/
+-rw-rw-rw-   0        0        0     3946 2023-05-08 01:39:15.061267 hivecode-0.0.0.8.18/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2023-04-11 20:04:04.000000 hivecode-0.0.0.8.18/README.rst
+-rw-rw-rw-   0        0        0     1387 2023-05-08 01:39:03.000000 hivecode-0.0.0.8.18/pyproject.toml
+-rw-rw-rw-   0        0        0      185 2023-02-13 02:12:12.000000 hivecode-0.0.0.8.18/requirements.txt
+-rw-rw-rw-   0        0        0     1304 2023-05-08 01:39:15.067310 hivecode-0.0.0.8.18/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:39:15.015698 hivecode-0.0.0.8.18/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 01:39:15.026787 hivecode-0.0.0.8.18/src/hiveadb/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/src/hiveadb/__init__.py
+-rw-rw-rw-   0        0        0     3690 2023-04-12 04:08:02.000000 hivecode-0.0.0.8.18/src/hiveadb/eda.py
+-rw-rw-rw-   0        0        0    11311 2023-04-12 03:58:56.000000 hivecode-0.0.0.8.18/src/hiveadb/function.py
+-rw-rw-rw-   0        0        0    86747 2023-04-11 23:45:25.000000 hivecode-0.0.0.8.18/src/hiveadb/io.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/src/hiveadb/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-08 01:39:15.042371 hivecode-0.0.0.8.18/src/hivecode.egg-info/
+-rw-rw-rw-   0        0        0     3946 2023-05-08 01:39:14.000000 hivecode-0.0.0.8.18/src/hivecode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      747 2023-05-08 01:39:15.000000 hivecode-0.0.0.8.18/src/hivecode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 01:39:14.000000 hivecode-0.0.0.8.18/src/hivecode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-08 01:34:18.000000 hivecode-0.0.0.8.18/src/hivecode.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      275 2023-05-08 01:39:14.000000 hivecode-0.0.0.8.18/src/hivecode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-05-08 01:39:14.000000 hivecode-0.0.0.8.18/src/hivecode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 01:39:15.054748 hivecode-0.0.0.8.18/src/hivecore/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/src/hivecore/__init__.py
+-rw-rw-rw-   0        0        0     1330 2023-05-08 01:20:28.000000 hivecode-0.0.0.8.18/src/hivecore/constant.py
+-rw-rw-rw-   0        0        0     9275 2023-04-24 04:05:22.000000 hivecode-0.0.0.8.18/src/hivecore/decorator.py
+-rw-rw-rw-   0        0        0     2744 2023-04-25 03:07:04.000000 hivecode-0.0.0.8.18/src/hivecore/eda.py
+-rw-rw-rw-   0        0        0     4261 2023-05-08 01:08:47.000000 hivecode-0.0.0.8.18/src/hivecore/function.py
+-rw-rw-rw-   0        0        0     1617 2023-04-12 05:20:34.000000 hivecode-0.0.0.8.18/src/hivecore/pattern.py
+-rw-rw-rw-   0        0        0    29856 2023-04-12 03:24:52.000000 hivecode-0.0.0.8.18/src/hivecore/preprocess.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/src/hivecore/py.typed
+-rw-rw-rw-   0        0        0     6276 2023-04-25 03:07:19.000000 hivecode-0.0.0.8.18/src/hivecore/visual.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:39:15.059745 hivecode-0.0.0.8.18/src/hivesignal/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/src/hivesignal/__init__.py
+-rw-rw-rw-   0        0        0     1683 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/src/hivesignal/analysis.py
+-rw-rw-rw-   0        0        0      292 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/src/hivesignal/eda.py
+-rw-rw-rw-   0        0        0     2383 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/src/hivesignal/io.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/src/hivesignal/py.typed
+-rw-rw-rw-   0        0        0     2126 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/src/hivesignal/transform.py
```

### Comparing `hivecode-0.0.0.8.17/PKG-INFO` & `hivecode-0.0.0.8.18/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,82 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2068 6976  : 2.1..Name: hiv
-00000020: 6563 6f64 650d 0a56 6572 7369 6f6e 3a20  ecode..Version: 
-00000030: 302e 302e 302e 382e 3137 0d0a 5375 6d6d  0.0.0.8.17..Summ
-00000040: 6172 793a 2048 6976 6563 6f64 6520 6973  ary: Hivecode is
-00000050: 2061 2073 6572 6965 7320 6f66 206c 6962   a series of lib
-00000060: 7261 7269 6573 2064 6573 6769 6e65 6420  raries desgined 
-00000070: 746f 206d 616b 6520 7072 6f67 7261 6d6d  to make programm
-00000080: 696e 6720 6c65 7373 206f 6620 616e 2061  ing less of an a
-00000090: 7274 6973 616e 2074 6173 6b20 616e 6420  rtisan task and 
-000000a0: 6d6f 7265 206f 6620 616e 2065 6e67 696e  more of an engin
-000000b0: 6565 7269 6e67 2074 6173 6b2e 2049 7420  eering task. It 
-000000c0: 696e 636c 7564 6573 2066 756e 6374 696f  includes functio
-000000d0: 6e73 2c20 6465 636f 7261 746f 7273 2061  ns, decorators a
-000000e0: 6e64 206d 756c 7469 706c 6520 636c 6173  nd multiple clas
-000000f0: 7365 7320 6465 7367 6969 6e65 6420 746f  ses desgiined to
-00000100: 206d 616b 6520 7468 6520 696d 706c 656d   make the implem
-00000110: 656e 7461 7469 6f6e 206f 6620 6465 7665  entation of deve
-00000120: 6c6f 706d 656e 7420 616e 6420 616e 616c  lopment and anal
-00000130: 7974 6963 616c 2070 726f 7965 6374 7320  ytical proyects 
-00000140: 6d6f 7265 206f 7269 656e 7465 6420 746f  more oriented to
-00000150: 2064 6573 6967 696e 2061 6e64 2061 7263   desigin and arc
-00000160: 6869 7465 6374 7572 6520 616e 6420 6c65  hitecture and le
-00000170: 7373 206f 6620 616e 2069 6d70 6c65 6d65  ss of an impleme
-00000180: 6e74 6174 696f 6e20 6865 6c6c 2e0d 0a41  ntation hell...A
-00000190: 7574 686f 723a 204a 7561 6e20 4d61 6e75  uthor: Juan Manu
-000001a0: 656c 204d 656a c3ad 6120 426f 7465 726f  el Mej..a Botero
-000001b0: 0d0a 5072 6f6a 6563 742d 5552 4c3a 2048  ..Project-URL: H
-000001c0: 6f6d 6570 6167 652c 2068 7474 7073 3a2f  omepage, https:/
-000001d0: 2f67 6974 6875 622e 636f 6d2f 4a75 616e  /github.com/Juan
-000001e0: 6d61 6d2f 6869 7665 636f 6465 0d0a 5072  mam/hivecode..Pr
-000001f0: 6f6a 6563 742d 5552 4c3a 2044 6f63 756d  oject-URL: Docum
-00000200: 656e 7461 7469 6f6e 2c20 6874 7470 733a  entation, https:
-00000210: 2f2f 6869 7665 636f 6465 2e72 6561 6474  //hivecode.readt
-00000220: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00000230: 6573 742f 0d0a 506c 6174 666f 726d 3a20  est/..Platform: 
-00000240: 756e 6978 0d0a 506c 6174 666f 726d 3a20  unix..Platform: 
-00000250: 6c69 6e75 780d 0a50 6c61 7466 6f72 6d3a  linux..Platform:
-00000260: 206f 7378 0d0a 506c 6174 666f 726d 3a20   osx..Platform: 
-00000270: 6379 6777 696e 0d0a 506c 6174 666f 726d  cygwin..Platform
-00000280: 3a20 7769 6e33 320d 0a43 6c61 7373 6966  : win32..Classif
-00000290: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-000002a0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000002b0: 686f 6e20 3a3a 2033 0d0a 436c 6173 7369  hon :: 3..Classi
-000002c0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000002d0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000002e0: 7468 6f6e 203a 3a20 3320 3a3a 204f 6e6c  thon :: 3 :: Onl
-000002f0: 790d 0a43 6c61 7373 6966 6965 723a 2050  y..Classifier: P
-00000300: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000310: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000320: 2033 2e38 0d0a 436c 6173 7369 6669 6572   3.8..Classifier
-00000330: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000340: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000350: 203a 3a20 332e 390d 0a43 6c61 7373 6966   :: 3.9..Classif
-00000360: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000370: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000380: 686f 6e20 3a3a 2033 2e31 300d 0a52 6571  hon :: 3.10..Req
-00000390: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
-000003a0: 332e 382e 300d 0a50 726f 7669 6465 732d  3.8.0..Provides-
-000003b0: 4578 7472 613a 2074 6573 7469 6e67 0d0a  Extra: testing..
-000003c0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-000003d0: 6465 760d 0a4c 6963 656e 7365 2d46 696c  dev..License-Fil
-000003e0: 653a 204c 4943 454e 5345 0d0a            e: LICENSE..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 2068 6976 6563 6f64 650d 0a64 6573   = hivecode..des
+00000020: 6372 6970 7469 6f6e 203d 2048 6976 6563  cription = Hivec
+00000030: 6f64 6520 6973 2061 2073 6572 6965 7320  ode is a series 
+00000040: 6f66 206c 6962 7261 7269 6573 2064 6573  of libraries des
+00000050: 6769 6e65 6420 746f 206d 616b 6520 7072  gined to make pr
+00000060: 6f67 7261 6d6d 696e 6720 6c65 7373 206f  ogramming less o
+00000070: 6620 616e 2061 7274 6973 616e 2074 6173  f an artisan tas
+00000080: 6b20 616e 6420 6d6f 7265 206f 6620 616e  k and more of an
+00000090: 2065 6e67 696e 6565 7269 6e67 2074 6173   engineering tas
+000000a0: 6b2e 2049 7420 696e 636c 7564 6573 2066  k. It includes f
+000000b0: 756e 6374 696f 6e73 2c20 6465 636f 7261  unctions, decora
+000000c0: 746f 7273 2061 6e64 206d 756c 7469 706c  tors and multipl
+000000d0: 6520 636c 6173 7365 7320 6465 7367 6969  e classes desgii
+000000e0: 6e65 6420 746f 206d 616b 6520 7468 6520  ned to make the 
+000000f0: 696d 706c 656d 656e 7461 7469 6f6e 206f  implementation o
+00000100: 6620 6465 7665 6c6f 706d 656e 7420 616e  f development an
+00000110: 6420 616e 616c 7974 6963 616c 2070 726f  d analytical pro
+00000120: 7965 6374 7320 6d6f 7265 206f 7269 656e  yects more orien
+00000130: 7465 6420 746f 2064 6573 6967 696e 2061  ted to desigin a
+00000140: 6e64 2061 7263 6869 7465 6374 7572 6520  nd architecture 
+00000150: 616e 6420 6c65 7373 206f 6620 616e 2069  and less of an i
+00000160: 6d70 6c65 6d65 6e74 6174 696f 6e20 6865  mplementation he
+00000170: 6c6c 2e0d 0a61 7574 686f 7220 3d20 4a75  ll...author = Ju
+00000180: 616e 204d 616e 7565 6c20 4d65 6ac3 ad61  an Manuel Mej..a
+00000190: 2042 6f74 6572 6f0d 0a70 6c61 7466 6f72   Botero..platfor
+000001a0: 6d73 203d 2075 6e69 782c 206c 696e 7578  ms = unix, linux
+000001b0: 2c20 6f73 782c 2063 7967 7769 6e2c 2077  , osx, cygwin, w
+000001c0: 696e 3332 0d0a 636c 6173 7369 6669 6572  in32..classifier
+000001d0: 7320 3d20 0d0a 0950 726f 6772 616d 6d69  s = ...Programmi
+000001e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001f0: 7974 686f 6e20 3a3a 2033 0d0a 0950 726f  ython :: 3...Pro
+00000200: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000210: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000220: 203a 3a20 4f6e 6c79 0d0a 0950 726f 6772   :: Only...Progr
+00000230: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000240: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
+00000250: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000260: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000270: 6e20 3a3a 2033 2e39 0d0a 0950 726f 6772  n :: 3.9...Progr
+00000280: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000290: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+000002a0: 300d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  0....[options]..
+000002b0: 7061 636b 6167 6573 203d 200d 0a09 6869  packages = ...hi
+000002c0: 7665 636f 7265 0d0a 0968 6976 6561 6462  vecore...hiveadb
+000002d0: 0d0a 0968 6976 6573 6967 6e61 6c0d 0a70  ...hivesignal..p
+000002e0: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+000002f0: 203e 3d33 2e38 2e30 0d0a 696e 7374 616c   >=3.8.0..instal
+00000300: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
+00000310: 7061 7261 6d69 6b6f 3d3d 322e 3131 2e30  paramiko==2.11.0
+00000320: 0d0a 0973 6370 3e3d 302e 3134 2e34 0d0a  ...scp>=0.14.4..
+00000330: 0973 6b6c 6561 726e 3e3d 302e 3234 2e31  .sklearn>=0.24.1
+00000340: 0d0a 0961 7a75 7265 2d63 6f73 6d6f 733e  ...azure-cosmos>
+00000350: 3d34 2e33 2e30 0d0a 096f 7065 6e70 7978  =4.3.0...openpyx
+00000360: 6c3e 3d33 2e30 2e31 300d 0a09 7471 646d  l>=3.0.10...tqdm
+00000370: 3e3d 342e 3634 2e31 0d0a 0973 6369 7079  >=4.64.1...scipy
+00000380: 3e3d 312e 362e 320d 0a09 6d61 7470 6c6f  >=1.6.2...matplo
+00000390: 746c 6962 3e3d 332e 342e 320d 0a09 6e75  tlib>=3.4.2...nu
+000003a0: 6d70 793e 3d31 2e32 302e 310d 0a09 7061  mpy>=1.20.1...pa
+000003b0: 6e64 6173 3e3d 312e 322e 340d 0a09 7365  ndas>=1.2.4...se
+000003c0: 6162 6f72 6e3e 3d30 2e31 312e 310d 0a09  aborn>=0.11.1...
+000003d0: 6b6f 616c 6173 0d0a 7061 636b 6167 655f  koalas..package_
+000003e0: 6469 7220 3d20 0d0a 093d 2073 7263 0d0a  dir = ...= src..
+000003f0: 7a69 705f 7361 6665 203d 206e 6f0d 0a0d  zip_safe = no...
+00000400: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
+00000410: 5f72 6571 7569 7265 5d0d 0a74 6573 7469  _require]..testi
+00000420: 6e67 203d 200d 0a09 7079 7465 7374 3e3d  ng = ...pytest>=
+00000430: 362e 300d 0a09 7079 7465 7374 2d63 6f76  6.0...pytest-cov
+00000440: 3e3d 322e 300d 0a09 6d79 7079 3e3d 302e  >=2.0...mypy>=0.
+00000450: 3931 300d 0a09 666c 616b 6538 3e3d 332e  910...flake8>=3.
+00000460: 390d 0a09 746f 783e 3d33 2e32 340d 0a0d  9...tox>=3.24...
+00000470: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+00000480: 655f 6461 7461 5d0d 0a68 6976 6563 6f72  e_data]..hivecor
+00000490: 6520 3d20 7079 2e74 7970 6564 0d0a 6869  e = py.typed..hi
+000004a0: 7665 6164 6220 3d20 7079 2e74 7970 6564  veadb = py.typed
+000004b0: 0d0a 6869 7665 7369 676e 616c 203d 2070  ..hivesignal = p
+000004c0: 792e 7479 7065 640d 0a0d 0a5b 666c 616b  y.typed....[flak
+000004d0: 6538 5d0d 0a6d 6178 2d6c 696e 652d 6c65  e8]..max-line-le
+000004e0: 6e67 7468 203d 2031 3630 0d0a 0d0a 5b65  ngth = 160....[e
+000004f0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+00000500: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+00000510: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `hivecode-0.0.0.8.17/pyproject.toml` & `hivecode-0.0.0.8.18/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [project]
 name = "hivecode"
 description = "Hivecode is a series of libraries desgined to make programming less of an artisan task and more of an engineering task. It includes functions, decorators and multiple classes desgiined to make the implementation of development and analytical proyects more oriented to desigin and architecture and less of an implementation hell."
-version = "0.0.0.8.17"
+version = "0.0.0.8.18"
 requires-python = ">=3.8.0"
+readme = "README.rst"
 authors = [
-    {name = "Juan Manuel Mejía Botero", author-email="juanmam941025@gmail.com"}
+    {name = "Juan Manuel Mejía Botero", email="juanmam941025@gmail.com"},
+    {name = "Sebastian López Valencia", email="sebaslv12@hotmail.com"}
 ]
 
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements.txt"] }
```

### Comparing `hivecode-0.0.0.8.17/src/hiveadb/function.py` & `hivecode-0.0.0.8.18/src/hiveadb/function.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,105 +1,151 @@
 from hivecore.constant import PANDAS_TYPES, PYSPARK_TYPES, KOALAS_TYPES, PANDAS_ON_SPARK_TYPES, PANDAS, KOALAS, SPARK, PYSPARK, PANDAS_ON_SPARK, IN_PANDAS_ON_SPARK, IN_PYSPARK
 from hivecore.function import lib_required
 
-from typing import List
+from typing import List, Union, Any
 
 # Pyspark
 from pyspark.context import SparkContext
 from pyspark.sql.session import SparkSession
 from pyspark.pandas import from_pandas as ps_from_pandas
 from databricks.koalas import from_pandas, DataFrame as KoalasDataFrame
 
 def get_spark() -> SparkSession:
     """
-    Fetches the current instance of spark. If none exists, creates a new one.
-    Returns:
-        SparkSession: The current spark session.
+    Fetches the current instance of Spark. If none exists, creates a new one.
+
+    :return: The current Spark session.
+    :rtype: pyspark.sql.SparkSession
     """
     # Spark
-    sc = SparkContext.getOrCreate()
+    sc: SparkContext = SparkContext.getOrCreate()
     return SparkSession(sc)
 
 
 # DBUtils
 try:
     # up to DBR 8.2
     from dbutils import DBUtils  # pylint: disable=import-error,wrong-import-position
 except:
     # above DBR 8.3
     from dbruntime.dbutils import DBUtils  # pylint: disable=import-error,wrong-import-position
 
 
 def get_dbutils(spark: SparkSession = None) -> DBUtils:
     """
-    Feches the current instance of DBUtils.
-    Args:
-        spark (SparkSession, optional): The current spark session. Defaults to None.
-    Returns:
-        DBUtils: _description_
+    Fetches the current instance of DBUtils.
+
+    :param spark: The current spark session. Defaults to None.
+    :type spark: pyspark.sql.SparkSession
+
+    :return: An instance of DBUtils.
+    :rtype: databricks.DBUtils
     """
         
     # We try to create dbutils from spark or by using IPython
     try:
         return DBUtils(spark)
     except:
         import IPython
         return IPython.get_ipython().user_ns["dbutils"]
 
 
 spark   = get_spark()
 dbutils = get_dbutils()
 
 
-def mount(storage:     str,
-          key:         str,
-          mount_point: str       = '/mnt/',
-          mounts:      List[str] = ["raw", "silver", "gold"], 
-          verbose:     bool      = False
-          ) -> None:
+from typing import List
+
+def mount(
+    storage: str,
+    key: str,
+    mount_point: str = '/mnt/',
+    mounts: List[str] = ["raw", "silver", "gold"],
+    postfix: str = '-zone',
+    include_tqdm: bool = False,
+    verbose: bool = False
+) -> None:
     """
     Mounts a set of zones into the system.
-    Args:
-        storage (str): The name of the storage to mount. This can be found at keys access in your storage account.
-        key (str): The key of the storage to mount. This can be found at keys access in your storage account.
-        mount_point (str, optional): The mount point to use. 
-            Defaults to '/mnt/'.
-        mounts (List[str], optional): A list of all the mounts you want. This doesn't include the prefix. Check example. 
-            Defaults to ["raw", "silver", "gold"].
-        postfix (str, optional): The postfix is the ending you want to put to your mount zones. Set it to an empty 
-        string if you don't want to apply it. 
-            Defaults to '-zone'.
-        include_tqdm (bool, optional): A flag to include tqdm bars for mounts. 
-            Defaults to False.
+
+    :param storage: The name of the storage to mount. This can be found at keys access in your storage account.
+    :type storage: str
+    
+    :param key: The key of the storage to mount. This can be found at keys access in your storage account.
+    :type key: str
+    
+    :param mount_point: The mount point to use, defaults to '/mnt/'.
+    :type mount_point: str, optional
+    
+    :param mounts: A list of all the mounts you want. This doesn't include the prefix. Check example. 
+        Defaults to ["raw", "silver", "gold"].
+    :type mounts: List[str], optional
+    
+    :param postfix: The postfix is the ending you want to put to your mount zones. Set it to an empty 
+        string if you don't want to apply it, defaults to '-zone'.
+    :type postfix: str, optional
+    
+    :param include_tqdm: A flag to include tqdm bars for mounts, defaults to False.
+    :type include_tqdm: bool, optional
+    
+    :param verbose: A flag to indicate whether to show tqdm progress bar or not, defaults to False.
+    :type verbose: bool, optional
+    
+    :return: None
+    :rtype: None
     """
     def __mount(mount_name: str) -> None:
         """
         Mounts a single zone to the system.
-        Args:
-            mount_name (str): The name of the zone to mount.
+
+        :param mount_name: The name of the zone to mount.
+        :type mount_name: str
+
+        :return: None
+        :rtype: None
         """
         if not f"{mount_point}{mount_name}" in list(map(lambda mount: mount.mountPoint, dbutils.fs.mounts())):
             dbutils.fs.mount(
-                source = f"wasbs://{mount_name}@{storage}.blob.core.windows.net/",
-                mount_point = f"{mount_point}{mount_name}",
-                extra_configs = { 
-                    f"fs.azure.account.key.{storage}.blob.core.windows.net": key
-                }
+                source=f"wasbs://{mount_name}@{storage}.blob.core.windows.net/",
+                mount_point=f"{mount_point}{mount_name}",
+                extra_configs={f"fs.azure.account.key.{storage}.blob.core.windows.net": key}
             )
 
     lib_required("tqdm")
     from tqdm import tqdm
 
-    if verbose:
-        list(map(lambda mount_name: __mount(mount_name), tqdm(mounts, desc="Mounts", position=0, leave=True)))
+    if include_tqdm:
+        mount_iterator = tqdm(mounts, desc="Mounts", position=0, leave=True)
     else:
-        list(map(lambda mount_name: __mount(mount_name), mounts))
+        mount_iterator = mounts
+
+    if verbose:
+        mount_iterator = tqdm(mount_iterator)
 
+    for mount_name in mount_iterator:
+        __mount(mount_name)
+
+import pandas
+import pyspark
+
+
+def data_convert(df: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame],
+                 as_type: str) -> Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]:
+    """
+    Converts a DataFrame between Koalas, Pandas, PySpark, and PySpark.pandas.
 
-def data_convert(df, as_type: str):
+    :param df: The DataFrame to be converted.
+    :type df: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]
+    
+    :param as_type: The type of DataFrame to convert to.
+    :type as_type: str
+    
+    :return: The converted DataFrame.
+    :rtype: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]
+    """
     # Koalas
     if df_type(df) == KOALAS:
         if as_type.lower() == PANDAS:
             return df.to_pandas()  # Koalas to Pandas
         elif as_type.lower() in IN_PYSPARK:
             return df.to_spark()   # Koalas to Spark
         elif as_type.lower() in IN_PANDAS_ON_SPARK:
@@ -161,26 +207,52 @@
                     raise
         elif as_type.lower() in IN_PYSPARK:
             return df.to_spark()
         elif as_type.lower() in IN_PANDAS_ON_SPARK:
             return df
 
 
-def select(df, columns: List[str]):
-    if str(type(df)) == PANDAS_TYPES.get("df"):
+def select(df: Union[pandas.DataFrame, pyspark.sql.DataFrame, KoalasDataFrame], 
+           columns: List[str]) -> Union[pandas.DataFrame, pyspark.sql.DataFrame, KoalasDataFrame]:
+    """
+    Select columns from a DataFrame.
+
+    :param df: The DataFrame to select columns from.
+    :type df: Union[pandas.DataFrame, pyspark.sql.DataFrame, KoalasDataFrame]
+    :param columns: The columns to select.
+    :type columns: List[str]
+    :return: A new DataFrame with only the selected columns.
+    :rtype: Union[pandas.DataFrame, pyspark.sql.DataFrame, KoalasDataFrame]
+    """
+    if isinstance(df, pandas.DataFrame):
         return df[columns]
-    elif str(type(df)) == PYSPARK_TYPES.get("df"):
+    elif isinstance(df, pyspark.sql.DataFrame):
         return df.select(columns)
-    elif str(type(df)) == KOALAS_TYPES.get("df"):
-        return df[columns]
-    elif str(type(df)) == PANDAS_ON_SPARK_TYPES.get("df"):
+    elif isinstance(df, KoalasDataFrame):
         return df[columns]
+    else:
+        raise ValueError("Unsupported DataFrame type")
 
 
-def to_list(df, columns: List[str] = None):
+def to_list(df: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame, pandas.Series], 
+            columns: List[str] = None) -> Union[List[Any], List[List[Any]]]:
+    """
+    Convert a DataFrame or Series to a list. If the input is a DataFrame, the output is a list of lists (one for each
+    column), otherwise, the output is a flat list. The input DataFrame can be of type KoalasDataFrame, pandas.DataFrame,
+    pyspark.sql.DataFrame, pyspark.pandas.DataFrame, or pandas.Series.
+
+    :param df: DataFrame or Series to convert.
+    :type df: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame, pandas.Series]
+
+    :param columns: Optional list of column names to convert. If not specified, all columns are converted.
+    :type columns: List[str], optional
+
+    :return: A list or list of lists, depending on the input DataFrame type.
+    :rtype: Union[List[Any], List[List[Any]]]
+    """
     if str(type(df)) in [KOALAS_TYPES.get("series"), PANDAS_TYPES.get("series"), PYSPARK_TYPES.get("series"), PANDAS_ON_SPARK_TYPES.get("series")]:
         if str(type(df)) == KOALAS_TYPES.get("series"):
             return df.to_list()
         elif str(type(df)) == PANDAS_TYPES.get("series"):
             return df.to_list()
         elif str(type(df)) == PYSPARK_TYPES.get("series"):
             return df.rdd.flatMap(lambda x: x).collect()
@@ -195,16 +267,26 @@
             return df.select(columns).rdd.flatMap(lambda x: x).collect()
         elif str(type(df)) == KOALAS_TYPES.get("df"):
             return list(map(lambda column: df[column].to_list(), columns))
         elif str(type(df)) == PANDAS_ON_SPARK_TYPES.get("df"):
             return list(map(lambda column: df[column].to_list(), columns))
 
 
-def df_type(df):
+def df_type(df: Union[pandas.DataFrame, KoalasDataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]) -> str:
+    """
+    Determines the type of DataFrame object passed as an argument.
+
+    :param df: A pandas DataFrame, Koalas DataFrame, Spark DataFrame, or PandasOnSpark DataFrame object.
+    :type df: Union[pandas.DataFrame, databricks.koalas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]
+    
+    :return: A string representing the type of the input DataFrame.
+    :rtype: str
+    """
+
     if str(type(df)) == "<class 'pandas.core.frame.DataFrame'>":
         return PANDAS
     elif str(type(df)) == "<class 'pyspark.sql.dataframe.DataFrame'>":
         return PYSPARK
     elif str(type(df)) == "<class 'databricks.koalas.frame.DataFrame'>":
         return KOALAS
     elif str(type(df)) == "<class 'pyspark.pandas.frame.DataFrame'>":
-        return PANDAS_ON_SPARK
+        return PANDAS_ON_SPARK
```

### Comparing `hivecode-0.0.0.8.17/src/hivecode.egg-info/SOURCES.txt` & `hivecode-0.0.0.8.18/src/hivecode.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-LICENSE
-README.md
+README.rst
 pyproject.toml
+requirements.txt
 setup.cfg
 setup.py
 src/hiveadb/__init__.py
+src/hiveadb/eda.py
 src/hiveadb/function.py
 src/hiveadb/io.py
 src/hiveadb/py.typed
 src/hivecode.egg-info/PKG-INFO
 src/hivecode.egg-info/SOURCES.txt
 src/hivecode.egg-info/dependency_links.txt
 src/hivecode.egg-info/not-zip-safe
 src/hivecode.egg-info/requires.txt
 src/hivecode.egg-info/top_level.txt
 src/hivecore/__init__.py
 src/hivecore/constant.py
 src/hivecore/decorator.py
+src/hivecore/eda.py
 src/hivecore/function.py
 src/hivecore/pattern.py
+src/hivecore/preprocess.py
 src/hivecore/py.typed
-src/hiveform/__init__.py
-src/hiveform/preprocess.py
+src/hivecore/visual.py
 src/hivesignal/__init__.py
 src/hivesignal/analysis.py
+src/hivesignal/eda.py
 src/hivesignal/io.py
 src/hivesignal/py.typed
-src/hivesignal/transform.py
-src/hivesignal/visual.py
+src/hivesignal/transform.py
```

### Comparing `hivecode-0.0.0.8.17/src/hivecore/constant.py` & `hivecode-0.0.0.8.18/src/hivecore/constant.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,8 +76,9 @@
 000004b0: 7061 726b 2e70 616e 6461 732e 6672 616d  park.pandas.fram
 000004c0: 652e 4461 7461 4672 616d 6527 3e22 2c0d  e.DataFrame'>",.
 000004d0: 0a20 2020 2022 7365 7269 6573 223a 2022  .    "series": "
 000004e0: 3c63 6c61 7373 2027 7079 7370 6172 6b2e  <class 'pyspark.
 000004f0: 7061 6e64 6173 2e73 6572 6965 732e 5365  pandas.series.Se
 00000500: 7269 6573 273e 220d 0a7d 0d0a 0d0a 5053  ries'>"..}....PS
 00000510: 5f54 5950 4553 203d 2050 414e 4441 535f  _TYPES = PANDAS_
-00000520: 4f4e 5f53 5041 524b 5f54 5950 4553       ON_SPARK_TYPES
+00000520: 4f4e 5f53 5041 524b 5f54 5950 4553 0d0a  ON_SPARK_TYPES..
+00000530: 0d0a                                     ..
```

### Comparing `hivecode-0.0.0.8.17/src/hivecore/pattern.py` & `hivecode-0.0.0.8.18/src/hivecore/pattern.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-from hivecore.decorator import Singleton
+from hivecore.decorator import singleton
 from typing import Any
 
-@Singleton
+@singleton
 class Observer:
     """
-    An observer class. This type of class let's you to add attributes,
-    fetch their values and remove them dynamiclly. Quite useful to access
-    data inside a defined scope as it behaves as a Singleton.
+    An observer class. This type of class let's you to add attributes, fetch their values and remove them dynamiclly. Quite useful to access data inside a defined scope as it behaves as a Singleton.
     """
 
     def set(self, key: str, val: Any) -> None:
         """
-        Let's you add and overwrite atributes given the name and value.
-        You could also overwrite it by just accessing the value, but
-        that may not be recommended as later version may change attributes
-        to be encapsulated.
-
-        Args:
-            key (str): Name of the attribute to create/modify.
-            val (Any): Value of the attribute to create/modify.
+        Let's you add and overwrite attributes given the name and value. You could also overwrite it by just accessing the value, but that may not be recommended as later versions may change attributes to be encapsulated.
+
+        :param key: Name of the attribute to create/modify.
+        :type key: str
+
+        :param val: Value of the attribute to create/modify.
+        :type val: Any
+        
+        :return: None
+        :rtype: None
         """
         setattr(self, key, val)
 
     def get(self, key: str) -> Any:
         """
-        Let's you fetch data from the Observer. Current version let's you
-        access data directly, but later version may not support this, so
-        the use of this method is highly recommended.
-
-        Args:
-            key (str): Name of the attribute you want to fetch.
+        Let's you fetch data from the Observer. Current version lets you access data directly, but later versions may not support this, so the use of this method is highly recommended.
 
-        Returns:
-            Any: The value stored in the attribute.
+        :param key: Name of the attribute you want to fetch.
+        :type key: str
+        
+        :return: The value stored in the attribute.
+        :rtype: Any
         """
         return getattr(self, key)
 
     def delete(self, key: str) -> None:
         """
         Let's you remove data from the Observer.
 
-        Args:
-            key (str): Name of the attribute to remove.
+        :param key: Name of the attribute to remove.
+        :type key: str
+        
+        :return: None
+        :rtype: None
         """
         delattr(self, key)
```

### Comparing `hivecode-0.0.0.8.17/src/hiveform/preprocess.py` & `hivecode-0.0.0.8.18/src/hivecore/preprocess.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,26 +14,51 @@
 from pyspark.pandas import DataFrame as ps_DataFrame, from_pandas as ps_from_pandas
 
 # Pyspark
 from pyspark.sql import Window
 from pyspark.sql.types import StringType
 
 # Koalas
-from databricks.koalas import from_pandas
+from databricks.koalas import from_pandas, DataFrame as KoalasDataFrame
 
-from typing import List
+from typing import List, Union
 from os import system
 from pyspark.sql.functions import abs as sabs, max as smax, min as smin, mean as _mean, stddev as _stddev, count as scount, first, last
 from sklearn.metrics.pairwise import cosine_similarity as sk_cosine_similarity
 from sklearn.feature_extraction.text import CountVectorizer, TfidfVectorizer
 from pandas import DataFrame, concat
 from typing import List
 
+import pandas
+import pyspark
+import databricks.koalas
+
 ##### NUMERIC FUNCTIONS #####
-def normalize(df, columns: List[str] = None, method: str = "max-abs", overwrite: bool = False):
+def normalize(df: Union[pandas.DataFrame, databricks.koalas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame], 
+              columns: List[str] = None, 
+              method: str = "max-abs", 
+              overwrite: bool = False) -> Union[pandas.DataFrame, databricks.koalas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]:
+    """
+    Normalize the values in the specified columns of a DataFrame using a given normalization method.
+
+    :param df: A DataFrame object to normalize.
+    :type df: Union[pandas.DataFrame, databricks.koalas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]
+
+    :param columns: A list of column names to normalize. If None, normalize all columns.
+    :type columns: List[str]
+
+    :param method: The normalization method to use. Default is "max-abs".
+    :type method: str
+
+    :param overwrite: If True, overwrite the original values in the DataFrame with the normalized values.
+    :type overwrite: bool
+
+    :return: A DataFrame object with the normalized values. If overwrite is True, return the same DataFrame object.
+    :rtype: Union[pandas.DataFrame, databricks.koalas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]
+    """
     engine = df_type(df)
     method = method.lower()
     if engine == PANDAS or engine == KOALAS or engine == PANDAS_ON_SPARK:
         if not columns:
             s = df.apply(lambda s: to_numeric(s, errors='coerce').notnull().all())
             if engine == KOALAS or engine == PANDAS_ON_SPARK:
                 columns = list(s[s].index.to_numpy())
@@ -41,15 +66,14 @@
                 columns = list(s[s].index)
             
         if not isinstance(columns, list):
             columns = [columns]
             
         df = df.copy()
 
-        print(columns)
         if method in ["max_abs", "max-abs", "max abs", "maximum_absolute", "maximum-absolute","maximum absolute"]:
             for column in columns:
                 if overwrite:
                     df[column] = df[column]  / df[column].abs().max()
                 else:
                     df[f"{column}_norm"] = df[column]  / df[column].abs().max()
         elif method in ["min_max", "min-max", "min max"]:
@@ -91,15 +115,32 @@
                     df = df.withColumn(column, ((df[column] - (df.select(_mean(df[column]).alias("mean")).collect()[0]["mean"])) / (df.select(_stddev(df[column]).alias("std")).collect()[0]["std"])).alias(f"{column}_normalized"))
                 else:
                     df = df.withColumn(f"{column}_norm", ((df[column] - (df.select(_mean(df[column]).alias("mean")).collect()[0]["mean"])) / (df.select(_stddev(df[column]).alias("std")).collect()[0]["std"])).alias(f"{column}_normalized"))
 
     return df
 
 
-def replace_na(df, columns: List[str] = None, method: str = "mean"):
+def replace_nas(df: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame],
+                columns: List[str] = None, 
+                method: str = "mean") -> Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]:
+    """
+    Replace missing values (NAs) in the specified columns of a DataFrame with a specified method.
+
+    :param df: The DataFrame to replace NAs in.
+    :type df: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]
+
+    :param columns: The list of columns to replace NAs in. If None, all columns with NAs will be replaced.
+    :type columns: List[str]
+
+    :param method: The method to use for replacing NAs. Available methods are "mean", "median", "mode", "ffill", and "bfill".
+    :type method: str
+
+    :return: The DataFrame with NAs replaced according to the specified method.
+    :rtype: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]
+    """
     engine = df_type(df)
     if not columns:
         if engine == KOALAS or engine == PANDAS_ON_SPARK:
             s = df.apply(lambda s: to_numeric(s, errors='coerce').notnull().all())
             columns = list(set(list(s[s].index.to_numpy())))
             df = df.copy()
         elif engine == PANDAS:
@@ -204,15 +245,47 @@
             df = df.dropna()
         if engine == PYSPARK:
             df = df.na.drop()
     return df
 
 
 ##### TEXT FUNCTIONS #####
-def text_similarity(df, columns: List[str], method: str = "tfid", threshold: float = 0.95, overwrite: bool = False, engine: str = "cosine"):
+def text_similarity(
+    df: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame], 
+    columns: List[str], 
+    method: str = "tfid", 
+    threshold: float = 0.95, 
+    overwrite: bool = False, 
+    engine: str = "cosine"
+) -> Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]:
+    """
+    Compute the similarity between strings in the specified dataframe columns.
+
+    :param df: The dataframe whose columns will be used for computing text similarity.
+    :type df: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]
+
+    :param columns: The list of column names whose string values will be compared.
+    :type columns: List[str]
+
+    :param method: The method to use for computing text similarity. Possible values are "tfid" and "count".
+    :type method: str
+
+    :param threshold: The threshold above which two strings are considered similar. Should be a value between 0 and 1.
+    :type threshold: float
+
+    :param overwrite: If True, the original column values will be overwritten with the most similar ones.
+    :type overwrite: bool
+
+    :param engine: The similarity computation engine to use. Possible values are "cosine_similarity", "jaro",
+                   "levenshtein", "damerau_levenshtein", "jaro_winkler", and "hamming".
+    :type engine: str
+
+    :return: A dataframe with the similarity values between strings.
+    :rtype: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]
+    """
     def cosine_similarity(documents: List[str], header: bool = True, engine="tfid", i:int = 0):
         if engine == "count":
             count_vect = CountVectorizer()
             trsfm = count_vect.fit_transform(documents)
         elif engine == "tfid":
             vectorizer = TfidfVectorizer()
             trsfm=vectorizer.fit_transform(documents)
@@ -438,15 +511,40 @@
                     df.loc[df[col_name] == corpus, f"{col_name}_similarity"] = most_similar(_df, threshold=threshold)
         if len(df) == 1:
             return df[0]
         else:
             return df
 
 
-def encode(df, columns, encoder: str = "categorical", overwrite: bool = False, as_type: str = None):
+def encode(df: Union[pandas.DataFrame, KoalasDataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame], 
+           columns: List[str], 
+           encoder: str = "categorical", 
+           overwrite: bool = False,
+           as_type: str = None) -> Union[pandas.DataFrame, KoalasDataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]:
+    """
+    Encodes columns in a dataframe using various encoders.
+
+    :param df: A Pandas, Koalas, PySpark DataFrame or PySpark Koalas DataFrame to encode.
+    :type df: Union[pandas.DataFrame, KoalasDataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]
+
+    :param columns: The names of the columns to encode.
+    :type columns: List[str]
+
+    :param encoder: The encoding method to use, Possible values are "categorical" or "onehot". defaults to "categorical".
+    :type encoder: str, optional
+
+    :param overwrite: If True, overwrites the original columns with the encoded values, defaults to False.
+    :type overwrite: bool, optional
+
+    :param as_type: The data type to convert the encoded columns to, defaults to None.
+    :type as_type: str, optional
+
+    :return: A Pandas, Koalas, PySpark DataFrame or PySpark Koalas DataFrame with the encoded columns.
+    :rtype: Union[pandas.DataFrame, KoalasDataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]
+    """
     if not isinstance(columns, list):
         columns = [columns]
     
     engine = df_type(df)
     original_columns = df.columns
 
     df = data_convert(df, engine)
@@ -509,8 +607,8 @@
                 indexer = StringIndexer(inputCol=column, outputCol=f'{column}_encoded')
                 indexer_fitted = indexer.fit(df)
                 df = indexer_fitted.transform(df).withColumn(f"{column}_encoded",col(f"{column}_encoded").cast("int"))
                 df = encoder.fit(df).transform(df).drop(f'{column}_encoded')
     if as_type:
         return data_convert(df, as_type)
     else:
-        return data_convert(df, engine)
+        return data_convert(df, engine)
```

### Comparing `hivecode-0.0.0.8.17/src/hivesignal/analysis.py` & `hivecode-0.0.0.8.18/src/hivesignal/analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pandas import DataFrame
 
 
-def nauca(df, NORMAL_FREQ_MIN: float, NORMAL_FREQ_MAX: float, amplitude_col: str = "amplitude", frequency_col: str = "frequency", alpha: float = 0.1, method: str = "amp", return_mode: str = "nauca"):
+def nauca(df, NORMAL_FREQ_MIN: float, NORMAL_FREQ_MAX: float, amplitude_col: str = "amplitud", frequency_col: str = "frequency", alpha: float = 0.1, method: str = "amp", return_mode: str = "nauca"):
     # AOC
     df = DataFrame({"frecuencia": df[frequency_col], "indicador": df[amplitude_col]})
     df["indicador"] = (df.indicador - df.indicador.min())/(df.indicador.max() - df.indicador.min())
 
     AUC = df.indicador.sum()
     MODE = df.loc[df.indicador == df.indicador.max(), "frecuencia"].to_list()[0]
```

### Comparing `hivecode-0.0.0.8.17/src/hivesignal/io.py` & `hivecode-0.0.0.8.18/src/hivesignal/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,13 +36,13 @@
     df_digital = concat(df_digital, axis = 1)
     df_digital.set_index("time", inplace=True)
     
     if return_mode == "analog":
         return df_analog
     elif return_mode == "digital":
         return df_digital
-    elif return_mode == "signals" or return_mode == "signal":
+    elif return_mode == "signals":
         return df_analog, df_digital
     elif return_mode == "all":
         return df_analog, df_digital, {"station_name": rec.station_name, "frequency": rec.frequency, "start_timestamp": rec.start_timestamp, "trigger_timestamp": rec.trigger_timestamp, "timestep": timestep}
     else:
         raise Exception(f"Parameter return_mode only accepts 'analog', 'digital' or 'all', but '' was given.")
```

### Comparing `hivecode-0.0.0.8.17/src/hivesignal/transform.py` & `hivecode-0.0.0.8.18/src/hivesignal/transform.py`

 * *Files identical despite different names*

