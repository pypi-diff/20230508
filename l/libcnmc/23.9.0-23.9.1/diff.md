# Comparing `tmp/libcnmc-23.9.0.tar.gz` & `tmp/libcnmc-23.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libcnmc-23.9.0.tar", last modified: Wed Feb  8 09:14:50 2023, max compression
+gzip compressed data, was "dist/libcnmc-23.9.1.tar", last modified: Thu Feb  9 10:58:26 2023, max compression
```

## Comparing `libcnmc-23.9.0.tar` & `libcnmc-23.9.1.tar`

### file list

```diff
@@ -1,209 +1,209 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 09:14:50.000000 libcnmc-23.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-08 09:14:50.000000 libcnmc-23.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-08 09:14:43.000000 libcnmc-23.9.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-02-08 09:14:43.000000 libcnmc-23.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 09:14:50.000000 libcnmc-23.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-08 09:14:43.000000 libcnmc-23.9.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc/
--rw-r--r--   0 runner    (1001) docker     (123)    28273 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cli_4_2015.py
--rw-r--r--   0 runner    (1001) docker     (123)    15507 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cli_4667.py
--rw-r--r--   0 runner    (1001) docker     (123)    26393 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cli_4666.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc/cir_4_2015/
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2015/F12.py
--rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2015/F10AT.py
--rw-r--r--   0 runner    (1001) docker     (123)    26499 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2015/F1.py
--rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2015/F11.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2015/F15.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2015/F20.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2015/F13.py
--rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2015/F1bis.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2015/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2015/F13bis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2015/F16.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2015/F10BT.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2015/create_celles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2015/F13C.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2015/F12bis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9808 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2015/F9.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2015/F14.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/cnmcmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc/models/res_4666/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4666/f7_4666.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4666/f8_4666.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4666/f6_4666.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4666/f3_4666.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4666/f1_4666.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4666/f5_4666.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4666/f2_4666.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4666/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4666/f4_4666.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc/models/res_4771/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4771/f7_4771.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4771/f4_4771.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4771/f2_4771.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4771/f6_4771.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4771/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4771/f1_4771.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4771/f8_4771.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4771/f5_4771.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4771/f3_4771.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc/models/res_4667/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4667/macro_4667.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4667/f2_4667.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4667/pro_4667.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4667/resumen_4667.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4667/f4_4667.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4667/f1_4667.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4667/f3_4667.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4667/f6_4667.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4667/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4667/f8_4667.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4667/resumen_ccaa_4667.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4667/f7_4667.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4667/f5_4667.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc/models/res_4131/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4131/f4_4131.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4131/f3_4131.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4131/f7_4131.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4131/f8_4131.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4131/f1_4131.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4131/f2_4131.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4131/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4131/f6_4131.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/models/res_4131/f5_4131.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc/cir_3_2015/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_3_2015/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_3_2015/F3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc/res_4666/
--rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4666/MAQ.py
--rw-r--r--   0 runner    (1001) docker     (123)    16871 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4666/LAT.py
--rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4666/CTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4666/SUB.py
--rw-r--r--   0 runner    (1001) docker     (123)    19565 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4666/MOD.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4666/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4666/LBT.py
--rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4666/FIA.py
--rw-r--r--   0 runner    (1001) docker     (123)    18185 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4666/POS.py
--rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4666/AUD_POS.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4666/DES.py
--rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4666/AUD_LBT.py
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4666/AUD_FIA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4666/CON.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4666/AUD_CTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    11998 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4666/AUD_LAT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc/core/
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/core/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/core/cnmc_inventari.py
--rw-r--r--   0 runner    (1001) docker     (123)    45428 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc/cir_4_2014/
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2014/F1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2014/F11.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2014/F1bis.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_4_2014/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc/res_4771/
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4771/MAQ.py
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4771/LAT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4771/CTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4771/SUB.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4771/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4771/LBT.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4771/FIA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4771/POS.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4771/DES.py
--rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4771/INV.py
--rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cli_6181.py
--rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cli_4131.py
--rw-r--r--   0 runner    (1001) docker     (123)    38942 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cli_8_2021.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    38513 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc/res_4603/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4603/update_cinis_trafo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4603/CINIMAQ.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4603/CINIPOS.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4603/MAQ.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4603/LAT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4603/CTS.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4603/update_trams_cinis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4603/SUB.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4603/update_cts_cinis.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4603/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4603/LBT.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4603/FIA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4603/create_celles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4603/POS.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4603/DES.py
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4603/INV.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc/res_4667/
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4667/MAQ.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4667/LAT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4667/PRO.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4667/MACRO.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4667/CT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4667/RES.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4667/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4667/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4667/LBT.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4667/FIA.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4667/POS.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4667/DES.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4667/RES_CCAA.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4667/Otros.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc/res_4131/
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4131/MAQ.py
--rw-r--r--   0 runner    (1001) docker     (123)    23150 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4131/LAT.py
--rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4131/CTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4131/SUB.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4131/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4131/LBT.py
--rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4131/FIA.py
--rw-r--r--   0 runner    (1001) docker     (123)    20902 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4131/POS.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4131/DES.py
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/res_4131/CON.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FB3_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FB2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FA5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FB3_2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19359 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FB6.py
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FB5_2.py
--rw-r--r--   0 runner    (1001) docker     (123)    30742 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FA1.py
--rw-r--r--   0 runner    (1001) docker     (123)    44236 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FB9.py
--rw-r--r--   0 runner    (1001) docker     (123)    46090 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FB1.py
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FB5.py
--rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FB2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FB7.py
--rw-r--r--   0 runner    (1001) docker     (123)    10933 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FA2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FB2_2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15432 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FB4.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FB3.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FB1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)    31654 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FD2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FA4.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FA3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FB3_1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/cir_8_2021/FB8.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 09:14:50.000000 libcnmc-23.9.0/libcnmc/audit_6181/
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/audit_6181/MAQ.py
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/audit_6181/LAT.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/audit_6181/CTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/audit_6181/SE.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/audit_6181/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/audit_6181/LBT.py
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/audit_6181/FIA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/audit_6181/POS.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-02-08 09:14:43.000000 libcnmc-23.9.0/libcnmc/audit_6181/DES.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-08 09:14:43.000000 libcnmc-23.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-02-08 09:14:43.000000 libcnmc-23.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:58:26.000000 libcnmc-23.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-09 10:58:26.000000 libcnmc-23.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-09 10:58:19.000000 libcnmc-23.9.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-02-09 10:58:19.000000 libcnmc-23.9.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 10:58:26.000000 libcnmc-23.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-09 10:58:19.000000 libcnmc-23.9.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc/
+-rw-r--r--   0 runner    (1001) docker     (123)    28273 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cli_4_2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15507 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cli_4667.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26393 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cli_4666.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc/cir_4_2015/
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2015/F12.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2015/F10AT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26499 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2015/F1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2015/F11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2015/F15.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2015/F20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2015/F13.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2015/F1bis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2015/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2015/F13bis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2015/F16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2015/F10BT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2015/create_celles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2015/F13C.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2015/F12bis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9808 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2015/F9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2015/F14.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/cnmcmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc/models/res_4666/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4666/f7_4666.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4666/f8_4666.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4666/f6_4666.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4666/f3_4666.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4666/f1_4666.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4666/f5_4666.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4666/f2_4666.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4666/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4666/f4_4666.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc/models/res_4771/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4771/f7_4771.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4771/f4_4771.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4771/f2_4771.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4771/f6_4771.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4771/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4771/f1_4771.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4771/f8_4771.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4771/f5_4771.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4771/f3_4771.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc/models/res_4667/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4667/macro_4667.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4667/f2_4667.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4667/pro_4667.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4667/resumen_4667.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4667/f4_4667.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4667/f1_4667.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4667/f3_4667.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4667/f6_4667.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4667/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4667/f8_4667.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4667/resumen_ccaa_4667.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4667/f7_4667.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4667/f5_4667.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc/models/res_4131/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4131/f4_4131.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4131/f3_4131.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4131/f7_4131.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4131/f8_4131.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4131/f1_4131.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4131/f2_4131.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4131/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4131/f6_4131.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/models/res_4131/f5_4131.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc/cir_3_2015/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_3_2015/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_3_2015/F3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc/res_4666/
+-rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4666/MAQ.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16871 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4666/LAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4666/CTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4666/SUB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19565 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4666/MOD.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4666/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4666/LBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4666/FIA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18185 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4666/POS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4666/AUD_POS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4666/DES.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4666/AUD_LBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4666/AUD_FIA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4666/CON.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4666/AUD_CTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11998 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4666/AUD_LAT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/core/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/core/cnmc_inventari.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45428 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc/cir_4_2014/
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2014/F1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2014/F11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2014/F1bis.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_4_2014/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc/res_4771/
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4771/MAQ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4771/LAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4771/CTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4771/SUB.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4771/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4771/LBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4771/FIA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4771/POS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4771/DES.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4771/INV.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cli_6181.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cli_4131.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38942 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cli_8_2021.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38513 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc/res_4603/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4603/update_cinis_trafo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4603/CINIMAQ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4603/CINIPOS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4603/MAQ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4603/LAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4603/CTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4603/update_trams_cinis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4603/SUB.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4603/update_cts_cinis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4603/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4603/LBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4603/FIA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4603/create_celles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4603/POS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4603/DES.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4603/INV.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc/res_4667/
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4667/MAQ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4667/LAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4667/PRO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4667/MACRO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4667/CT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4667/RES.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4667/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4667/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4667/LBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4667/FIA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4667/POS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4667/DES.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4667/RES_CCAA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4667/Otros.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc/res_4131/
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4131/MAQ.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23150 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4131/LAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4131/CTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4131/SUB.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4131/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4131/LBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4131/FIA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20902 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4131/POS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4131/DES.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/res_4131/CON.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FB3_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FB2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FA5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FB3_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19359 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FB6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FB5_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30742 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FA1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44236 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FB9.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46090 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FB1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FB5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FB2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FB7.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10933 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FA2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FB2_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15432 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FB4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FB3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FB1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31654 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FD2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FA4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FA3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FB3_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/cir_8_2021/FB8.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:58:26.000000 libcnmc-23.9.1/libcnmc/audit_6181/
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/audit_6181/MAQ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/audit_6181/LAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/audit_6181/CTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/audit_6181/SE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/audit_6181/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/audit_6181/LBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/audit_6181/FIA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/audit_6181/POS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-02-09 10:58:19.000000 libcnmc-23.9.1/libcnmc/audit_6181/DES.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-09 10:58:19.000000 libcnmc-23.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-02-09 10:58:19.000000 libcnmc-23.9.1/README.md
```

### Comparing `libcnmc-23.9.0/setup.py` & `libcnmc-23.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     INSTALL_REQUIRES += ['multiprocessing']
 
 setup(name='libcnmc',
       description='Generació fitxers CNMC',
       author='GISCE-TI, S.L.',
       author_email='devel@gisce.net',
       url='http://www.gisce.net',
-      version='23.9.0',
+      version='23.9.1',
       license='General Public Licence 2',
       long_description='''Long description''',
       provides=['libcnmc'],
       install_requires=INSTALL_REQUIRES,
       tests_require=TESTS_REQUIRE,
       packages=find_packages(exclude=['tests']),
       dependency_links=DEPENDENCY_LINKS,
```

### Comparing `libcnmc-23.9.0/libcnmc.egg-info/SOURCES.txt` & `libcnmc-23.9.1/libcnmc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cli_4_2015.py` & `libcnmc-23.9.1/libcnmc/cli_4_2015.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cli_4667.py` & `libcnmc-23.9.1/libcnmc/cli_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cli_4666.py` & `libcnmc-23.9.1/libcnmc/cli_4666.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_4_2015/F12.py` & `libcnmc-23.9.1/libcnmc/cir_4_2015/F12.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_4_2015/F10AT.py` & `libcnmc-23.9.1/libcnmc/cir_4_2015/F10AT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_4_2015/F1.py` & `libcnmc-23.9.1/libcnmc/cir_4_2015/F1.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_4_2015/F11.py` & `libcnmc-23.9.1/libcnmc/cir_4_2015/F11.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_4_2015/F15.py` & `libcnmc-23.9.1/libcnmc/cir_4_2015/F15.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_4_2015/F20.py` & `libcnmc-23.9.1/libcnmc/cir_4_2015/F20.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_4_2015/F13.py` & `libcnmc-23.9.1/libcnmc/cir_4_2015/F13.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_4_2015/F1bis.py` & `libcnmc-23.9.1/libcnmc/cir_4_2015/F1bis.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_4_2015/F13bis.py` & `libcnmc-23.9.1/libcnmc/cir_4_2015/F13bis.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_4_2015/F16.py` & `libcnmc-23.9.1/libcnmc/cir_4_2015/F16.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_4_2015/F10BT.py` & `libcnmc-23.9.1/libcnmc/cir_4_2015/F10BT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_4_2015/create_celles.py` & `libcnmc-23.9.1/libcnmc/cir_4_2015/create_celles.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_4_2015/F13C.py` & `libcnmc-23.9.1/libcnmc/cir_4_2015/F13C.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_4_2015/F12bis.py` & `libcnmc-23.9.1/libcnmc/cir_4_2015/F12bis.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_4_2015/F9.py` & `libcnmc-23.9.1/libcnmc/cir_4_2015/F9.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_4_2015/F14.py` & `libcnmc-23.9.1/libcnmc/cir_4_2015/F14.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/fields.py` & `libcnmc-23.9.1/libcnmc/models/fields.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/cnmcmodel.py` & `libcnmc-23.9.1/libcnmc/models/cnmcmodel.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4666/f7_4666.py` & `libcnmc-23.9.1/libcnmc/models/res_4666/f7_4666.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4666/f8_4666.py` & `libcnmc-23.9.1/libcnmc/models/res_4666/f8_4666.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4666/f6_4666.py` & `libcnmc-23.9.1/libcnmc/models/res_4666/f6_4666.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4666/f3_4666.py` & `libcnmc-23.9.1/libcnmc/models/res_4666/f3_4666.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4666/f1_4666.py` & `libcnmc-23.9.1/libcnmc/models/res_4666/f1_4666.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4666/f5_4666.py` & `libcnmc-23.9.1/libcnmc/models/res_4666/f5_4666.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4666/f2_4666.py` & `libcnmc-23.9.1/libcnmc/models/res_4666/f2_4666.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4666/f4_4666.py` & `libcnmc-23.9.1/libcnmc/models/res_4666/f4_4666.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4771/f7_4771.py` & `libcnmc-23.9.1/libcnmc/models/res_4771/f7_4771.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4771/f4_4771.py` & `libcnmc-23.9.1/libcnmc/models/res_4771/f4_4771.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4771/f2_4771.py` & `libcnmc-23.9.1/libcnmc/models/res_4771/f2_4771.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4771/f6_4771.py` & `libcnmc-23.9.1/libcnmc/models/res_4771/f6_4771.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4771/f1_4771.py` & `libcnmc-23.9.1/libcnmc/models/res_4771/f1_4771.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4771/f8_4771.py` & `libcnmc-23.9.1/libcnmc/models/res_4771/f8_4771.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4771/f5_4771.py` & `libcnmc-23.9.1/libcnmc/models/res_4771/f5_4771.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4771/f3_4771.py` & `libcnmc-23.9.1/libcnmc/models/res_4771/f3_4771.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/__init__.py` & `libcnmc-23.9.1/libcnmc/models/__init__.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4667/macro_4667.py` & `libcnmc-23.9.1/libcnmc/models/res_4667/macro_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4667/f2_4667.py` & `libcnmc-23.9.1/libcnmc/models/res_4667/f2_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4667/pro_4667.py` & `libcnmc-23.9.1/libcnmc/models/res_4667/pro_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4667/resumen_4667.py` & `libcnmc-23.9.1/libcnmc/models/res_4667/resumen_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4667/f4_4667.py` & `libcnmc-23.9.1/libcnmc/models/res_4667/f4_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4667/f1_4667.py` & `libcnmc-23.9.1/libcnmc/models/res_4667/f1_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4667/f3_4667.py` & `libcnmc-23.9.1/libcnmc/models/res_4667/f3_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4667/f6_4667.py` & `libcnmc-23.9.1/libcnmc/models/res_4667/f6_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4667/f8_4667.py` & `libcnmc-23.9.1/libcnmc/models/res_4667/f8_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4667/resumen_ccaa_4667.py` & `libcnmc-23.9.1/libcnmc/models/res_4667/resumen_ccaa_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4667/f7_4667.py` & `libcnmc-23.9.1/libcnmc/models/res_4667/f7_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4667/f5_4667.py` & `libcnmc-23.9.1/libcnmc/models/res_4667/f5_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4131/f4_4131.py` & `libcnmc-23.9.1/libcnmc/models/res_4131/f4_4131.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4131/f3_4131.py` & `libcnmc-23.9.1/libcnmc/models/res_4131/f3_4131.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4131/f7_4131.py` & `libcnmc-23.9.1/libcnmc/models/res_4131/f7_4131.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4131/f8_4131.py` & `libcnmc-23.9.1/libcnmc/models/res_4131/f8_4131.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4131/f1_4131.py` & `libcnmc-23.9.1/libcnmc/models/res_4131/f1_4131.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4131/f2_4131.py` & `libcnmc-23.9.1/libcnmc/models/res_4131/f2_4131.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4131/f6_4131.py` & `libcnmc-23.9.1/libcnmc/models/res_4131/f6_4131.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/models/res_4131/f5_4131.py` & `libcnmc-23.9.1/libcnmc/models/res_4131/f5_4131.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_3_2015/F3.py` & `libcnmc-23.9.1/libcnmc/cir_3_2015/F3.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4666/MAQ.py` & `libcnmc-23.9.1/libcnmc/res_4666/MAQ.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4666/LAT.py` & `libcnmc-23.9.1/libcnmc/res_4666/LAT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4666/CTS.py` & `libcnmc-23.9.1/libcnmc/res_4666/CTS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4666/SUB.py` & `libcnmc-23.9.1/libcnmc/res_4666/SUB.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4666/MOD.py` & `libcnmc-23.9.1/libcnmc/res_4666/MOD.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4666/LBT.py` & `libcnmc-23.9.1/libcnmc/res_4666/LBT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4666/FIA.py` & `libcnmc-23.9.1/libcnmc/res_4666/FIA.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4666/POS.py` & `libcnmc-23.9.1/libcnmc/res_4666/POS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4666/AUD_POS.py` & `libcnmc-23.9.1/libcnmc/res_4666/AUD_POS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4666/DES.py` & `libcnmc-23.9.1/libcnmc/res_4666/DES.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4666/AUD_LBT.py` & `libcnmc-23.9.1/libcnmc/res_4666/AUD_LBT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4666/AUD_FIA.py` & `libcnmc-23.9.1/libcnmc/res_4666/AUD_FIA.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4666/CON.py` & `libcnmc-23.9.1/libcnmc/res_4666/CON.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4666/AUD_CTS.py` & `libcnmc-23.9.1/libcnmc/res_4666/AUD_CTS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4666/AUD_LAT.py` & `libcnmc-23.9.1/libcnmc/res_4666/AUD_LAT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/core/backend.py` & `libcnmc-23.9.1/libcnmc/core/backend.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/core/__init__.py` & `libcnmc-23.9.1/libcnmc/core/__init__.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/core/cnmc_inventari.py` & `libcnmc-23.9.1/libcnmc/core/cnmc_inventari.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cli.py` & `libcnmc-23.9.1/libcnmc/cli.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_4_2014/F1.py` & `libcnmc-23.9.1/libcnmc/cir_4_2014/F1.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_4_2014/F11.py` & `libcnmc-23.9.1/libcnmc/cir_4_2014/F11.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_4_2014/F1bis.py` & `libcnmc-23.9.1/libcnmc/cir_4_2014/F1bis.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4771/MAQ.py` & `libcnmc-23.9.1/libcnmc/res_4771/MAQ.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4771/LAT.py` & `libcnmc-23.9.1/libcnmc/res_4771/LAT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4771/CTS.py` & `libcnmc-23.9.1/libcnmc/res_4771/CTS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4771/SUB.py` & `libcnmc-23.9.1/libcnmc/res_4771/SUB.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4771/LBT.py` & `libcnmc-23.9.1/libcnmc/res_4771/LBT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4771/FIA.py` & `libcnmc-23.9.1/libcnmc/res_4771/FIA.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4771/POS.py` & `libcnmc-23.9.1/libcnmc/res_4771/POS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4771/DES.py` & `libcnmc-23.9.1/libcnmc/res_4771/DES.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4771/INV.py` & `libcnmc-23.9.1/libcnmc/res_4771/INV.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cli_6181.py` & `libcnmc-23.9.1/libcnmc/cli_6181.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cli_4131.py` & `libcnmc-23.9.1/libcnmc/cli_4131.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cli_8_2021.py` & `libcnmc-23.9.1/libcnmc/cli_8_2021.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/utils.py` & `libcnmc-23.9.1/libcnmc/utils.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/checker.py` & `libcnmc-23.9.1/libcnmc/checker.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4603/CINIMAQ.py` & `libcnmc-23.9.1/libcnmc/res_4603/CINIMAQ.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4603/CINIPOS.py` & `libcnmc-23.9.1/libcnmc/res_4603/CINIPOS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4603/MAQ.py` & `libcnmc-23.9.1/libcnmc/res_4603/MAQ.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4603/LAT.py` & `libcnmc-23.9.1/libcnmc/res_4603/LAT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4603/CTS.py` & `libcnmc-23.9.1/libcnmc/res_4603/CTS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4603/SUB.py` & `libcnmc-23.9.1/libcnmc/res_4603/SUB.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4603/LBT.py` & `libcnmc-23.9.1/libcnmc/res_4603/LBT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4603/FIA.py` & `libcnmc-23.9.1/libcnmc/res_4603/FIA.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4603/create_celles.py` & `libcnmc-23.9.1/libcnmc/res_4603/create_celles.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4603/POS.py` & `libcnmc-23.9.1/libcnmc/res_4603/POS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4603/DES.py` & `libcnmc-23.9.1/libcnmc/res_4603/DES.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4603/INV.py` & `libcnmc-23.9.1/libcnmc/res_4603/INV.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4667/MAQ.py` & `libcnmc-23.9.1/libcnmc/res_4667/MAQ.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4667/LAT.py` & `libcnmc-23.9.1/libcnmc/res_4667/LAT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4667/PRO.py` & `libcnmc-23.9.1/libcnmc/res_4667/PRO.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4667/MACRO.py` & `libcnmc-23.9.1/libcnmc/res_4667/MACRO.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4667/CT.py` & `libcnmc-23.9.1/libcnmc/res_4667/CT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4667/RES.py` & `libcnmc-23.9.1/libcnmc/res_4667/RES.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4667/LBT.py` & `libcnmc-23.9.1/libcnmc/res_4667/LBT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4667/FIA.py` & `libcnmc-23.9.1/libcnmc/res_4667/FIA.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4667/POS.py` & `libcnmc-23.9.1/libcnmc/res_4667/POS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4667/DES.py` & `libcnmc-23.9.1/libcnmc/res_4667/DES.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4667/RES_CCAA.py` & `libcnmc-23.9.1/libcnmc/res_4667/RES_CCAA.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4667/Otros.py` & `libcnmc-23.9.1/libcnmc/res_4667/Otros.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4131/MAQ.py` & `libcnmc-23.9.1/libcnmc/res_4131/MAQ.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4131/LAT.py` & `libcnmc-23.9.1/libcnmc/res_4131/LAT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4131/CTS.py` & `libcnmc-23.9.1/libcnmc/res_4131/CTS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4131/SUB.py` & `libcnmc-23.9.1/libcnmc/res_4131/SUB.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4131/LBT.py` & `libcnmc-23.9.1/libcnmc/res_4131/LBT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4131/FIA.py` & `libcnmc-23.9.1/libcnmc/res_4131/FIA.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4131/POS.py` & `libcnmc-23.9.1/libcnmc/res_4131/POS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4131/DES.py` & `libcnmc-23.9.1/libcnmc/res_4131/DES.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/res_4131/CON.py` & `libcnmc-23.9.1/libcnmc/res_4131/CON.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FB3_3.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FB3_3.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FB2_1.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FB2_1.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FA5.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FA5.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FB3_2.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FB3_2.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FB6.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FB6.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FB5_2.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FB5_2.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FA1.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FA1.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FB9.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FB9.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FB1.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FB1.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FB5.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FB5.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FB2.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FB2.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FB7.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FB7.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FA2.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FA2.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FB2_2.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FB2_2.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FB4.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FB4.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FB3.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FB3.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FB1_1.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FB1_1.py`

 * *Files 10% similar despite different names*

```diff
@@ -80,26 +80,26 @@
                     try:
                         dest = points[o_position + 1]
                         if dest:
                             # Vertex inici
                             o_inicio = '{} 0'.format(p)
                             inicio = o_inicio.split(' ')
                             vertex_inicio = {
-                                'x': inicio[0],
-                                'y': inicio[1]
+                                'x': float(inicio[0]),
+                                'y': float(inicio[1])
                             }
                             res_srid_inicio = convert_srid(get_srid(o), (vertex_inicio['x'], vertex_inicio['y']))
                             o_inicio_z = ''
 
                             # Vertex final
                             o_final = '{} 0'.format(dest)
                             final = o_final.split(' ')
                             vertex_final = {
-                                'x': final[0],
-                                'y': final[1]
+                                'x': float(final[0]),
+                                'y': float(final[1])
                             }
                             res_srid_final = convert_srid(get_srid(o), (vertex_final['x'], vertex_final['y']))
                             o_final_z = ''
 
                             self.output_q.put([
                                 '{}_{}'.format(o_segmento, o_position + 1),  # CÓDIGO SEGMENTO
                                 o_tram,                                      # IDENTIFICADOR DE TRAMO
```

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FD2.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FD2.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FA4.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FA4.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FA3.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FA3.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FB3_1.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FB3_1.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/cir_8_2021/FB8.py` & `libcnmc-23.9.1/libcnmc/cir_8_2021/FB8.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/audit_6181/MAQ.py` & `libcnmc-23.9.1/libcnmc/audit_6181/MAQ.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/audit_6181/LAT.py` & `libcnmc-23.9.1/libcnmc/audit_6181/LAT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/audit_6181/CTS.py` & `libcnmc-23.9.1/libcnmc/audit_6181/CTS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/audit_6181/SE.py` & `libcnmc-23.9.1/libcnmc/audit_6181/SE.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/audit_6181/LBT.py` & `libcnmc-23.9.1/libcnmc/audit_6181/LBT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/audit_6181/FIA.py` & `libcnmc-23.9.1/libcnmc/audit_6181/FIA.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/audit_6181/POS.py` & `libcnmc-23.9.1/libcnmc/audit_6181/POS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-23.9.0/libcnmc/audit_6181/DES.py` & `libcnmc-23.9.1/libcnmc/audit_6181/DES.py`

 * *Files identical despite different names*

