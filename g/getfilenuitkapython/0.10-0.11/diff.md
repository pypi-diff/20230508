# Comparing `tmp/getfilenuitkapython-0.10.tar.gz` & `tmp/getfilenuitkapython-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getfilenuitkapython-0.10.tar", last modified: Mon May  8 01:50:41 2023, max compression
+gzip compressed data, was "getfilenuitkapython-0.11.tar", last modified: Mon May  8 05:12:08 2023, max compression
```

## Comparing `getfilenuitkapython-0.10.tar` & `getfilenuitkapython-0.11.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 01:50:41.550441 getfilenuitkapython-0.10/
--rw-rw-rw-   0        0        0     1148 2023-05-08 01:50:37.000000 getfilenuitkapython-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      165 2023-05-08 01:50:36.000000 getfilenuitkapython-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     2638 2023-05-08 01:50:41.550441 getfilenuitkapython-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     1954 2023-05-08 01:48:00.000000 getfilenuitkapython-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 01:50:41.547454 getfilenuitkapython-0.10/getfilenuitkapython/
--rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 getfilenuitkapython-0.10/getfilenuitkapython/LICENSE
--rw-rw-rw-   0        0        0     1954 2023-05-08 01:48:00.000000 getfilenuitkapython-0.10/getfilenuitkapython/README.md
--rw-rw-rw-   0        0        0     1711 2023-05-08 01:48:58.000000 getfilenuitkapython-0.10/getfilenuitkapython/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-08 01:50:40.000000 getfilenuitkapython-0.10/getfilenuitkapython/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-05-08 01:50:40.000000 getfilenuitkapython-0.10/getfilenuitkapython/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-05-08 01:50:41.549443 getfilenuitkapython-0.10/getfilenuitkapython.egg-info/
--rw-rw-rw-   0        0        0     2638 2023-05-08 01:50:41.000000 getfilenuitkapython-0.10/getfilenuitkapython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-05-08 01:50:41.000000 getfilenuitkapython-0.10/getfilenuitkapython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 01:50:41.000000 getfilenuitkapython-0.10/getfilenuitkapython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-08 01:50:41.000000 getfilenuitkapython-0.10/getfilenuitkapython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-05-08 01:50:41.550987 getfilenuitkapython-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1335 2023-05-08 01:50:40.000000 getfilenuitkapython-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 05:12:08.345006 getfilenuitkapython-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-05-08 05:12:01.000000 getfilenuitkapython-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      128 2023-05-08 05:12:00.000000 getfilenuitkapython-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     2697 2023-05-08 05:12:08.346003 getfilenuitkapython-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     2013 2023-05-08 05:10:46.000000 getfilenuitkapython-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 05:12:08.342014 getfilenuitkapython-0.11/getfilenuitkapython/
+-rw-rw-rw-   0        0        0     2013 2023-05-08 05:10:46.000000 getfilenuitkapython-0.11/getfilenuitkapython/README.md
+-rw-rw-rw-   0        0        0     2913 2023-05-08 05:09:24.000000 getfilenuitkapython-0.11/getfilenuitkapython/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-08 05:12:07.000000 getfilenuitkapython-0.11/getfilenuitkapython/requirements.txt
+-rw-rw-rw-   0        0        0     2515 2023-05-08 05:12:07.000000 getfilenuitkapython-0.11/getfilenuitkapython/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-05-08 05:12:08.345006 getfilenuitkapython-0.11/getfilenuitkapython.egg-info/
+-rw-rw-rw-   0        0        0     2697 2023-05-08 05:12:08.000000 getfilenuitkapython-0.11/getfilenuitkapython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2023-05-08 05:12:08.000000 getfilenuitkapython-0.11/getfilenuitkapython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 05:12:08.000000 getfilenuitkapython-0.11/getfilenuitkapython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 05:12:08.000000 getfilenuitkapython-0.11/getfilenuitkapython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-08 05:12:08.000000 getfilenuitkapython-0.11/getfilenuitkapython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-08 05:12:08.346003 getfilenuitkapython-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1427 2023-05-08 05:12:07.000000 getfilenuitkapython-0.11/setup.py
```

### Comparing `getfilenuitkapython-0.10/LICENSE.rst` & `getfilenuitkapython-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `getfilenuitkapython-0.10/PKG-INFO` & `getfilenuitkapython-0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getfilenuitkapython
-Version: 0.10
+Version: 0.11
 Summary: A function that locates files in python environments and compiled exe files (Nuitka)
 Home-page: https://github.com/hansalemaos/getfilenuitkapython
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: nuitka,locate,files
 Classifier: Development Status :: 4 - Beta
@@ -41,14 +41,16 @@
 
 1. The directory containing the script that was invoked from the command line.
 2. The directory containing the current module file (__file__).
 3. The parent directory of the directory containing the script that was invoked from the command line.
 4. The parent directory of the directory containing the current module file (__file__).
 5. The directory containing the calling function (sys._getframe(1)).
 6. The parent directory of the directory containing the calling function.
+7. Search in PATH
+8. Search in every folder in basedirs 
 
 If the file is found in any of these locations, the function returns the full path to the file. If the file is not found in any of these locations, the function returns the filename itself.
 
 
 from getfilenuitkapython import get_filepath
 get_filepath('pythonw.exe')
 Out[3]: 'C:\\ProgramData\\anaconda3\\envs\\dfdir\\pythonw.exe'
```

### Comparing `getfilenuitkapython-0.10/README.md` & `getfilenuitkapython-0.11/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 
 1. The directory containing the script that was invoked from the command line.
 2. The directory containing the current module file (__file__).
 3. The parent directory of the directory containing the script that was invoked from the command line.
 4. The parent directory of the directory containing the current module file (__file__).
 5. The directory containing the calling function (sys._getframe(1)).
 6. The parent directory of the directory containing the calling function.
+7. Search in PATH
+8. Search in every folder in basedirs 
 
 If the file is found in any of these locations, the function returns the full path to the file. If the file is not found in any of these locations, the function returns the filename itself.
 
 
 from getfilenuitkapython import get_filepath
 get_filepath('pythonw.exe')
 Out[3]: 'C:\\ProgramData\\anaconda3\\envs\\dfdir\\pythonw.exe'
```

### Comparing `getfilenuitkapython-0.10/getfilenuitkapython/LICENSE` & `getfilenuitkapython-0.11/getfilenuitkapython/thirdparty.json`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,158 @@
-00000000: 0d0d 0a20 5468 6520 4d49 5420 4c69 6365  ... The MIT Lice
-00000010: 6e73 6520 284d 4954 290d 0d0a 2043 6f70  nse (MIT)... Cop
-00000020: 7972 6967 6874 2028 6329 2032 3032 3320  yright (c) 2023 
-00000030: 4a6f 6861 6e6e 6573 2046 6973 6368 6572  Johannes Fischer
-00000040: 0d0d 0a20 0d0d 0a20 5065 726d 6973 7369  ... ... Permissi
-00000050: 6f6e 2069 7320 6865 7265 6279 2067 7261  on is hereby gra
-00000060: 6e74 6564 2c20 6672 6565 206f 6620 6368  nted, free of ch
-00000070: 6172 6765 2c20 746f 2061 6e79 2070 6572  arge, to any per
-00000080: 736f 6e20 6f62 7461 696e 696e 6720 6120  son obtaining a 
-00000090: 636f 7079 0d0d 0a20 6f66 2074 6869 7320  copy... of this 
-000000a0: 736f 6674 7761 7265 2061 6e64 2061 7373  software and ass
-000000b0: 6f63 6961 7465 6420 646f 6375 6d65 6e74  ociated document
-000000c0: 6174 696f 6e20 6669 6c65 7320 2874 6865  ation files (the
-000000d0: 2022 536f 6674 7761 7265 2229 2c20 746f   "Software"), to
-000000e0: 2064 6561 6c0d 0d0a 2069 6e20 7468 6520   deal... in the 
-000000f0: 536f 6674 7761 7265 2077 6974 686f 7574  Software without
-00000100: 2072 6573 7472 6963 7469 6f6e 2c20 696e   restriction, in
-00000110: 636c 7564 696e 6720 7769 7468 6f75 7420  cluding without 
-00000120: 6c69 6d69 7461 7469 6f6e 2074 6865 2072  limitation the r
-00000130: 6967 6874 730d 0d0a 2074 6f20 7573 652c  ights... to use,
-00000140: 2063 6f70 792c 206d 6f64 6966 792c 206d   copy, modify, m
-00000150: 6572 6765 2c20 7075 626c 6973 682c 2064  erge, publish, d
-00000160: 6973 7472 6962 7574 652c 2073 7562 6c69  istribute, subli
-00000170: 6365 6e73 652c 2061 6e64 2f6f 7220 7365  cense, and/or se
-00000180: 6c6c 0d0d 0a20 636f 7069 6573 206f 6620  ll... copies of 
-00000190: 7468 6520 536f 6674 7761 7265 2c20 616e  the Software, an
-000001a0: 6420 746f 2070 6572 6d69 7420 7065 7273  d to permit pers
-000001b0: 6f6e 7320 746f 2077 686f 6d20 7468 6520  ons to whom the 
-000001c0: 536f 6674 7761 7265 2069 730d 0d0a 2066  Software is... f
-000001d0: 7572 6e69 7368 6564 2074 6f20 646f 2073  urnished to do s
-000001e0: 6f2c 2073 7562 6a65 6374 2074 6f20 7468  o, subject to th
-000001f0: 6520 666f 6c6c 6f77 696e 6720 636f 6e64  e following cond
-00000200: 6974 696f 6e73 3a0d 0d0a 200d 0d0a 2054  itions:... ... T
-00000210: 6865 2061 626f 7665 2063 6f70 7972 6967  he above copyrig
-00000220: 6874 206e 6f74 6963 6520 616e 6420 7468  ht notice and th
-00000230: 6973 2070 6572 6d69 7373 696f 6e20 6e6f  is permission no
-00000240: 7469 6365 2073 6861 6c6c 2062 6520 696e  tice shall be in
-00000250: 636c 7564 6564 2069 6e20 616c 6c0d 0d0a  cluded in all...
-00000260: 2063 6f70 6965 7320 6f72 2073 7562 7374   copies or subst
-00000270: 616e 7469 616c 2070 6f72 7469 6f6e 7320  antial portions 
-00000280: 6f66 2074 6865 2053 6f66 7477 6172 652e  of the Software.
-00000290: 0d0d 0a20 0d0d 0a20 5448 4520 534f 4654  ... ... THE SOFT
-000002a0: 5741 5245 2049 5320 5052 4f56 4944 4544  WARE IS PROVIDED
-000002b0: 2022 4153 2049 5322 2c20 5749 5448 4f55   "AS IS", WITHOU
-000002c0: 5420 5741 5252 414e 5459 204f 4620 414e  T WARRANTY OF AN
-000002d0: 5920 4b49 4e44 2c0d 0d0a 2045 5850 5245  Y KIND,... EXPRE
-000002e0: 5353 204f 5220 494d 504c 4945 442c 2049  SS OR IMPLIED, I
-000002f0: 4e43 4c55 4449 4e47 2042 5554 204e 4f54  NCLUDING BUT NOT
-00000300: 204c 494d 4954 4544 2054 4f20 5448 4520   LIMITED TO THE 
-00000310: 5741 5252 414e 5449 4553 204f 460d 0d0a  WARRANTIES OF...
-00000320: 204d 4552 4348 414e 5441 4249 4c49 5459   MERCHANTABILITY
-00000330: 2c20 4649 544e 4553 5320 464f 5220 4120  , FITNESS FOR A 
-00000340: 5041 5254 4943 554c 4152 2050 5552 504f  PARTICULAR PURPO
-00000350: 5345 2041 4e44 204e 4f4e 494e 4652 494e  SE AND NONINFRIN
-00000360: 4745 4d45 4e54 2e0d 0d0a 2049 4e20 4e4f  GEMENT.... IN NO
-00000370: 2045 5645 4e54 2053 4841 4c4c 2054 4845   EVENT SHALL THE
-00000380: 2041 5554 484f 5253 204f 5220 434f 5059   AUTHORS OR COPY
-00000390: 5249 4748 5420 484f 4c44 4552 5320 4245  RIGHT HOLDERS BE
-000003a0: 204c 4941 424c 4520 464f 5220 414e 5920   LIABLE FOR ANY 
-000003b0: 434c 4149 4d2c 0d0d 0a20 4441 4d41 4745  CLAIM,... DAMAGE
-000003c0: 5320 4f52 204f 5448 4552 204c 4941 4249  S OR OTHER LIABI
-000003d0: 4c49 5459 2c20 5748 4554 4845 5220 494e  LITY, WHETHER IN
-000003e0: 2041 4e20 4143 5449 4f4e 204f 4620 434f   AN ACTION OF CO
-000003f0: 4e54 5241 4354 2c20 544f 5254 204f 520d  NTRACT, TORT OR.
-00000400: 0d0a 204f 5448 4552 5749 5345 2c20 4152  .. OTHERWISE, AR
-00000410: 4953 494e 4720 4652 4f4d 2c20 4f55 5420  ISING FROM, OUT 
-00000420: 4f46 204f 5220 494e 2043 4f4e 4e45 4354  OF OR IN CONNECT
-00000430: 494f 4e20 5749 5448 2054 4845 2053 4f46  ION WITH THE SOF
-00000440: 5457 4152 4520 4f52 2054 4845 2055 5345  TWARE OR THE USE
-00000450: 0d0d 0a20 4f52 204f 5448 4552 2044 4541  ... OR OTHER DEA
-00000460: 4c49 4e47 5320 494e 2054 4845 2053 4f46  LINGS IN THE SOF
-00000470: 5457 4152 452e 0d0d 0a0d 0d0a            TWARE.......
+00000000: 5b7b 224c 6963 656e 7365 223a 224d 4954  [{"License":"MIT
+00000010: 222c 224c 6963 656e 7365 5465 7874 223a  ","LicenseText":
+00000020: 225c 6e5c 6e20 5468 6520 4d49 5420 4c69  "\n\n The MIT Li
+00000030: 6365 6e73 6520 284d 4954 295c 6e5c 6e20  cense (MIT)\n\n 
+00000040: 436f 7079 7269 6768 7420 2863 2920 3230  Copyright (c) 20
+00000050: 3233 204a 6f68 616e 6e65 7320 4669 7363  23 Johannes Fisc
+00000060: 6865 725c 6e5c 6e20 5c6e 5c6e 2050 6572  her\n\n \n\n Per
+00000070: 6d69 7373 696f 6e20 6973 2068 6572 6562  mission is hereb
+00000080: 7920 6772 616e 7465 642c 2066 7265 6520  y granted, free 
+00000090: 6f66 2063 6861 7267 652c 2074 6f20 616e  of charge, to an
+000000a0: 7920 7065 7273 6f6e 206f 6274 6169 6e69  y person obtaini
+000000b0: 6e67 2061 2063 6f70 795c 6e5c 6e20 6f66  ng a copy\n\n of
+000000c0: 2074 6869 7320 736f 6674 7761 7265 2061   this software a
+000000d0: 6e64 2061 7373 6f63 6961 7465 6420 646f  nd associated do
+000000e0: 6375 6d65 6e74 6174 696f 6e20 6669 6c65  cumentation file
+000000f0: 7320 2874 6865 205c 2253 6f66 7477 6172  s (the \"Softwar
+00000100: 655c 2229 2c20 746f 2064 6561 6c5c 6e5c  e\"), to deal\n\
+00000110: 6e20 696e 2074 6865 2053 6f66 7477 6172  n in the Softwar
+00000120: 6520 7769 7468 6f75 7420 7265 7374 7269  e without restri
+00000130: 6374 696f 6e2c 2069 6e63 6c75 6469 6e67  ction, including
+00000140: 2077 6974 686f 7574 206c 696d 6974 6174   without limitat
+00000150: 696f 6e20 7468 6520 7269 6768 7473 5c6e  ion the rights\n
+00000160: 5c6e 2074 6f20 7573 652c 2063 6f70 792c  \n to use, copy,
+00000170: 206d 6f64 6966 792c 206d 6572 6765 2c20   modify, merge, 
+00000180: 7075 626c 6973 682c 2064 6973 7472 6962  publish, distrib
+00000190: 7574 652c 2073 7562 6c69 6365 6e73 652c  ute, sublicense,
+000001a0: 2061 6e64 5c2f 6f72 2073 656c 6c5c 6e5c   and\/or sell\n\
+000001b0: 6e20 636f 7069 6573 206f 6620 7468 6520  n copies of the 
+000001c0: 536f 6674 7761 7265 2c20 616e 6420 746f  Software, and to
+000001d0: 2070 6572 6d69 7420 7065 7273 6f6e 7320   permit persons 
+000001e0: 746f 2077 686f 6d20 7468 6520 536f 6674  to whom the Soft
+000001f0: 7761 7265 2069 735c 6e5c 6e20 6675 726e  ware is\n\n furn
+00000200: 6973 6865 6420 746f 2064 6f20 736f 2c20  ished to do so, 
+00000210: 7375 626a 6563 7420 746f 2074 6865 2066  subject to the f
+00000220: 6f6c 6c6f 7769 6e67 2063 6f6e 6469 7469  ollowing conditi
+00000230: 6f6e 733a 5c6e 5c6e 205c 6e5c 6e20 5468  ons:\n\n \n\n Th
+00000240: 6520 6162 6f76 6520 636f 7079 7269 6768  e above copyrigh
+00000250: 7420 6e6f 7469 6365 2061 6e64 2074 6869  t notice and thi
+00000260: 7320 7065 726d 6973 7369 6f6e 206e 6f74  s permission not
+00000270: 6963 6520 7368 616c 6c20 6265 2069 6e63  ice shall be inc
+00000280: 6c75 6465 6420 696e 2061 6c6c 5c6e 5c6e  luded in all\n\n
+00000290: 2063 6f70 6965 7320 6f72 2073 7562 7374   copies or subst
+000002a0: 616e 7469 616c 2070 6f72 7469 6f6e 7320  antial portions 
+000002b0: 6f66 2074 6865 2053 6f66 7477 6172 652e  of the Software.
+000002c0: 5c6e 5c6e 205c 6e5c 6e20 5448 4520 534f  \n\n \n\n THE SO
+000002d0: 4654 5741 5245 2049 5320 5052 4f56 4944  FTWARE IS PROVID
+000002e0: 4544 205c 2241 5320 4953 5c22 2c20 5749  ED \"AS IS\", WI
+000002f0: 5448 4f55 5420 5741 5252 414e 5459 204f  THOUT WARRANTY O
+00000300: 4620 414e 5920 4b49 4e44 2c5c 6e5c 6e20  F ANY KIND,\n\n 
+00000310: 4558 5052 4553 5320 4f52 2049 4d50 4c49  EXPRESS OR IMPLI
+00000320: 4544 2c20 494e 434c 5544 494e 4720 4255  ED, INCLUDING BU
+00000330: 5420 4e4f 5420 4c49 4d49 5445 4420 544f  T NOT LIMITED TO
+00000340: 2054 4845 2057 4152 5241 4e54 4945 5320   THE WARRANTIES 
+00000350: 4f46 5c6e 5c6e 204d 4552 4348 414e 5441  OF\n\n MERCHANTA
+00000360: 4249 4c49 5459 2c20 4649 544e 4553 5320  BILITY, FITNESS 
+00000370: 464f 5220 4120 5041 5254 4943 554c 4152  FOR A PARTICULAR
+00000380: 2050 5552 504f 5345 2041 4e44 204e 4f4e   PURPOSE AND NON
+00000390: 494e 4652 494e 4745 4d45 4e54 2e5c 6e5c  INFRINGEMENT.\n\
+000003a0: 6e20 494e 204e 4f20 4556 454e 5420 5348  n IN NO EVENT SH
+000003b0: 414c 4c20 5448 4520 4155 5448 4f52 5320  ALL THE AUTHORS 
+000003c0: 4f52 2043 4f50 5952 4947 4854 2048 4f4c  OR COPYRIGHT HOL
+000003d0: 4445 5253 2042 4520 4c49 4142 4c45 2046  DERS BE LIABLE F
+000003e0: 4f52 2041 4e59 2043 4c41 494d 2c5c 6e5c  OR ANY CLAIM,\n\
+000003f0: 6e20 4441 4d41 4745 5320 4f52 204f 5448  n DAMAGES OR OTH
+00000400: 4552 204c 4941 4249 4c49 5459 2c20 5748  ER LIABILITY, WH
+00000410: 4554 4845 5220 494e 2041 4e20 4143 5449  ETHER IN AN ACTI
+00000420: 4f4e 204f 4620 434f 4e54 5241 4354 2c20  ON OF CONTRACT, 
+00000430: 544f 5254 204f 525c 6e5c 6e20 4f54 4845  TORT OR\n\n OTHE
+00000440: 5257 4953 452c 2041 5249 5349 4e47 2046  RWISE, ARISING F
+00000450: 524f 4d2c 204f 5554 204f 4620 4f52 2049  ROM, OUT OF OR I
+00000460: 4e20 434f 4e4e 4543 5449 4f4e 2057 4954  N CONNECTION WIT
+00000470: 4820 5448 4520 534f 4654 5741 5245 204f  H THE SOFTWARE O
+00000480: 5220 5448 4520 5553 455c 6e5c 6e20 4f52  R THE USE\n\n OR
+00000490: 204f 5448 4552 2044 4541 4c49 4e47 5320   OTHER DEALINGS 
+000004a0: 494e 2054 4845 2053 4f46 5457 4152 452e  IN THE SOFTWARE.
+000004b0: 5c6e 5c6e 5c6e 5c6e 222c 224e 616d 6522  \n\n\n\n","Name"
+000004c0: 3a22 6c69 7374 2d61 6c6c 2d66 696c 6573  :"list-all-files
+000004d0: 2d72 6563 7572 7369 7665 6c79 222c 2256  -recursively","V
+000004e0: 6572 7369 6f6e 223a 2230 2e31 3222 7d2c  ersion":"0.12"},
+000004f0: 7b22 4c69 6365 6e73 6522 3a22 4d49 5422  {"License":"MIT"
+00000500: 2c22 4c69 6365 6e73 6554 6578 7422 3a22  ,"LicenseText":"
+00000510: 5c6e 5c6e 2054 6865 204d 4954 204c 6963  \n\n The MIT Lic
+00000520: 656e 7365 2028 4d49 5429 5c6e 5c6e 2043  ense (MIT)\n\n C
+00000530: 6f70 7972 6967 6874 2028 6329 2032 3032  opyright (c) 202
+00000540: 3320 4a6f 6861 6e6e 6573 2046 6973 6368  3 Johannes Fisch
+00000550: 6572 5c6e 5c6e 205c 6e5c 6e20 5065 726d  er\n\n \n\n Perm
+00000560: 6973 7369 6f6e 2069 7320 6865 7265 6279  ission is hereby
+00000570: 2067 7261 6e74 6564 2c20 6672 6565 206f   granted, free o
+00000580: 6620 6368 6172 6765 2c20 746f 2061 6e79  f charge, to any
+00000590: 2070 6572 736f 6e20 6f62 7461 696e 696e   person obtainin
+000005a0: 6720 6120 636f 7079 5c6e 5c6e 206f 6620  g a copy\n\n of 
+000005b0: 7468 6973 2073 6f66 7477 6172 6520 616e  this software an
+000005c0: 6420 6173 736f 6369 6174 6564 2064 6f63  d associated doc
+000005d0: 756d 656e 7461 7469 6f6e 2066 696c 6573  umentation files
+000005e0: 2028 7468 6520 5c22 536f 6674 7761 7265   (the \"Software
+000005f0: 5c22 292c 2074 6f20 6465 616c 5c6e 5c6e  \"), to deal\n\n
+00000600: 2069 6e20 7468 6520 536f 6674 7761 7265   in the Software
+00000610: 2077 6974 686f 7574 2072 6573 7472 6963   without restric
+00000620: 7469 6f6e 2c20 696e 636c 7564 696e 6720  tion, including 
+00000630: 7769 7468 6f75 7420 6c69 6d69 7461 7469  without limitati
+00000640: 6f6e 2074 6865 2072 6967 6874 735c 6e5c  on the rights\n\
+00000650: 6e20 746f 2075 7365 2c20 636f 7079 2c20  n to use, copy, 
+00000660: 6d6f 6469 6679 2c20 6d65 7267 652c 2070  modify, merge, p
+00000670: 7562 6c69 7368 2c20 6469 7374 7269 6275  ublish, distribu
+00000680: 7465 2c20 7375 626c 6963 656e 7365 2c20  te, sublicense, 
+00000690: 616e 645c 2f6f 7220 7365 6c6c 5c6e 5c6e  and\/or sell\n\n
+000006a0: 2063 6f70 6965 7320 6f66 2074 6865 2053   copies of the S
+000006b0: 6f66 7477 6172 652c 2061 6e64 2074 6f20  oftware, and to 
+000006c0: 7065 726d 6974 2070 6572 736f 6e73 2074  permit persons t
+000006d0: 6f20 7768 6f6d 2074 6865 2053 6f66 7477  o whom the Softw
+000006e0: 6172 6520 6973 5c6e 5c6e 2066 7572 6e69  are is\n\n furni
+000006f0: 7368 6564 2074 6f20 646f 2073 6f2c 2073  shed to do so, s
+00000700: 7562 6a65 6374 2074 6f20 7468 6520 666f  ubject to the fo
+00000710: 6c6c 6f77 696e 6720 636f 6e64 6974 696f  llowing conditio
+00000720: 6e73 3a5c 6e5c 6e20 5c6e 5c6e 2054 6865  ns:\n\n \n\n The
+00000730: 2061 626f 7665 2063 6f70 7972 6967 6874   above copyright
+00000740: 206e 6f74 6963 6520 616e 6420 7468 6973   notice and this
+00000750: 2070 6572 6d69 7373 696f 6e20 6e6f 7469   permission noti
+00000760: 6365 2073 6861 6c6c 2062 6520 696e 636c  ce shall be incl
+00000770: 7564 6564 2069 6e20 616c 6c5c 6e5c 6e20  uded in all\n\n 
+00000780: 636f 7069 6573 206f 7220 7375 6273 7461  copies or substa
+00000790: 6e74 6961 6c20 706f 7274 696f 6e73 206f  ntial portions o
+000007a0: 6620 7468 6520 536f 6674 7761 7265 2e5c  f the Software.\
+000007b0: 6e5c 6e20 5c6e 5c6e 2054 4845 2053 4f46  n\n \n\n THE SOF
+000007c0: 5457 4152 4520 4953 2050 524f 5649 4445  TWARE IS PROVIDE
+000007d0: 4420 5c22 4153 2049 535c 222c 2057 4954  D \"AS IS\", WIT
+000007e0: 484f 5554 2057 4152 5241 4e54 5920 4f46  HOUT WARRANTY OF
+000007f0: 2041 4e59 204b 494e 442c 5c6e 5c6e 2045   ANY KIND,\n\n E
+00000800: 5850 5245 5353 204f 5220 494d 504c 4945  XPRESS OR IMPLIE
+00000810: 442c 2049 4e43 4c55 4449 4e47 2042 5554  D, INCLUDING BUT
+00000820: 204e 4f54 204c 494d 4954 4544 2054 4f20   NOT LIMITED TO 
+00000830: 5448 4520 5741 5252 414e 5449 4553 204f  THE WARRANTIES O
+00000840: 465c 6e5c 6e20 4d45 5243 4841 4e54 4142  F\n\n MERCHANTAB
+00000850: 494c 4954 592c 2046 4954 4e45 5353 2046  ILITY, FITNESS F
+00000860: 4f52 2041 2050 4152 5449 4355 4c41 5220  OR A PARTICULAR 
+00000870: 5055 5250 4f53 4520 414e 4420 4e4f 4e49  PURPOSE AND NONI
+00000880: 4e46 5249 4e47 454d 454e 542e 5c6e 5c6e  NFRINGEMENT.\n\n
+00000890: 2049 4e20 4e4f 2045 5645 4e54 2053 4841   IN NO EVENT SHA
+000008a0: 4c4c 2054 4845 2041 5554 484f 5253 204f  LL THE AUTHORS O
+000008b0: 5220 434f 5059 5249 4748 5420 484f 4c44  R COPYRIGHT HOLD
+000008c0: 4552 5320 4245 204c 4941 424c 4520 464f  ERS BE LIABLE FO
+000008d0: 5220 414e 5920 434c 4149 4d2c 5c6e 5c6e  R ANY CLAIM,\n\n
+000008e0: 2044 414d 4147 4553 204f 5220 4f54 4845   DAMAGES OR OTHE
+000008f0: 5220 4c49 4142 494c 4954 592c 2057 4845  R LIABILITY, WHE
+00000900: 5448 4552 2049 4e20 414e 2041 4354 494f  THER IN AN ACTIO
+00000910: 4e20 4f46 2043 4f4e 5452 4143 542c 2054  N OF CONTRACT, T
+00000920: 4f52 5420 4f52 5c6e 5c6e 204f 5448 4552  ORT OR\n\n OTHER
+00000930: 5749 5345 2c20 4152 4953 494e 4720 4652  WISE, ARISING FR
+00000940: 4f4d 2c20 4f55 5420 4f46 204f 5220 494e  OM, OUT OF OR IN
+00000950: 2043 4f4e 4e45 4354 494f 4e20 5749 5448   CONNECTION WITH
+00000960: 2054 4845 2053 4f46 5457 4152 4520 4f52   THE SOFTWARE OR
+00000970: 2054 4845 2055 5345 5c6e 5c6e 204f 5220   THE USE\n\n OR 
+00000980: 4f54 4845 5220 4445 414c 494e 4753 2049  OTHER DEALINGS I
+00000990: 4e20 5448 4520 534f 4654 5741 5245 2e5c  N THE SOFTWARE.\
+000009a0: 6e5c 6e5c 6e5c 6e22 2c22 4e61 6d65 223a  n\n\n\n","Name":
+000009b0: 2273 686c 6578 7768 6963 6870 6c75 7322  "shlexwhichplus"
+000009c0: 2c22 5665 7273 696f 6e22 3a22 302e 3130  ,"Version":"0.10
+000009d0: 227d 5d                                  "}]
```

### Comparing `getfilenuitkapython-0.10/getfilenuitkapython/README.md` & `getfilenuitkapython-0.11/getfilenuitkapython/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 
 1. The directory containing the script that was invoked from the command line.
 2. The directory containing the current module file (__file__).
 3. The parent directory of the directory containing the script that was invoked from the command line.
 4. The parent directory of the directory containing the current module file (__file__).
 5. The directory containing the calling function (sys._getframe(1)).
 6. The parent directory of the directory containing the calling function.
+7. Search in PATH
+8. Search in every folder in basedirs 
 
 If the file is found in any of these locations, the function returns the full path to the file. If the file is not found in any of these locations, the function returns the filename itself.
 
 
 from getfilenuitkapython import get_filepath
 get_filepath('pythonw.exe')
 Out[3]: 'C:\\ProgramData\\anaconda3\\envs\\dfdir\\pythonw.exe'
```

### Comparing `getfilenuitkapython-0.10/getfilenuitkapython.egg-info/PKG-INFO` & `getfilenuitkapython-0.11/getfilenuitkapython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getfilenuitkapython
-Version: 0.10
+Version: 0.11
 Summary: A function that locates files in python environments and compiled exe files (Nuitka)
 Home-page: https://github.com/hansalemaos/getfilenuitkapython
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: nuitka,locate,files
 Classifier: Development Status :: 4 - Beta
@@ -41,14 +41,16 @@
 
 1. The directory containing the script that was invoked from the command line.
 2. The directory containing the current module file (__file__).
 3. The parent directory of the directory containing the script that was invoked from the command line.
 4. The parent directory of the directory containing the current module file (__file__).
 5. The directory containing the calling function (sys._getframe(1)).
 6. The parent directory of the directory containing the calling function.
+7. Search in PATH
+8. Search in every folder in basedirs 
 
 If the file is found in any of these locations, the function returns the full path to the file. If the file is not found in any of these locations, the function returns the filename itself.
 
 
 from getfilenuitkapython import get_filepath
 get_filepath('pythonw.exe')
 Out[3]: 'C:\\ProgramData\\anaconda3\\envs\\dfdir\\pythonw.exe'
```

### Comparing `getfilenuitkapython-0.10/setup.py` & `getfilenuitkapython-0.11/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''A function that locates files in python environments and compiled exe files (Nuitka)'''
 
 # Setting up
 setup(
     name="getfilenuitkapython",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/getfilenuitkapython',
     author="Johannes Fischer",
     author_email="aulasparticularesdealemaosp@gmail.com",
     description=DESCRIPTION,
 long_description = long_description,
 long_description_content_type="text/markdown",
-    #packages=[],
+    #packages=['list_all_files_recursively', 'shlexwhichplus'],
     keywords=['nuitka', 'locate', 'files'],
     classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
-    install_requires=[],
+    install_requires=['list_all_files_recursively', 'shlexwhichplus'],
     include_package_data=True
 )
 #python setup.py sdist bdist_wheel
 #twine upload dist/*
```

