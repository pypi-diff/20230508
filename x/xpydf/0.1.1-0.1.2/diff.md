# Comparing `tmp/xpydf-0.1.1.tar.gz` & `tmp/xpydf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpydf-0.1.1.tar", last modified: Wed Apr 19 13:30:29 2023, max compression
+gzip compressed data, was "xpydf-0.1.2.tar", last modified: Mon May  8 14:03:04 2023, max compression
```

## Comparing `xpydf-0.1.1.tar` & `xpydf-0.1.2.tar`

### file list

```diff
@@ -1,254 +1,257 @@
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-04-19 13:30:29.390088 xpydf-0.1.1/
--rw-r--r--   0 matthijs   (501) staff       (20)    35149 2023-02-17 12:43:21.000000 xpydf-0.1.1/LICENSE
--rw-r--r--   0 matthijs   (501) staff       (20)      118 2023-04-12 11:54:25.000000 xpydf-0.1.1/MANIFEST.in
--rw-r--r--   0 matthijs   (501) staff       (20)     1133 2023-04-19 13:30:29.390182 xpydf-0.1.1/PKG-INFO
--rw-r--r--   0 matthijs   (501) staff       (20)      240 2023-04-12 11:54:25.000000 xpydf-0.1.1/README.md
--rw-r--r--   0 matthijs   (501) staff       (20)      724 2023-04-12 11:56:31.000000 xpydf-0.1.1/pyproject.toml
--rw-r--r--   0 matthijs   (501) staff       (20)      824 2023-04-19 13:30:29.390511 xpydf-0.1.1/setup.cfg
--rw-r--r--   0 matthijs   (501) staff       (20)     1953 2023-04-12 14:51:50.000000 xpydf-0.1.1/setup.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-04-19 13:30:29.319178 xpydf-0.1.1/src/
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-04-19 13:30:29.324737 xpydf-0.1.1/src/xpdf-4.04/
--rw-r--r--   0 matthijs   (501) staff       (20)     8196 2023-04-13 10:48:09.000000 xpydf-0.1.1/src/xpdf-4.04/.DS_Store
--rw-r--r--   0 matthijs   (501) staff       (20)     1330 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/ANNOUNCE
--rw-r--r--   0 matthijs   (501) staff       (20)   139475 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/CHANGES
--rw-r--r--   0 matthijs   (501) staff       (20)     1053 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/CMakeLists.txt
--rw-r--r--   0 matthijs   (501) staff       (20)    17982 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/COPYING
--rw-r--r--   0 matthijs   (501) staff       (20)    35147 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/COPYING3
--rw-r--r--   0 matthijs   (501) staff       (20)     5614 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/INSTALL
--rw-r--r--   0 matthijs   (501) staff       (20)    13778 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/README
--rw-r--r--   0 matthijs   (501) staff       (20)     2002 2023-04-12 11:54:25.000000 xpydf-0.1.1/src/xpdf-4.04/aconf.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1985 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/aconf.h.in
--rw-r--r--   0 matthijs   (501) staff       (20)      941 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/aconf2.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10676 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/cmake-config.txt
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-04-19 13:30:29.327472 xpydf-0.1.1/src/xpdf-4.04/fofi/
--rw-r--r--   0 matthijs   (501) staff       (20)     3275 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiBase.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1344 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiBase.h
--rw-r--r--   0 matthijs   (501) staff       (20)    14853 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiEncodings.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1005 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiEncodings.h
--rw-r--r--   0 matthijs   (501) staff       (20)    21889 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiIdentifier.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1659 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiIdentifier.h
--rw-r--r--   0 matthijs   (501) staff       (20)    77637 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiTrueType.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     8227 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiTrueType.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8796 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiType1.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1434 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiType1.h
--rw-r--r--   0 matthijs   (501) staff       (20)    97383 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiType1C.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     8299 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiType1C.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-04-19 13:30:29.331566 xpydf-0.1.1/src/xpdf-4.04/goo/
--rw-r--r--   0 matthijs   (501) staff       (20)     2748 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/goo/FixedPoint.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     7361 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/goo/FixedPoint.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6201 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/goo/GHash.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2209 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/goo/GHash.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2276 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/goo/GList.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2724 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/goo/GList.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2629 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/goo/GMutex.h
--rw-r--r--   0 matthijs   (501) staff       (20)    17722 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/goo/GString.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4269 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/goo/GString.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2406 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/goo/Trace.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1171 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/goo/Trace.h
--rw-r--r--   0 matthijs   (501) staff       (20)    17381 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/goo/gfile.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4565 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/goo/gfile.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8259 2023-03-01 15:38:49.000000 xpydf-0.1.1/src/xpdf-4.04/goo/gmem.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2029 2023-03-01 15:38:49.000000 xpydf-0.1.1/src/xpdf-4.04/goo/gmem.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1005 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/goo/gmempp.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1714 2023-03-01 15:38:49.000000 xpydf-0.1.1/src/xpdf-4.04/goo/gmempp.h
--rw-r--r--   0 matthijs   (501) staff       (20)      562 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/goo/gtypes.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1583 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/goo/parseargs.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-04-19 13:30:29.340597 xpydf-0.1.1/src/xpdf-4.04/splash/
--rw-r--r--   0 matthijs   (501) staff       (20)   230071 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/Splash.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    20193 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/Splash.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6603 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashBitmap.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2881 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashBitmap.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11473 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashClip.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4007 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashClip.h
--rw-r--r--   0 matthijs   (501) staff       (20)      930 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashErrorCodes.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13929 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashFTFont.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1345 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashFTFont.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8902 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashFTFontEngine.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2248 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashFTFontEngine.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4055 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashFTFontFile.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2241 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashFTFontFile.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4995 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashFont.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3666 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashFont.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9673 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashFontEngine.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3358 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashFontEngine.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1589 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashFontFile.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2168 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashFontFile.h
--rw-r--r--   0 matthijs   (501) staff       (20)      603 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashFontFileID.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      687 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashFontFileID.h
--rw-r--r--   0 matthijs   (501) staff       (20)      758 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashGlyphBitmap.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9510 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashMath.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5135 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashPath.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3876 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashPath.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1042 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashPattern.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1447 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashPattern.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9844 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashScreen.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2167 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashScreen.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9521 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashState.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3669 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashState.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4155 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashTypes.h
--rw-r--r--   0 matthijs   (501) staff       (20)    17088 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashXPath.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3761 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashXPath.h
--rw-r--r--   0 matthijs   (501) staff       (20)    12936 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashXPathScanner.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2482 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/splash/SplashXPathScanner.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-04-19 13:30:29.381129 xpydf-0.1.1/src/xpdf-4.04/xpdf/
--rw-r--r--   0 matthijs   (501) staff       (20)   104168 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/AcroForm.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     5229 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/AcroForm.h
--rw-r--r--   0 matthijs   (501) staff       (20)    38840 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Annot.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4895 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Annot.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1385 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Array.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1400 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Array.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1387 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/BuiltinFont.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1080 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/BuiltinFont.h
--rw-r--r--   0 matthijs   (501) staff       (20)   229548 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/BuiltinFontTables.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      556 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/BuiltinFontTables.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10417 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/CMap.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3178 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/CMap.h
--rw-r--r--   0 matthijs   (501) staff       (20)    28608 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Catalog.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4742 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Catalog.h
--rw-r--r--   0 matthijs   (501) staff       (20)    19175 2023-04-13 10:47:41.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/CharCodeToUnicode.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3702 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/CharCodeToUnicode.h
--rw-r--r--   0 matthijs   (501) staff       (20)      526 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/CharTypes.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8379 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/CompactFontTables.h
--rw-r--r--   0 matthijs   (501) staff       (20)    45644 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Decrypt.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3530 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Decrypt.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2993 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Dict.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2088 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Dict.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5247 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/DisplayState.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     5225 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/DisplayState.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2123 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Error.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1353 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Error.h
--rw-r--r--   0 matthijs   (501) staff       (20)      984 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/ErrorCodes.h
--rw-r--r--   0 matthijs   (501) staff       (20)    21312 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/FontEncodingTables.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      564 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/FontEncodingTables.h
--rw-r--r--   0 matthijs   (501) staff       (20)    36553 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Function.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     6722 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Function.h
--rw-r--r--   0 matthijs   (501) staff       (20)   144837 2023-04-13 10:47:44.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Gfx.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    11911 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Gfx.h
--rw-r--r--   0 matthijs   (501) staff       (20)    65646 2023-04-13 10:47:45.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/GfxFont.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    12828 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/GfxFont.h
--rw-r--r--   0 matthijs   (501) staff       (20)   120789 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/GfxState.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    43452 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/GfxState.h
--rw-r--r--   0 matthijs   (501) staff       (20)   103543 2023-02-21 10:47:30.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/GlobalParams.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    23054 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/GlobalParams.h
--rw-r--r--   0 matthijs   (501) staff       (20)    34442 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/HTMLGen.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3131 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/HTMLGen.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11293 2023-02-27 14:41:14.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/ImageOutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3942 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/ImageOutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8327 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/JArithmeticDecoder.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2802 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/JArithmeticDecoder.h
--rw-r--r--   0 matthijs   (501) staff       (20)   109724 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/JBIG2Stream.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4824 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/JBIG2Stream.h
--rw-r--r--   0 matthijs   (501) staff       (20)   107255 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/JPXStream.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    11092 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/JPXStream.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11674 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Lexer.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2035 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Lexer.h
--rw-r--r--   0 matthijs   (501) staff       (20)    21632 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Link.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    11370 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Link.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2191 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/NameToCharCode.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      726 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/NameToCharCode.h
--rw-r--r--   0 matthijs   (501) staff       (20)   117065 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/NameToUnicodeTable.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4471 2023-03-01 15:38:49.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Object.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     9081 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Object.h
--rw-r--r--   0 matthijs   (501) staff       (20)    12818 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/OptionalContent.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3617 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/OptionalContent.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4001 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Outline.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1774 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Outline.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4131 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/OutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     8935 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/OutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)    87382 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/PDF417Barcode.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      838 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/PDF417Barcode.h
--rw-r--r--   0 matthijs   (501) staff       (20)    51111 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/PDFCore.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    11579 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/PDFCore.h
--rw-r--r--   0 matthijs   (501) staff       (20)    16078 2023-03-01 14:01:13.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/PDFDoc.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     6774 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/PDFDoc.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2530 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/PDFDocEncoding.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      339 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/PDFDocEncoding.h
--rw-r--r--   0 matthijs   (501) staff       (20)   230372 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/PSOutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    19106 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/PSOutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)     3295 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/PSTokenizer.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      771 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/PSTokenizer.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13874 2023-03-01 15:38:49.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Page.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     6412 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Page.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8100 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Parser.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1674 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Parser.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8588 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/PreScanOutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4810 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/PreScanOutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10354 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/SecurityHandler.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3962 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/SecurityHandler.h
--rw-r--r--   0 matthijs   (501) staff       (20)    37941 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/ShadingImage.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3215 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/ShadingImage.h
--rw-r--r--   0 matthijs   (501) staff       (20)   127634 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/SplashOutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    10811 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/SplashOutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)    17471 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Stream-CCITT.h
--rw-r--r--   0 matthijs   (501) staff       (20)   131758 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Stream.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    31826 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Stream.h
--rw-r--r--   0 matthijs   (501) staff       (20)   183404 2023-04-13 10:47:47.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/TextOutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    27134 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/TextOutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4302 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/TextString.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1587 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/TextString.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13862 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/TileCache.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2041 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/TileCache.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10913 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/TileCompositor.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1895 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/TileCompositor.h
--rw-r--r--   0 matthijs   (501) staff       (20)    44674 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/TileMap.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     8164 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/TileMap.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4636 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/UTF8.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1408 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/UTF8.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6033 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/UnicodeMap.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2971 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/UnicodeMap.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11532 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/UnicodeMapTables.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5024 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/UnicodeRemapping.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1138 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/UnicodeRemapping.h
--rw-r--r--   0 matthijs   (501) staff       (20)    73118 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/UnicodeTypeTable.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      719 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/UnicodeTypeTable.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10592 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/WebFont.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2139 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/WebFont.h
--rw-r--r--   0 matthijs   (501) staff       (20)    18912 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/XFAScanner.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4518 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/XFAScanner.h
--rw-r--r--   0 matthijs   (501) staff       (20)    33740 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/XRef.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     5955 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/XRef.h
--rw-r--r--   0 matthijs   (501) staff       (20)    23997 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Zoox.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     6378 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/Zoox.h
--rw-r--r--   0 matthijs   (501) staff       (20)     3128 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/config.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5663 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/pdfdetach.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    12108 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/pdffonts.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4538 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/pdfimages.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    15031 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/pdfinfo.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     8525 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/pdftohtml.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    10873 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/pdftopng.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     7820 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/pdftoppm.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    11515 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/pdftops.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     9928 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf/pdftotext.cc
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-04-19 13:30:29.385176 xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/
--rw-r--r--   0 matthijs   (501) staff       (20)    30301 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/QtPDFCore.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     6596 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/QtPDFCore.h
--rw-r--r--   0 matthijs   (501) staff       (20)    14925 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/XpdfApp.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2452 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/XpdfApp.h
--rw-r--r--   0 matthijs   (501) staff       (20)   148791 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/XpdfViewer.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    18968 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/XpdfViewer.h
--rw-r--r--   0 matthijs   (501) staff       (20)    54075 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/XpdfWidget.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    39531 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/XpdfWidget.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13035 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      520 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1327 2022-04-18 21:11:23.000000 xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/xpdf.cc
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-04-19 13:30:29.388524 xpydf-0.1.1/src/xpydf/
--rw-r--r--   0 matthijs   (501) staff       (20)     6148 2023-04-06 11:10:10.000000 xpydf-0.1.1/src/xpydf/.DS_Store
--rw-r--r--   0 matthijs   (501) staff       (20)     1121 2023-04-12 11:54:25.000000 xpydf-0.1.1/src/xpydf/ImageInfoDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      941 2023-04-12 11:54:25.000000 xpydf-0.1.1/src/xpydf/ImageInfoDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4042 2023-04-19 13:00:59.000000 xpydf-0.1.1/src/xpydf/PdfLoader.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1039 2023-04-19 13:00:59.000000 xpydf-0.1.1/src/xpydf/PdfLoader.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6101 2023-04-19 13:00:59.000000 xpydf-0.1.1/src/xpydf/PdfLoaderWrapper.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2198 2023-04-12 11:54:25.000000 xpydf-0.1.1/src/xpydf/PyCppConversion.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      441 2023-04-12 11:54:25.000000 xpydf-0.1.1/src/xpydf/PyCppConversion.h
--rw-r--r--   0 matthijs   (501) staff       (20)        0 2023-04-12 11:54:25.000000 xpydf-0.1.1/src/xpydf/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)        0 2023-04-12 11:54:25.000000 xpydf-0.1.1/src/xpydf/__init__.pyi
--rw-r--r--   0 matthijs   (501) staff       (20)      630 2023-04-19 13:03:02.000000 xpydf-0.1.1/src/xpydf/cXpdfPython.pyi
--rw-r--r--   0 matthijs   (501) staff       (20)     4124 2023-04-19 13:03:54.000000 xpydf-0.1.1/src/xpydf/pdf_loader.py
--rw-r--r--   0 matthijs   (501) staff       (20)     1045 2023-04-19 13:03:32.000000 xpydf-0.1.1/src/xpydf/pdf_loader.pyi
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-04-19 13:30:29.389515 xpydf-0.1.1/src/xpydf.egg-info/
--rw-r--r--   0 matthijs   (501) staff       (20)     1133 2023-04-19 13:30:29.000000 xpydf-0.1.1/src/xpydf.egg-info/PKG-INFO
--rw-r--r--   0 matthijs   (501) staff       (20)     7602 2023-04-19 13:30:29.000000 xpydf-0.1.1/src/xpydf.egg-info/SOURCES.txt
--rw-r--r--   0 matthijs   (501) staff       (20)        1 2023-04-19 13:30:29.000000 xpydf-0.1.1/src/xpydf.egg-info/dependency_links.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       18 2023-04-19 13:30:29.000000 xpydf-0.1.1/src/xpydf.egg-info/top_level.txt
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-04-19 13:30:29.389735 xpydf-0.1.1/tests/
--rw-r--r--   0 matthijs   (501) staff       (20)     2849 2023-04-19 13:06:17.000000 xpydf-0.1.1/tests/test_pdf_loader.py
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 14:03:04.828535 xpydf-0.1.2/
+-rw-r--r--   0 matthijs   (501) staff       (20)    35149 2023-02-17 12:43:21.000000 xpydf-0.1.2/LICENSE
+-rw-r--r--   0 matthijs   (501) staff       (20)      118 2023-04-12 11:54:25.000000 xpydf-0.1.2/MANIFEST.in
+-rw-r--r--   0 matthijs   (501) staff       (20)     1133 2023-05-08 14:03:04.828638 xpydf-0.1.2/PKG-INFO
+-rw-r--r--   0 matthijs   (501) staff       (20)      240 2023-04-12 11:54:25.000000 xpydf-0.1.2/README.md
+-rw-r--r--   0 matthijs   (501) staff       (20)      789 2023-05-08 14:00:22.000000 xpydf-0.1.2/pyproject.toml
+-rw-r--r--   0 matthijs   (501) staff       (20)      840 2023-05-08 14:03:04.828942 xpydf-0.1.2/setup.cfg
+-rw-r--r--   0 matthijs   (501) staff       (20)     1998 2023-05-05 08:47:39.000000 xpydf-0.1.2/setup.py
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 14:03:04.732598 xpydf-0.1.2/src/
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 14:03:04.746826 xpydf-0.1.2/src/xpdf-4.04/
+-rw-r--r--   0 matthijs   (501) staff       (20)     8196 2023-04-13 10:48:09.000000 xpydf-0.1.2/src/xpdf-4.04/.DS_Store
+-rw-r--r--   0 matthijs   (501) staff       (20)     1330 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/ANNOUNCE
+-rw-r--r--   0 matthijs   (501) staff       (20)   139475 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/CHANGES
+-rw-r--r--   0 matthijs   (501) staff       (20)     1053 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/CMakeLists.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)    17982 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/COPYING
+-rw-r--r--   0 matthijs   (501) staff       (20)    35147 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/COPYING3
+-rw-r--r--   0 matthijs   (501) staff       (20)     5614 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/INSTALL
+-rw-r--r--   0 matthijs   (501) staff       (20)    13778 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/README
+-rw-r--r--   0 matthijs   (501) staff       (20)     2002 2023-04-12 11:54:25.000000 xpydf-0.1.2/src/xpdf-4.04/aconf.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1985 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/aconf.h.in
+-rw-r--r--   0 matthijs   (501) staff       (20)      941 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/aconf2.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    10676 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/cmake-config.txt
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 14:03:04.755121 xpydf-0.1.2/src/xpdf-4.04/fofi/
+-rw-r--r--   0 matthijs   (501) staff       (20)     3275 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiBase.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1344 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiBase.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    14853 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiEncodings.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1005 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiEncodings.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    21889 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiIdentifier.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1659 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiIdentifier.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    77637 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiTrueType.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     8227 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiTrueType.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8796 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiType1.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1434 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiType1.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    97383 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiType1C.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     8299 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiType1C.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 14:03:04.764702 xpydf-0.1.2/src/xpdf-4.04/goo/
+-rw-r--r--   0 matthijs   (501) staff       (20)     2748 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/goo/FixedPoint.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     7361 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/goo/FixedPoint.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     6201 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/goo/GHash.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2209 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/goo/GHash.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2276 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/goo/GList.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2724 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/goo/GList.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2629 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/goo/GMutex.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    17722 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/goo/GString.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4269 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/goo/GString.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2406 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/goo/Trace.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1171 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/goo/Trace.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    17381 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/goo/gfile.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4565 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/goo/gfile.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8259 2023-03-01 15:38:49.000000 xpydf-0.1.2/src/xpdf-4.04/goo/gmem.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2029 2023-03-01 15:38:49.000000 xpydf-0.1.2/src/xpdf-4.04/goo/gmem.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1005 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/goo/gmempp.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1714 2023-03-01 15:38:49.000000 xpydf-0.1.2/src/xpdf-4.04/goo/gmempp.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      562 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/goo/gtypes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1583 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/goo/parseargs.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 14:03:04.780015 xpydf-0.1.2/src/xpdf-4.04/splash/
+-rw-r--r--   0 matthijs   (501) staff       (20)   230071 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/Splash.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    20193 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/Splash.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     6603 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashBitmap.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2881 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashBitmap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    11473 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashClip.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4007 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashClip.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      930 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashErrorCodes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    13929 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashFTFont.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1345 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashFTFont.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8902 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashFTFontEngine.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2248 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashFTFontEngine.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4055 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashFTFontFile.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2241 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashFTFontFile.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4995 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashFont.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3666 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashFont.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     9673 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashFontEngine.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3358 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashFontEngine.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1589 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashFontFile.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2168 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashFontFile.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      603 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashFontFileID.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      687 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashFontFileID.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      758 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashGlyphBitmap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     9510 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashMath.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5135 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashPath.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3876 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashPath.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1042 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashPattern.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1447 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashPattern.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     9844 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashScreen.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2167 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashScreen.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     9521 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashState.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3669 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashState.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4155 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashTypes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    17088 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashXPath.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3761 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashXPath.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    12936 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashXPathScanner.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2482 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/splash/SplashXPathScanner.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 14:03:04.819873 xpydf-0.1.2/src/xpdf-4.04/xpdf/
+-rw-r--r--   0 matthijs   (501) staff       (20)   104168 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/AcroForm.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     5229 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/AcroForm.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    38840 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Annot.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4895 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Annot.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1385 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Array.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1400 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Array.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1387 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/BuiltinFont.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1080 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/BuiltinFont.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   229548 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/BuiltinFontTables.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      556 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/BuiltinFontTables.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    10417 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/CMap.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3178 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/CMap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    28608 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Catalog.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4742 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Catalog.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    19175 2023-04-13 10:47:41.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/CharCodeToUnicode.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3702 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/CharCodeToUnicode.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      526 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/CharTypes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8379 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/CompactFontTables.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    45644 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Decrypt.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3530 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Decrypt.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2993 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Dict.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2088 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Dict.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5247 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/DisplayState.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     5225 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/DisplayState.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2123 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Error.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1353 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Error.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      984 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/ErrorCodes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    21312 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/FontEncodingTables.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      564 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/FontEncodingTables.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    36553 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Function.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     6722 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Function.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   144837 2023-04-13 10:47:44.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Gfx.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    11911 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Gfx.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    65646 2023-04-13 10:47:45.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/GfxFont.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    12828 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/GfxFont.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   120789 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/GfxState.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    43452 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/GfxState.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   103543 2023-02-21 10:47:30.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/GlobalParams.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    23054 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/GlobalParams.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    34442 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/HTMLGen.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3131 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/HTMLGen.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    11293 2023-05-02 12:54:18.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/ImageOutputDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3942 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/ImageOutputDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8327 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/JArithmeticDecoder.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2802 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/JArithmeticDecoder.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   109724 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/JBIG2Stream.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4824 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/JBIG2Stream.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   107255 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/JPXStream.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    11092 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/JPXStream.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    11674 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Lexer.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2035 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Lexer.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    21632 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Link.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    11370 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Link.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2191 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/NameToCharCode.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      726 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/NameToCharCode.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   117065 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/NameToUnicodeTable.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4471 2023-03-01 15:38:49.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Object.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     9081 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Object.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    12818 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/OptionalContent.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3617 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/OptionalContent.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4001 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Outline.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1774 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Outline.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4131 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/OutputDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     8935 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/OutputDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    87382 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/PDF417Barcode.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      838 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/PDF417Barcode.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    51111 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/PDFCore.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    11579 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/PDFCore.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    16078 2023-03-01 14:01:13.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/PDFDoc.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     6774 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/PDFDoc.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2530 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/PDFDocEncoding.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      339 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/PDFDocEncoding.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   230372 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/PSOutputDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    19106 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/PSOutputDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     3295 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/PSTokenizer.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      771 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/PSTokenizer.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    13874 2023-03-01 15:38:49.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Page.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     6412 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Page.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8100 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Parser.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1674 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Parser.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8588 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/PreScanOutputDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4810 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/PreScanOutputDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    10354 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/SecurityHandler.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3962 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/SecurityHandler.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    37941 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/ShadingImage.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3215 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/ShadingImage.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   127634 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/SplashOutputDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    10811 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/SplashOutputDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    17471 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Stream-CCITT.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   131758 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Stream.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    31826 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Stream.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   183404 2023-04-13 10:47:47.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/TextOutputDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    27134 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/TextOutputDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4302 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/TextString.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1587 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/TextString.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    13862 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/TileCache.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2041 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/TileCache.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    10913 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/TileCompositor.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1895 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/TileCompositor.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    44674 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/TileMap.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     8164 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/TileMap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4636 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/UTF8.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1408 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/UTF8.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     6033 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/UnicodeMap.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2971 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/UnicodeMap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    11532 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/UnicodeMapTables.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5024 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/UnicodeRemapping.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1138 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/UnicodeRemapping.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    73118 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/UnicodeTypeTable.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      719 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/UnicodeTypeTable.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    10592 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/WebFont.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2139 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/WebFont.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    18912 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/XFAScanner.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4518 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/XFAScanner.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    33740 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/XRef.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     5955 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/XRef.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    23997 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Zoox.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     6378 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/Zoox.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     3128 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/config.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5663 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/pdfdetach.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    12108 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/pdffonts.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4538 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/pdfimages.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    15031 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/pdfinfo.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     8525 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/pdftohtml.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    10873 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/pdftopng.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     7820 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/pdftoppm.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    11515 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/pdftops.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     9928 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf/pdftotext.cc
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 14:03:04.823240 xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/
+-rw-r--r--   0 matthijs   (501) staff       (20)    30301 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/QtPDFCore.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     6596 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/QtPDFCore.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    14925 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/XpdfApp.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2452 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/XpdfApp.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   148791 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/XpdfViewer.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    18968 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/XpdfViewer.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    54075 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/XpdfWidget.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    39531 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/XpdfWidget.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    13035 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      520 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1327 2022-04-18 21:11:23.000000 xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/xpdf.cc
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 14:03:04.827242 xpydf-0.1.2/src/xpydf/
+-rw-r--r--   0 matthijs   (501) staff       (20)     6148 2023-05-01 14:11:15.000000 xpydf-0.1.2/src/xpydf/.DS_Store
+-rw-r--r--   0 matthijs   (501) staff       (20)     3555 2023-05-05 08:47:39.000000 xpydf-0.1.2/src/xpydf/ImageDataDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1095 2023-05-05 08:47:39.000000 xpydf-0.1.2/src/xpydf/ImageDataDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1121 2023-04-12 11:54:25.000000 xpydf-0.1.2/src/xpydf/ImageInfoDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      941 2023-04-12 11:54:25.000000 xpydf-0.1.2/src/xpydf/ImageInfoDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4729 2023-05-08 13:59:17.000000 xpydf-0.1.2/src/xpydf/PdfLoader.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1118 2023-05-08 13:59:17.000000 xpydf-0.1.2/src/xpydf/PdfLoader.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     7478 2023-05-08 13:59:17.000000 xpydf-0.1.2/src/xpydf/PdfLoaderWrapper.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2198 2023-04-12 11:54:25.000000 xpydf-0.1.2/src/xpydf/PyCppConversion.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      441 2023-04-12 11:54:25.000000 xpydf-0.1.2/src/xpydf/PyCppConversion.h
+-rw-r--r--   0 matthijs   (501) staff       (20)        0 2023-04-12 11:54:25.000000 xpydf-0.1.2/src/xpydf/__init__.py
+-rw-r--r--   0 matthijs   (501) staff       (20)        0 2023-04-12 11:54:25.000000 xpydf-0.1.2/src/xpydf/__init__.pyi
+-rw-r--r--   0 matthijs   (501) staff       (20)      760 2023-05-08 13:59:17.000000 xpydf-0.1.2/src/xpydf/cXpdfPython.pyi
+-rw-r--r--   0 matthijs   (501) staff       (20)     4684 2023-05-08 13:59:17.000000 xpydf-0.1.2/src/xpydf/pdf_loader.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     1159 2023-05-08 13:59:17.000000 xpydf-0.1.2/src/xpydf/pdf_loader.pyi
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 14:03:04.828184 xpydf-0.1.2/src/xpydf.egg-info/
+-rw-r--r--   0 matthijs   (501) staff       (20)     1133 2023-05-08 14:03:04.000000 xpydf-0.1.2/src/xpydf.egg-info/PKG-INFO
+-rw-r--r--   0 matthijs   (501) staff       (20)     7685 2023-05-08 14:03:04.000000 xpydf-0.1.2/src/xpydf.egg-info/SOURCES.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)        1 2023-05-08 14:03:04.000000 xpydf-0.1.2/src/xpydf.egg-info/dependency_links.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       14 2023-05-08 14:03:04.000000 xpydf-0.1.2/src/xpydf.egg-info/requires.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       18 2023-05-08 14:03:04.000000 xpydf-0.1.2/src/xpydf.egg-info/top_level.txt
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 14:03:04.828357 xpydf-0.1.2/tests/
+-rw-r--r--   0 matthijs   (501) staff       (20)     4094 2023-05-08 13:59:17.000000 xpydf-0.1.2/tests/test_pdf_loader.py
```

### Comparing `xpydf-0.1.1/LICENSE` & `xpydf-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/PKG-INFO` & `xpydf-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpydf
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python wrapper around the pdftotext and pdfimages functionalities of xpdf.
 Home-page: https://github.com/Bladieblah/xpdf-python
 Author: Matthijs Wesseling
 Author-email: Matthijs Wesseling <matthijs.wesseling@bigdatarepublic.nl>
 Maintainer: Matthijs Wesseling
 Maintainer-email: matthijs.wesseling@bigdatarepublic.nl
 License: GNU General Public License v3 (GPLv3)
```

### Comparing `xpydf-0.1.1/pyproject.toml` & `xpydf-0.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 [project]
 name = "xpydf"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name  = "Matthijs Wesseling", email = "matthijs.wesseling@bigdatarepublic.nl" },
 ]
 
 description = "Python wrapper around the pdftotext and pdfimages functionalities of xpdf."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 ]
+dependencies = [
+    "numpy == 1.21.6",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/Bladieblah/xpdf-python"
 "Bug Tracker" = "https://github.com/Bladieblah/xpdf-python/issues"
 
 [build-system]
 requires = [
     "setuptools>=42",
+    "numpy == 1.21.6",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [tool.black]
 line-length = 120
```

### Comparing `xpydf-0.1.1/setup.cfg` & `xpydf-0.1.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xpydf
-version = 0.1.1
+version = 0.1.2
 description = Python wrapper around the pdftotext functionality of xpdf.
 author = Matthijs Wesseling
 author_email = matthijs.wesseling@bigdatarepublic.nl
 maintainer = Matthijs Wesseling
 maintainer_email = matthijs.wesseling@bigdatarepublic.nl
 url = https://github.com/Bladieblah/xpdf-python
 license = GNU General Public License v3 (GPLv3)
@@ -19,13 +19,14 @@
 [options]
 package_dir = 
 	= src
 packages = xpydf
 requires = 
 	requires-python >= 3.7
 	setuptools >= 42
+	numpy >=1.21.6
 build_backend = setuptools.build_meta
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `xpydf-0.1.1/setup.py` & `xpydf-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from glob import glob
 from pathlib import Path
+import numpy as np
 
 from setuptools import Extension, setup
 
 python_dir = Path("src/xpydf")
 xpdf_dir = Path("src/xpdf-4.04/xpdf")
 splash_dir = Path("src/xpdf-4.04/splash")
 fofi_dir = Path("src/xpdf-4.04/fofi")
@@ -76,14 +77,15 @@
     include_dirs=[
         "src/xpdf-4.04",
         str(xpdf_dir),
         str(fofi_dir),
         str(splash_dir),
         str(goo_dir),
         str(python_dir),
+        np.get_include(),
     ],
     libraries = linker_libs,
     extra_compile_args=[
         "-std=c++11",
     ],
 )
```

### Comparing `xpydf-0.1.1/src/xpdf-4.04/.DS_Store` & `xpydf-0.1.2/src/xpdf-4.04/.DS_Store`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/ANNOUNCE` & `xpydf-0.1.2/src/xpdf-4.04/ANNOUNCE`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/CHANGES` & `xpydf-0.1.2/src/xpdf-4.04/CHANGES`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/CMakeLists.txt` & `xpydf-0.1.2/src/xpdf-4.04/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/COPYING` & `xpydf-0.1.2/src/xpdf-4.04/COPYING`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/COPYING3` & `xpydf-0.1.2/src/xpdf-4.04/COPYING3`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/INSTALL` & `xpydf-0.1.2/src/xpdf-4.04/INSTALL`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/README` & `xpydf-0.1.2/src/xpdf-4.04/README`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/aconf.h` & `xpydf-0.1.2/src/xpdf-4.04/aconf.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/aconf.h.in` & `xpydf-0.1.2/src/xpdf-4.04/aconf.h.in`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/aconf2.h` & `xpydf-0.1.2/src/xpdf-4.04/aconf2.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/cmake-config.txt` & `xpydf-0.1.2/src/xpdf-4.04/cmake-config.txt`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiBase.cc` & `xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiBase.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiBase.h` & `xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiBase.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiEncodings.cc` & `xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiEncodings.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiEncodings.h` & `xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiEncodings.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiIdentifier.cc` & `xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiIdentifier.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiIdentifier.h` & `xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiIdentifier.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiTrueType.cc` & `xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiTrueType.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiTrueType.h` & `xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiTrueType.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiType1.cc` & `xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiType1.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiType1.h` & `xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiType1.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiType1C.cc` & `xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiType1C.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/fofi/FoFiType1C.h` & `xpydf-0.1.2/src/xpdf-4.04/fofi/FoFiType1C.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/goo/FixedPoint.cc` & `xpydf-0.1.2/src/xpdf-4.04/goo/FixedPoint.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/goo/FixedPoint.h` & `xpydf-0.1.2/src/xpdf-4.04/goo/FixedPoint.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/goo/GHash.cc` & `xpydf-0.1.2/src/xpdf-4.04/goo/GHash.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/goo/GHash.h` & `xpydf-0.1.2/src/xpdf-4.04/goo/GHash.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/goo/GList.cc` & `xpydf-0.1.2/src/xpdf-4.04/goo/GList.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/goo/GList.h` & `xpydf-0.1.2/src/xpdf-4.04/goo/GList.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/goo/GMutex.h` & `xpydf-0.1.2/src/xpdf-4.04/goo/GMutex.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/goo/GString.cc` & `xpydf-0.1.2/src/xpdf-4.04/goo/GString.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/goo/GString.h` & `xpydf-0.1.2/src/xpdf-4.04/goo/GString.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/goo/Trace.cc` & `xpydf-0.1.2/src/xpdf-4.04/goo/Trace.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/goo/Trace.h` & `xpydf-0.1.2/src/xpdf-4.04/goo/Trace.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/goo/gfile.cc` & `xpydf-0.1.2/src/xpdf-4.04/goo/gfile.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/goo/gfile.h` & `xpydf-0.1.2/src/xpdf-4.04/goo/gfile.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/goo/gmem.cc` & `xpydf-0.1.2/src/xpdf-4.04/goo/gmem.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/goo/gmem.h` & `xpydf-0.1.2/src/xpdf-4.04/goo/gmem.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/goo/gmempp.cc` & `xpydf-0.1.2/src/xpdf-4.04/goo/gmempp.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/goo/gmempp.h` & `xpydf-0.1.2/src/xpdf-4.04/goo/gmempp.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/goo/gtypes.h` & `xpydf-0.1.2/src/xpdf-4.04/goo/gtypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/goo/parseargs.h` & `xpydf-0.1.2/src/xpdf-4.04/goo/parseargs.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/Splash.cc` & `xpydf-0.1.2/src/xpdf-4.04/splash/Splash.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/Splash.h` & `xpydf-0.1.2/src/xpdf-4.04/splash/Splash.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashBitmap.cc` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashBitmap.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashBitmap.h` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashBitmap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashClip.cc` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashClip.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashClip.h` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashClip.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashErrorCodes.h` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashErrorCodes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashFTFont.cc` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashFTFont.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashFTFont.h` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashFTFont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashFTFontEngine.cc` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashFTFontEngine.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashFTFontEngine.h` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashFTFontEngine.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashFTFontFile.cc` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashFTFontFile.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashFTFontFile.h` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashFTFontFile.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashFont.cc` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashFont.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashFont.h` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashFont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashFontEngine.cc` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashFontEngine.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashFontEngine.h` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashFontEngine.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashFontFile.cc` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashFontFile.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashFontFile.h` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashFontFile.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashFontFileID.cc` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashFontFileID.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashFontFileID.h` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashFontFileID.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashGlyphBitmap.h` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashGlyphBitmap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashMath.h` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashMath.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashPath.cc` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashPath.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashPath.h` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashPath.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashPattern.cc` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashPattern.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashPattern.h` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashPattern.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashScreen.cc` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashScreen.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashScreen.h` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashScreen.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashState.cc` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashState.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashState.h` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashState.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashTypes.h` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashTypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashXPath.cc` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashXPath.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashXPath.h` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashXPath.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashXPathScanner.cc` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashXPathScanner.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/splash/SplashXPathScanner.h` & `xpydf-0.1.2/src/xpdf-4.04/splash/SplashXPathScanner.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/AcroForm.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/AcroForm.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/AcroForm.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/AcroForm.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Annot.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Annot.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Annot.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Annot.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Array.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Array.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Array.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Array.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/BuiltinFont.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/BuiltinFont.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/BuiltinFont.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/BuiltinFont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/BuiltinFontTables.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/BuiltinFontTables.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/BuiltinFontTables.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/BuiltinFontTables.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/CMap.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/CMap.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/CMap.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/CMap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Catalog.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Catalog.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Catalog.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Catalog.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/CharCodeToUnicode.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/CharCodeToUnicode.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/CharCodeToUnicode.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/CharCodeToUnicode.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/CharTypes.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/CharTypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/CompactFontTables.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/CompactFontTables.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Decrypt.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Decrypt.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Decrypt.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Decrypt.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Dict.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Dict.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Dict.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Dict.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/DisplayState.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/DisplayState.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/DisplayState.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/DisplayState.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Error.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Error.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Error.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Error.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/ErrorCodes.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/ErrorCodes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/FontEncodingTables.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/FontEncodingTables.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/FontEncodingTables.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/FontEncodingTables.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Function.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Function.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Function.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Function.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Gfx.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Gfx.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Gfx.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Gfx.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/GfxFont.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/GfxFont.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/GfxFont.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/GfxFont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/GfxState.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/GfxState.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/GfxState.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/GfxState.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/GlobalParams.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/GlobalParams.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/GlobalParams.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/GlobalParams.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/HTMLGen.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/HTMLGen.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/HTMLGen.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/HTMLGen.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/ImageOutputDev.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/ImageOutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/ImageOutputDev.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/ImageOutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/JArithmeticDecoder.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/JArithmeticDecoder.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/JArithmeticDecoder.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/JArithmeticDecoder.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/JBIG2Stream.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/JBIG2Stream.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/JBIG2Stream.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/JBIG2Stream.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/JPXStream.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/JPXStream.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/JPXStream.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/JPXStream.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Lexer.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Lexer.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Lexer.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Lexer.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Link.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Link.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Link.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Link.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/NameToCharCode.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/NameToCharCode.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/NameToCharCode.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/NameToCharCode.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/NameToUnicodeTable.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/NameToUnicodeTable.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Object.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Object.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Object.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Object.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/OptionalContent.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/OptionalContent.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/OptionalContent.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/OptionalContent.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Outline.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Outline.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Outline.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Outline.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/OutputDev.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/OutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/OutputDev.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/OutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/PDF417Barcode.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/PDF417Barcode.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/PDF417Barcode.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/PDF417Barcode.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/PDFCore.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/PDFCore.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/PDFCore.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/PDFCore.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/PDFDoc.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/PDFDoc.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/PDFDoc.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/PDFDoc.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/PDFDocEncoding.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/PDFDocEncoding.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/PSOutputDev.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/PSOutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/PSOutputDev.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/PSOutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/PSTokenizer.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/PSTokenizer.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/PSTokenizer.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/PSTokenizer.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Page.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Page.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Page.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Page.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Parser.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Parser.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Parser.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Parser.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/PreScanOutputDev.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/PreScanOutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/PreScanOutputDev.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/PreScanOutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/SecurityHandler.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/SecurityHandler.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/SecurityHandler.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/SecurityHandler.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/ShadingImage.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/ShadingImage.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/ShadingImage.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/ShadingImage.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/SplashOutputDev.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/SplashOutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/SplashOutputDev.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/SplashOutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Stream-CCITT.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Stream-CCITT.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Stream.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Stream.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Stream.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Stream.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/TextOutputDev.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/TextOutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/TextOutputDev.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/TextOutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/TextString.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/TextString.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/TextString.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/TextString.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/TileCache.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/TileCache.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/TileCache.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/TileCache.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/TileCompositor.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/TileCompositor.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/TileCompositor.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/TileCompositor.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/TileMap.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/TileMap.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/TileMap.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/TileMap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/UTF8.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/UTF8.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/UTF8.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/UTF8.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/UnicodeMap.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/UnicodeMap.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/UnicodeMap.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/UnicodeMap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/UnicodeMapTables.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/UnicodeMapTables.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/UnicodeRemapping.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/UnicodeRemapping.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/UnicodeRemapping.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/UnicodeRemapping.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/UnicodeTypeTable.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/UnicodeTypeTable.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/UnicodeTypeTable.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/UnicodeTypeTable.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/WebFont.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/WebFont.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/WebFont.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/WebFont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/XFAScanner.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/XFAScanner.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/XFAScanner.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/XFAScanner.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/XRef.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/XRef.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/XRef.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/XRef.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Zoox.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Zoox.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/Zoox.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/Zoox.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/config.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/config.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/pdfdetach.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/pdfdetach.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/pdffonts.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/pdffonts.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/pdfimages.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/pdfimages.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/pdfinfo.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/pdfinfo.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/pdftohtml.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/pdftohtml.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/pdftopng.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/pdftopng.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/pdftoppm.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/pdftoppm.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/pdftops.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/pdftops.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf/pdftotext.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf/pdftotext.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/QtPDFCore.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/QtPDFCore.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/QtPDFCore.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/QtPDFCore.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/XpdfApp.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/XpdfApp.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/XpdfApp.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/XpdfApp.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/XpdfViewer.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/XpdfViewer.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/XpdfViewer.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/XpdfViewer.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/XpdfWidget.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/XpdfWidget.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/XpdfWidget.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/XpdfWidget.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.h` & `xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpdf-4.04/xpdf-qt/xpdf.cc` & `xpydf-0.1.2/src/xpdf-4.04/xpdf-qt/xpdf.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpydf/ImageInfoDev.cc` & `xpydf-0.1.2/src/xpydf/ImageInfoDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpydf/ImageInfoDev.h` & `xpydf-0.1.2/src/xpydf/ImageInfoDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpydf/PdfLoader.cc` & `xpydf-0.1.2/src/xpydf/PdfLoader.cc`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 #include "CharTypes.h"
 #include "UnicodeMap.h"
 #include "TextString.h"
 #include "Error.h"
 #include "config.h"
 
 #include "PdfLoader.h"
+#include "ImageDataDev.h"
 #include "ImageInfoDev.h"
 
 
 static void outputToStringStream(void *stream, const char *text, int len) {
   ((std::stringstream *)stream)->write(text, len);
 }
 
@@ -126,15 +127,15 @@
 
   Object::memCheck(stderr);
   gMemReport(stderr);
 
   return pages;
 }
 
-std::vector<PageImageInfo> PdfLoader::extractImages() {
+std::vector<PageImageInfo> PdfLoader::extractPageInfo() {
   ImageInfoDev *imageOut;
   int firstPage, lastPage;
   std::vector<PageImageInfo> pagesInfo;
   char dummyFile[1] = "";
 
   if (!doc->isOk()) {
     goto err;
@@ -170,17 +171,51 @@
 
   Object::memCheck(stderr);
   gMemReport(stderr);
 
   return pagesInfo;
 }
 
+std::vector<Image> PdfLoader::extractImages(int pageNum) {
+  ImageDataDev *imageOut;
+  std::vector<Image> images;
+  char dummyFile[1] = "";
+
+  if (!doc->isOk()) {
+    goto err;
+  }
+  
+  imageOut = new ImageDataDev(dummyFile, gFalse, gFalse, gTrue, &images);
+
+  if (imageOut->isOk()) {
+    doc->displayPages(imageOut, pageNum, pageNum, 72, 72, 0, gFalse, gTrue, gFalse);
+  }
+
+  delete imageOut;
+ err:
+
+  Object::memCheck(stderr);
+  gMemReport(stderr);
+
+  return images;
+}
+
 bool PdfLoader::isOk() {
   if (!doc) {
     return false;
   }  
   return (bool)doc->isOk();
 }
 
 int PdfLoader::getErrorCode() {
   return (int)doc->getErrorCode();
 }
+
+int main() {
+  char filename[100] = "tests/test_data/xpdf_tests.pdf";
+  LoaderConfig config;
+  PdfLoader loader = PdfLoader(config, filename);
+
+  loader.extractImages(1);
+
+  return 0;
+}
```

### Comparing `xpydf-0.1.1/src/xpydf/PdfLoader.h` & `xpydf-0.1.2/src/xpydf/PdfLoader.h`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 #include <vector>
 
 #include "gtypes.h"
 #include "GlobalParams.h"
 #include "PDFDoc.h"
 #include "TextOutputDev.h"
 
+#include "ImageDataDev.h"
 #include "ImageInfoDev.h"
 
 typedef struct LoaderConfig {
   GBool clipText = gFalse;
   GBool discardDiag = gTrue;
   GBool discardRotatedText = gTrue;
   GBool noPageBreaks = gFalse;
@@ -31,15 +32,16 @@
 } PageImageInfo;
 
 class PdfLoader {
 public:
     PdfLoader(LoaderConfig config, char *fileName, char *ownerPw = NULL, char *userPw = NULL);
     ~PdfLoader();
     std::vector<std::string> extractText();
-    std::vector<PageImageInfo> extractImages();
+    std::vector<PageImageInfo> extractPageInfo();
+    std::vector<Image> extractImages(int pageNum);
     bool isOk();
     int getErrorCode();
 private:
   TextOutputControl textOutControl;
   PDFDoc *doc;
   GString *textFileName;
 };
```

### Comparing `xpydf-0.1.1/src/xpydf/PdfLoaderWrapper.cc` & `xpydf-0.1.2/src/xpydf/PdfLoaderWrapper.cc`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 #include <stdio.h>
 #include <iostream>
 #include <string>
 #include <vector>
 
-#include "Python.h"
+#include <Python.h>
+#define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
+#include <numpy/arrayobject.h>
+
 #include "PdfLoader.h"
 #include "PyCppConversion.h"
 #include "ErrorCodes.h"
 
 using namespace std;
 
 // ------------------- Class wrappers -------------------
@@ -106,27 +109,60 @@
     PdfLoader *loader = (PdfLoader *)PyCapsule_GetPointer(loaderCapsule, "loaderPtr");
     vector<string> result = loader->extractText();
     
     PyObject *converted = vectorStringToList(result);
     return Py_BuildValue("O", converted);
 }
 
-PyObject *extractImages(PyObject *self, PyObject *args) {
+PyObject *extractPageInfo(PyObject *self, PyObject *args) {
     vector<string> res;
     
     PyObject *loaderCapsule;
     PyArg_ParseTuple(args, "O", &loaderCapsule);
 
     PdfLoader *loader = (PdfLoader *)PyCapsule_GetPointer(loaderCapsule, "loaderPtr");
-    vector<PageImageInfo> result = loader->extractImages();
+    vector<PageImageInfo> result = loader->extractPageInfo();
     
     PyObject *converted = vectorPagesToList(result);
     return Py_BuildValue("O", converted);
 }
 
+PyObject *extractImages(PyObject *self, PyObject *args) {
+    vector<string> res;
+    
+    PyObject *loaderCapsule;
+    int pageNum;
+    PyArg_ParseTuple(args, "Oi", &loaderCapsule, &pageNum);
+
+    PdfLoader *loader = (PdfLoader *)PyCapsule_GetPointer(loaderCapsule, "loaderPtr");
+    vector<Image> images = loader->extractImages(pageNum);
+    
+    PyObject *imageList = PyList_New(images.size());
+    PyObject *array;
+    
+    for (size_t i = 0; i < images.size(); i++) {
+      Image image = images[i];
+      npy_intp dims[1] = {image.size};
+      array = PyArray_SimpleNewFromData(1, dims, NPY_UINT8, image.data);
+      
+      // Only reshape P6 images, P4 contain multiple pixels per byte
+      if (image.image_type == IMAGE_TYPES::P5) {
+        PyObject *shape = Py_BuildValue("ii", image.height, image.width);
+        array = PyArray_Reshape((PyArrayObject *)array, shape);
+      } else if (image.image_type == IMAGE_TYPES::P6) {
+        PyObject *shape = Py_BuildValue("iii", image.height, image.width, 3);
+        array = PyArray_Reshape((PyArrayObject *)array, shape);
+      }
+
+      PyList_SetItem(imageList, i, array);
+    }
+
+    return Py_BuildValue("O", imageList);
+}
+
 PyObject *deleteObject(PyObject *self, PyObject *args) {
     PyObject *loaderCapsule;
     PyArg_ParseTuple(args, "O", &loaderCapsule);
     
     PdfLoader *loader = (PdfLoader *)PyCapsule_GetPointer(loaderCapsule, "loaderPtr");
     
     if (loader) {
@@ -147,17 +183,21 @@
       construct, METH_VARARGS,
      "Create `PdfLoader` object"},
     
     {"extractText",
       extractText, METH_VARARGS,
      "Extract text as bytes"},
     
+    {"extractPageInfo",
+      extractPageInfo, METH_VARARGS,
+     "Extract image metadata"},
+    
     {"extractImages",
       extractImages, METH_VARARGS,
-     "Extract image metadata"},
+     "Extract images"},
     
     {"deleteObject",
       deleteObject, METH_VARARGS,
      "Delete `PdfLoader` object"},
 
     {NULL, NULL, 0, NULL}      // Last function description must be empty.
                                // Otherwise, it will create seg fault while
@@ -177,9 +217,10 @@
    // Docstring for the module.
    -1,                   // Used by sub-interpreters, if you do not know what
                          // it is then you do not need it, keep -1 .
    cXpdfPythonFunctions
 };
 
 PyMODINIT_FUNC PyInit_cXpdfPython(void) {
+    import_array();
     return PyModule_Create(&cXpdfPythonModule);
 }
```

### Comparing `xpydf-0.1.1/src/xpydf/PyCppConversion.cc` & `xpydf-0.1.2/src/xpydf/PyCppConversion.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.1/src/xpydf/cXpdfPython.pyi` & `xpydf-0.1.2/src/xpydf/cXpdfPython.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import List, Optional
+
+from typing import Any, List, Optional
+import numpy.typing as npt
 
 from xpydf.pdf_loader import PageInfo
 
 class XpdfPythonCapsule: ...
 
 def construct(
     filename: str,
@@ -14,9 +16,10 @@
     mode: int,
     mapNumericCharNames: bool = False,
     mapUnknownCharNames: bool = True,
     ownerPw: Optional[str] = None,
     userPw: Optional[str] = None,
 ) -> XpdfPythonCapsule: ...
 def extractText(capsule: XpdfPythonCapsule) -> List[bytes]: ...
-def extractImages(capsule: XpdfPythonCapsule) -> List[PageInfo]: ...
+def extractPageInfo(capsule: XpdfPythonCapsule) -> List[PageInfo]: ...
+def extractImages(capsule: XpdfPythonCapsule, page_number: int) -> List[npt.NDArray[Any]]: ...
 def deleteObject(capsule: XpdfPythonCapsule) -> None: ...
```

### Comparing `xpydf-0.1.1/src/xpydf/pdf_loader.py` & `xpydf-0.1.2/src/xpydf/pdf_loader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import List, Optional, TypedDict
+from typing import Any, List, Optional, TypedDict
 
 import cXpdfPython
+import numpy.typing as npt
 
 
 class ImageInfo(TypedDict):
     """Container for image metadata
 
     Attributes
     ----------
@@ -128,25 +129,44 @@
         -------
         List[str]
             The text of each page, decoded as unicode
         """
         pages = self.extract_bytes()
         return [page.decode("unicode_escape", "replace") for page in pages]
 
-    def extract_images(self) -> List[PageInfo]:
+    def extract_page_info(self) -> List[PageInfo]:
         """Return image related metadata from the pdf
 
         Returns
         -------
         List[PageInfo]
             A PageInfo object for each page
         """
         images: List[PageInfo] = []
         if self.capsule is not None:
-            images = cXpdfPython.extractImages(self.capsule)
+            images = cXpdfPython.extractPageInfo(self.capsule)
+
+        return images
+
+    def extract_images(self, page_number: int) -> List[npt.NDArray[Any]]:
+        """Extract raw image data from a page, as a numpy array.
+
+        Parameters
+        ----------
+        page_number : int
+            Page to extract images from
+
+        Returns
+        -------
+        List[npt.NDArray[Any]]
+            Image data.
+        """
+        images: List[npt.NDArray[Any]] = []
+        if self.capsule is not None:
+            images = cXpdfPython.extractImages(self.capsule, page_number)
 
         return images
 
     def __del__(self):
         if self.capsule:
             cXpdfPython.deleteObject(self.capsule)
             del self.capsule
```

### Comparing `xpydf-0.1.1/src/xpydf/pdf_loader.pyi` & `xpydf-0.1.2/src/xpydf/pdf_loader.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import List, Optional, TypedDict
+from typing import Any, List, Optional, TypedDict
+
+import numpy.typing as npt
 
 class XpdfPythonCapsule: ...
 
 class ImageInfo(TypedDict):
     width: float
     height: float
 
@@ -30,9 +32,10 @@
         map_numeric_char_names: bool = False,
         map_unknown_char_names: bool = True,
         owner_password: Optional[str] = None,
         user_password: Optional[str] = None,
     ) -> None: ...
     def extract_bytes(self) -> List[bytes]: ...
     def extract_strings(self) -> List[str]: ...
-    def extract_images(self) -> List[PageInfo]: ...
+    def extract_page_info(self) -> List[PageInfo]: ...
+    def extract_images(self, page_number: int) -> List[npt.NDArray[Any]]: ...
     def __del__(self) -> None: ...
```

### Comparing `xpydf-0.1.1/src/xpydf.egg-info/PKG-INFO` & `xpydf-0.1.2/src/xpydf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpydf
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python wrapper around the pdftotext and pdfimages functionalities of xpdf.
 Home-page: https://github.com/Bladieblah/xpdf-python
 Author: Matthijs Wesseling
 Author-email: Matthijs Wesseling <matthijs.wesseling@bigdatarepublic.nl>
 Maintainer: Matthijs Wesseling
 Maintainer-email: matthijs.wesseling@bigdatarepublic.nl
 License: GNU General Public License v3 (GPLv3)
```

### Comparing `xpydf-0.1.1/src/xpydf.egg-info/SOURCES.txt` & `xpydf-0.1.2/src/xpydf.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -219,14 +219,16 @@
 src/xpdf-4.04/xpdf-qt/XpdfViewer.h
 src/xpdf-4.04/xpdf-qt/XpdfWidget.cc
 src/xpdf-4.04/xpdf-qt/XpdfWidget.h
 src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.cc
 src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.h
 src/xpdf-4.04/xpdf-qt/xpdf.cc
 src/xpydf/.DS_Store
+src/xpydf/ImageDataDev.cc
+src/xpydf/ImageDataDev.h
 src/xpydf/ImageInfoDev.cc
 src/xpydf/ImageInfoDev.h
 src/xpydf/PdfLoader.cc
 src/xpydf/PdfLoader.h
 src/xpydf/PdfLoaderWrapper.cc
 src/xpydf/PyCppConversion.cc
 src/xpydf/PyCppConversion.h
@@ -234,9 +236,10 @@
 src/xpydf/__init__.pyi
 src/xpydf/cXpdfPython.pyi
 src/xpydf/pdf_loader.py
 src/xpydf/pdf_loader.pyi
 src/xpydf.egg-info/PKG-INFO
 src/xpydf.egg-info/SOURCES.txt
 src/xpydf.egg-info/dependency_links.txt
+src/xpydf.egg-info/requires.txt
 src/xpydf.egg-info/top_level.txt
 tests/test_pdf_loader.py
```

