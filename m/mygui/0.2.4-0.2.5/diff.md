# Comparing `tmp/mygui-0.2.4.tar.gz` & `tmp/mygui-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mygui-0.2.4.tar", last modified: Mon May  8 18:44:39 2023, max compression
+gzip compressed data, was "mygui-0.2.5.tar", last modified: Mon May  8 18:56:28 2023, max compression
```

## Comparing `mygui-0.2.4.tar` & `mygui-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 18:44:39.091572 mygui-0.2.4/
--rw-rw-rw-   0        0        0     1143 2022-07-22 19:19:58.000000 mygui-0.2.4/LICENSE.md
--rw-rw-rw-   0        0        0     1514 2023-05-08 18:44:39.091572 mygui-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      629 2023-05-08 18:43:43.000000 mygui-0.2.4/README.md
--rw-rw-rw-   0        0        0       94 2022-07-01 15:14:17.000000 mygui-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0     1012 2023-05-08 18:44:39.091572 mygui-0.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-08 18:44:39.028723 mygui-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 18:44:39.060073 mygui-0.2.4/src/mygui/
-drwxrwxrwx   0        0        0        0 2023-05-08 18:44:39.075606 mygui-0.2.4/src/mygui/Examples/
--rw-rw-rw-   0        0        0      304 2022-06-10 17:13:36.000000 mygui-0.2.4/src/mygui/Examples/LgridExamples.py
--rw-rw-rw-   0        0        0      180 2022-06-15 17:08:58.000000 mygui-0.2.4/src/mygui/Examples/MYGUI-egrid.py
--rw-rw-rw-   0        0        0      275 2022-06-15 17:06:42.000000 mygui-0.2.4/src/mygui/Examples/MYGUI-lgrid.py
--rw-rw-rw-   0        0        0      238 2022-06-10 17:11:27.000000 mygui-0.2.4/src/mygui/Examples/testmygui.py
--rw-rw-rw-   0        0        0      838 2022-09-29 18:16:50.000000 mygui-0.2.4/src/mygui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 18:44:39.091572 mygui-0.2.4/src/mygui/test/
--rw-rw-rw-   0        0        0      866 2022-06-15 18:45:44.000000 mygui-0.2.4/src/mygui/test/lgridegridtest.py
--rw-rw-rw-   0        0        0      268 2022-09-29 18:18:15.000000 mygui-0.2.4/src/mygui/test/testmygui.py
-drwxrwxrwx   0        0        0        0 2023-05-08 18:44:39.060073 mygui-0.2.4/src/mygui.egg-info/
--rw-rw-rw-   0        0        0     1514 2023-05-08 18:44:38.000000 mygui-0.2.4/src/mygui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-05-08 18:44:38.000000 mygui-0.2.4/src/mygui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 18:44:38.000000 mygui-0.2.4/src/mygui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-08 18:44:38.000000 mygui-0.2.4/src/mygui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 18:56:28.885733 mygui-0.2.5/
+-rw-rw-rw-   0        0        0     1143 2023-05-08 18:50:30.000000 mygui-0.2.5/LICENSE.md
+-rw-rw-rw-   0        0        0     1516 2023-05-08 18:56:28.885733 mygui-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2023-05-08 18:53:07.000000 mygui-0.2.5/README.md
+-rw-rw-rw-   0        0        0       94 2022-07-01 15:14:17.000000 mygui-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1014 2023-05-08 18:56:28.885733 mygui-0.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 18:56:28.870103 mygui-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 18:56:28.870103 mygui-0.2.5/src/mygui/
+drwxrwxrwx   0        0        0        0 2023-05-08 18:56:28.885733 mygui-0.2.5/src/mygui/Examples/
+-rw-rw-rw-   0        0        0      304 2022-06-10 17:13:36.000000 mygui-0.2.5/src/mygui/Examples/LgridExamples.py
+-rw-rw-rw-   0        0        0      180 2022-06-15 17:08:58.000000 mygui-0.2.5/src/mygui/Examples/MYGUI-egrid.py
+-rw-rw-rw-   0        0        0      275 2022-06-15 17:06:42.000000 mygui-0.2.5/src/mygui/Examples/MYGUI-lgrid.py
+-rw-rw-rw-   0        0        0      238 2022-06-10 17:11:27.000000 mygui-0.2.5/src/mygui/Examples/testmygui.py
+-rw-rw-rw-   0        0        0      838 2022-09-29 18:16:50.000000 mygui-0.2.5/src/mygui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 18:56:28.885733 mygui-0.2.5/src/mygui/test/
+-rw-rw-rw-   0        0        0      866 2022-06-15 18:45:44.000000 mygui-0.2.5/src/mygui/test/lgridegridtest.py
+-rw-rw-rw-   0        0        0      268 2022-09-29 18:18:15.000000 mygui-0.2.5/src/mygui/test/testmygui.py
+drwxrwxrwx   0        0        0        0 2023-05-08 18:56:28.885733 mygui-0.2.5/src/mygui.egg-info/
+-rw-rw-rw-   0        0        0     1516 2023-05-08 18:56:28.000000 mygui-0.2.5/src/mygui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-05-08 18:56:28.000000 mygui-0.2.5/src/mygui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 18:56:28.000000 mygui-0.2.5/src/mygui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-08 18:56:28.000000 mygui-0.2.5/src/mygui.egg-info/top_level.txt
```

### Comparing `mygui-0.2.4/LICENSE.md` & `mygui-0.2.5/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-## Copyright (c) 2020 - 2022 Michael Mulvey
+## Copyright (c) 2020 - 2023 Michael Mulvey
 
     Permission is hereby granted, free of charge, to any person obtaining a copy
     of this software and associated documentation files (the "Software"), to deal
     in the Software without restriction, including without limitation the rights
     to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
     copies of the Software, and to permit persons to whom the Software is
     furnished to do so, subject to the following conditions:
```

### Comparing `mygui-0.2.4/PKG-INFO` & `mygui-0.2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: mygui
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Simple icon to replace the tkinter feather for your programs
 Home-page: https://github.com/Caveman-Software/mygui
 Author: Michael E Mulvey
-Author-email: michael.e.mulvey@gmail.com
+Author-email: "michael.e.mulvey@gmail.com"
 Project-URL: Bug Tracker, https://github.com/Caveman-Software/mygui/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 
-# mygui 0.2.4
+# mygui 0.2.5
 
-# <img src="https://raw.githubusercontent.com/Caveman-Software/mygui/main/Icon.png" width="35" height="35">  Caveman Software® 2022
+# <img src="https://raw.githubusercontent.com/Caveman-Software/mygui/main/Icon.png" width="35" height="35">  Caveman Software® 2023
 
 ## lgrid
 
 example:
 
 ---
```

### Comparing `mygui-0.2.4/README.md` & `mygui-0.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
-# mygui 0.2.4
+# mygui 0.2.5
 
-# <img src="https://raw.githubusercontent.com/Caveman-Software/mygui/main/Icon.png" width="35" height="35">  Caveman Software® 2022
+# <img src="https://raw.githubusercontent.com/Caveman-Software/mygui/main/Icon.png" width="35" height="35">  Caveman Software® 2023
 
 ## lgrid
 
 example:
 
 ---
```

### Comparing `mygui-0.2.4/setup.cfg` & `mygui-0.2.5/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 7967 7569 0d0a 7665 7273 696f   = mygui..versio
-00000020: 6e20 3d20 302e 322e 340d 0a61 7574 686f  n = 0.2.4..autho
+00000020: 6e20 3d20 302e 322e 350d 0a61 7574 686f  n = 0.2.5..autho
 00000030: 7220 3d20 4d69 6368 6165 6c20 4520 4d75  r = Michael E Mu
 00000040: 6c76 6579 0d0a 6175 7468 6f72 5f65 6d61  lvey..author_ema
-00000050: 696c 203d 206d 6963 6861 656c 2e65 2e6d  il = michael.e.m
-00000060: 756c 7665 7940 676d 6169 6c2e 636f 6d0d  ulvey@gmail.com.
-00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
-00000080: 2053 696d 706c 6520 6963 6f6e 2074 6f20   Simple icon to 
-00000090: 7265 706c 6163 6520 7468 6520 746b 696e  replace the tkin
-000000a0: 7465 7220 6665 6174 6865 7220 666f 7220  ter feather for 
-000000b0: 796f 7572 2070 726f 6772 616d 730d 0a6c  your programs..l
-000000c0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
-000000d0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
-000000e0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
-000000f0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-00000100: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-00000110: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
-00000120: 6769 7468 7562 2e63 6f6d 2f43 6176 656d  github.com/Cavem
-00000130: 616e 2d53 6f66 7477 6172 652f 6d79 6775  an-Software/mygu
-00000140: 690d 0a70 726f 6a65 6374 5f75 726c 7320  i..project_urls 
-00000150: 3d20 0d0a 0942 7567 2054 7261 636b 6572  = ...Bug Tracker
-00000160: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-00000170: 622e 636f 6d2f 4361 7665 6d61 6e2d 536f  b.com/Caveman-So
-00000180: 6674 7761 7265 2f6d 7967 7569 2f69 7373  ftware/mygui/iss
-00000190: 7565 730d 0a63 6c61 7373 6966 6965 7273  ues..classifiers
-000001a0: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
-000001b0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000001c0: 7468 6f6e 203a 3a20 3320 3a3a 204f 6e6c  thon :: 3 :: Onl
-000001d0: 790d 0a09 5072 6f67 7261 6d6d 696e 6720  y...Programming 
-000001e0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000001f0: 6f6e 203a 3a20 332e 380d 0a09 5072 6f67  on :: 3.8...Prog
-00000200: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000210: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000220: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
-00000230: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000240: 6f6e 203a 3a20 332e 3130 0d0a 0950 726f  on :: 3.10...Pro
-00000250: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000260: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000270: 2e31 310d 0a09 4c69 6365 6e73 6520 3a3a  .11...License ::
-00000280: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-00000290: 204d 4954 204c 6963 656e 7365 0d0a 094f   MIT License...O
-000002a0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-000002b0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-000002c0: 740d 0a09 4f70 6572 6174 696e 6720 5379  t...Operating Sy
-000002d0: 7374 656d 203a 3a20 4d69 6372 6f73 6f66  stem :: Microsof
-000002e0: 7420 3a3a 2057 696e 646f 7773 203a 3a20  t :: Windows :: 
-000002f0: 5769 6e64 6f77 7320 3130 0d0a 0d0a 5b6f  Windows 10....[o
-00000300: 7074 696f 6e73 5d0d 0a69 6e63 6c75 6465  ptions]..include
-00000310: 5f70 6163 6b61 6765 5f64 6174 6120 3d20  _package_data = 
-00000320: 5472 7565 0d0a 7061 636b 6167 655f 6469  True..package_di
-00000330: 7220 3d20 0d0a 093d 2073 7263 0d0a 7061  r = ...= src..pa
-00000340: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
-00000350: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
-00000360: 3d20 3e3d 332e 380d 0a0d 0a5b 6f70 7469  = >=3.8....[opti
-00000370: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
-00000380: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
-00000390: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
-000003a0: 6167 655f 6461 7461 5d0d 0a2a 203d 2045  age_data]..* = E
-000003b0: 7861 6d70 6c65 732f 2a2e 7079 2c74 6573  xamples/*.py,tes
-000003c0: 742f 2a2e 7079 0d0a 0d0a 5b65 6767 5f69  t/*.py....[egg_i
-000003d0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-000003e0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-000003f0: 0d0a 0d0a                                ....
+00000050: 696c 203d 2022 6d69 6368 6165 6c2e 652e  il = "michael.e.
+00000060: 6d75 6c76 6579 4067 6d61 696c 2e63 6f6d  mulvey@gmail.com
+00000070: 220d 0a64 6573 6372 6970 7469 6f6e 203d  "..description =
+00000080: 2041 2053 696d 706c 6520 6963 6f6e 2074   A Simple icon t
+00000090: 6f20 7265 706c 6163 6520 7468 6520 746b  o replace the tk
+000000a0: 696e 7465 7220 6665 6174 6865 7220 666f  inter feather fo
+000000b0: 7220 796f 7572 2070 726f 6772 616d 730d  r your programs.
+000000c0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+000000d0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
+000000e0: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
+000000f0: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
+00000100: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
+00000110: 776e 0d0a 7572 6c20 3d20 6874 7470 733a  wn..url = https:
+00000120: 2f2f 6769 7468 7562 2e63 6f6d 2f43 6176  //github.com/Cav
+00000130: 656d 616e 2d53 6f66 7477 6172 652f 6d79  eman-Software/my
+00000140: 6775 690d 0a70 726f 6a65 6374 5f75 726c  gui..project_url
+00000150: 7320 3d20 0d0a 0942 7567 2054 7261 636b  s = ...Bug Track
+00000160: 6572 203d 2068 7474 7073 3a2f 2f67 6974  er = https://git
+00000170: 6875 622e 636f 6d2f 4361 7665 6d61 6e2d  hub.com/Caveman-
+00000180: 536f 6674 7761 7265 2f6d 7967 7569 2f69  Software/mygui/i
+00000190: 7373 7565 730d 0a63 6c61 7373 6966 6965  ssues..classifie
+000001a0: 7273 203d 200d 0a09 5072 6f67 7261 6d6d  rs = ...Programm
+000001b0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000001c0: 5079 7468 6f6e 203a 3a20 3320 3a3a 204f  Python :: 3 :: O
+000001d0: 6e6c 790d 0a09 5072 6f67 7261 6d6d 696e  nly...Programmin
+000001e0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000001f0: 7468 6f6e 203a 3a20 332e 380d 0a09 5072  thon :: 3.8...Pr
+00000200: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000210: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000220: 332e 390d 0a09 5072 6f67 7261 6d6d 696e  3.9...Programmin
+00000230: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000240: 7468 6f6e 203a 3a20 332e 3130 0d0a 0950  thon :: 3.10...P
+00000250: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000260: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000270: 2033 2e31 310d 0a09 4c69 6365 6e73 6520   3.11...License 
+00000280: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+00000290: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
+000002a0: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+000002b0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+000002c0: 656e 740d 0a09 4f70 6572 6174 696e 6720  ent...Operating 
+000002d0: 5379 7374 656d 203a 3a20 4d69 6372 6f73  System :: Micros
+000002e0: 6f66 7420 3a3a 2057 696e 646f 7773 203a  oft :: Windows :
+000002f0: 3a20 5769 6e64 6f77 7320 3130 0d0a 0d0a  : Windows 10....
+00000300: 5b6f 7074 696f 6e73 5d0d 0a69 6e63 6c75  [options]..inclu
+00000310: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
+00000320: 3d20 5472 7565 0d0a 7061 636b 6167 655f  = True..package_
+00000330: 6469 7220 3d20 0d0a 093d 2073 7263 0d0a  dir = ...= src..
+00000340: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+00000350: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
+00000360: 7320 3d20 3e3d 332e 380d 0a0d 0a5b 6f70  s = >=3.8....[op
+00000370: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
+00000380: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
+00000390: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  c....[options.pa
+000003a0: 636b 6167 655f 6461 7461 5d0d 0a2a 203d  ckage_data]..* =
+000003b0: 2045 7861 6d70 6c65 732f 2a2e 7079 2c74   Examples/*.py,t
+000003c0: 6573 742f 2a2e 7079 0d0a 0d0a 5b65 6767  est/*.py....[egg
+000003d0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+000003e0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+000003f0: 2030 0d0a 0d0a                            0....
```

### Comparing `mygui-0.2.4/src/mygui/__init__.py` & `mygui-0.2.5/src/mygui/__init__.py`

 * *Files identical despite different names*

### Comparing `mygui-0.2.4/src/mygui/test/lgridegridtest.py` & `mygui-0.2.5/src/mygui/test/lgridegridtest.py`

 * *Files identical despite different names*

### Comparing `mygui-0.2.4/src/mygui.egg-info/PKG-INFO` & `mygui-0.2.5/src/mygui.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: mygui
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Simple icon to replace the tkinter feather for your programs
 Home-page: https://github.com/Caveman-Software/mygui
 Author: Michael E Mulvey
-Author-email: michael.e.mulvey@gmail.com
+Author-email: "michael.e.mulvey@gmail.com"
 Project-URL: Bug Tracker, https://github.com/Caveman-Software/mygui/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 
-# mygui 0.2.4
+# mygui 0.2.5
 
-# <img src="https://raw.githubusercontent.com/Caveman-Software/mygui/main/Icon.png" width="35" height="35">  Caveman Software® 2022
+# <img src="https://raw.githubusercontent.com/Caveman-Software/mygui/main/Icon.png" width="35" height="35">  Caveman Software® 2023
 
 ## lgrid
 
 example:
 
 ---
```

