# Comparing `tmp/python-gdcm-3.0.9.0.tar.gz` & `tmp/python-gdcm-3.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-gdcm-3.0.9.0.tar", last modified: Tue Jun 29 18:10:46 2021, max compression
+gzip compressed data, was "python-gdcm-3.0.9.1.tar", last modified: Mon Jul 26 22:48:01 2021, max compression
```

## Comparing `python-gdcm-3.0.9.0.tar` & `python-gdcm-3.0.9.1.tar`

### file list

```diff
@@ -1,1639 +1,1639 @@
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.159193 python-gdcm-3.0.9.0/
--rw-r--r--   0 thiago    (1000) thiago    (1000)       66 2021-02-26 23:15:40.000000 python-gdcm-3.0.9.0/MANIFEST.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3045 2021-06-29 18:10:46.159193 python-gdcm-3.0.9.0/PKG-INFO
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1383 2021-03-12 15:24:02.000000 python-gdcm-3.0.9.0/README.md
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.020193 python-gdcm-3.0.9.0/_gdcm/
--rw-r--r--   0 thiago    (1000) thiago    (1000)        0 2021-02-26 18:58:47.000000 python-gdcm-3.0.9.0/_gdcm/__init__.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3148 2021-02-26 18:58:47.000000 python-gdcm-3.0.9.0/gdcm.py
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.022193 python-gdcm-3.0.9.0/gdcm_src/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2001 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/.clang-format
--rw-r--r--   0 thiago    (1000) thiago    (1000)       33 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/.git
--rw-r--r--   0 thiago    (1000) thiago    (1000)      177 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/.gitattributes
--rw-r--r--   0 thiago    (1000) thiago    (1000)      126 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/.gitignore
--rw-r--r--   0 thiago    (1000) thiago    (1000)       93 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/.gitmodules
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6809 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/.travis.yml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1934 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/AUTHORS
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.022193 python-gdcm-3.0.9.0/gdcm_src/Applications/
--rw-r--r--   0 thiago    (1000) thiago    (1000)       22 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/CMakeLists.txt
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.024193 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/
--rw-r--r--   0 thiago    (1000) thiago    (1000)    10329 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3248 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/deflate.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1406 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcm.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    24845 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmanon.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)      778 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmcheck.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    48643 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmconv.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)      103 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmdictdump.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8419 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmdiff.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    50674 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmdump.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2018 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmfile.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8936 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmgendir.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    40757 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmimg.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    23254 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcminfo.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1149 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmkey.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4528 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmoverlay.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    18038 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmpap3.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    19092 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmpdf.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11310 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmraw.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8632 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmscanner.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    24310 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmscu.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    32064 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmstream.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    53280 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmtar.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    24999 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmxml.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)      580 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/pdf2dcm.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    37725 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/puff.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1506 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/puff.h
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.024193 python-gdcm-3.0.9.0/gdcm_src/Applications/Python/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2319 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Python/README
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2983 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Python/accessdata.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3675 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Python/images.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1049 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Python/lib.py
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)     5740 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/Python/wado.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)      462 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Applications/README.txt
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.028193 python-gdcm-3.0.9.0/gdcm_src/CMake/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2024 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/CMakeCSharpCompiler.cmake.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3428 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/CMakeCSharpInformation.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2396 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/CMakeDetermineCSharpCompiler.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2325 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/CMakeTestCSharpCompiler.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1326 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/COPYING-CMAKE-SCRIPTS
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2731 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/CTestCustom.ctest.in
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.028193 python-gdcm-3.0.9.0/gdcm_src/CMake/ExportConfiguration/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4040 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/ExportConfiguration/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1779 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/ExportConfiguration/GDCMConfig.cmake.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)      803 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/ExportConfiguration/GDCMConfigVersion.cmake.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)      866 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/ExportConfiguration/UseGDCM.cmake.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1522 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindACTIVIZ.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)      647 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindCSharp.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)      903 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindCharLS.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4123 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindDCMTK.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1392 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindDICOM3TOOLS.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1823 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindDotNETFrameworkSDK.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1073 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindJSON.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2890 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindJavaProperties.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)      400 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindKAKADU.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)      977 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindKWStyle.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1088 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindLJPEG.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1012 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindMAGIC.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2582 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindMONO.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1793 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindMd5sum.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1221 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindOpenJPEG.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4523 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindOpenSSL.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1015 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindPAPYRUS3.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1370 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindPHP5.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)      832 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindPVRGJPEG.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)      959 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindPoppler.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)      599 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindRsync.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)      930 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindSOCKET++.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)      598 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindSQLITE3.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1733 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/FindUUID.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1284 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/GetSystemProperty.java
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2594 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/InstallMacros.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2453 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/InstallRequiredVTKLibraries.cmake
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.028193 python-gdcm-3.0.9.0/gdcm_src/CMake/Release/
--rw-r--r--   0 thiago    (1000) thiago    (1000)        0 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/Release/README.cygwin.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)        0 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/Release/cygwin-package.sh.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)        0 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/Release/cygwin-patch.diff.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)        0 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/Release/cygwin-setup.hint.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1397 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/Toolchain-gcc-arm-linux-gnueabi.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1273 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/Toolchain-gcc-m32.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1723 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/Toolchain-gcc-powerpc.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1138 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/Toolchain-mingw32.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1042 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/Toolchain-mingw64.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6861 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/UseCSharp.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2325 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/UseCSharpTest.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)      773 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/UseCopyright.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6494 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/UseDebian.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)      230 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/UseDotNETFrameworkSDK.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3244 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/UseJavaTest.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1542 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/UseMONO.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3539 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/UsePythonTest.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)      506 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/dcmqrscp.cfg.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2673 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CMake/gdcmValgrind.supp
--rw-r--r--   0 thiago    (1000) thiago    (1000)    40125 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)      229 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/CTestConfig.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1863 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Copyright.txt
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.028193 python-gdcm-3.0.9.0/gdcm_src/Examples/
--rw-r--r--   0 thiago    (1000) thiago    (1000)      561 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/CMakeLists.txt
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.030193 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4169 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/BasicAnonymizer.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2534 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/BasicImageAnonymizer.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2167 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9910 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/ClinicalTrialIdentificationWorkflow.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2664 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/CompressLossyJPEG.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2739 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/DecompressImage.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4425 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/DecompressImageMultiframe.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3038 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/DecompressJPEGFile.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2233 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/DumpCSA.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2370 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/ExtractEncapsulatedFile.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3280 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/ExtractImageRegion.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3349 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/ExtractImageRegionWithLUT.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2670 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/ExtractOneFrame.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1667 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/FileAnonymize.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6879 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/FileChangeTS.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7039 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/FileChangeTSLossy.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1965 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/FileStreaming.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1728 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/GenerateDICOMDIR.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2673 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/GetArray.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1708 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/ManipulateFile.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13712 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/MpegVideoInfo.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2297 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/NewSequence.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3006 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/ReformatFile.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1926 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/RescaleImage.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2202 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/ScanDirectory.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1161 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/SendFileSCU.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2383 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/SimplePrint.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1763 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/SimplePrintPatientName.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)      973 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/SortImage2.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3765 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/StandardizeFiles.cs
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.035193 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5632 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5096 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/CStoreQtProgress.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2838 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ChangePrivateTags.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2719 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ChangeSequenceUltrasound.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3144 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/CheckBigEndianBug.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2846 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ClinicalTrialAnnotate.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2310 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/CompressImage.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4290 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ConvertToQImage.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2047 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/CreateARGBImage.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2046 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/CreateCMYKImage.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2595 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/CreateJPIPDataSet.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3005 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DeriveSeries.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1847 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DiffFile.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8029 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DiscriminateVolume.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9908 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DumpADAC.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    20848 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DumpExamCard.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    17452 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DumpGEMSMovieGroup.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4798 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DumpImageHeaderInfo.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13224 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DumpPhilipsECHO.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2543 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DumpSiemensBase64.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3890 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DumpToSQLITE3.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3266 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DumpToshibaDTI.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4072 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DumpVisusChange.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7037 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DuplicatePCDE.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6156 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ELSCINT1WaveToText.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1751 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/EmptyMask.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2388 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/EncapsulateFileInRawData.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2060 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ExtractEncryptedContent.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2848 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ExtractIconFromFile.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    14393 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/Extracting_All_Resolution.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7200 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/Fake_Image_Using_Stream_Image_Writer.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3969 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/FixBrokenJ2K.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6637 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/FixJAIBugJPEGLS.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2298 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/FixOrientation.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4564 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/GenAllVR.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5271 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/GenFakeIdentifyFile.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4043 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/GenFakeImage.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2875 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/GenLongSeqs.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3134 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/GenSeqs.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2109 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/GenerateStandardSOPClasses.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4146 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/GetJPEGSamplePrecision.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4250 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/GetSequenceUltrasound.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6467 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/GetSubSequenceData.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2616 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/HelloVizWorld.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2431 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/HelloWorld.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5882 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/LargeVRDSExplicit.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1896 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/MakeTemplate.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2597 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/MergeTwoFiles.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    23542 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/MrProtocol.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3194 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/PatchFile.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1234 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/PrintLUT.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2274 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/PublicDict.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1471 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/QIDO-RS.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8215 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ReadAndDumpDICOMDIR.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    14929 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ReadAndDumpDICOMDIR2.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3506 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ReadAndPrintAttributes.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1506 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ReadExplicitLengthSQIVR.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4935 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ReadGEMSSDO.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1898 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ReadMultiTimesException.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3322 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ReadUTF8QtDir.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4153 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/SimpleScanner.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3427 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/SortImage.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8838 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/StreamImageReaderTest.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3807 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/TemplateEmptyImage.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2488 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/TraverseModules.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5185 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/VolumeSorter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5182 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/csa2img.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3519 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/iU22tomultisc.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7848 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/pmsct_rgb1.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7606 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/rle2img.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1569 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/uid_unique.cxx
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.036193 python-gdcm-3.0.9.0/gdcm_src/Examples/Java/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1447 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Java/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2071 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Java/DecompressImage.java
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2279 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Java/DecompressPixmap.java
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2575 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Java/ExtractImageRegion.java
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2006 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Java/FileAnonymize.java
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1269 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Java/HelloSimple.java
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2897 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Java/ReadFiles.java
--rw-r--r--   0 thiago    (1000) thiago    (1000)    10761 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Java/ScanDirectory.java
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2323 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Java/SimplePrint.java
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.037193 python-gdcm-3.0.9.0/gdcm_src/Examples/PHP/
--rw-r--r--   0 thiago    (1000) thiago    (1000)       80 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/PHP/README.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1200 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/PHP/export_pnm.php
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2600 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/PHP/hello_world.php
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1355 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/PHP/modify_file.php
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1349 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/PHP/qido.php
--rw-r--r--   0 thiago    (1000) thiago    (1000)      973 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/PHP/rewrite_header.php
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.038193 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1122 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/AddPrivateAttribute.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)        0 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2912 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/ConvertMPL.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2527 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/ConvertNumpy.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3015 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/ConvertPIL.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4303 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/CreateRAWStorage.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1969 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/DecompressImage.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3888 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/DumbAnonymizer.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2650 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/ExtractImageRegion.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1350 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/FindAllPatientName.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1886 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/FixCommaBug.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1878 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/GetPortionCSAHeader.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1604 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/HelloWorld.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3918 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/ManipulateFile.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2284 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/ManipulateSequence.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1715 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/MergeFile.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1657 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/NewSequence.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1841 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/PhilipsPrivateRescaleInterceptSlope.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2328 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/PlaySound.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1170 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/PrivateDict.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3151 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/ReWriteSCAsMR.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8113 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/ReadAndDumpDICOMDIR.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1330 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/RemovePrivateTags.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1945 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/ScanDirectory.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1104 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/SortImage.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3758 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Examples/Python/WriteBuffer.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1965 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/INSTALL.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1954 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/PACKAGER
--rw-r--r--   0 thiago    (1000) thiago    (1000)      257 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/README.Copyright.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1908 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/README.md
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.038193 python-gdcm-3.0.9.0/gdcm_src/Source/
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.038193 python-gdcm-3.0.9.0/gdcm_src/Source/Attribute/
--rw-r--r--   0 thiago    (1000) thiago    (1000)        0 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Attribute/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)        9 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Attribute/README.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)      293 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/CMakeLists.txt
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.045193 python-gdcm-3.0.9.0/gdcm_src/Source/Common/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6487 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)       82 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/README.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2960 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmASN1.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1216 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmASN1.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5505 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmBase64.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1911 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmBase64.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4127 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmBoxRegion.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2135 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmBoxRegion.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      634 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmByteSwap.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1490 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmByteSwap.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4657 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmByteSwap.txx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1082 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmCAPICryptoFactory.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)      931 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmCAPICryptoFactory.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    16467 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmCAPICryptographicMessageSyntax.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2020 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmCAPICryptographicMessageSyntax.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      696 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmCommand.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5140 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmCommand.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5891 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmConfigure.h.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1871 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmCryptoFactory.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1911 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmCryptoFactory.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      608 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmCryptographicMessageSyntax.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1806 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmCryptographicMessageSyntax.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      633 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmDataEvent.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1601 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmDataEvent.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      615 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmDeflateStream.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)      678 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmDeflateStream.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5687 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmDirectory.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3170 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmDirectory.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1130 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmDummyValueGenerator.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1179 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmDummyValueGenerator.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      795 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmEvent.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3149 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmEvent.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      634 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmException.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3339 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmException.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      637 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmFileNameEvent.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1576 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmFileNameEvent.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4395 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmFilename.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2319 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmFilename.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3371 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmFilenameGenerator.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2153 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmFilenameGenerator.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3336 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmLegacyMacro.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3259 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmMD5.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1442 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmMD5.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      896 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmObject.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3052 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmObject.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      898 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmOpenSSLCryptoFactory.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1204 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmOpenSSLCryptoFactory.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7130 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmOpenSSLCryptographicMessageSyntax.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2141 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmOpenSSLCryptographicMessageSyntax.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      666 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmOpenSSLP7CryptoFactory.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1151 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmOpenSSLP7CryptoFactory.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11907 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmOpenSSLP7CryptographicMessageSyntax.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2429 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmOpenSSLP7CryptographicMessageSyntax.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      637 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmProgressEvent.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1522 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmProgressEvent.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      763 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmRegion.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1718 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmRegion.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2860 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSHA1.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1425 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSHA1.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2944 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSmartPointer.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1508 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmStaticAssert.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      631 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmString.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4510 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmString.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5504 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSubject.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2501 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSubject.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1434 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSwapCode.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1555 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSwapCode.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1638 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSwapper.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6287 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSwapper.txx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    27870 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSystem.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5534 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSystem.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6555 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmTerminal.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1595 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmTerminal.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      993 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmTestDriver.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    17376 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmTesting.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4528 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmTesting.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3382 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmTrace.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9125 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmTrace.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2002 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmTypes.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1744 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmUnpacker12Bits.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1760 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmUnpacker12Bits.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      948 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmVersion.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1481 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmVersion.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3164 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmWin32.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    10890 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/zipstreamimpl.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    24174 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/Common/zipstreamimpl.hpp
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.058193 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9091 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/06_03_list.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3036 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/Agfa.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3728 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1730 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/COPYRIGHT.dicom3tools
--rw-r--r--   0 thiago    (1000) thiago    (1000)    14472 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/CSADefaultDicts.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)    41260 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/CSAHeader.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)    14508 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/DefaultDicts.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13747 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/DefaultPrivateDicts.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)   230891 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/HarvestedPrivate.xml
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)    11884 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/ParseDicts.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)   601260 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/Part6.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13466 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/Part6.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13212 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/Part67.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6339 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/Part6PDF.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6121 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/Part6todcm4che.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1140 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/Part7.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8270 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/Part7a.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3075 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/Part7b.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2104 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/PartToGDCM.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)      934 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/README.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6062 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/Siemens.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2215 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/TagKeywords.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4468 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/TagToType.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2686 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/TagToVR.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3567 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/UIDToC++.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)    36696 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/UIDs.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1113 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/VM.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)    12348 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/cp699.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8667 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/dcmtk.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3546 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/dicom3tools.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)   196316 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/dicomhdr.html
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1844 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/dicomhdr.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)    33659 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmCSAHeaderDefaultDicts.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2872 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmCSAHeaderDict.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2805 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmCSAHeaderDictEntry.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)  1194766 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmDefaultDicts.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3339 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmDefaultGroupNames.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9699 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmDict.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    10532 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmDictConverter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2095 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmDictConverter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2962 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmDictEntry.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4393 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmDictEntry.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3802 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmDicts.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2230 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmDicts.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5376 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmGlobal.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3449 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmGlobal.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1298 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmGroupDict.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2349 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmGroupDict.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1702 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmPrepDict.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3290 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmPrepGroupName.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)   824526 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmPrivateDefaultDicts.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)       91 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmRoot.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11378 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmSOPClassUIDToIOD.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1506 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmSOPClassUIDToIOD.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)   251256 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmTagKeywords.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)  1049572 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmTagToType.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    34653 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmUIDs.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    62655 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmUIDs.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1304 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmconformancetests.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)      874 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/getname.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)      991 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/getowner.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1190 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/getretired.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1229 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/order.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3918 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/priv2html.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)   908801 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/privatedicts.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2995 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/redo.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2760 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/redo2.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)      729 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/sort.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1772 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/uppercase.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1601 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/vital.xml
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.066193 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2846 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)       55 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/README.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)    33191 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmAttribute.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3340 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmBasicOffsetTable.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2508 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmByteBuffer.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4443 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmByteSwapFilter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1183 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmByteSwapFilter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8758 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmByteValue.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7040 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmByteValue.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1901 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCP246ExplicitDataElement.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1627 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCP246ExplicitDataElement.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6671 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCP246ExplicitDataElement.txx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4602 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCSAElement.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    51796 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCSAHeader.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4845 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCSAHeader.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1123 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCodeString.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3761 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCodeString.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6347 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataElement.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9125 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataElement.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4855 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataSet.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11013 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataSet.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    17355 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataSet.txx
--rw-r--r--   0 thiago    (1000) thiago    (1000)      636 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataSetEvent.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1522 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataSetEvent.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    25371 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmElement.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2303 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitDataElement.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1391 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitDataElement.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    16681 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitDataElement.txx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1918 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitImplicitDataElement.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1856 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitImplicitDataElement.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    15059 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitImplicitDataElement.txx
--rw-r--r--   0 thiago    (1000) thiago    (1000)      935 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFile.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2162 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFile.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    29687 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFileMetaInformation.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5097 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFileMetaInformation.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1013 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFileSet.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1662 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFileSet.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1201 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFragment.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6273 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFragment.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      711 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFragment.txx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2017 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmImplicitDataElement.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1527 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmImplicitDataElement.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    19182 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmImplicitDataElement.txx
--rw-r--r--   0 thiago    (1000) thiago    (1000)      654 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmItem.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9885 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmItem.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1864 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmItem.txx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1850 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmLO.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    22959 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmMediaStorage.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7914 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmMediaStorage.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5921 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmMrProtocol.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2226 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmMrProtocol.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1738 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPDBElement.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8224 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPDBHeader.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3001 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPDBHeader.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      642 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmParseException.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2379 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmParseException.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2251 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmParser.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4075 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmParser.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2067 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPreamble.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1943 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPreamble.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2937 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPrivateTag.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2565 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPrivateTag.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    25113 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmReader.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4496 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmReader.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1504 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmReader.strict.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3995 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfFragments.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11390 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfFragments.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      756 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfFragments.txx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2004 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfItems.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8605 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfItems.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1251 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfItems.txx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2812 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTag.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9961 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTag.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)   113222 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTagToVR.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)      734 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTagToVR.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8659 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTransferSyntax.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4442 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTransferSyntax.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1900 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitDataElement.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1492 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitDataElement.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6337 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitDataElement.txx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1924 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitImplicitDataElement.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1842 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitImplicitDataElement.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2137 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitImplicitDataElement.txx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3304 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVL.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8480 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVM.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5128 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVM.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13182 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVR.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11086 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVR.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1906 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVR16ExplicitDataElement.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1605 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVR16ExplicitDataElement.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9062 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVR16ExplicitDataElement.txx
--rw-r--r--   0 thiago    (1000) thiago    (1000)      711 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmValue.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1395 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmValue.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      681 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmValue.txx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1036 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmValueIO.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2308 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmValueIO.txx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4670 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmWriter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3104 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmWriter.h
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.076193 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2153 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/CMakeLists.txt
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)    18708 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/ParseAttributes.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)  2336000 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/Part3.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)    41130 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/Part3.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8311 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/Part3New.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)    21272 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/Part4.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6396 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/Part4.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1889 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/Part4ToC++.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)      487 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/README.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2168 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/Template.xml.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)    20305 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/ValueRepresentation.xsd
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1108 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/extract.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)      613 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmDefinedTerms.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1598 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmDefinedTerms.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    12108 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmDefs.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2052 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmDefs.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      617 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmEnumeratedValues.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1569 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmEnumeratedValues.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1522 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmIOD.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1899 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmIOD.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1217 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmIODEntry.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3040 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmIODEntry.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2074 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmIODs.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2289 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmMacro.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3010 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmMacro.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2635 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmMacroEntry.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      608 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmMacros.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2106 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmMacros.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3691 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmModule.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3230 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmModule.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2583 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmModuleEntry.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      609 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmModules.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2122 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmModules.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      602 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmNestedModuleEntries.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1925 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmNestedModuleEntries.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      607 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmPatient.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)      904 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmPatient.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      607 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmSeries.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)      814 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmSeries.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      606 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmStudy.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)      861 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmStudy.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      630 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmTable.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1611 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmTable.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1090 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmTableEntry.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13943 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmTableReader.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3053 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmTableReader.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      692 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmTables.h.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1050 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmType.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1900 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmType.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1153 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmUsage.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2670 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmUsage.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5425 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmXMLDictReader.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1426 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmXMLDictReader.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6306 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmXMLPrivateDictReader.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1495 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmXMLPrivateDictReader.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2113 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/getelements.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2113 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/ma2html.xsl
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5856 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/ma2pdf.xsl
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.091193 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6609 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3679 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/FileMetaInformation.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6444 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/README.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1392 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/TODO.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)      638 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAnonymizeEvent.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1556 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAnonymizeEvent.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    37487 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAnonymizer.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6841 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAnonymizer.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      618 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmApplicationEntity.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1850 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmApplicationEntity.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      812 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAudioCodec.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1047 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAudioCodec.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    36184 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmBitmap.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5967 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmBitmap.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1291 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmBitmapToBitmapFilter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1262 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmBitmapToBitmapFilter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      809 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmCodec.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1322 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmCoder.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1643 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmConstCharWrapper.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    17226 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmCurve.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2622 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmCurve.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      609 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDICOMDIR.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1027 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDICOMDIR.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    39052 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDICOMDIRGenerator.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3943 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDICOMDIRGenerator.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11928 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDataSetHelper.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1247 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDataSetHelper.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1199 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDecoder.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1176 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDeltaEncodingCodec.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1104 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDeltaEncodingCodec.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    16004 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDictPrinter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1070 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDictPrinter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3988 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDirectionCosines.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1982 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDirectionCosines.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    10775 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDirectoryHelper.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3596 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDirectoryHelper.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      608 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDumper.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1030 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDumper.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    15380 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEmptyMaskGenerator.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2706 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEmptyMaskGenerator.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      621 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEncapsulatedDocument.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)      874 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEncapsulatedDocument.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3987 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEquipmentManufacturer.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1039 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEquipmentManufacturer.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      610 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFiducials.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)      808 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFiducials.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    16306 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileAnonymizer.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2920 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileAnonymizer.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    15260 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileChangeTransferSyntax.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2257 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileChangeTransferSyntax.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3858 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileDecompressLookupTable.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1554 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileDecompressLookupTable.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    15433 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileDerivation.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3262 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileDerivation.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6609 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileExplicitFilter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2497 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileExplicitFilter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    25738 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileStreamer.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4241 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileStreamer.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    10468 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIPPSorter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4732 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIPPSorter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3968 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImage.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2526 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImage.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    18763 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImageFilter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2431 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImageFilter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    32738 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImageGenerator.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3168 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImageGenerator.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4202 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImage.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3757 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImage.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3649 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageApplyLookupTable.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1221 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageApplyLookupTable.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    10161 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangePhotometricInterpretation.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3820 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangePhotometricInterpretation.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4612 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangePlanarConfiguration.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2772 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangePlanarConfiguration.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    20383 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangeTransferSyntax.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3382 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangeTransferSyntax.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    20953 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageCodec.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4773 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageCodec.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      976 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageConverter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1297 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageConverter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3240 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageFragmentSplitter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1571 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageFragmentSplitter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)   109059 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageHelper.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7091 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageHelper.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4480 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageReader.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1604 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageReader.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    16862 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageRegionReader.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2653 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageRegionReader.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      940 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageToImageFilter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1189 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageToImageFilter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    14224 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageWriter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1905 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageWriter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      885 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG12Codec.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1346 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG12Codec.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      885 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG16Codec.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1338 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG16Codec.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    53281 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG2000Codec.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3179 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG2000Codec.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      878 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG8Codec.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1337 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG8Codec.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    55015 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEGBITSCodec.hxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    21598 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEGCodec.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3438 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEGCodec.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    17200 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEGLSCodec.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3175 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEGLSCodec.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    30175 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJSON.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1148 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJSON.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6324 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmKAKADUCodec.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1135 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmKAKADUCodec.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    21951 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmLookupTable.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3639 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmLookupTable.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3435 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmMeshPrimitive.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2397 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmMeshPrimitive.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3806 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmOrientation.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1817 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmOrientation.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    18989 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmOverlay.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3822 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmOverlay.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      800 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPDFCodec.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1039 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPDFCodec.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2784 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPGXCodec.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1277 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPGXCodec.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9336 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPNMCodec.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1595 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPNMCodec.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5528 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPVRGCodec.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1496 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPVRGCodec.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      612 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPersonName.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2511 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPersonName.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5806 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPhotometricInterpretation.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2817 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPhotometricInterpretation.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7358 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixelFormat.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7667 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixelFormat.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2752 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmap.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2485 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmap.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    49226 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapReader.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2098 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapReader.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1032 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapToPixmapFilter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1190 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapToPixmapFilter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    28937 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapWriter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2056 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapWriter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    32806 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPrinter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2909 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPrinter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6168 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRAWCodec.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1548 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRAWCodec.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    29497 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRLECodec.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2693 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRLECodec.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    17021 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRescaler.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4682 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRescaler.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13221 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmScanner.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7559 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmScanner.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5664 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegment.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4283 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegment.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1033 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentHelper.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2226 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentHelper.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11333 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentReader.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1625 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentReader.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13570 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentWriter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1568 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentWriter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7596 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentedPaletteColorLookupTable.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1210 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentedPaletteColorLookupTable.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    14055 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSerieHelper.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3170 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSerieHelper.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6130 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSimpleSubjectWatcher.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2952 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSimpleSubjectWatcher.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4413 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSorter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2608 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSorter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3644 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSpacing.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5170 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSpacing.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      613 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSpectroscopy.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)      832 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSpectroscopy.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    12942 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSplitMosaicFilter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2889 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSplitMosaicFilter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    16667 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStreamImageReader.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5525 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStreamImageReader.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    17213 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStreamImageWriter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6340 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStreamImageWriter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13733 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStrictScanner.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6765 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStrictScanner.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    15620 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStringFilter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2901 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStringFilter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11908 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurface.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7783 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurface.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4376 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceHelper.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6464 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceHelper.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    23677 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceReader.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1300 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceReader.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    38471 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceWriter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1664 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceWriter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3041 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmTagPath.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1491 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmTagPath.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7820 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmUIDGenerator.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3491 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmUIDGenerator.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2458 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmUUIDGenerator.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1062 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmUUIDGenerator.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1416 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmValidate.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)      973 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmValidate.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      609 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmWaveform.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)      808 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmWaveform.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    16112 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmXMLPrinter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3620 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmXMLPrinter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    15885 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcm_j2k.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5936 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcm_jp2.h
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.102193 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3167 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1312 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/README.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4316 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAAbortPDU.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1510 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAAbortPDU.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9036 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateACPDU.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3340 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateACPDU.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3816 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateRJPDU.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1427 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateRJPDU.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9538 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateRQPDU.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5580 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateRQPDU.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2331 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmARTIMTimer.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2518 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmARTIMTimer.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2251 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAReleaseRPPDU.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1353 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAReleaseRPPDU.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2268 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAReleaseRQPDU.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1353 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAReleaseRQPDU.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3281 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAbstractSyntax.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1820 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAbstractSyntax.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2631 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmApplicationContext.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1598 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmApplicationContext.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3527 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAsynchronousOperationsWindowSub.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1407 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAsynchronousOperationsWindowSub.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2437 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseCompositeMessage.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2278 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseNormalizedMessage.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1993 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmBasePDU.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9074 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseQuery.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2723 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseQuery.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3304 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseRootQuery.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4419 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseRootQuery.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2468 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCEchoMessages.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1486 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCEchoMessages.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3722 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCFindMessages.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1684 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCFindMessages.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4092 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCMoveMessages.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1912 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCMoveMessages.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    10553 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCStoreMessages.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1847 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCStoreMessages.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      988 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCommandDataSet.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1753 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCommandDataSet.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2595 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCompositeMessageFactory.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2476 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCompositeMessageFactory.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    15215 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCompositeNetworkFunctions.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5993 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCompositeNetworkFunctions.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2675 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmDIMSE.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8703 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmFindPatientRootQuery.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1266 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmFindPatientRootQuery.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7918 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmFindStudyRootQuery.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1483 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmFindStudyRootQuery.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2571 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationClassUIDSub.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1303 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationClassUIDSub.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1281 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationUIDSub.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1170 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationUIDSub.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2578 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationVersionNameSub.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1313 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationVersionNameSub.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2589 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmMaximumLengthSub.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1427 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmMaximumLengthSub.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6312 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmModalityPerformedProcedureStepCreateQuery.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1350 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmModalityPerformedProcedureStepCreateQuery.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2216 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmModalityPerformedProcedureStepSetQuery.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1329 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmModalityPerformedProcedureStepSetQuery.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8866 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmMovePatientRootQuery.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1278 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmMovePatientRootQuery.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7546 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmMoveStudyRootQuery.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1258 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmMoveStudyRootQuery.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1393 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNActionMessages.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1309 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNActionMessages.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3000 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNCreateMessages.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1309 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNCreateMessages.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1393 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNDeleteMessages.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1309 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNDeleteMessages.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1488 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNEventReportMessages.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1354 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNEventReportMessages.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1384 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNGetMessages.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1282 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNGetMessages.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2740 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNSetMessages.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1282 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNSetMessages.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1982 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNetworkEvents.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2740 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNetworkStateID.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2779 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNormalizedMessageFactory.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1681 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNormalizedMessageFactory.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9804 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNormalizedNetworkFunctions.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3102 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNormalizedNetworkFunctions.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11783 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPDUFactory.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3479 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPDUFactory.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3697 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPDataTFPDU.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1981 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPDataTFPDU.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1684 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContext.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2266 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContext.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3396 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextAC.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1816 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextAC.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5348 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextGenerator.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3884 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextGenerator.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5736 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextRQ.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3257 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextRQ.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7392 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationDataValue.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2765 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationDataValue.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1351 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryBase.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3549 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryBase.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8610 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryFactory.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3647 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryFactory.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2977 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryImage.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1521 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryImage.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3078 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryPatient.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1505 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryPatient.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2397 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQuerySeries.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1499 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQuerySeries.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4748 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryStudy.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1494 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryStudy.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4357 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmRoleSelectionSub.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1392 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmRoleSelectionSub.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3585 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmSOPClassExtendedNegociationSub.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1602 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmSOPClassExtendedNegociationSub.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4345 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmServiceClassApplicationInformation.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1314 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmServiceClassApplicationInformation.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    42855 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmServiceClassUser.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4048 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmServiceClassUser.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3060 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmTransferSyntaxSub.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1693 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmTransferSyntaxSub.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3468 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULAction.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3412 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAA.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3813 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAA.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9911 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAE.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3844 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAE.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5256 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAR.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4267 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAR.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9152 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionDT.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1774 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionDT.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1289 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULBasicCallback.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2086 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULBasicCallback.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9409 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnection.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5412 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnection.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2520 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnectionCallback.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3686 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnectionInfo.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2675 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnectionInfo.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    52315 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnectionManager.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7098 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnectionManager.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2696 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULEvent.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    21423 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULTransitionTable.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3552 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULTransitionTable.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2463 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULWritingCallback.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1854 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULWritingCallback.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8215 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmUserInformation.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2191 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmUserInformation.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3164 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmWLMFindQuery.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1328 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmWLMFindQuery.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    21774 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/TODO
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.103193 python-gdcm-3.0.9.0/gdcm_src/Utilities/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4619 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/CMakeLists.txt
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.103193 python-gdcm-3.0.9.0/gdcm_src/Utilities/KWStyle/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1505 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/KWStyle/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)      254 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/KWStyle/GDCM.kws.xml.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)      582 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/KWStyle/GDCMFiles.txt.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)      564 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/KWStyle/GDCMHeader.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)       33 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/KWStyle/GDCMOverwrite.txt
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.104193 python-gdcm-3.0.9.0/gdcm_src/Utilities/Release/
--rw-r--r--   0 thiago    (1000) thiago    (1000)      341 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/Release/README.md
--rw-r--r--   0 thiago    (1000) thiago    (1000)      103 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/Release/README.txt
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)     2776 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/Release/bootstrap.sh
--rw-r--r--   0 thiago    (1000) thiago    (1000)      568 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/Release/config.linux
--rw-r--r--   0 thiago    (1000) thiago    (1000)      570 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/Release/config.win32
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      129 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/Release/makerelease.sh
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)     1985 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/Release/release.bat
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)     6692 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/Release/release.sh
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)     6661 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/Release/upload.sh
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.107193 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/
--rw-r--r--   0 thiago    (1000) thiago    (1000)       39 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/.NoDartCoverage
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.108193 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Applications/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1608 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Applications/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2878 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Applications/gdcm2pnm.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    32683 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Applications/gdcm2vtk.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    30657 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Applications/gdcmviewer.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3401 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/AssemblyInfo.cs.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)    33668 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)       10 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/CscArgs.txt.in
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.108193 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/
--rw-r--r--   0 thiago    (1000) thiago    (1000)      244 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/CMakeLists.txt
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.108193 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2334 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4396 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/HelloActiviz.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3111 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/HelloActiviz2.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1433 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/HelloActiviz3.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1431 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/HelloActiviz4.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3061 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/HelloActiviz5.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1811 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/HelloVTKWorld.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1680 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/HelloVTKWorld2.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3422 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/MetaImageMD5Activiz.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2016 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/RefCounting.cs
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.110193 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2206 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2827 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/Compute3DSpacing.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2078 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/Convert16BitsTo8Bits.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2570 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/ConvertMultiFrameToSingleFrame.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2141 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/ConvertRGBToLuminance.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2722 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/ConvertSingleBitTo8Bits.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3495 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/CreateFakePET.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4113 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/CreateFakeRTDOSE.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7553 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/GenerateRTSTRUCT.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2552 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/MagnifyFile.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    15377 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmorthoplanes.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4698 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmreslice.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13377 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmrtionplan.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    12052 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmrtplan.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3916 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmscene.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4177 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmtexture.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2936 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmvolume.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2544 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/offscreenimage.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    20078 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/reslicesphere.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3777 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/rtstructapp.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7595 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/threadgdcm.cxx
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.110193 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Java/
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13048 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Java/AWTMedical3.java
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2213 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Java/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3463 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Java/HelloVTKWorld.java
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5693 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Java/MIPViewer.java
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4396 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Java/MPRViewer.java
--rw-r--r--   0 thiago    (1000) thiago    (1000)    10464 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Java/MPRViewer2.java
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3111 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Java/ReadSeriesIntoVTK.java
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.111193 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/PHP/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1657 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/PHP/generate_png.php
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.111193 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Python/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5458 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Python/CastConvertPhilips.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1429 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Python/headsq2dcm.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)      570 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/GDCMImageGUI.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1430 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/GDCMImageReader.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)      144 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/JavaDependencies.cmake.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8386 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/MummySettings.xml.in
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.111193 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/
--rw-r--r--   0 thiago    (1000) thiago    (1000)      213 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/CMakeLists.txt
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.112193 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2603 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2230 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageActor.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3179 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5842 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader1.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3022 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader2_1.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3261 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader2_2.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6015 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader2_3.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5310 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader3.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4924 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader4.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2208 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReaderIsLossy.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1936 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageViewer.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9169 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageWriter1.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5805 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageWriter2.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1966 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageWriterIsLossy.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4935 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMMetaImageWriter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4941 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMMetaImageWriter2.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2309 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMPolyDataReader.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7314 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMThreadedImageReader.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7167 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMThreadedImageReader2.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2730 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkImageChangeInformation.cxx
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.112193 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Java/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1720 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Java/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1255 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Java/TestvtkGDCMImageReader.java
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.113193 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Python/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1644 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Python/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1338 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Python/TestMultiframeGrayscaleWordSecondaryCaptureImageStorage.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1821 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Python/TestvtkGDCMImageReader.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1273 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Python/TestvtkGDCMImageReader2.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1301 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Python/TestvtkGDCMImageWriter.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4221 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Python/TestvtkGDCMThreadedImageReader.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3427 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Python/TestvtkGDCMThreadedImageReader2.py
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.113193 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/VTK4/
--rw-r--r--   0 thiago    (1000) thiago    (1000)    28837 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/VTK4/vtkMedicalImageProperties.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13579 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/VTK4/vtkMedicalImageProperties.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1747 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/VTK4/vtkStringArray.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1521 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/VTK4/vtkStringArray.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)       75 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/dllexportconf.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)      336 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/gccxml.cxx.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)       20 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/manifest.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)    56647 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMImageReader.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11929 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMImageReader.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    46426 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMImageReader2.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    10399 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMImageReader2.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1036 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMImageReader_Extra.cs
--rw-r--r--   0 thiago    (1000) thiago    (1000)    44149 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMImageWriter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6284 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMImageWriter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2343 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMMedicalImageProperties.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    12413 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMMedicalImageProperties.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    34698 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMPolyDataReader.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2969 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMPolyDataReader.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    31645 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMPolyDataWriter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2904 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMPolyDataWriter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    25079 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMTesting.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1526 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMTesting.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    20966 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMThreadedImageReader.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3712 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMThreadedImageReader.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    12912 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMThreadedImageReader2.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5110 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMThreadedImageReader2.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    26341 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImageColorViewer.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8955 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImageColorViewer.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    10635 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImageMapToColors16.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4299 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImageMapToColors16.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    15092 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImageMapToWindowLevelColors2.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3707 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImageMapToWindowLevelColors2.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4983 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImagePlanarComponentsToComponents.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2860 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImagePlanarComponentsToComponents.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4668 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImageRGBToYBR.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2179 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImageRGBToYBR.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6182 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImageYBRToRGB.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2179 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImageYBRToRGB.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13969 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkLookupTable16.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2880 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkLookupTable16.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    12424 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkRTStructSetProperties.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4318 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkRTStructSetProperties.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    15979 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkgdcm.i
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2157 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkgdcm.py
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.113193 python-gdcm-3.0.9.0/gdcm_src/Utilities/dicom3tools/
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)     1200 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/dicom3tools/process.sh
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.114193 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13703 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)      572 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/README
--rw-r--r--   0 thiago    (1000) thiago    (1000)      286 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/README.txt.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)       29 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/TestsList.txt.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1870 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/authors.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)   105666 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/doxyfile.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1555 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/footer.html
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.117193 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2984 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcm2pnm.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8469 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcm2vtk.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13995 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmanon.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)    18207 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmconv.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2894 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmdiff.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)    50466 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmdump.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4232 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmgendir.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)    12430 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmimg.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7160 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcminfo.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3950 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmpap3.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7394 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmpdf.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8136 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmraw.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4195 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmscanner.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)    14578 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmscu.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6584 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmtar.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4252 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmviewer.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3457 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmxml.xml
--rw-r--r--   0 thiago    (1000) thiago    (1000)      391 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/patchtex.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)       15 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/version.txt.in
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.117193 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/vtk/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5234 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/vtk/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)    12758 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/vtk/doc_makeall.sh.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6400 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/vtk/doxyfile.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)      838 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcm_charls.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      784 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcm_expat.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      966 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcm_ljpeg12.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      966 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcm_ljpeg16.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      958 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcm_ljpeg8.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      766 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcm_md5.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      815 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcm_openjpeg.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      778 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcm_uuid.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      841 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcm_zlib.h
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.119193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/
--rw-r--r--   0 thiago    (1000) thiago    (1000)       39 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/.NoDartCoverage
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3283 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1500 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/License.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1537 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/README.GDCM.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5000 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/charls.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5188 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/colortransform.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2230 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/context.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2347 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/contextrunmode.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8146 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/decoderstrategy.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3681 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/defaulttraits.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5756 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/encoderstrategy.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11241 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/interface.cpp
--rw-r--r--   0 thiago    (1000) thiago    (1000)      490 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/jlscodecfactory.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      678 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/jpegimagedatasegment.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5769 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/jpegls.cpp
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2602 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/jpegmarkercode.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4956 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/jpegmarkersegment.cpp
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3014 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/jpegmarkersegment.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      447 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/jpegsegment.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    12357 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/jpegstreamreader.cpp
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1644 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/jpegstreamreader.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2267 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/jpegstreamwriter.cpp
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2580 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/jpegstreamwriter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1272 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/lookuptable.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3478 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/losslesstraits.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    12857 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/processline.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11515 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/publictypes.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    28568 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/scan.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1239 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/styleanddesign.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4408 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/util.h
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.120193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/
--rw-r--r--   0 thiago    (1000) thiago    (1000)       39 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/.NoDartCoverage
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1416 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1208 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/COPYING
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7934 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/Changes
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4728 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/README
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.121193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/doc/
--rw-r--r--   0 thiago    (1000) thiago    (1000)    92234 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/doc/reference.html
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1340 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/doc/style.css
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7900 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/doc/xmlwf.1
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13884 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/doc/xmlwf.sgml
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.121193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/examples/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1631 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/examples/elements.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2405 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/examples/outline.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2470 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/expat_config.h.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5672 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/expat_mangle.h.in
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.122193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/
--rw-r--r--   0 thiago    (1000) thiago    (1000)      711 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1813 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/ascii.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1760 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/asciitab.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    40313 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/expat.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3562 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/expat_external.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1830 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/iasciitab.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2003 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/internal.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1813 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/latin1tab.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7050 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/nametab.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1763 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/utf8tab.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)   192313 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/xmlparse.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    32423 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/xmlrole.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3023 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/xmlrole.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    41138 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/xmltok.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11184 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/xmltok.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    44476 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/xmltok_impl.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)      661 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/xmltok_impl.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2950 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/xmltok_ns.c
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.123193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/
--rw-r--r--   0 thiago    (1000) thiago    (1000)      572 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/README.txt
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.123193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/benchmark/
--rw-r--r--   0 thiago    (1000) thiago    (1000)      546 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/benchmark/README.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2788 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/benchmark/benchmark.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3038 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/chardata.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)      791 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/chardata.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4098 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/minicheck.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2061 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/minicheck.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    46055 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/runtests.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)      185 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/runtestspp.cpp
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)     3512 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/xmltest.sh
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.124193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)     1302 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/codepage.c
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      196 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/codepage.h
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)     2912 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/ct.c
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      500 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/filemap.h
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)     1457 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/readfilemap.c
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)     1114 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/unixfilemap.c
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)     2143 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/win32filemap.c
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)     5768 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlfile.c
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      509 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlfile.h
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)     3218 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlmime.c
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      493 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlmime.h
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      825 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/xmltchar.h
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      224 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlurl.h
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)    20812 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlwf.c
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)     8813 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlwin32url.cxx
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.133193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/
--rw-r--r--   0 thiago    (1000) thiago    (1000)       39 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/.NoDartCoverage
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.133193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/12/
--rw-r--r--   0 thiago    (1000) thiago    (1000)      994 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/12/CMakeLists.txt
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.133193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/16/
--rw-r--r--   0 thiago    (1000) thiago    (1000)      988 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/16/CMakeLists.txt
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.133193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/8/
--rw-r--r--   0 thiago    (1000) thiago    (1000)      988 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/8/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4759 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11510 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/COPYRIGHT.dcmtk
--rw-r--r--   0 thiago    (1000) thiago    (1000)    15141 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/Jfif.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)    19942 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/README
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3153 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/README.GDCM.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9284 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/change.log
--rw-r--r--   0 thiago    (1000) thiago    (1000)      825 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/dcmtk.sh
--rw-r--r--   0 thiago    (1000) thiago    (1000)    17112 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/example.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9279 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/filelist.doc
--rw-r--r--   0 thiago    (1000) thiago    (1000)    52070 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/install.doc
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9148 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcapimin.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5896 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcapistd.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    16975 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jccoefct.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    14959 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jccolor.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    12883 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcdctmgr.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    14345 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcdiffct.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9255 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jchuff.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1734 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jchuff.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1855 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcinit.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    18923 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jclhuff.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1960 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jclossls.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1971 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jclossy.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9598 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcmainct.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    18002 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcmarker.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    22262 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcmaster.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1085 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcodec.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3110 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcomapi.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5372 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jconfig.doc
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1648 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jconfig.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    23643 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcparam.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    25962 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcphuff.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8365 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcpred.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    12259 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcprepct.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    19062 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcsample.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1497 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcscale.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    20094 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcshuff.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    15168 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jctrans.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    12873 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdapimin.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9387 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdapistd.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5265 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdatadst.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7636 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdatasrc.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    25907 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdcoefct.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13594 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdcolor.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7083 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdct.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8480 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jddctmgr.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13180 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jddiffct.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11554 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdhuff.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9317 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdhuff.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    12176 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdinput.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9709 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdlhuff.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2408 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdlossls.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7434 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdlossy.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    20702 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdmainct.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    41541 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdmarker.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    16164 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdmaster.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    14083 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdmerge.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    21204 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdphuff.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9922 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdpostct.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8041 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdpred.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    16602 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdsample.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3137 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdscale.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11642 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdshuff.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4969 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdtrans.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7822 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jerror.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    14869 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jerror.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5446 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jfdctflt.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7538 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jfdctfst.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11045 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jfdctint.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8466 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jidctflt.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13220 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jidctfst.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    14778 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jidctint.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13474 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jidctred.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3250 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jinclude.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4824 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jlossls.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3902 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jlossy.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    42776 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jmemmgr.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3013 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jmemnobs.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5259 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jmemsrc.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8329 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jmemsys.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    14136 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jmorecfg.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      957 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jpegcmake.h.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)    15146 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jpegint.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    47947 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jpeglib.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    31572 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jquant1.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    48684 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jquant2.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5260 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jutils.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)      360 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jversion.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)   159668 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/libjpeg.doc
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8703 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/mangle_jpeg.h.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)    55618 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/structure.doc
--rw-r--r--   0 thiago    (1000) thiago    (1000)    27170 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/usage.doc
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9759 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/wizard.doc
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.134193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmmd5/
--rw-r--r--   0 thiago    (1000) thiago    (1000)       39 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmmd5/.NoDartCoverage
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2292 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmmd5/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)      965 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmmd5/COPYING
--rw-r--r--   0 thiago    (1000) thiago    (1000)      318 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmmd5/README.GDCM.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)    12434 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmmd5/md5.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3765 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmmd5/md5.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1215 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmmd5/md5_mangle.h.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1625 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmmd5/md5cmp.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4259 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmmd5/md5main.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2594 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmmd5/tst2md5.c
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.134193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/
--rw-r--r--   0 thiago    (1000) thiago    (1000)    14506 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2112 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/LICENSE
--rw-r--r--   0 thiago    (1000) thiago    (1000)      888 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/README.GDCM.txt
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.135193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1215 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/CTestCustom.cmake.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)      928 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/EnsureFileInclude.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)      332 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/FindCPPCHECK.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)      612 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/FindFCGI.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)      170 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/FindJPYLYZER.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)      483 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/FindKAKADU.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1131 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/FindLCMS.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1168 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/FindLCMS2.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)      165 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/JPIPTestDriver.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3004 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/OpenJPEGCPack.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1535 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/OpenJPEGConfig.cmake.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)      305 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/TestFileOffsetBits.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)      615 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/TestLargeFiles.c.cmake.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5529 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/TestLargeFiles.cmake
--rw-r--r--   0 thiago    (1000) thiago    (1000)      113 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/TestWindowsFSeek.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)      832 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/openjpeg_valgrind.supp
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.136193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/doc/
--rw-r--r--   0 thiago    (1000) thiago    (1000)        0 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/doc/.gitkeep
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.019193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.136193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/
--rw-r--r--   0 thiago    (1000) thiago    (1000)      307 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/CMakeLists.txt
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.141193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8436 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5931 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/bio.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4380 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/bio.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9376 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/cidx_manager.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2738 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/cidx_manager.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    24430 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/cio.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    15575 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/cio.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)   102917 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/dwt.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5187 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/dwt.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5052 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/event.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3971 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/event.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4375 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/function_list.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4490 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/function_list.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9857 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/image.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2616 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/image.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6342 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/indexbox_manager.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    10421 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/invert.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2825 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/invert.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)   454063 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/j2k.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    30350 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/j2k.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)   116780 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/jp2.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    16292 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/jp2.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      446 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/libopenjp2.pc.cmake.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)    17642 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/mct.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6002 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/mct.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    18934 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/mqc.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9166 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/mqc.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6306 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/mqc_inl.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    35505 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/openjpeg.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    59398 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/openjpeg.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    23913 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/openjpeg_mangle.h.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2806 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_clock.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2283 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_clock.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8027 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_codec.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1994 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_common.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      424 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_config.h.cmake.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1807 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_config_private.h.cmake.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7252 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_includes.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7418 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_intmath.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1995 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_inttypes.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8339 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_malloc.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3827 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_malloc.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2171 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_stdint.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8856 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/phix_manager.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    81900 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/pi.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6889 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/pi.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8922 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/ppix_manager.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    15738 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/sparse_array.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7072 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/sparse_array.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    80906 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t1.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9423 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t1.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    10168 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t1_generate_luts.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13378 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t1_luts.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    58004 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t2.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5542 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t2.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)   111287 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tcd.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    18390 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tcd.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    10571 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tgt.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5538 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tgt.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5416 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/thix_manager.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    24398 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/thread.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8595 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/thread.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1743 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tls_keys.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7235 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tpix_manager.c
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.141193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmrle/
--rw-r--r--   0 thiago    (1000) thiago    (1000)      210 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmrle/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3405 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmrle/info.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2454 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmrle/info.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3070 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmrle/io.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1505 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmrle/io.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2199 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmrle/main.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)    17205 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmrle/rle.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3114 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmrle/rle.h
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.142193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmutfcpp/
--rw-r--r--   0 thiago    (1000) thiago    (1000)      411 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmutfcpp/README.GDCM.txt
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.142193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmutfcpp/utf8/
--rw-r--r--   0 thiago    (1000) thiago    (1000)    12172 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmutfcpp/utf8/checked.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    10697 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmutfcpp/utf8/core.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8907 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmutfcpp/utf8/unchecked.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1521 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmutfcpp/utf8.h
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.143193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/
--rw-r--r--   0 thiago    (1000) thiago    (1000)       39 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/.NoDartCoverage
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3477 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1552 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/COPYING
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2202 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/compare.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    10948 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/gen_uuid.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2292 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/pack.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2510 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/parse.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2129 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/unpack.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2569 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/unparse.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4115 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/uuid.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2462 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/uuidP.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1392 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/uuid_mangle.h.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4411 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/uuid_time.c
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.146193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/
--rw-r--r--   0 thiago    (1000) thiago    (1000)       39 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/.NoDartCoverage
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1587 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1335 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/COPYING
--rw-r--r--   0 thiago    (1000) thiago    (1000)    42928 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/ChangeLog
--rw-r--r--   0 thiago    (1000) thiago    (1000)    15080 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/FAQ
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1318 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/INDEX
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5696 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/README
--rw-r--r--   0 thiago    (1000) thiago    (1000)      302 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/README.GDCM.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4559 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/adler32.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9336 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/algorithm.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2489 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/compress.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13193 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/crc32.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    30568 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/crc32.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    64163 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/deflate.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    12114 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/deflate.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    16398 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/example.c
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.147193 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1515 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/README.examples
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8594 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/fitblk.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    25499 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/gun.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    16838 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/gzappend.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    14014 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/gzjoin.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11532 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/gzlog.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2899 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/gzlog.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    28639 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/zlib_how.html
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5815 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/zpipe.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    15306 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/zran.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    31103 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/gzio.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    22164 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/infback.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    12568 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/inffast.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)      407 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/inffast.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6343 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/inffixed.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    48977 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/inflate.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5916 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/inflate.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    13756 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/inftrees.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2373 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/inftrees.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8018 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/minigzip.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    44027 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/trees.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8444 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/trees.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2087 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/uncompr.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9667 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/zconf.in.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4486 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/zlib.3
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4391 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/zlib.def.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)    66188 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/zlib.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      897 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/zlib.rc
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7136 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/zutil.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6859 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/zutil.h
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.148193 python-gdcm-3.0.9.0/gdcm_src/Utilities/getopt/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2461 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/getopt/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1956 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/getopt/COPYING
--rw-r--r--   0 thiago    (1000) thiago    (1000)      136 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/getopt/README
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2287 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/getopt/ex_getopt.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4069 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/getopt/getopt.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4258 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/getopt/getopt.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    14212 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/getopt/getopt_long.c
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.150193 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2642 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/CHANGES
--rw-r--r--   0 thiago    (1000) thiago    (1000)      867 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1078 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/COPYING
--rw-r--r--   0 thiago    (1000) thiago    (1000)      364 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/PORTABILITY
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7310 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/README
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2599 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/SETUP
--rw-r--r--   0 thiago    (1000) thiago    (1000)     8487 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/chendct.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    15098 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/codec.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2147 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/csize.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4348 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/dct.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7386 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/globals.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    16992 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/huffman.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    31290 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/io.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6489 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/jpeg.1
--rw-r--r--   0 thiago    (1000) thiago    (1000)    67620 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/jpeg.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     9200 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/leedct.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    80188 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/lexer.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    30298 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/lexer.l
--rw-r--r--   0 thiago    (1000) thiago    (1000)    18149 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/marker.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1803 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/marker.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3941 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/param.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5130 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/prototypes.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)      827 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/pvrgjpeg.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)    24638 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/stream.c
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1606 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/stream.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3745 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/system.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4706 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/tables.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11653 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/transform.c
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.150193 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/
--rw-r--r--   0 thiago    (1000) thiago    (1000)       39 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/.NoDartCoverage
--rw-r--r--   0 thiago    (1000) thiago    (1000)      149 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/AUTHORS
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1527 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/CMakeLists.txt
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      491 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/COPYING
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.152193 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2736 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3994 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/config.h.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1679 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/echo.cpp
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1291 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/echo.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4840 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/fork.cpp
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1676 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/fork.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7107 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/ftp.cpp
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4072 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/ftp.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3556 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/local.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4104 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/pipestream.cpp
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1967 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/pipestream.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1495 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/protocol.cpp
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1619 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/protocol.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5737 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/sig.cpp
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3584 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/sig.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3359 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/smtp.cpp
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2393 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/smtp.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    10809 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/sockinet.cpp
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5274 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/sockinet.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    26669 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/sockstream.cpp
--rw-r--r--   0 thiago    (1000) thiago    (1000)    11920 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/sockstream.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3559 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/sockunix.cpp
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2629 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/sockunix.h
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.152193 python-gdcm-3.0.9.0/gdcm_src/Wrapping/
--rw-r--r--   0 thiago    (1000) thiago    (1000)      300 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/CMakeLists.txt
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.154193 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Csharp/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3643 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Csharp/AssemblyInfo.cs.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4198 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Csharp/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)      260 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Csharp/Notes.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)   301592 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Csharp/docstrings.i
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)    15682 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Csharp/doxy2swig.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)    30607 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Csharp/gdcm.i
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5365 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Csharp/gdcm_arrays_csharp.i
--rw-r--r--   0 thiago    (1000) thiago    (1000)      596 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Csharp/key.snk
--rw-r--r--   0 thiago    (1000) thiago    (1000)     4435 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Csharp/std_set.i
--rw-r--r--   0 thiago    (1000) thiago    (1000)      934 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Csharp/version.rc.in
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.154193 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Java/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     5702 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Java/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)    31360 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Java/gdcm.i
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1355 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Java/main.java
--rw-r--r--   0 thiago    (1000) thiago    (1000)     2284 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Java/std_set.i
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.154193 python-gdcm-3.0.9.0/gdcm_src/Wrapping/PHP/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3263 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/PHP/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)    21536 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/PHP/gdcm.i
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.155193 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Perl/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1895 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Perl/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)    18850 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Perl/gdcm.i
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.157193 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/
--rw-r--r--   0 thiago    (1000) thiago    (1000)       39 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/.NoDartCoverage
--rw-r--r--   0 thiago    (1000) thiago    (1000)     7637 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/CMakeLists.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1956 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/Python.h.in
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)     4766 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/TestWrap.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)   539801 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/docstrings.i
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)    15572 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/doxy2swig.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)        9 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/gdcm.pth.in
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3136 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/gdcm.py
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6794 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/gdcmPythonFilter.cxx
--rw-r--r--   0 thiago    (1000) thiago    (1000)     1443 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/gdcmPythonFilter.h
--rw-r--r--   0 thiago    (1000) thiago    (1000)    25606 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/gdcmswig.i
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.157193 python-gdcm-3.0.9.0/gdcm_src/Wrapping/SWIGCommon/
--rw-r--r--   0 thiago    (1000) thiago    (1000)    20885 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/Wrapping/SWIGCommon/gdcmcommon.i
--rw-r--r--   0 thiago    (1000) thiago    (1000)     6193 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.0/gdcm_src/appveyor.yml
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.158193 python-gdcm-3.0.9.0/python_gdcm.egg-info/
--rw-r--r--   0 thiago    (1000) thiago    (1000)     3045 2021-06-29 18:10:45.000000 python-gdcm-3.0.9.0/python_gdcm.egg-info/PKG-INFO
--rw-r--r--   0 thiago    (1000) thiago    (1000)    78387 2021-06-29 18:10:45.000000 python-gdcm-3.0.9.0/python_gdcm.egg-info/SOURCES.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)        1 2021-06-29 18:10:45.000000 python-gdcm-3.0.9.0/python_gdcm.egg-info/dependency_links.txt
--rw-r--r--   0 thiago    (1000) thiago    (1000)        1 2021-06-29 18:10:45.000000 python-gdcm-3.0.9.0/python_gdcm.egg-info/not-zip-safe
--rw-r--r--   0 thiago    (1000) thiago    (1000)       11 2021-06-29 18:10:45.000000 python-gdcm-3.0.9.0/python_gdcm.egg-info/top_level.txt
-drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-06-29 18:10:46.159193 python-gdcm-3.0.9.0/scripts/
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.0/scripts/gdcmanon
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.0/scripts/gdcmconv
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.0/scripts/gdcmdiff
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.0/scripts/gdcmdump
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.0/scripts/gdcmgendir
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.0/scripts/gdcmimg
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.0/scripts/gdcminfo
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.0/scripts/gdcmpap3
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.0/scripts/gdcmraw
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.0/scripts/gdcmscanner
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.0/scripts/gdcmscu
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.0/scripts/gdcmtar
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.0/scripts/gdcmxml
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)       67 2021-06-29 18:10:46.159193 python-gdcm-3.0.9.0/setup.cfg
--rwxr-xr-x   0 thiago    (1000) thiago    (1000)     7468 2021-05-10 18:12:57.000000 python-gdcm-3.0.9.0/setup.py
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.253879 python-gdcm-3.0.9.1/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       66 2021-02-26 23:15:40.000000 python-gdcm-3.0.9.1/MANIFEST.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3146 2021-07-26 22:48:01.253879 python-gdcm-3.0.9.1/PKG-INFO
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1383 2021-03-12 15:24:02.000000 python-gdcm-3.0.9.1/README.md
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.140880 python-gdcm-3.0.9.1/_gdcm/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)        0 2021-02-26 18:58:47.000000 python-gdcm-3.0.9.1/_gdcm/__init__.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3148 2021-02-26 18:58:47.000000 python-gdcm-3.0.9.1/gdcm.py
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.141880 python-gdcm-3.0.9.1/gdcm_src/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2001 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/.clang-format
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       33 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/.git
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      177 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/.gitattributes
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      126 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/.gitignore
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       93 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/.gitmodules
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6809 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/.travis.yml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1934 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/AUTHORS
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.141880 python-gdcm-3.0.9.1/gdcm_src/Applications/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       22 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/CMakeLists.txt
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.143880 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    10329 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3248 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/deflate.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1406 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcm.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    24845 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmanon.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      778 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmcheck.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    48643 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmconv.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      103 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmdictdump.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8419 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmdiff.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    50674 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmdump.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2018 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmfile.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8936 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmgendir.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    40757 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmimg.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    23254 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcminfo.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1149 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmkey.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4528 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmoverlay.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    18038 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmpap3.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    19092 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmpdf.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11310 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmraw.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8632 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmscanner.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    24310 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmscu.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    32064 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmstream.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    53280 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmtar.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    24999 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmxml.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      580 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/pdf2dcm.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    37725 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/puff.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1506 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/puff.h
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.144880 python-gdcm-3.0.9.1/gdcm_src/Applications/Python/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2319 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Python/README
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2983 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Python/accessdata.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3675 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Python/images.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1049 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Python/lib.py
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)     5740 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/Python/wado.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      462 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Applications/README.txt
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.147880 python-gdcm-3.0.9.1/gdcm_src/CMake/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2024 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/CMakeCSharpCompiler.cmake.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3428 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/CMakeCSharpInformation.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2396 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/CMakeDetermineCSharpCompiler.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2325 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/CMakeTestCSharpCompiler.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1326 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/COPYING-CMAKE-SCRIPTS
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2731 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/CTestCustom.ctest.in
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.147880 python-gdcm-3.0.9.1/gdcm_src/CMake/ExportConfiguration/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4040 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/ExportConfiguration/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1779 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/ExportConfiguration/GDCMConfig.cmake.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      803 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/ExportConfiguration/GDCMConfigVersion.cmake.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      866 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/ExportConfiguration/UseGDCM.cmake.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1522 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindACTIVIZ.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      647 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindCSharp.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      903 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindCharLS.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4123 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindDCMTK.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1392 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindDICOM3TOOLS.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1823 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindDotNETFrameworkSDK.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1073 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindJSON.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2890 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindJavaProperties.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      400 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindKAKADU.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      977 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindKWStyle.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1088 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindLJPEG.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1012 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindMAGIC.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2582 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindMONO.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1793 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindMd5sum.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1221 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindOpenJPEG.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4523 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindOpenSSL.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1015 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindPAPYRUS3.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1370 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindPHP5.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      832 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindPVRGJPEG.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      959 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindPoppler.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      599 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindRsync.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      930 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindSOCKET++.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      598 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindSQLITE3.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1733 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/FindUUID.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1284 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/GetSystemProperty.java
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2594 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/InstallMacros.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2453 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/InstallRequiredVTKLibraries.cmake
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.147880 python-gdcm-3.0.9.1/gdcm_src/CMake/Release/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)        0 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/Release/README.cygwin.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)        0 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/Release/cygwin-package.sh.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)        0 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/Release/cygwin-patch.diff.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)        0 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/Release/cygwin-setup.hint.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1397 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/Toolchain-gcc-arm-linux-gnueabi.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1273 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/Toolchain-gcc-m32.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1723 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/Toolchain-gcc-powerpc.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1138 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/Toolchain-mingw32.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1042 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/Toolchain-mingw64.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6861 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/UseCSharp.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2325 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/UseCSharpTest.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      773 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/UseCopyright.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6494 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/UseDebian.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      230 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/UseDotNETFrameworkSDK.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3244 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/UseJavaTest.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1542 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/UseMONO.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3539 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/UsePythonTest.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      506 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/dcmqrscp.cfg.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2673 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CMake/gdcmValgrind.supp
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    40125 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      229 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/CTestConfig.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1863 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Copyright.txt
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.147880 python-gdcm-3.0.9.1/gdcm_src/Examples/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      561 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/CMakeLists.txt
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.149880 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4169 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/BasicAnonymizer.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2534 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/BasicImageAnonymizer.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2167 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9910 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/ClinicalTrialIdentificationWorkflow.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2664 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/CompressLossyJPEG.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2739 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/DecompressImage.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4425 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/DecompressImageMultiframe.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3038 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/DecompressJPEGFile.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2233 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/DumpCSA.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2370 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/ExtractEncapsulatedFile.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3280 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/ExtractImageRegion.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3349 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/ExtractImageRegionWithLUT.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2670 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/ExtractOneFrame.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1667 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/FileAnonymize.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6879 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/FileChangeTS.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7039 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/FileChangeTSLossy.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1965 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/FileStreaming.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1728 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/GenerateDICOMDIR.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2673 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/GetArray.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1708 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/ManipulateFile.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13712 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/MpegVideoInfo.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2297 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/NewSequence.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3006 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/ReformatFile.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1926 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/RescaleImage.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2202 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/ScanDirectory.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1161 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/SendFileSCU.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2383 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/SimplePrint.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1763 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/SimplePrintPatientName.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      973 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/SortImage2.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3765 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/StandardizeFiles.cs
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.154880 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5632 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5096 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/CStoreQtProgress.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2838 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ChangePrivateTags.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2719 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ChangeSequenceUltrasound.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3144 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/CheckBigEndianBug.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2846 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ClinicalTrialAnnotate.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2310 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/CompressImage.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4290 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ConvertToQImage.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2047 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/CreateARGBImage.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2046 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/CreateCMYKImage.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2595 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/CreateJPIPDataSet.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3005 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DeriveSeries.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1847 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DiffFile.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8029 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DiscriminateVolume.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9908 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DumpADAC.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    20848 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DumpExamCard.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    17452 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DumpGEMSMovieGroup.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4798 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DumpImageHeaderInfo.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13224 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DumpPhilipsECHO.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2543 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DumpSiemensBase64.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3890 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DumpToSQLITE3.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3266 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DumpToshibaDTI.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4072 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DumpVisusChange.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7037 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DuplicatePCDE.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6156 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ELSCINT1WaveToText.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1751 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/EmptyMask.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2388 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/EncapsulateFileInRawData.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2060 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ExtractEncryptedContent.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2848 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ExtractIconFromFile.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    14393 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/Extracting_All_Resolution.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7200 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/Fake_Image_Using_Stream_Image_Writer.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3969 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/FixBrokenJ2K.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6637 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/FixJAIBugJPEGLS.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2298 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/FixOrientation.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4564 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/GenAllVR.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5271 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/GenFakeIdentifyFile.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4043 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/GenFakeImage.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2875 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/GenLongSeqs.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3134 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/GenSeqs.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2109 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/GenerateStandardSOPClasses.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4146 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/GetJPEGSamplePrecision.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4250 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/GetSequenceUltrasound.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6467 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/GetSubSequenceData.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2616 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/HelloVizWorld.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2431 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/HelloWorld.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5882 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/LargeVRDSExplicit.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1896 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/MakeTemplate.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2597 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/MergeTwoFiles.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    23542 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/MrProtocol.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3194 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/PatchFile.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1234 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/PrintLUT.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2274 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/PublicDict.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1471 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/QIDO-RS.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8215 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ReadAndDumpDICOMDIR.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    14929 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ReadAndDumpDICOMDIR2.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3506 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ReadAndPrintAttributes.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1506 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ReadExplicitLengthSQIVR.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4935 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ReadGEMSSDO.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1898 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ReadMultiTimesException.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3322 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ReadUTF8QtDir.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4153 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/SimpleScanner.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3427 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/SortImage.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8838 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/StreamImageReaderTest.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3807 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/TemplateEmptyImage.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2488 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/TraverseModules.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5185 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/VolumeSorter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5182 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/csa2img.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3519 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/iU22tomultisc.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7848 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/pmsct_rgb1.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7606 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/rle2img.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1569 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/uid_unique.cxx
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.155880 python-gdcm-3.0.9.1/gdcm_src/Examples/Java/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1447 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Java/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2071 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Java/DecompressImage.java
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2279 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Java/DecompressPixmap.java
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2575 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Java/ExtractImageRegion.java
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2006 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Java/FileAnonymize.java
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1269 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Java/HelloSimple.java
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2897 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Java/ReadFiles.java
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    10761 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Java/ScanDirectory.java
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2323 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Java/SimplePrint.java
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.155880 python-gdcm-3.0.9.1/gdcm_src/Examples/PHP/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       80 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/PHP/README.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1200 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/PHP/export_pnm.php
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2600 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/PHP/hello_world.php
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1355 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/PHP/modify_file.php
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1349 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/PHP/qido.php
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      973 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/PHP/rewrite_header.php
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.157880 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1122 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/AddPrivateAttribute.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)        0 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2912 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/ConvertMPL.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2527 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/ConvertNumpy.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3015 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/ConvertPIL.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4303 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/CreateRAWStorage.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1969 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/DecompressImage.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3888 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/DumbAnonymizer.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2650 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/ExtractImageRegion.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1350 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/FindAllPatientName.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1886 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/FixCommaBug.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1878 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/GetPortionCSAHeader.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1604 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/HelloWorld.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3918 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/ManipulateFile.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2284 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/ManipulateSequence.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1715 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/MergeFile.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1657 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/NewSequence.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1841 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/PhilipsPrivateRescaleInterceptSlope.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2328 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/PlaySound.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1170 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/PrivateDict.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3151 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/ReWriteSCAsMR.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8113 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/ReadAndDumpDICOMDIR.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1330 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/RemovePrivateTags.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1945 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/ScanDirectory.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1104 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/SortImage.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3758 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Examples/Python/WriteBuffer.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1965 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/INSTALL.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1954 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/PACKAGER
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      257 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/README.Copyright.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1908 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/README.md
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.157880 python-gdcm-3.0.9.1/gdcm_src/Source/
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.157880 python-gdcm-3.0.9.1/gdcm_src/Source/Attribute/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)        0 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Attribute/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)        9 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Attribute/README.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      293 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/CMakeLists.txt
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.163880 python-gdcm-3.0.9.1/gdcm_src/Source/Common/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6487 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       82 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/README.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2960 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmASN1.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1216 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmASN1.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5505 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmBase64.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1911 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmBase64.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4127 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmBoxRegion.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2135 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmBoxRegion.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      634 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmByteSwap.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1490 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmByteSwap.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4657 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmByteSwap.txx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1082 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmCAPICryptoFactory.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      931 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmCAPICryptoFactory.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    16467 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmCAPICryptographicMessageSyntax.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2020 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmCAPICryptographicMessageSyntax.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      696 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmCommand.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5140 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmCommand.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5891 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmConfigure.h.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1871 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmCryptoFactory.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1911 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmCryptoFactory.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      608 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmCryptographicMessageSyntax.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1806 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmCryptographicMessageSyntax.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      633 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmDataEvent.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1601 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmDataEvent.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      615 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmDeflateStream.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      678 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmDeflateStream.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5687 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmDirectory.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3170 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmDirectory.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1130 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmDummyValueGenerator.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1179 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmDummyValueGenerator.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      795 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmEvent.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3149 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmEvent.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      634 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmException.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3339 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmException.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      637 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmFileNameEvent.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1576 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmFileNameEvent.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4395 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmFilename.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2319 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmFilename.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3371 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmFilenameGenerator.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2153 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmFilenameGenerator.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3336 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmLegacyMacro.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3259 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmMD5.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1442 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmMD5.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      896 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmObject.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3052 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmObject.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      898 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmOpenSSLCryptoFactory.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1204 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmOpenSSLCryptoFactory.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7130 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmOpenSSLCryptographicMessageSyntax.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2141 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmOpenSSLCryptographicMessageSyntax.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      666 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmOpenSSLP7CryptoFactory.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1151 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmOpenSSLP7CryptoFactory.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11907 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmOpenSSLP7CryptographicMessageSyntax.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2429 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmOpenSSLP7CryptographicMessageSyntax.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      637 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmProgressEvent.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1522 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmProgressEvent.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      763 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmRegion.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1718 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmRegion.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2860 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSHA1.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1425 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSHA1.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2944 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSmartPointer.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1508 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmStaticAssert.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      631 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmString.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4510 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmString.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5504 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSubject.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2501 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSubject.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1434 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSwapCode.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1555 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSwapCode.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1638 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSwapper.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6287 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSwapper.txx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    27870 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSystem.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5534 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSystem.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6555 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmTerminal.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1595 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmTerminal.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      993 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmTestDriver.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    17376 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmTesting.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4528 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmTesting.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3382 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmTrace.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9125 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmTrace.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2002 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmTypes.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1744 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmUnpacker12Bits.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1760 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmUnpacker12Bits.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      948 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmVersion.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1481 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmVersion.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3164 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmWin32.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    10890 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/zipstreamimpl.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    24174 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/Common/zipstreamimpl.hpp
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.170880 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9091 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/06_03_list.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3036 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/Agfa.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3728 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1730 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/COPYRIGHT.dicom3tools
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    14472 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/CSADefaultDicts.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    41260 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/CSAHeader.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    14508 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/DefaultDicts.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13747 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/DefaultPrivateDicts.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)   230891 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/HarvestedPrivate.xml
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)    11884 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/ParseDicts.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)   601260 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/Part6.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13466 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/Part6.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13212 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/Part67.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6339 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/Part6PDF.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6121 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/Part6todcm4che.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1140 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/Part7.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8270 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/Part7a.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3075 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/Part7b.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2104 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/PartToGDCM.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      934 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/README.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6062 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/Siemens.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2215 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/TagKeywords.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4468 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/TagToType.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2686 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/TagToVR.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3567 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/UIDToC++.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    36696 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/UIDs.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1113 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/VM.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    12348 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/cp699.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8667 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/dcmtk.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3546 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/dicom3tools.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)   196316 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/dicomhdr.html
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1844 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/dicomhdr.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    33659 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmCSAHeaderDefaultDicts.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2872 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmCSAHeaderDict.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2805 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmCSAHeaderDictEntry.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)  1194766 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmDefaultDicts.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3339 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmDefaultGroupNames.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9699 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmDict.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    10532 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmDictConverter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2095 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmDictConverter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2962 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmDictEntry.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4393 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmDictEntry.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3802 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmDicts.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2230 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmDicts.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5376 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmGlobal.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3449 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmGlobal.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1298 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmGroupDict.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2349 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmGroupDict.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1702 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmPrepDict.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3290 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmPrepGroupName.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)   824526 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmPrivateDefaultDicts.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       91 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmRoot.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11378 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmSOPClassUIDToIOD.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1506 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmSOPClassUIDToIOD.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)   251256 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmTagKeywords.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)  1049572 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmTagToType.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    34653 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmUIDs.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    62655 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmUIDs.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1304 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmconformancetests.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      874 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/getname.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      991 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/getowner.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1190 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/getretired.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1229 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/order.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3918 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/priv2html.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)   908801 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/privatedicts.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2995 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/redo.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2760 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/redo2.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      729 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/sort.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1772 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/uppercase.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1601 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/vital.xml
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.177880 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2846 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       55 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/README.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    33191 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmAttribute.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3340 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmBasicOffsetTable.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2508 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmByteBuffer.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4443 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmByteSwapFilter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1183 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmByteSwapFilter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8758 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmByteValue.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7040 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmByteValue.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1901 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCP246ExplicitDataElement.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1627 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCP246ExplicitDataElement.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6671 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCP246ExplicitDataElement.txx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4602 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCSAElement.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    51796 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCSAHeader.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4845 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCSAHeader.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1123 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCodeString.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3761 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCodeString.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6347 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataElement.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9125 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataElement.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4855 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataSet.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11013 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataSet.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    17355 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataSet.txx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      636 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataSetEvent.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1522 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataSetEvent.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    25371 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmElement.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2303 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitDataElement.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1391 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitDataElement.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    16681 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitDataElement.txx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1918 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitImplicitDataElement.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1856 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitImplicitDataElement.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    15059 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitImplicitDataElement.txx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      935 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFile.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2162 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFile.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    29687 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFileMetaInformation.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5097 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFileMetaInformation.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1013 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFileSet.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1662 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFileSet.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1201 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFragment.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6273 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFragment.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      711 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFragment.txx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2017 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmImplicitDataElement.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1527 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmImplicitDataElement.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    19182 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmImplicitDataElement.txx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      654 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmItem.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9885 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmItem.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1864 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmItem.txx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1850 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmLO.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    22959 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmMediaStorage.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7914 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmMediaStorage.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5921 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmMrProtocol.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2226 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmMrProtocol.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1738 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPDBElement.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8224 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPDBHeader.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3001 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPDBHeader.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      642 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmParseException.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2379 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmParseException.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2251 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmParser.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4075 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmParser.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2067 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPreamble.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1943 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPreamble.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2937 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPrivateTag.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2565 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPrivateTag.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    25113 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmReader.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4496 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmReader.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1504 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmReader.strict.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3995 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfFragments.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11390 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfFragments.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      756 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfFragments.txx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2004 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfItems.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8605 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfItems.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1251 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfItems.txx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2812 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTag.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9961 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTag.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)   113222 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTagToVR.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      734 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTagToVR.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8659 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTransferSyntax.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4442 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTransferSyntax.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1900 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitDataElement.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1492 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitDataElement.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6337 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitDataElement.txx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1924 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitImplicitDataElement.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1842 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitImplicitDataElement.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2137 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitImplicitDataElement.txx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3304 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVL.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8480 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVM.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5128 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVM.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13182 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVR.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11086 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVR.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1906 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVR16ExplicitDataElement.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1605 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVR16ExplicitDataElement.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9062 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVR16ExplicitDataElement.txx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      711 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmValue.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1395 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmValue.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      681 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmValue.txx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1036 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmValueIO.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2308 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmValueIO.txx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4670 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmWriter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3104 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmWriter.h
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.182880 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2153 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/CMakeLists.txt
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)    18708 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/ParseAttributes.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)  2336000 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/Part3.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    41130 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/Part3.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8311 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/Part3New.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    21272 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/Part4.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6396 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/Part4.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1889 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/Part4ToC++.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      487 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/README.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2168 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/Template.xml.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    20305 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/ValueRepresentation.xsd
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1108 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/extract.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      613 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmDefinedTerms.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1598 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmDefinedTerms.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    12108 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmDefs.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2052 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmDefs.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      617 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmEnumeratedValues.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1569 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmEnumeratedValues.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1522 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmIOD.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1899 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmIOD.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1217 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmIODEntry.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3040 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmIODEntry.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2074 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmIODs.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2289 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmMacro.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3010 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmMacro.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2635 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmMacroEntry.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      608 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmMacros.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2106 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmMacros.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3691 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmModule.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3230 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmModule.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2583 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmModuleEntry.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      609 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmModules.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2122 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmModules.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      602 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmNestedModuleEntries.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1925 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmNestedModuleEntries.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      607 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmPatient.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      904 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmPatient.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      607 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmSeries.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      814 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmSeries.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      606 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmStudy.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      861 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmStudy.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      630 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmTable.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1611 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmTable.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1090 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmTableEntry.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13943 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmTableReader.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3053 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmTableReader.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      692 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmTables.h.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1050 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmType.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1900 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmType.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1153 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmUsage.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2670 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmUsage.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5425 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmXMLDictReader.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1426 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmXMLDictReader.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6306 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmXMLPrivateDictReader.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1495 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmXMLPrivateDictReader.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2113 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/getelements.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2113 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/ma2html.xsl
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5856 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/ma2pdf.xsl
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.196879 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6609 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3679 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/FileMetaInformation.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6444 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/README.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1392 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/TODO.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      638 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAnonymizeEvent.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1556 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAnonymizeEvent.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    37487 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAnonymizer.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6841 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAnonymizer.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      618 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmApplicationEntity.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1850 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmApplicationEntity.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      812 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAudioCodec.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1047 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAudioCodec.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    36184 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmBitmap.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5967 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmBitmap.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1291 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmBitmapToBitmapFilter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1262 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmBitmapToBitmapFilter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      809 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmCodec.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1322 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmCoder.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1643 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmConstCharWrapper.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    17226 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmCurve.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2622 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmCurve.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      609 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDICOMDIR.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1027 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDICOMDIR.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    39052 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDICOMDIRGenerator.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3943 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDICOMDIRGenerator.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11928 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDataSetHelper.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1247 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDataSetHelper.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1199 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDecoder.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1176 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDeltaEncodingCodec.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1104 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDeltaEncodingCodec.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    16004 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDictPrinter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1070 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDictPrinter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3988 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDirectionCosines.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1982 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDirectionCosines.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    10775 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDirectoryHelper.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3596 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDirectoryHelper.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      608 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDumper.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1030 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDumper.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    15380 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEmptyMaskGenerator.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2706 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEmptyMaskGenerator.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      621 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEncapsulatedDocument.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      874 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEncapsulatedDocument.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3987 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEquipmentManufacturer.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1039 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEquipmentManufacturer.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      610 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFiducials.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      808 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFiducials.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    16306 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileAnonymizer.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2920 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileAnonymizer.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    15260 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileChangeTransferSyntax.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2257 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileChangeTransferSyntax.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3858 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileDecompressLookupTable.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1554 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileDecompressLookupTable.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    15433 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileDerivation.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3262 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileDerivation.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6609 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileExplicitFilter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2497 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileExplicitFilter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    25738 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileStreamer.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4241 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileStreamer.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    10468 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIPPSorter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4732 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIPPSorter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3968 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImage.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2526 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImage.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    18763 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImageFilter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2431 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImageFilter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    32738 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImageGenerator.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3168 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImageGenerator.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4220 2021-07-26 22:46:44.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImage.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3757 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImage.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3649 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageApplyLookupTable.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1221 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageApplyLookupTable.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    10161 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangePhotometricInterpretation.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3838 2021-07-26 22:46:44.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangePhotometricInterpretation.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4612 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangePlanarConfiguration.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2772 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangePlanarConfiguration.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    20383 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangeTransferSyntax.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3382 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangeTransferSyntax.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    20953 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageCodec.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4773 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageCodec.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      976 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageConverter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1297 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageConverter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3240 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageFragmentSplitter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1571 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageFragmentSplitter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)   109059 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageHelper.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7091 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageHelper.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4480 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageReader.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1604 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageReader.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    16862 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageRegionReader.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2653 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageRegionReader.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      940 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageToImageFilter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1189 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageToImageFilter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    14224 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageWriter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1905 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageWriter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      885 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG12Codec.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1346 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG12Codec.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      885 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG16Codec.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1338 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG16Codec.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    53281 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG2000Codec.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3179 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG2000Codec.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      878 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG8Codec.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1337 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG8Codec.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    55015 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEGBITSCodec.hxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    21598 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEGCodec.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3438 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEGCodec.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    17200 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEGLSCodec.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3175 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEGLSCodec.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    30175 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJSON.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1148 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJSON.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6324 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmKAKADUCodec.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1135 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmKAKADUCodec.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    21951 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmLookupTable.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3639 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmLookupTable.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3435 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmMeshPrimitive.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2397 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmMeshPrimitive.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3806 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmOrientation.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1817 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmOrientation.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    18989 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmOverlay.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3822 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmOverlay.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      800 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPDFCodec.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1039 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPDFCodec.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2784 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPGXCodec.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1277 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPGXCodec.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9336 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPNMCodec.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1595 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPNMCodec.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5528 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPVRGCodec.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1496 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPVRGCodec.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      612 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPersonName.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2511 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPersonName.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5806 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPhotometricInterpretation.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2817 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPhotometricInterpretation.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7358 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixelFormat.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7667 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixelFormat.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2752 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmap.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2485 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmap.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    49226 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapReader.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2098 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapReader.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1032 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapToPixmapFilter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1190 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapToPixmapFilter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    28937 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapWriter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2056 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapWriter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    32806 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPrinter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2909 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPrinter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6168 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRAWCodec.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1548 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRAWCodec.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    29497 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRLECodec.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2693 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRLECodec.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    17021 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRescaler.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4682 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRescaler.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13221 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmScanner.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7559 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmScanner.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5664 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegment.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4283 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegment.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1033 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentHelper.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2226 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentHelper.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11333 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentReader.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1625 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentReader.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13570 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentWriter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1568 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentWriter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7596 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentedPaletteColorLookupTable.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1210 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentedPaletteColorLookupTable.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    14055 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSerieHelper.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3170 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSerieHelper.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6130 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSimpleSubjectWatcher.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2952 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSimpleSubjectWatcher.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4413 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSorter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2608 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSorter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3644 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSpacing.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5170 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSpacing.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      613 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSpectroscopy.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      832 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSpectroscopy.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    12942 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSplitMosaicFilter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2889 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSplitMosaicFilter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    16667 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStreamImageReader.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5525 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStreamImageReader.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    17213 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStreamImageWriter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6340 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStreamImageWriter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13733 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStrictScanner.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6765 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStrictScanner.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    15620 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStringFilter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2901 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStringFilter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11908 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurface.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7783 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurface.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4376 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceHelper.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6464 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceHelper.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    23677 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceReader.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1300 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceReader.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    38471 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceWriter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1664 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceWriter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3041 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmTagPath.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1491 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmTagPath.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7820 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmUIDGenerator.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3491 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmUIDGenerator.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2458 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmUUIDGenerator.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1062 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmUUIDGenerator.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1416 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmValidate.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      973 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmValidate.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      609 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmWaveform.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      808 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmWaveform.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    16112 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmXMLPrinter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3620 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmXMLPrinter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    15885 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcm_j2k.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5936 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcm_jp2.h
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.206879 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3167 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1312 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/README.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4316 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAAbortPDU.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1510 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAAbortPDU.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9036 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateACPDU.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3340 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateACPDU.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3816 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateRJPDU.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1427 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateRJPDU.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9538 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateRQPDU.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5580 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateRQPDU.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2331 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmARTIMTimer.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2518 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmARTIMTimer.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2251 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAReleaseRPPDU.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1353 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAReleaseRPPDU.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2268 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAReleaseRQPDU.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1353 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAReleaseRQPDU.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3281 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAbstractSyntax.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1820 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAbstractSyntax.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2631 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmApplicationContext.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1598 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmApplicationContext.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3527 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAsynchronousOperationsWindowSub.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1407 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAsynchronousOperationsWindowSub.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2437 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseCompositeMessage.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2278 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseNormalizedMessage.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1993 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmBasePDU.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9074 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseQuery.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2723 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseQuery.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3304 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseRootQuery.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4419 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseRootQuery.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2468 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCEchoMessages.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1486 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCEchoMessages.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3722 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCFindMessages.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1684 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCFindMessages.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4092 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCMoveMessages.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1912 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCMoveMessages.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    10553 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCStoreMessages.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1847 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCStoreMessages.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      988 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCommandDataSet.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1753 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCommandDataSet.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2595 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCompositeMessageFactory.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2476 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCompositeMessageFactory.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    15215 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCompositeNetworkFunctions.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5993 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCompositeNetworkFunctions.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2675 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmDIMSE.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8703 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmFindPatientRootQuery.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1266 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmFindPatientRootQuery.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7918 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmFindStudyRootQuery.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1483 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmFindStudyRootQuery.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2571 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationClassUIDSub.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1303 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationClassUIDSub.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1281 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationUIDSub.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1170 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationUIDSub.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2578 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationVersionNameSub.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1313 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationVersionNameSub.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2589 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmMaximumLengthSub.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1427 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmMaximumLengthSub.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6312 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmModalityPerformedProcedureStepCreateQuery.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1350 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmModalityPerformedProcedureStepCreateQuery.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2216 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmModalityPerformedProcedureStepSetQuery.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1329 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmModalityPerformedProcedureStepSetQuery.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8866 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmMovePatientRootQuery.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1278 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmMovePatientRootQuery.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7546 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmMoveStudyRootQuery.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1258 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmMoveStudyRootQuery.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1393 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNActionMessages.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1309 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNActionMessages.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3000 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNCreateMessages.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1309 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNCreateMessages.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1393 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNDeleteMessages.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1309 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNDeleteMessages.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1488 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNEventReportMessages.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1354 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNEventReportMessages.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1384 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNGetMessages.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1282 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNGetMessages.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2740 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNSetMessages.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1282 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNSetMessages.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1982 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNetworkEvents.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2740 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNetworkStateID.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2779 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNormalizedMessageFactory.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1681 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNormalizedMessageFactory.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9804 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNormalizedNetworkFunctions.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3102 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNormalizedNetworkFunctions.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11783 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPDUFactory.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3479 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPDUFactory.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3697 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPDataTFPDU.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1981 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPDataTFPDU.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1684 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContext.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2266 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContext.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3396 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextAC.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1816 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextAC.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5348 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextGenerator.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3884 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextGenerator.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5736 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextRQ.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3257 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextRQ.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7392 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationDataValue.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2765 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationDataValue.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1351 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryBase.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3549 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryBase.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8610 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryFactory.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3647 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryFactory.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2977 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryImage.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1521 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryImage.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3078 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryPatient.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1505 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryPatient.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2397 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQuerySeries.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1499 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQuerySeries.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4748 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryStudy.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1494 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryStudy.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4357 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmRoleSelectionSub.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1392 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmRoleSelectionSub.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3585 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmSOPClassExtendedNegociationSub.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1602 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmSOPClassExtendedNegociationSub.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4345 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmServiceClassApplicationInformation.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1314 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmServiceClassApplicationInformation.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    42855 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmServiceClassUser.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4048 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmServiceClassUser.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3060 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmTransferSyntaxSub.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1693 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmTransferSyntaxSub.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3468 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULAction.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3412 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAA.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3813 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAA.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9911 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAE.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3844 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAE.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5256 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAR.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4267 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAR.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9152 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionDT.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1774 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionDT.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1289 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULBasicCallback.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2086 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULBasicCallback.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9409 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnection.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5412 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnection.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2520 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnectionCallback.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3686 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnectionInfo.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2675 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnectionInfo.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    52315 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnectionManager.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7098 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnectionManager.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2696 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULEvent.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    21423 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULTransitionTable.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3552 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULTransitionTable.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2463 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULWritingCallback.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1854 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULWritingCallback.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8215 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmUserInformation.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2191 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmUserInformation.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3164 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmWLMFindQuery.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1328 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmWLMFindQuery.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    21774 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/TODO
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.207879 python-gdcm-3.0.9.1/gdcm_src/Utilities/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4619 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/CMakeLists.txt
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.207879 python-gdcm-3.0.9.1/gdcm_src/Utilities/KWStyle/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1505 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/KWStyle/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      254 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/KWStyle/GDCM.kws.xml.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      582 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/KWStyle/GDCMFiles.txt.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      564 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/KWStyle/GDCMHeader.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       33 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/KWStyle/GDCMOverwrite.txt
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.208880 python-gdcm-3.0.9.1/gdcm_src/Utilities/Release/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      341 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/Release/README.md
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      103 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/Release/README.txt
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)     2776 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/Release/bootstrap.sh
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      568 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/Release/config.linux
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      570 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/Release/config.win32
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      129 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/Release/makerelease.sh
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)     1985 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/Release/release.bat
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)     6692 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/Release/release.sh
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)     6661 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/Release/upload.sh
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.211880 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       39 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/.NoDartCoverage
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.211880 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Applications/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1608 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Applications/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2878 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Applications/gdcm2pnm.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    32683 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Applications/gdcm2vtk.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    30657 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Applications/gdcmviewer.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3401 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/AssemblyInfo.cs.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    33668 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       10 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/CscArgs.txt.in
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.211880 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      244 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/CMakeLists.txt
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.212880 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2334 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4396 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/HelloActiviz.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3111 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/HelloActiviz2.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1433 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/HelloActiviz3.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1431 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/HelloActiviz4.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3061 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/HelloActiviz5.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1811 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/HelloVTKWorld.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1680 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/HelloVTKWorld2.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3422 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/MetaImageMD5Activiz.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2016 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/RefCounting.cs
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.214879 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2206 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2827 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/Compute3DSpacing.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2078 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/Convert16BitsTo8Bits.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2570 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/ConvertMultiFrameToSingleFrame.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2141 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/ConvertRGBToLuminance.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2722 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/ConvertSingleBitTo8Bits.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3495 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/CreateFakePET.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4113 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/CreateFakeRTDOSE.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7553 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/GenerateRTSTRUCT.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2552 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/MagnifyFile.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    15377 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmorthoplanes.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4698 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmreslice.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13377 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmrtionplan.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    12052 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmrtplan.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3916 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmscene.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4177 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmtexture.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2936 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmvolume.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2544 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/offscreenimage.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    20078 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/reslicesphere.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3777 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/rtstructapp.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7595 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/threadgdcm.cxx
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.214879 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Java/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13048 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Java/AWTMedical3.java
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2213 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Java/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3463 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Java/HelloVTKWorld.java
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5693 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Java/MIPViewer.java
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4396 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Java/MPRViewer.java
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    10464 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Java/MPRViewer2.java
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3111 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Java/ReadSeriesIntoVTK.java
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.214879 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/PHP/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1657 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/PHP/generate_png.php
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.214879 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Python/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5458 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Python/CastConvertPhilips.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1429 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Python/headsq2dcm.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      570 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/GDCMImageGUI.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1430 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/GDCMImageReader.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      144 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/JavaDependencies.cmake.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8386 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/MummySettings.xml.in
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.214879 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      213 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/CMakeLists.txt
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.216879 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2603 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2230 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageActor.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3179 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5842 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader1.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3022 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader2_1.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3261 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader2_2.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6015 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader2_3.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5310 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader3.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4924 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader4.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2208 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReaderIsLossy.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1936 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageViewer.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9169 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageWriter1.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5805 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageWriter2.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1966 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageWriterIsLossy.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4935 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMMetaImageWriter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4941 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMMetaImageWriter2.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2309 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMPolyDataReader.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7314 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMThreadedImageReader.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7167 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMThreadedImageReader2.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2730 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkImageChangeInformation.cxx
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.216879 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Java/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1720 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Java/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1255 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Java/TestvtkGDCMImageReader.java
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.216879 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Python/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1644 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Python/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1338 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Python/TestMultiframeGrayscaleWordSecondaryCaptureImageStorage.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1821 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Python/TestvtkGDCMImageReader.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1273 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Python/TestvtkGDCMImageReader2.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1301 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Python/TestvtkGDCMImageWriter.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4221 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Python/TestvtkGDCMThreadedImageReader.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3427 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Python/TestvtkGDCMThreadedImageReader2.py
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.217879 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/VTK4/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    28837 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/VTK4/vtkMedicalImageProperties.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13579 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/VTK4/vtkMedicalImageProperties.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1747 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/VTK4/vtkStringArray.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1521 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/VTK4/vtkStringArray.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       75 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/dllexportconf.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      336 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/gccxml.cxx.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       20 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/manifest.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    56647 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMImageReader.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11929 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMImageReader.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    46426 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMImageReader2.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    10399 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMImageReader2.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1036 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMImageReader_Extra.cs
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    44149 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMImageWriter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6284 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMImageWriter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2343 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMMedicalImageProperties.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    12413 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMMedicalImageProperties.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    34698 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMPolyDataReader.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2969 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMPolyDataReader.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    31645 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMPolyDataWriter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2904 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMPolyDataWriter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    25079 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMTesting.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1526 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMTesting.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    20966 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMThreadedImageReader.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3712 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMThreadedImageReader.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    12912 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMThreadedImageReader2.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5110 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMThreadedImageReader2.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    26341 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImageColorViewer.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8955 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImageColorViewer.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    10635 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImageMapToColors16.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4299 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImageMapToColors16.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    15092 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImageMapToWindowLevelColors2.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3707 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImageMapToWindowLevelColors2.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4983 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImagePlanarComponentsToComponents.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2860 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImagePlanarComponentsToComponents.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4668 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImageRGBToYBR.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2179 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImageRGBToYBR.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6182 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImageYBRToRGB.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2179 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImageYBRToRGB.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13969 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkLookupTable16.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2880 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkLookupTable16.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    12424 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkRTStructSetProperties.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4318 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkRTStructSetProperties.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    15979 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkgdcm.i
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2157 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkgdcm.py
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.217879 python-gdcm-3.0.9.1/gdcm_src/Utilities/dicom3tools/
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)     1200 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/dicom3tools/process.sh
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.217879 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13703 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      572 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/README
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      286 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/README.txt.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       29 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/TestsList.txt.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1870 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/authors.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)   105666 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/doxyfile.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1555 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/footer.html
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.219879 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2984 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcm2pnm.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8469 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcm2vtk.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13995 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmanon.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    18207 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmconv.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2894 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmdiff.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    50466 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmdump.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4232 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmgendir.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    12430 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmimg.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7160 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcminfo.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3950 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmpap3.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7394 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmpdf.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8136 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmraw.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4195 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmscanner.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    14578 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmscu.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6584 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmtar.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4252 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmviewer.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3457 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmxml.xml
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      391 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/patchtex.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       15 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/version.txt.in
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.219879 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/vtk/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5234 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/vtk/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    12758 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/vtk/doc_makeall.sh.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6400 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/vtk/doxyfile.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      838 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcm_charls.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      784 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcm_expat.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      966 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcm_ljpeg12.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      966 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcm_ljpeg16.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      958 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcm_ljpeg8.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      766 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcm_md5.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      815 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcm_openjpeg.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      778 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcm_uuid.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      841 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcm_zlib.h
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.221879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       39 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/.NoDartCoverage
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3283 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1500 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/License.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1537 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/README.GDCM.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5000 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/charls.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5188 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/colortransform.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2230 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/context.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2347 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/contextrunmode.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8146 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/decoderstrategy.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3681 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/defaulttraits.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5756 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/encoderstrategy.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11241 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/interface.cpp
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      490 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/jlscodecfactory.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      678 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/jpegimagedatasegment.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5769 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/jpegls.cpp
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2602 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/jpegmarkercode.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4956 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/jpegmarkersegment.cpp
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3014 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/jpegmarkersegment.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      447 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/jpegsegment.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    12357 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/jpegstreamreader.cpp
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1644 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/jpegstreamreader.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2267 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/jpegstreamwriter.cpp
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2580 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/jpegstreamwriter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1272 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/lookuptable.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3478 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/losslesstraits.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    12857 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/processline.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11515 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/publictypes.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    28568 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/scan.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1239 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/styleanddesign.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4408 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/util.h
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.221879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       39 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/.NoDartCoverage
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1416 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1208 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/COPYING
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7934 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/Changes
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4728 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/README
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.222880 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/doc/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    92234 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/doc/reference.html
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1340 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/doc/style.css
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7900 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/doc/xmlwf.1
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13884 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/doc/xmlwf.sgml
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.222880 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/examples/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1631 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/examples/elements.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2405 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/examples/outline.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2470 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/expat_config.h.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5672 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/expat_mangle.h.in
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.223879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      711 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1813 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/ascii.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1760 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/asciitab.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    40313 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/expat.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3562 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/expat_external.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1830 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/iasciitab.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2003 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/internal.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1813 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/latin1tab.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7050 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/nametab.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1763 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/utf8tab.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)   192313 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/xmlparse.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    32423 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/xmlrole.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3023 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/xmlrole.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    41138 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/xmltok.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11184 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/xmltok.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    44476 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/xmltok_impl.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      661 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/xmltok_impl.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2950 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/xmltok_ns.c
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.224879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      572 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/README.txt
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.224879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/benchmark/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      546 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/benchmark/README.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2788 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/benchmark/benchmark.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3038 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/chardata.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      791 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/chardata.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4098 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/minicheck.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2061 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/minicheck.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    46055 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/runtests.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      185 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/runtestspp.cpp
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)     3512 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/xmltest.sh
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.225880 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)     1302 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/codepage.c
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      196 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/codepage.h
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)     2912 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/ct.c
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      500 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/filemap.h
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)     1457 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/readfilemap.c
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)     1114 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/unixfilemap.c
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)     2143 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/win32filemap.c
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)     5768 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlfile.c
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      509 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlfile.h
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)     3218 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlmime.c
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      493 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlmime.h
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      825 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/xmltchar.h
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      224 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlurl.h
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)    20812 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlwf.c
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)     8813 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlwin32url.cxx
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.232879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       39 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/.NoDartCoverage
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.232879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/12/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      994 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/12/CMakeLists.txt
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.232879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/16/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      988 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/16/CMakeLists.txt
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.232879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/8/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      988 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/8/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4759 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11510 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/COPYRIGHT.dcmtk
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    15141 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/Jfif.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    19942 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/README
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3153 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/README.GDCM.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9284 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/change.log
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      825 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/dcmtk.sh
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    17112 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/example.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9279 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/filelist.doc
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    52070 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/install.doc
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9148 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcapimin.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5896 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcapistd.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    16975 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jccoefct.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    14959 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jccolor.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    12883 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcdctmgr.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    14345 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcdiffct.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9255 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jchuff.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1734 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jchuff.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1855 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcinit.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    18923 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jclhuff.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1960 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jclossls.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1971 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jclossy.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9598 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcmainct.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    18002 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcmarker.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    22262 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcmaster.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1085 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcodec.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3110 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcomapi.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5372 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jconfig.doc
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1648 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jconfig.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    23643 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcparam.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    25962 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcphuff.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8365 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcpred.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    12259 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcprepct.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    19062 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcsample.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1497 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcscale.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    20094 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcshuff.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    15168 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jctrans.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    12873 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdapimin.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9387 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdapistd.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5265 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdatadst.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7636 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdatasrc.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    25907 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdcoefct.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13594 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdcolor.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7083 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdct.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8480 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jddctmgr.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13180 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jddiffct.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11554 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdhuff.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9317 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdhuff.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    12176 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdinput.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9709 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdlhuff.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2408 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdlossls.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7434 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdlossy.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    20702 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdmainct.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    41541 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdmarker.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    16164 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdmaster.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    14083 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdmerge.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    21204 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdphuff.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9922 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdpostct.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8041 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdpred.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    16602 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdsample.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3137 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdscale.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11642 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdshuff.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4969 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdtrans.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7822 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jerror.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    14869 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jerror.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5446 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jfdctflt.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7538 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jfdctfst.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11045 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jfdctint.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8466 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jidctflt.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13220 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jidctfst.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    14778 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jidctint.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13474 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jidctred.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3250 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jinclude.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4824 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jlossls.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3902 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jlossy.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    42776 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jmemmgr.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3013 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jmemnobs.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5259 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jmemsrc.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8329 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jmemsys.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    14136 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jmorecfg.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      957 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jpegcmake.h.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    15146 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jpegint.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    47947 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jpeglib.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    31572 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jquant1.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    48684 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jquant2.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5260 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jutils.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      360 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jversion.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)   159668 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/libjpeg.doc
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8703 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/mangle_jpeg.h.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    55618 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/structure.doc
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    27170 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/usage.doc
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9759 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/wizard.doc
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.233879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmmd5/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       39 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmmd5/.NoDartCoverage
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2292 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmmd5/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      965 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmmd5/COPYING
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      318 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmmd5/README.GDCM.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    12434 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmmd5/md5.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3765 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmmd5/md5.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1215 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmmd5/md5_mangle.h.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1625 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmmd5/md5cmp.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4259 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmmd5/md5main.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2594 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmmd5/tst2md5.c
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.233879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    14506 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2112 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/LICENSE
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      888 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/README.GDCM.txt
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.234879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1215 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/CTestCustom.cmake.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      928 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/EnsureFileInclude.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      332 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/FindCPPCHECK.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      612 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/FindFCGI.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      170 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/FindJPYLYZER.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      483 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/FindKAKADU.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1131 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/FindLCMS.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1168 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/FindLCMS2.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      165 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/JPIPTestDriver.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3004 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/OpenJPEGCPack.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1535 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/OpenJPEGConfig.cmake.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      305 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/TestFileOffsetBits.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      615 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/TestLargeFiles.c.cmake.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5529 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/TestLargeFiles.cmake
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      113 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/TestWindowsFSeek.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      832 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/openjpeg_valgrind.supp
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.234879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/doc/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)        0 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/doc/.gitkeep
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.139880 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.234879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      307 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/CMakeLists.txt
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.239879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8436 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5931 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/bio.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4380 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/bio.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9376 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/cidx_manager.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2738 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/cidx_manager.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    24430 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/cio.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    15575 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/cio.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)   102917 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/dwt.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5187 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/dwt.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5052 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/event.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3971 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/event.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4375 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/function_list.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4490 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/function_list.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9857 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/image.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2616 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/image.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6342 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/indexbox_manager.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    10421 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/invert.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2825 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/invert.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)   454063 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/j2k.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    30350 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/j2k.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)   116780 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/jp2.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    16292 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/jp2.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      446 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/libopenjp2.pc.cmake.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    17642 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/mct.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6002 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/mct.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    18934 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/mqc.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9166 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/mqc.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6306 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/mqc_inl.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    35505 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/openjpeg.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    59398 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/openjpeg.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    23913 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/openjpeg_mangle.h.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2806 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_clock.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2283 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_clock.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8027 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_codec.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1994 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_common.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      424 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_config.h.cmake.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1807 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_config_private.h.cmake.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7252 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_includes.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7418 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_intmath.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1995 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_inttypes.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8339 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_malloc.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3827 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_malloc.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2171 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_stdint.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8856 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/phix_manager.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    81900 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/pi.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6889 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/pi.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8922 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/ppix_manager.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    15738 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/sparse_array.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7072 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/sparse_array.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    80906 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t1.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9423 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t1.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    10168 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t1_generate_luts.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13378 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t1_luts.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    58004 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t2.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5542 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t2.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)   111287 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tcd.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    18390 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tcd.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    10571 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tgt.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5538 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tgt.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5416 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/thix_manager.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    24398 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/thread.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8595 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/thread.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1743 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tls_keys.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7235 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tpix_manager.c
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.240879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmrle/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      210 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmrle/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3405 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmrle/info.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2454 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmrle/info.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3070 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmrle/io.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1505 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmrle/io.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2199 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmrle/main.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    17205 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmrle/rle.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3114 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmrle/rle.h
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.240879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmutfcpp/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      411 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmutfcpp/README.GDCM.txt
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.240879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmutfcpp/utf8/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    12172 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmutfcpp/utf8/checked.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    10697 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmutfcpp/utf8/core.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8907 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmutfcpp/utf8/unchecked.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1521 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmutfcpp/utf8.h
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.241879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       39 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/.NoDartCoverage
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3477 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1552 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/COPYING
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2202 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/compare.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    10948 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/gen_uuid.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2292 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/pack.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2510 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/parse.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2129 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/unpack.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2569 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/unparse.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4115 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/uuid.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2462 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/uuidP.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1392 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/uuid_mangle.h.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4411 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/uuid_time.c
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.243879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       39 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/.NoDartCoverage
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1587 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1335 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/COPYING
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    42928 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/ChangeLog
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    15080 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/FAQ
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1318 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/INDEX
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5696 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/README
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      302 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/README.GDCM.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4559 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/adler32.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9336 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/algorithm.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2489 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/compress.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13193 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/crc32.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    30568 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/crc32.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    64163 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/deflate.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    12114 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/deflate.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    16398 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/example.c
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.244879 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1515 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/README.examples
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8594 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/fitblk.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    25499 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/gun.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    16838 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/gzappend.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    14014 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/gzjoin.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11532 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/gzlog.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2899 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/gzlog.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    28639 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/zlib_how.html
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5815 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/zpipe.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    15306 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/zran.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    31103 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/gzio.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    22164 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/infback.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    12568 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/inffast.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      407 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/inffast.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6343 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/inffixed.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    48977 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/inflate.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5916 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/inflate.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    13756 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/inftrees.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2373 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/inftrees.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8018 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/minigzip.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    44027 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/trees.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8444 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/trees.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2087 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/uncompr.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9667 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/zconf.in.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4486 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/zlib.3
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4391 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/zlib.def.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    66188 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/zlib.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      897 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/zlib.rc
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7136 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/zutil.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6859 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/zutil.h
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.245879 python-gdcm-3.0.9.1/gdcm_src/Utilities/getopt/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2461 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/getopt/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1956 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/getopt/COPYING
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      136 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/getopt/README
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2287 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/getopt/ex_getopt.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4069 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/getopt/getopt.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4258 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/getopt/getopt.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    14212 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/getopt/getopt_long.c
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.247879 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2642 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/CHANGES
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      867 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1078 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/COPYING
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      364 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/PORTABILITY
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7310 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/README
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2599 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/SETUP
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     8487 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/chendct.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    15098 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/codec.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2147 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/csize.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4348 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/dct.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7386 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/globals.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    16992 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/huffman.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    31290 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/io.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6489 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/jpeg.1
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    67620 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/jpeg.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     9200 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/leedct.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    80188 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/lexer.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    30298 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/lexer.l
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    18149 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/marker.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1803 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/marker.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3941 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/param.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5130 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/prototypes.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      827 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/pvrgjpeg.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    24638 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/stream.c
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1606 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/stream.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3745 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/system.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4706 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/tables.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11653 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/transform.c
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.247879 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       39 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/.NoDartCoverage
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      149 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/AUTHORS
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1527 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/CMakeLists.txt
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      491 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/COPYING
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.249879 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2736 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3994 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/config.h.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1679 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/echo.cpp
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1291 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/echo.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4840 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/fork.cpp
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1676 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/fork.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7107 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/ftp.cpp
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4072 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/ftp.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3556 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/local.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4104 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/pipestream.cpp
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1967 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/pipestream.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1495 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/protocol.cpp
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1619 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/protocol.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5737 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/sig.cpp
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3584 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/sig.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3359 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/smtp.cpp
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2393 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/smtp.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    10809 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/sockinet.cpp
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5274 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/sockinet.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    26669 2021-05-10 18:11:59.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/sockstream.cpp
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    11920 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/sockstream.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3559 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/sockunix.cpp
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2629 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/sockunix.h
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.249879 python-gdcm-3.0.9.1/gdcm_src/Wrapping/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      300 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/CMakeLists.txt
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.250879 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Csharp/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3643 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Csharp/AssemblyInfo.cs.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4198 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Csharp/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      260 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Csharp/Notes.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)   301592 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Csharp/docstrings.i
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)    15682 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Csharp/doxy2swig.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    30607 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Csharp/gdcm.i
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5365 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Csharp/gdcm_arrays_csharp.i
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      596 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Csharp/key.snk
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     4435 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Csharp/std_set.i
+-rw-r--r--   0 thiago    (1000) thiago    (1000)      934 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Csharp/version.rc.in
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.250879 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Java/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     5702 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Java/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    31360 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Java/gdcm.i
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1355 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Java/main.java
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     2284 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Java/std_set.i
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.250879 python-gdcm-3.0.9.1/gdcm_src/Wrapping/PHP/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3263 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/PHP/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    21536 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/PHP/gdcm.i
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.250879 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Perl/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1895 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Perl/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    18850 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Perl/gdcm.i
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.251879 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       39 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/.NoDartCoverage
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     7637 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/CMakeLists.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1956 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/Python.h.in
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)     4766 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/TestWrap.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)   539801 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/docstrings.i
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)    15572 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/doxy2swig.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)        9 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/gdcm.pth.in
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3136 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/gdcm.py
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6794 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/gdcmPythonFilter.cxx
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     1443 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/gdcmPythonFilter.h
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    25606 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/gdcmswig.i
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.251879 python-gdcm-3.0.9.1/gdcm_src/Wrapping/SWIGCommon/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    20885 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/Wrapping/SWIGCommon/gdcmcommon.i
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     6193 2021-02-26 19:23:16.000000 python-gdcm-3.0.9.1/gdcm_src/appveyor.yml
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.252879 python-gdcm-3.0.9.1/python_gdcm.egg-info/
+-rw-r--r--   0 thiago    (1000) thiago    (1000)     3146 2021-07-26 22:48:01.000000 python-gdcm-3.0.9.1/python_gdcm.egg-info/PKG-INFO
+-rw-r--r--   0 thiago    (1000) thiago    (1000)    78387 2021-07-26 22:48:01.000000 python-gdcm-3.0.9.1/python_gdcm.egg-info/SOURCES.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)        1 2021-07-26 22:48:01.000000 python-gdcm-3.0.9.1/python_gdcm.egg-info/dependency_links.txt
+-rw-r--r--   0 thiago    (1000) thiago    (1000)        1 2021-07-26 22:48:01.000000 python-gdcm-3.0.9.1/python_gdcm.egg-info/not-zip-safe
+-rw-r--r--   0 thiago    (1000) thiago    (1000)       11 2021-07-26 22:48:01.000000 python-gdcm-3.0.9.1/python_gdcm.egg-info/top_level.txt
+drwxr-xr-x   0 thiago    (1000) thiago    (1000)        0 2021-07-26 22:48:01.252879 python-gdcm-3.0.9.1/scripts/
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.1/scripts/gdcmanon
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.1/scripts/gdcmconv
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.1/scripts/gdcmdiff
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.1/scripts/gdcmdump
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.1/scripts/gdcmgendir
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.1/scripts/gdcmimg
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.1/scripts/gdcminfo
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.1/scripts/gdcmpap3
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.1/scripts/gdcmraw
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.1/scripts/gdcmscanner
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.1/scripts/gdcmscu
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.1/scripts/gdcmtar
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)      270 2021-03-11 20:05:40.000000 python-gdcm-3.0.9.1/scripts/gdcmxml
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)       67 2021-07-26 22:48:01.253879 python-gdcm-3.0.9.1/setup.cfg
+-rwxr-xr-x   0 thiago    (1000) thiago    (1000)     7567 2021-07-26 17:03:50.000000 python-gdcm-3.0.9.1/setup.py
```

### Comparing `python-gdcm-3.0.9.0/PKG-INFO` & `python-gdcm-3.0.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gdcm
-Version: 3.0.9.0
+Version: 3.0.9.1
 Summary: Grassroots DICOM runtime libraries
 Home-page: https://github.com/tfmoraes/python-gdcm/
 Author: Thiago Franco de Moraes
 Author-email: totonixsame@gmail.com
 License: BSD
 Description: # Python-GDCM
         
@@ -69,14 +69,16 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
```

### Comparing `python-gdcm-3.0.9.0/README.md` & `python-gdcm-3.0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm.py` & `python-gdcm-3.0.9.1/gdcm.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/.clang-format` & `python-gdcm-3.0.9.1/gdcm_src/.clang-format`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/.travis.yml` & `python-gdcm-3.0.9.1/gdcm_src/.travis.yml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/AUTHORS` & `python-gdcm-3.0.9.1/gdcm_src/AUTHORS`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/deflate.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/deflate.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcm.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcm.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmanon.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmanon.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmcheck.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmcheck.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmconv.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmconv.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmdiff.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmdiff.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmdump.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmdump.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmfile.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmfile.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmgendir.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmgendir.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmimg.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmimg.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcminfo.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcminfo.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmkey.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmkey.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmoverlay.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmoverlay.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmpap3.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmpap3.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmpdf.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmpdf.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmraw.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmraw.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmscanner.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmscanner.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmscu.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmscu.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmstream.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmstream.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmtar.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmtar.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/gdcmxml.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/gdcmxml.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/pdf2dcm.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/pdf2dcm.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/puff.c` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/puff.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Cxx/puff.h` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Cxx/puff.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Python/README` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Python/README`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Python/accessdata.py` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Python/accessdata.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Python/images.py` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Python/images.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Python/lib.py` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Python/lib.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Applications/Python/wado.py` & `python-gdcm-3.0.9.1/gdcm_src/Applications/Python/wado.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/CMakeCSharpCompiler.cmake.in` & `python-gdcm-3.0.9.1/gdcm_src/CMake/CMakeCSharpCompiler.cmake.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/CMakeCSharpInformation.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/CMakeCSharpInformation.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/CMakeDetermineCSharpCompiler.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/CMakeDetermineCSharpCompiler.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/CMakeTestCSharpCompiler.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/CMakeTestCSharpCompiler.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/COPYING-CMAKE-SCRIPTS` & `python-gdcm-3.0.9.1/gdcm_src/CMake/COPYING-CMAKE-SCRIPTS`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/CTestCustom.ctest.in` & `python-gdcm-3.0.9.1/gdcm_src/CMake/CTestCustom.ctest.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/ExportConfiguration/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/CMake/ExportConfiguration/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/ExportConfiguration/GDCMConfig.cmake.in` & `python-gdcm-3.0.9.1/gdcm_src/CMake/ExportConfiguration/GDCMConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/ExportConfiguration/GDCMConfigVersion.cmake.in` & `python-gdcm-3.0.9.1/gdcm_src/CMake/ExportConfiguration/GDCMConfigVersion.cmake.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/ExportConfiguration/UseGDCM.cmake.in` & `python-gdcm-3.0.9.1/gdcm_src/CMake/ExportConfiguration/UseGDCM.cmake.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindACTIVIZ.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindACTIVIZ.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindCSharp.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindCSharp.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindCharLS.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindCharLS.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindDCMTK.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindDCMTK.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindDICOM3TOOLS.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindDICOM3TOOLS.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindDotNETFrameworkSDK.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindDotNETFrameworkSDK.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindJSON.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindJSON.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindJavaProperties.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindJavaProperties.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindKWStyle.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindKWStyle.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindLJPEG.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindLJPEG.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindMAGIC.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindMAGIC.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindMONO.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindMONO.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindMd5sum.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindMd5sum.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindOpenJPEG.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindOpenJPEG.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindOpenSSL.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindOpenSSL.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindPAPYRUS3.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindPAPYRUS3.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindPHP5.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindPHP5.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindPVRGJPEG.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindPVRGJPEG.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindPoppler.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindPoppler.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindRsync.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindRsync.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindSOCKET++.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindSOCKET++.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindSQLITE3.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindSQLITE3.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/FindUUID.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/FindUUID.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/GetSystemProperty.java` & `python-gdcm-3.0.9.1/gdcm_src/CMake/GetSystemProperty.java`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/InstallMacros.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/InstallMacros.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/InstallRequiredVTKLibraries.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/InstallRequiredVTKLibraries.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/Toolchain-gcc-arm-linux-gnueabi.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/Toolchain-gcc-arm-linux-gnueabi.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/Toolchain-gcc-m32.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/Toolchain-gcc-m32.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/Toolchain-gcc-powerpc.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/Toolchain-gcc-powerpc.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/Toolchain-mingw32.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/Toolchain-mingw32.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/Toolchain-mingw64.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/Toolchain-mingw64.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/UseCSharp.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/UseCSharp.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/UseCSharpTest.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/UseCSharpTest.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/UseCopyright.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/UseCopyright.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/UseDebian.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/UseDebian.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/UseJavaTest.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/UseJavaTest.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/UseMONO.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/UseMONO.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/UsePythonTest.cmake` & `python-gdcm-3.0.9.1/gdcm_src/CMake/UsePythonTest.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMake/gdcmValgrind.supp` & `python-gdcm-3.0.9.1/gdcm_src/CMake/gdcmValgrind.supp`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Copyright.txt` & `python-gdcm-3.0.9.1/gdcm_src/Copyright.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/BasicAnonymizer.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/BasicAnonymizer.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/BasicImageAnonymizer.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/BasicImageAnonymizer.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/ClinicalTrialIdentificationWorkflow.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/ClinicalTrialIdentificationWorkflow.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/CompressLossyJPEG.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/CompressLossyJPEG.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/DecompressImage.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/DecompressImage.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/DecompressImageMultiframe.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/DecompressImageMultiframe.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/DecompressJPEGFile.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/DecompressJPEGFile.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/DumpCSA.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/DumpCSA.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/ExtractEncapsulatedFile.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/ExtractEncapsulatedFile.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/ExtractImageRegion.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/ExtractImageRegion.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/ExtractImageRegionWithLUT.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/ExtractImageRegionWithLUT.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/ExtractOneFrame.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/ExtractOneFrame.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/FileAnonymize.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/FileAnonymize.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/FileChangeTS.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/FileChangeTS.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/FileChangeTSLossy.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/FileChangeTSLossy.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/FileStreaming.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/FileStreaming.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/GenerateDICOMDIR.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/GenerateDICOMDIR.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/GetArray.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/GetArray.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/ManipulateFile.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/ManipulateFile.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/MpegVideoInfo.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/MpegVideoInfo.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/NewSequence.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/NewSequence.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/ReformatFile.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/ReformatFile.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/RescaleImage.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/RescaleImage.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/ScanDirectory.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/ScanDirectory.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/SendFileSCU.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/SendFileSCU.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/SimplePrint.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/SimplePrint.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/SimplePrintPatientName.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/SimplePrintPatientName.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/SortImage2.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/SortImage2.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Csharp/StandardizeFiles.cs` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Csharp/StandardizeFiles.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/CStoreQtProgress.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/CStoreQtProgress.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ChangePrivateTags.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ChangePrivateTags.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ChangeSequenceUltrasound.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ChangeSequenceUltrasound.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/CheckBigEndianBug.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/CheckBigEndianBug.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ClinicalTrialAnnotate.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ClinicalTrialAnnotate.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/CompressImage.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/CompressImage.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ConvertToQImage.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ConvertToQImage.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/CreateARGBImage.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/CreateARGBImage.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/CreateCMYKImage.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/CreateCMYKImage.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/CreateJPIPDataSet.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/CreateJPIPDataSet.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DeriveSeries.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DeriveSeries.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DiffFile.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DiffFile.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DiscriminateVolume.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DiscriminateVolume.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DumpADAC.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DumpADAC.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DumpExamCard.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DumpExamCard.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DumpGEMSMovieGroup.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DumpGEMSMovieGroup.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DumpImageHeaderInfo.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DumpImageHeaderInfo.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DumpPhilipsECHO.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DumpPhilipsECHO.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DumpSiemensBase64.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DumpSiemensBase64.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DumpToSQLITE3.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DumpToSQLITE3.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DumpToshibaDTI.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DumpToshibaDTI.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DumpVisusChange.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DumpVisusChange.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/DuplicatePCDE.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/DuplicatePCDE.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ELSCINT1WaveToText.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ELSCINT1WaveToText.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/EmptyMask.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/EmptyMask.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/EncapsulateFileInRawData.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/EncapsulateFileInRawData.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ExtractEncryptedContent.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ExtractEncryptedContent.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ExtractIconFromFile.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ExtractIconFromFile.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/Extracting_All_Resolution.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/Extracting_All_Resolution.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/Fake_Image_Using_Stream_Image_Writer.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/Fake_Image_Using_Stream_Image_Writer.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/FixBrokenJ2K.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/FixBrokenJ2K.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/FixJAIBugJPEGLS.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/FixJAIBugJPEGLS.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/FixOrientation.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/FixOrientation.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/GenAllVR.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/GenAllVR.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/GenFakeIdentifyFile.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/GenFakeIdentifyFile.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/GenFakeImage.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/GenFakeImage.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/GenLongSeqs.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/GenLongSeqs.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/GenSeqs.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/GenSeqs.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/GenerateStandardSOPClasses.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/GenerateStandardSOPClasses.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/GetJPEGSamplePrecision.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/GetJPEGSamplePrecision.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/GetSequenceUltrasound.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/GetSequenceUltrasound.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/GetSubSequenceData.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/GetSubSequenceData.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/HelloVizWorld.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/HelloVizWorld.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/HelloWorld.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/HelloWorld.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/LargeVRDSExplicit.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/LargeVRDSExplicit.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/MakeTemplate.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/MakeTemplate.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/MergeTwoFiles.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/MergeTwoFiles.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/MrProtocol.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/MrProtocol.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/PatchFile.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/PatchFile.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/PrintLUT.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/PrintLUT.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/PublicDict.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/PublicDict.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/QIDO-RS.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/QIDO-RS.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ReadAndDumpDICOMDIR.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ReadAndDumpDICOMDIR.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ReadAndDumpDICOMDIR2.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ReadAndDumpDICOMDIR2.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ReadAndPrintAttributes.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ReadAndPrintAttributes.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ReadExplicitLengthSQIVR.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ReadExplicitLengthSQIVR.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ReadGEMSSDO.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ReadGEMSSDO.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ReadMultiTimesException.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ReadMultiTimesException.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/ReadUTF8QtDir.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/ReadUTF8QtDir.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/SimpleScanner.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/SimpleScanner.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/SortImage.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/SortImage.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/StreamImageReaderTest.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/StreamImageReaderTest.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/TemplateEmptyImage.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/TemplateEmptyImage.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/TraverseModules.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/TraverseModules.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/VolumeSorter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/VolumeSorter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/csa2img.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/csa2img.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/iU22tomultisc.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/iU22tomultisc.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/pmsct_rgb1.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/pmsct_rgb1.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/rle2img.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/rle2img.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Cxx/uid_unique.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Cxx/uid_unique.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Java/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Java/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Java/DecompressImage.java` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Java/DecompressImage.java`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Java/DecompressPixmap.java` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Java/DecompressPixmap.java`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Java/ExtractImageRegion.java` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Java/ExtractImageRegion.java`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Java/FileAnonymize.java` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Java/FileAnonymize.java`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Java/HelloSimple.java` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Java/HelloSimple.java`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Java/ReadFiles.java` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Java/ReadFiles.java`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Java/ScanDirectory.java` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Java/ScanDirectory.java`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Java/SimplePrint.java` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Java/SimplePrint.java`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/PHP/export_pnm.php` & `python-gdcm-3.0.9.1/gdcm_src/Examples/PHP/export_pnm.php`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/PHP/hello_world.php` & `python-gdcm-3.0.9.1/gdcm_src/Examples/PHP/hello_world.php`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/PHP/modify_file.php` & `python-gdcm-3.0.9.1/gdcm_src/Examples/PHP/modify_file.php`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/PHP/qido.php` & `python-gdcm-3.0.9.1/gdcm_src/Examples/PHP/qido.php`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/PHP/rewrite_header.php` & `python-gdcm-3.0.9.1/gdcm_src/Examples/PHP/rewrite_header.php`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/AddPrivateAttribute.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/AddPrivateAttribute.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/ConvertMPL.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/ConvertMPL.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/ConvertNumpy.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/ConvertNumpy.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/ConvertPIL.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/ConvertPIL.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/CreateRAWStorage.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/CreateRAWStorage.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/DecompressImage.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/DecompressImage.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/DumbAnonymizer.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/DumbAnonymizer.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/ExtractImageRegion.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/ExtractImageRegion.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/FindAllPatientName.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/FindAllPatientName.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/FixCommaBug.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/FixCommaBug.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/GetPortionCSAHeader.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/GetPortionCSAHeader.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/HelloWorld.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/HelloWorld.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/ManipulateFile.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/ManipulateFile.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/ManipulateSequence.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/ManipulateSequence.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/MergeFile.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/MergeFile.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/NewSequence.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/NewSequence.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/PhilipsPrivateRescaleInterceptSlope.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/PhilipsPrivateRescaleInterceptSlope.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/PlaySound.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/PlaySound.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/PrivateDict.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/PrivateDict.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/ReWriteSCAsMR.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/ReWriteSCAsMR.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/ReadAndDumpDICOMDIR.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/ReadAndDumpDICOMDIR.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/RemovePrivateTags.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/RemovePrivateTags.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/ScanDirectory.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/ScanDirectory.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/SortImage.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/SortImage.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Examples/Python/WriteBuffer.py` & `python-gdcm-3.0.9.1/gdcm_src/Examples/Python/WriteBuffer.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/INSTALL.txt` & `python-gdcm-3.0.9.1/gdcm_src/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/PACKAGER` & `python-gdcm-3.0.9.1/gdcm_src/PACKAGER`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/README.md` & `python-gdcm-3.0.9.1/gdcm_src/README.md`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmASN1.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmASN1.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmASN1.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmASN1.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmBase64.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmBase64.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmBase64.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmBase64.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmBoxRegion.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmBoxRegion.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmBoxRegion.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmBoxRegion.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmByteSwap.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmByteSwap.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmByteSwap.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmByteSwap.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmByteSwap.txx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmByteSwap.txx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmCAPICryptoFactory.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmCAPICryptoFactory.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmCAPICryptoFactory.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmCAPICryptoFactory.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmCAPICryptographicMessageSyntax.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmCAPICryptographicMessageSyntax.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmCAPICryptographicMessageSyntax.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmCAPICryptographicMessageSyntax.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmCommand.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmCommand.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmCommand.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmCommand.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmConfigure.h.in` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmConfigure.h.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmCryptoFactory.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmCryptoFactory.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmCryptoFactory.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmCryptoFactory.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmCryptographicMessageSyntax.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmCryptographicMessageSyntax.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmCryptographicMessageSyntax.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmCryptographicMessageSyntax.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmDataEvent.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmDataEvent.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmDataEvent.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmDataEvent.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmDeflateStream.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmDeflateStream.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmDeflateStream.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmDeflateStream.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmDirectory.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmDirectory.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmDirectory.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmDirectory.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmDummyValueGenerator.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmDummyValueGenerator.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmDummyValueGenerator.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmDummyValueGenerator.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmEvent.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmEvent.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmEvent.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmEvent.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmException.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmException.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmException.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmException.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmFileNameEvent.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmFileNameEvent.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmFileNameEvent.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmFileNameEvent.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmFilename.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmFilename.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmFilename.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmFilename.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmFilenameGenerator.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmFilenameGenerator.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmFilenameGenerator.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmFilenameGenerator.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmLegacyMacro.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmLegacyMacro.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmMD5.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmMD5.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmMD5.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmMD5.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmObject.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmObject.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmObject.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmObject.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmOpenSSLCryptoFactory.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmOpenSSLCryptoFactory.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmOpenSSLCryptoFactory.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmOpenSSLCryptoFactory.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmOpenSSLCryptographicMessageSyntax.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmOpenSSLCryptographicMessageSyntax.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmOpenSSLCryptographicMessageSyntax.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmOpenSSLCryptographicMessageSyntax.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmOpenSSLP7CryptoFactory.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmOpenSSLP7CryptoFactory.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmOpenSSLP7CryptoFactory.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmOpenSSLP7CryptoFactory.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmOpenSSLP7CryptographicMessageSyntax.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmOpenSSLP7CryptographicMessageSyntax.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmOpenSSLP7CryptographicMessageSyntax.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmOpenSSLP7CryptographicMessageSyntax.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmProgressEvent.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmProgressEvent.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmProgressEvent.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmProgressEvent.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmRegion.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmRegion.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmRegion.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmRegion.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSHA1.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSHA1.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSHA1.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSHA1.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSmartPointer.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSmartPointer.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmStaticAssert.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmStaticAssert.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmString.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmString.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmString.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmString.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSubject.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSubject.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSubject.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSubject.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSwapCode.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSwapCode.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSwapCode.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSwapCode.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSwapper.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSwapper.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSwapper.txx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSwapper.txx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSystem.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSystem.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmSystem.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmSystem.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmTerminal.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmTerminal.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmTerminal.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmTerminal.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmTestDriver.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmTestDriver.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmTesting.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmTesting.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmTesting.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmTesting.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmTrace.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmTrace.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmTrace.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmTrace.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmTypes.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmTypes.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmUnpacker12Bits.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmUnpacker12Bits.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmUnpacker12Bits.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmUnpacker12Bits.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmVersion.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmVersion.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmVersion.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmVersion.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/gdcmWin32.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/gdcmWin32.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/zipstreamimpl.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/zipstreamimpl.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/Common/zipstreamimpl.hpp` & `python-gdcm-3.0.9.1/gdcm_src/Source/Common/zipstreamimpl.hpp`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/06_03_list.txt` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/06_03_list.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/Agfa.xml` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/Agfa.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/COPYRIGHT.dicom3tools` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/COPYRIGHT.dicom3tools`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/CSADefaultDicts.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/CSADefaultDicts.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/CSAHeader.xml` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/CSAHeader.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/DefaultDicts.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/DefaultDicts.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/DefaultPrivateDicts.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/DefaultPrivateDicts.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/HarvestedPrivate.xml` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/HarvestedPrivate.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/ParseDicts.py` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/ParseDicts.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/Part6.xml` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/Part6.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/Part6.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/Part6.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/Part67.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/Part67.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/Part6PDF.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/Part6PDF.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/Part6todcm4che.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/Part6todcm4che.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/Part7.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/Part7.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/Part7a.xml` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/Part7a.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/Part7b.xml` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/Part7b.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/PartToGDCM.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/PartToGDCM.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/README.txt` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/README.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/Siemens.xml` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/Siemens.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/TagKeywords.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/TagKeywords.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/TagToType.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/TagToType.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/TagToVR.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/TagToVR.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/UIDToC++.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/UIDToC++.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/UIDs.xml` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/UIDs.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/VM.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/VM.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/cp699.xml` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/cp699.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/dcmtk.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/dcmtk.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/dicom3tools.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/dicom3tools.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/dicomhdr.html` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/dicomhdr.html`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/dicomhdr.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/dicomhdr.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmCSAHeaderDefaultDicts.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmCSAHeaderDefaultDicts.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmCSAHeaderDict.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmCSAHeaderDict.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmCSAHeaderDictEntry.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmCSAHeaderDictEntry.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmDefaultDicts.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmDefaultDicts.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmDefaultGroupNames.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmDefaultGroupNames.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmDict.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmDict.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmDictConverter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmDictConverter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmDictConverter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmDictConverter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmDictEntry.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmDictEntry.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmDictEntry.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmDictEntry.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmDicts.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmDicts.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmDicts.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmDicts.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmGlobal.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmGlobal.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmGlobal.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmGlobal.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmGroupDict.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmGroupDict.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmGroupDict.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmGroupDict.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmPrepDict.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmPrepDict.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmPrepGroupName.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmPrepGroupName.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmPrivateDefaultDicts.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmPrivateDefaultDicts.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmSOPClassUIDToIOD.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmSOPClassUIDToIOD.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmSOPClassUIDToIOD.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmSOPClassUIDToIOD.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmTagKeywords.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmTagKeywords.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmTagToType.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmTagToType.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmUIDs.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmUIDs.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmUIDs.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmUIDs.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/gdcmconformancetests.xml` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/gdcmconformancetests.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/getname.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/getname.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/getowner.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/getowner.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/getretired.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/getretired.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/order.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/order.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/priv2html.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/priv2html.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/privatedicts.xml` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/privatedicts.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/redo.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/redo.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/redo2.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/redo2.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/sort.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/sort.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/uppercase.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/uppercase.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataDictionary/vital.xml` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataDictionary/vital.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmAttribute.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmAttribute.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmBasicOffsetTable.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmBasicOffsetTable.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmByteBuffer.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmByteBuffer.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmByteSwapFilter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmByteSwapFilter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmByteSwapFilter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmByteSwapFilter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmByteValue.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmByteValue.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmByteValue.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmByteValue.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCP246ExplicitDataElement.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCP246ExplicitDataElement.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCP246ExplicitDataElement.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCP246ExplicitDataElement.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCP246ExplicitDataElement.txx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCP246ExplicitDataElement.txx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCSAElement.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCSAElement.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCSAHeader.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCSAHeader.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCSAHeader.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCSAHeader.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCodeString.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCodeString.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCodeString.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmCodeString.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataElement.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataElement.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataElement.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataElement.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataSet.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataSet.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataSet.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataSet.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataSet.txx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataSet.txx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataSetEvent.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataSetEvent.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataSetEvent.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmDataSetEvent.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmElement.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmElement.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitDataElement.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitDataElement.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitDataElement.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitDataElement.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitDataElement.txx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitDataElement.txx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitImplicitDataElement.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitImplicitDataElement.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitImplicitDataElement.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitImplicitDataElement.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitImplicitDataElement.txx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmExplicitImplicitDataElement.txx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFile.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFile.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFile.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFile.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFileMetaInformation.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFileMetaInformation.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFileMetaInformation.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFileMetaInformation.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFileSet.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFileSet.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFileSet.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFileSet.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFragment.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFragment.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFragment.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFragment.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFragment.txx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmFragment.txx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmImplicitDataElement.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmImplicitDataElement.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmImplicitDataElement.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmImplicitDataElement.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmImplicitDataElement.txx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmImplicitDataElement.txx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmItem.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmItem.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmItem.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmItem.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmItem.txx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmItem.txx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmLO.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmLO.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmMediaStorage.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmMediaStorage.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmMediaStorage.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmMediaStorage.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmMrProtocol.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmMrProtocol.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmMrProtocol.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmMrProtocol.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPDBElement.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPDBElement.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPDBHeader.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPDBHeader.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPDBHeader.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPDBHeader.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmParseException.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmParseException.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmParseException.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmParseException.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmParser.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmParser.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmParser.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmParser.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPreamble.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPreamble.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPreamble.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPreamble.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPrivateTag.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPrivateTag.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPrivateTag.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmPrivateTag.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmReader.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmReader.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmReader.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmReader.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmReader.strict.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmReader.strict.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfFragments.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfFragments.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfFragments.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfFragments.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfFragments.txx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfFragments.txx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfItems.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfItems.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfItems.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfItems.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfItems.txx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmSequenceOfItems.txx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTag.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTag.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTag.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTag.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTagToVR.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTagToVR.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTagToVR.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTagToVR.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTransferSyntax.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTransferSyntax.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTransferSyntax.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmTransferSyntax.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitDataElement.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitDataElement.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitDataElement.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitDataElement.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitDataElement.txx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitDataElement.txx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitImplicitDataElement.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitImplicitDataElement.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitImplicitDataElement.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitImplicitDataElement.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitImplicitDataElement.txx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmUNExplicitImplicitDataElement.txx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVL.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVL.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVM.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVM.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVM.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVM.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVR.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVR.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVR.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVR.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVR16ExplicitDataElement.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVR16ExplicitDataElement.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVR16ExplicitDataElement.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVR16ExplicitDataElement.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVR16ExplicitDataElement.txx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmVR16ExplicitDataElement.txx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmValue.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmValue.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmValue.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmValue.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmValue.txx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmValue.txx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmValueIO.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmValueIO.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmValueIO.txx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmValueIO.txx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmWriter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmWriter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmWriter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/DataStructureAndEncodingDefinition/gdcmWriter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/ParseAttributes.py` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/ParseAttributes.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/Part3.xml` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/Part3.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/Part3.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/Part3.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/Part3New.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/Part3New.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/Part4.xml` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/Part4.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/Part4.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/Part4.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/Part4ToC++.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/Part4ToC++.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/Template.xml.in` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/Template.xml.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/ValueRepresentation.xsd` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/ValueRepresentation.xsd`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/extract.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/extract.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmDefinedTerms.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmDefinedTerms.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmDefinedTerms.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmDefinedTerms.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmDefs.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmDefs.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmDefs.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmDefs.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmEnumeratedValues.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmEnumeratedValues.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmEnumeratedValues.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmEnumeratedValues.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmIOD.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmIOD.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmIOD.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmIOD.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmIODEntry.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmIODEntry.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmIODEntry.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmIODEntry.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmIODs.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmIODs.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmMacro.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmMacro.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmMacro.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmMacro.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmMacroEntry.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmMacroEntry.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmMacros.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmMacros.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmMacros.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmMacros.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmModule.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmModule.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmModule.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmModule.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmModuleEntry.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmModuleEntry.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmModules.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmModules.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmModules.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmModules.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmNestedModuleEntries.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmNestedModuleEntries.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmNestedModuleEntries.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmNestedModuleEntries.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmPatient.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmPatient.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmPatient.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmPatient.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmSeries.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmSeries.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmSeries.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmSeries.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmStudy.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmStudy.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmStudy.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmStudy.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmTable.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmTable.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmTable.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmTable.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmTableEntry.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmTableEntry.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmTableReader.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmTableReader.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmTableReader.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmTableReader.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmTables.h.in` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmTables.h.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmType.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmType.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmType.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmType.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmUsage.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmUsage.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmUsage.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmUsage.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmXMLDictReader.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmXMLDictReader.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmXMLDictReader.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmXMLDictReader.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmXMLPrivateDictReader.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmXMLPrivateDictReader.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/gdcmXMLPrivateDictReader.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/gdcmXMLPrivateDictReader.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/getelements.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/getelements.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/ma2html.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/ma2html.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/InformationObjectDefinition/ma2pdf.xsl` & `python-gdcm-3.0.9.1/gdcm_src/Source/InformationObjectDefinition/ma2pdf.xsl`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/FileMetaInformation.txt` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/FileMetaInformation.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/README.txt` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/README.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/TODO.txt` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/TODO.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAnonymizeEvent.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAnonymizeEvent.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAnonymizeEvent.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAnonymizeEvent.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAnonymizer.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAnonymizer.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAnonymizer.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAnonymizer.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmApplicationEntity.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmApplicationEntity.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmApplicationEntity.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmApplicationEntity.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAudioCodec.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAudioCodec.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAudioCodec.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmAudioCodec.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmBitmap.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmBitmap.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmBitmap.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmBitmap.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmBitmapToBitmapFilter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmBitmapToBitmapFilter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmBitmapToBitmapFilter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmBitmapToBitmapFilter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmCodec.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmCodec.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmCoder.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmCoder.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmConstCharWrapper.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmConstCharWrapper.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmCurve.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmCurve.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmCurve.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmCurve.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDICOMDIR.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDICOMDIR.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDICOMDIR.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDICOMDIR.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDICOMDIRGenerator.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDICOMDIRGenerator.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDICOMDIRGenerator.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDICOMDIRGenerator.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDataSetHelper.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDataSetHelper.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDataSetHelper.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDataSetHelper.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDecoder.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDecoder.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDeltaEncodingCodec.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDeltaEncodingCodec.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDeltaEncodingCodec.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDeltaEncodingCodec.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDictPrinter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDictPrinter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDictPrinter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDictPrinter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDirectionCosines.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDirectionCosines.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDirectionCosines.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDirectionCosines.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDirectoryHelper.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDirectoryHelper.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDirectoryHelper.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDirectoryHelper.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDumper.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDumper.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDumper.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmDumper.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEmptyMaskGenerator.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEmptyMaskGenerator.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEmptyMaskGenerator.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEmptyMaskGenerator.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEncapsulatedDocument.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEncapsulatedDocument.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEncapsulatedDocument.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEncapsulatedDocument.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEquipmentManufacturer.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEquipmentManufacturer.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEquipmentManufacturer.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmEquipmentManufacturer.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFiducials.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFiducials.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFiducials.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFiducials.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileAnonymizer.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileAnonymizer.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileAnonymizer.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileAnonymizer.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileChangeTransferSyntax.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileChangeTransferSyntax.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileChangeTransferSyntax.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileChangeTransferSyntax.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileDecompressLookupTable.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileDecompressLookupTable.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileDecompressLookupTable.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileDecompressLookupTable.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileDerivation.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileDerivation.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileDerivation.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileDerivation.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileExplicitFilter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileExplicitFilter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileExplicitFilter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileExplicitFilter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileStreamer.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileStreamer.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileStreamer.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmFileStreamer.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIPPSorter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIPPSorter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIPPSorter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIPPSorter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImage.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImage.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImage.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImage.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImageFilter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImageFilter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImageFilter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImageFilter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImageGenerator.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImageGenerator.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImageGenerator.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmIconImageGenerator.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImage.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImage.cxx`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #include "gdcmExplicitDataElement.h"
 #include "gdcmByteValue.h"
 #include "gdcmDataSet.h"
 #include "gdcmSequenceOfFragments.h"
 #include "gdcmFragment.h"
 
 #include <iostream>
+#include <limits>
 
 namespace gdcm
 {
 
 const double *Image::GetSpacing() const
 {
   assert( NumberOfDimensions );
```

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImage.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImage.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageApplyLookupTable.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageApplyLookupTable.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageApplyLookupTable.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageApplyLookupTable.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangePhotometricInterpretation.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangePhotometricInterpretation.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangePhotometricInterpretation.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangePhotometricInterpretation.h`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 =========================================================================*/
 #ifndef GDCMIMAGECHANGEPHOTOMETRICINTERPRETATION_H
 #define GDCMIMAGECHANGEPHOTOMETRICINTERPRETATION_H
 
 #include "gdcmImageToImageFilter.h"
 #include "gdcmPhotometricInterpretation.h"
+#include <limits>
 
 namespace gdcm
 {
 
 class DataElement;
 /**
  * \brief ImageChangePhotometricInterpretation class
```

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangePlanarConfiguration.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangePlanarConfiguration.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangePlanarConfiguration.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangePlanarConfiguration.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangeTransferSyntax.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangeTransferSyntax.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangeTransferSyntax.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageChangeTransferSyntax.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageCodec.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageCodec.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageCodec.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageCodec.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageConverter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageConverter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageConverter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageConverter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageFragmentSplitter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageFragmentSplitter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageFragmentSplitter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageFragmentSplitter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageHelper.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageHelper.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageHelper.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageHelper.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageReader.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageReader.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageReader.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageReader.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageRegionReader.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageRegionReader.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageRegionReader.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageRegionReader.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageToImageFilter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageToImageFilter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageToImageFilter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageToImageFilter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageWriter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageWriter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageWriter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmImageWriter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG12Codec.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG12Codec.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG12Codec.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG12Codec.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG16Codec.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG16Codec.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG16Codec.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG16Codec.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG2000Codec.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG2000Codec.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG2000Codec.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG2000Codec.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG8Codec.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG8Codec.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG8Codec.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEG8Codec.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEGBITSCodec.hxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEGBITSCodec.hxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEGCodec.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEGCodec.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEGCodec.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEGCodec.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEGLSCodec.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEGLSCodec.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEGLSCodec.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJPEGLSCodec.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJSON.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJSON.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJSON.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmJSON.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmKAKADUCodec.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmKAKADUCodec.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmKAKADUCodec.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmKAKADUCodec.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmLookupTable.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmLookupTable.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmLookupTable.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmLookupTable.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmMeshPrimitive.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmMeshPrimitive.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmMeshPrimitive.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmMeshPrimitive.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmOrientation.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmOrientation.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmOrientation.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmOrientation.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmOverlay.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmOverlay.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmOverlay.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmOverlay.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPDFCodec.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPDFCodec.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPDFCodec.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPDFCodec.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPGXCodec.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPGXCodec.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPGXCodec.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPGXCodec.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPNMCodec.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPNMCodec.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPNMCodec.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPNMCodec.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPVRGCodec.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPVRGCodec.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPVRGCodec.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPVRGCodec.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPersonName.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPersonName.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPersonName.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPersonName.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPhotometricInterpretation.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPhotometricInterpretation.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPhotometricInterpretation.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPhotometricInterpretation.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixelFormat.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixelFormat.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixelFormat.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixelFormat.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmap.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmap.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmap.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmap.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapReader.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapReader.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapReader.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapReader.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapToPixmapFilter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapToPixmapFilter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapToPixmapFilter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapToPixmapFilter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapWriter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapWriter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapWriter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPixmapWriter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPrinter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPrinter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPrinter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmPrinter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRAWCodec.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRAWCodec.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRAWCodec.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRAWCodec.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRLECodec.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRLECodec.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRLECodec.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRLECodec.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRescaler.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRescaler.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRescaler.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmRescaler.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmScanner.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmScanner.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmScanner.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmScanner.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegment.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegment.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegment.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegment.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentHelper.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentHelper.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentHelper.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentHelper.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentReader.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentReader.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentReader.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentReader.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentWriter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentWriter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentWriter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentWriter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentedPaletteColorLookupTable.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentedPaletteColorLookupTable.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentedPaletteColorLookupTable.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSegmentedPaletteColorLookupTable.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSerieHelper.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSerieHelper.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSerieHelper.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSerieHelper.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSimpleSubjectWatcher.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSimpleSubjectWatcher.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSimpleSubjectWatcher.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSimpleSubjectWatcher.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSorter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSorter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSorter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSorter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSpacing.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSpacing.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSpacing.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSpacing.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSpectroscopy.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSpectroscopy.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSpectroscopy.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSpectroscopy.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSplitMosaicFilter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSplitMosaicFilter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSplitMosaicFilter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSplitMosaicFilter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStreamImageReader.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStreamImageReader.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStreamImageReader.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStreamImageReader.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStreamImageWriter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStreamImageWriter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStreamImageWriter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStreamImageWriter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStrictScanner.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStrictScanner.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStrictScanner.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStrictScanner.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStringFilter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStringFilter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStringFilter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmStringFilter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurface.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurface.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurface.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurface.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceHelper.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceHelper.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceHelper.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceHelper.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceReader.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceReader.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceReader.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceReader.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceWriter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceWriter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceWriter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmSurfaceWriter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmTagPath.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmTagPath.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmTagPath.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmTagPath.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmUIDGenerator.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmUIDGenerator.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmUIDGenerator.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmUIDGenerator.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmUUIDGenerator.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmUUIDGenerator.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmUUIDGenerator.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmUUIDGenerator.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmValidate.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmValidate.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmValidate.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmValidate.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmWaveform.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmWaveform.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmWaveform.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmWaveform.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmXMLPrinter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmXMLPrinter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcmXMLPrinter.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcmXMLPrinter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcm_j2k.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcm_j2k.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MediaStorageAndFileFormat/gdcm_jp2.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MediaStorageAndFileFormat/gdcm_jp2.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/README.txt` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/README.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAAbortPDU.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAAbortPDU.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAAbortPDU.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAAbortPDU.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateACPDU.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateACPDU.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateACPDU.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateACPDU.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateRJPDU.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateRJPDU.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateRJPDU.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateRJPDU.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateRQPDU.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateRQPDU.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateRQPDU.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAAssociateRQPDU.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmARTIMTimer.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmARTIMTimer.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmARTIMTimer.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmARTIMTimer.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAReleaseRPPDU.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAReleaseRPPDU.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAReleaseRPPDU.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAReleaseRPPDU.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAReleaseRQPDU.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAReleaseRQPDU.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAReleaseRQPDU.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAReleaseRQPDU.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAbstractSyntax.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAbstractSyntax.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAbstractSyntax.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAbstractSyntax.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmApplicationContext.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmApplicationContext.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmApplicationContext.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmApplicationContext.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAsynchronousOperationsWindowSub.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAsynchronousOperationsWindowSub.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmAsynchronousOperationsWindowSub.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmAsynchronousOperationsWindowSub.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseCompositeMessage.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseCompositeMessage.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseNormalizedMessage.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseNormalizedMessage.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmBasePDU.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmBasePDU.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseQuery.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseQuery.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseQuery.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseQuery.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseRootQuery.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseRootQuery.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseRootQuery.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmBaseRootQuery.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCEchoMessages.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCEchoMessages.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCEchoMessages.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCEchoMessages.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCFindMessages.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCFindMessages.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCFindMessages.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCFindMessages.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCMoveMessages.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCMoveMessages.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCMoveMessages.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCMoveMessages.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCStoreMessages.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCStoreMessages.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCStoreMessages.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCStoreMessages.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCommandDataSet.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCommandDataSet.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCommandDataSet.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCommandDataSet.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCompositeMessageFactory.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCompositeMessageFactory.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCompositeMessageFactory.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCompositeMessageFactory.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCompositeNetworkFunctions.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCompositeNetworkFunctions.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmCompositeNetworkFunctions.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmCompositeNetworkFunctions.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmDIMSE.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmDIMSE.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmFindPatientRootQuery.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmFindPatientRootQuery.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmFindPatientRootQuery.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmFindPatientRootQuery.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmFindStudyRootQuery.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmFindStudyRootQuery.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmFindStudyRootQuery.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmFindStudyRootQuery.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationClassUIDSub.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationClassUIDSub.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationClassUIDSub.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationClassUIDSub.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationUIDSub.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationUIDSub.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationUIDSub.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationUIDSub.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationVersionNameSub.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationVersionNameSub.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationVersionNameSub.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmImplementationVersionNameSub.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmMaximumLengthSub.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmMaximumLengthSub.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmMaximumLengthSub.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmMaximumLengthSub.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmModalityPerformedProcedureStepCreateQuery.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmModalityPerformedProcedureStepCreateQuery.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmModalityPerformedProcedureStepCreateQuery.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmModalityPerformedProcedureStepCreateQuery.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmModalityPerformedProcedureStepSetQuery.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmModalityPerformedProcedureStepSetQuery.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmModalityPerformedProcedureStepSetQuery.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmModalityPerformedProcedureStepSetQuery.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmMovePatientRootQuery.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmMovePatientRootQuery.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmMovePatientRootQuery.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmMovePatientRootQuery.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmMoveStudyRootQuery.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmMoveStudyRootQuery.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmMoveStudyRootQuery.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmMoveStudyRootQuery.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNActionMessages.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNActionMessages.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNActionMessages.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNActionMessages.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNCreateMessages.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNCreateMessages.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNCreateMessages.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNCreateMessages.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNDeleteMessages.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNDeleteMessages.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNDeleteMessages.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNDeleteMessages.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNEventReportMessages.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNEventReportMessages.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNEventReportMessages.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNEventReportMessages.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNGetMessages.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNGetMessages.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNGetMessages.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNGetMessages.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNSetMessages.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNSetMessages.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNSetMessages.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNSetMessages.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNetworkEvents.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNetworkEvents.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNetworkStateID.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNetworkStateID.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNormalizedMessageFactory.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNormalizedMessageFactory.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNormalizedMessageFactory.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNormalizedMessageFactory.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNormalizedNetworkFunctions.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNormalizedNetworkFunctions.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmNormalizedNetworkFunctions.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmNormalizedNetworkFunctions.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPDUFactory.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPDUFactory.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPDUFactory.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPDUFactory.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPDataTFPDU.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPDataTFPDU.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPDataTFPDU.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPDataTFPDU.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContext.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContext.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContext.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContext.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextAC.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextAC.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextAC.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextAC.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextGenerator.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextGenerator.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextGenerator.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextGenerator.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextRQ.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextRQ.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextRQ.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationContextRQ.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationDataValue.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationDataValue.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationDataValue.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmPresentationDataValue.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryBase.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryBase.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryBase.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryBase.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryFactory.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryFactory.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryFactory.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryFactory.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryImage.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryImage.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryImage.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryImage.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryPatient.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryPatient.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryPatient.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryPatient.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQuerySeries.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQuerySeries.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQuerySeries.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQuerySeries.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryStudy.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryStudy.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryStudy.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmQueryStudy.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmRoleSelectionSub.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmRoleSelectionSub.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmRoleSelectionSub.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmRoleSelectionSub.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmSOPClassExtendedNegociationSub.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmSOPClassExtendedNegociationSub.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmSOPClassExtendedNegociationSub.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmSOPClassExtendedNegociationSub.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmServiceClassApplicationInformation.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmServiceClassApplicationInformation.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmServiceClassApplicationInformation.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmServiceClassApplicationInformation.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmServiceClassUser.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmServiceClassUser.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmServiceClassUser.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmServiceClassUser.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmTransferSyntaxSub.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmTransferSyntaxSub.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmTransferSyntaxSub.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmTransferSyntaxSub.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULAction.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULAction.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAA.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAA.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAA.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAA.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAE.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAE.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAE.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAE.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAR.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAR.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAR.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionAR.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionDT.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionDT.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionDT.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULActionDT.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULBasicCallback.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULBasicCallback.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULBasicCallback.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULBasicCallback.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnection.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnection.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnection.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnection.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnectionCallback.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnectionCallback.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnectionInfo.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnectionInfo.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnectionInfo.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnectionInfo.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnectionManager.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnectionManager.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnectionManager.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULConnectionManager.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULEvent.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULEvent.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULTransitionTable.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULTransitionTable.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULTransitionTable.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULTransitionTable.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULWritingCallback.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULWritingCallback.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmULWritingCallback.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmULWritingCallback.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmUserInformation.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmUserInformation.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmUserInformation.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmUserInformation.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmWLMFindQuery.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmWLMFindQuery.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Source/MessageExchangeDefinition/gdcmWLMFindQuery.h` & `python-gdcm-3.0.9.1/gdcm_src/Source/MessageExchangeDefinition/gdcmWLMFindQuery.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/TODO` & `python-gdcm-3.0.9.1/gdcm_src/TODO`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/KWStyle/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/KWStyle/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/KWStyle/GDCMFiles.txt.in` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/KWStyle/GDCMFiles.txt.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/KWStyle/GDCMHeader.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/KWStyle/GDCMHeader.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/Release/bootstrap.sh` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/Release/bootstrap.sh`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/Release/config.linux` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/Release/config.linux`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/Release/config.win32` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/Release/config.win32`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/Release/release.bat` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/Release/release.bat`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/Release/release.sh` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/Release/release.sh`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/Release/upload.sh` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/Release/upload.sh`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Applications/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Applications/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Applications/gdcm2pnm.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Applications/gdcm2pnm.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Applications/gdcm2vtk.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Applications/gdcm2vtk.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Applications/gdcmviewer.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Applications/gdcmviewer.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/AssemblyInfo.cs.in` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/AssemblyInfo.cs.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/HelloActiviz.cs` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/HelloActiviz.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/HelloActiviz2.cs` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/HelloActiviz2.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/HelloActiviz3.cs` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/HelloActiviz3.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/HelloActiviz4.cs` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/HelloActiviz4.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/HelloActiviz5.cs` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/HelloActiviz5.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/HelloVTKWorld.cs` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/HelloVTKWorld.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/HelloVTKWorld2.cs` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/HelloVTKWorld2.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/MetaImageMD5Activiz.cs` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/MetaImageMD5Activiz.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Csharp/RefCounting.cs` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Csharp/RefCounting.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/Compute3DSpacing.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/Compute3DSpacing.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/Convert16BitsTo8Bits.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/Convert16BitsTo8Bits.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/ConvertMultiFrameToSingleFrame.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/ConvertMultiFrameToSingleFrame.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/ConvertRGBToLuminance.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/ConvertRGBToLuminance.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/ConvertSingleBitTo8Bits.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/ConvertSingleBitTo8Bits.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/CreateFakePET.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/CreateFakePET.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/CreateFakeRTDOSE.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/CreateFakeRTDOSE.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/GenerateRTSTRUCT.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/GenerateRTSTRUCT.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/MagnifyFile.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/MagnifyFile.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmorthoplanes.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmorthoplanes.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmreslice.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmreslice.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmrtionplan.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmrtionplan.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmrtplan.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmrtplan.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmscene.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmscene.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmtexture.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmtexture.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmvolume.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/gdcmvolume.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/offscreenimage.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/offscreenimage.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/reslicesphere.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/reslicesphere.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/rtstructapp.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/rtstructapp.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Cxx/threadgdcm.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Cxx/threadgdcm.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Java/AWTMedical3.java` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Java/AWTMedical3.java`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Java/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Java/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Java/HelloVTKWorld.java` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Java/HelloVTKWorld.java`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Java/MIPViewer.java` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Java/MIPViewer.java`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Java/MPRViewer.java` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Java/MPRViewer.java`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Java/MPRViewer2.java` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Java/MPRViewer2.java`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Java/ReadSeriesIntoVTK.java` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Java/ReadSeriesIntoVTK.java`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/PHP/generate_png.php` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/PHP/generate_png.php`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Python/CastConvertPhilips.py` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Python/CastConvertPhilips.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Examples/Python/headsq2dcm.py` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Examples/Python/headsq2dcm.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/GDCMImageGUI.xml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/GDCMImageGUI.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/GDCMImageReader.xml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/GDCMImageReader.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/MummySettings.xml.in` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/MummySettings.xml.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageActor.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageActor.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader1.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader1.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader2_1.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader2_1.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader2_2.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader2_2.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader2_3.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader2_3.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader3.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader3.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader4.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReader4.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReaderIsLossy.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageReaderIsLossy.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageViewer.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageViewer.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageWriter1.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageWriter1.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageWriter2.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageWriter2.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageWriterIsLossy.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMImageWriterIsLossy.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMMetaImageWriter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMMetaImageWriter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMMetaImageWriter2.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMMetaImageWriter2.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMPolyDataReader.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMPolyDataReader.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMThreadedImageReader.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMThreadedImageReader.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMThreadedImageReader2.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkGDCMThreadedImageReader2.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkImageChangeInformation.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Cxx/TestvtkImageChangeInformation.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Java/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Java/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Java/TestvtkGDCMImageReader.java` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Java/TestvtkGDCMImageReader.java`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Python/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Python/TestMultiframeGrayscaleWordSecondaryCaptureImageStorage.py` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Python/TestMultiframeGrayscaleWordSecondaryCaptureImageStorage.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Python/TestvtkGDCMImageReader.py` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Python/TestvtkGDCMImageReader.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Python/TestvtkGDCMImageReader2.py` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Python/TestvtkGDCMImageReader2.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Python/TestvtkGDCMImageWriter.py` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Python/TestvtkGDCMImageWriter.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Python/TestvtkGDCMThreadedImageReader.py` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Python/TestvtkGDCMThreadedImageReader.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/Testing/Python/TestvtkGDCMThreadedImageReader2.py` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/Testing/Python/TestvtkGDCMThreadedImageReader2.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/VTK4/vtkMedicalImageProperties.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/VTK4/vtkMedicalImageProperties.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/VTK4/vtkMedicalImageProperties.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/VTK4/vtkMedicalImageProperties.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/VTK4/vtkStringArray.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/VTK4/vtkStringArray.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/VTK4/vtkStringArray.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/VTK4/vtkStringArray.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMImageReader.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMImageReader.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMImageReader.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMImageReader.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMImageReader2.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMImageReader2.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMImageReader2.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMImageReader2.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMImageReader_Extra.cs` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMImageReader_Extra.cs`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMImageWriter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMImageWriter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMImageWriter.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMImageWriter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMMedicalImageProperties.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMMedicalImageProperties.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMMedicalImageProperties.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMMedicalImageProperties.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMPolyDataReader.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMPolyDataReader.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMPolyDataReader.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMPolyDataReader.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMPolyDataWriter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMPolyDataWriter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMPolyDataWriter.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMPolyDataWriter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMTesting.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMTesting.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMTesting.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMTesting.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMThreadedImageReader.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMThreadedImageReader.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMThreadedImageReader.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMThreadedImageReader.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMThreadedImageReader2.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMThreadedImageReader2.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkGDCMThreadedImageReader2.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkGDCMThreadedImageReader2.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImageColorViewer.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImageColorViewer.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImageColorViewer.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImageColorViewer.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImageMapToColors16.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImageMapToColors16.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImageMapToColors16.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImageMapToColors16.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImageMapToWindowLevelColors2.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImageMapToWindowLevelColors2.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImageMapToWindowLevelColors2.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImageMapToWindowLevelColors2.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImagePlanarComponentsToComponents.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImagePlanarComponentsToComponents.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImagePlanarComponentsToComponents.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImagePlanarComponentsToComponents.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImageRGBToYBR.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImageRGBToYBR.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImageRGBToYBR.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImageRGBToYBR.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImageYBRToRGB.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImageYBRToRGB.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkImageYBRToRGB.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkImageYBRToRGB.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkLookupTable16.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkLookupTable16.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkLookupTable16.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkLookupTable16.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkRTStructSetProperties.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkRTStructSetProperties.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkRTStructSetProperties.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkRTStructSetProperties.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkgdcm.i` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkgdcm.i`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/VTK/vtkgdcm.py` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/VTK/vtkgdcm.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/dicom3tools/process.sh` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/dicom3tools/process.sh`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/README` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/README`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/authors.xml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/authors.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/doxyfile.in` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/doxyfile.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/footer.html` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/footer.html`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcm2pnm.xml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcm2pnm.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcm2vtk.xml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcm2vtk.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmanon.xml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmanon.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmconv.xml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmconv.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmdiff.xml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmdiff.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmdump.xml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmdump.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmgendir.xml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmgendir.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmimg.xml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmimg.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcminfo.xml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcminfo.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmpap3.xml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmpap3.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmpdf.xml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmpdf.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmraw.xml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmraw.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmscanner.xml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmscanner.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmscu.xml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmscu.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmtar.xml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmtar.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmviewer.xml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmviewer.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/man/gdcmxml.xml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/man/gdcmxml.xml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/vtk/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/vtk/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/vtk/doc_makeall.sh.in` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/vtk/doc_makeall.sh.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/doxygen/vtk/doxyfile.in` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/doxygen/vtk/doxyfile.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcm_charls.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcm_charls.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcm_expat.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcm_expat.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcm_ljpeg12.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcm_ljpeg12.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcm_ljpeg16.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcm_ljpeg16.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcm_ljpeg8.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcm_ljpeg8.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcm_md5.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcm_md5.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcm_openjpeg.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcm_openjpeg.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcm_uuid.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcm_uuid.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcm_zlib.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcm_zlib.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/License.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/License.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/README.GDCM.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/README.GDCM.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/charls.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/charls.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/colortransform.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/colortransform.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/context.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/context.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/contextrunmode.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/contextrunmode.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/decoderstrategy.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/decoderstrategy.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/defaulttraits.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/defaulttraits.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/encoderstrategy.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/encoderstrategy.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/interface.cpp` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/interface.cpp`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/jpegimagedatasegment.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/jpegimagedatasegment.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/jpegls.cpp` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/jpegls.cpp`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/jpegmarkercode.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/jpegmarkercode.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/jpegmarkersegment.cpp` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/jpegmarkersegment.cpp`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/jpegmarkersegment.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/jpegmarkersegment.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/jpegstreamreader.cpp` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/jpegstreamreader.cpp`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/jpegstreamreader.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/jpegstreamreader.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/jpegstreamwriter.cpp` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/jpegstreamwriter.cpp`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/jpegstreamwriter.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/jpegstreamwriter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/lookuptable.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/lookuptable.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/losslesstraits.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/losslesstraits.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/processline.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/processline.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/publictypes.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/publictypes.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/scan.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/scan.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/styleanddesign.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/styleanddesign.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmcharls/util.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmcharls/util.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/COPYING` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/COPYING`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/Changes` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/Changes`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/README` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/README`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/doc/reference.html` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/doc/reference.html`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/doc/style.css` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/doc/style.css`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/doc/xmlwf.1` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/doc/xmlwf.1`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/doc/xmlwf.sgml` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/doc/xmlwf.sgml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/examples/elements.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/examples/elements.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/examples/outline.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/examples/outline.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/expat_config.h.in` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/expat_config.h.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/expat_mangle.h.in` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/expat_mangle.h.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/ascii.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/ascii.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/asciitab.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/asciitab.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/expat.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/expat.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/expat_external.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/expat_external.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/iasciitab.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/iasciitab.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/internal.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/internal.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/latin1tab.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/latin1tab.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/nametab.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/nametab.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/utf8tab.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/utf8tab.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/xmlparse.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/xmlparse.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/xmlrole.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/xmlrole.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/xmlrole.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/xmlrole.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/xmltok.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/xmltok.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/xmltok.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/xmltok.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/xmltok_impl.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/xmltok_impl.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/xmltok_impl.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/xmltok_impl.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/lib/xmltok_ns.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/lib/xmltok_ns.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/README.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/README.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/benchmark/README.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/benchmark/README.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/benchmark/benchmark.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/benchmark/benchmark.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/chardata.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/chardata.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/chardata.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/chardata.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/minicheck.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/minicheck.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/minicheck.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/minicheck.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/runtests.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/runtests.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/tests/xmltest.sh` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/tests/xmltest.sh`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/codepage.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/codepage.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/ct.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/ct.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/readfilemap.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/readfilemap.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/unixfilemap.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/unixfilemap.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/win32filemap.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/win32filemap.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlfile.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlfile.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlmime.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlmime.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/xmltchar.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/xmltchar.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlwf.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlwf.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlwin32url.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmexpat/xmlwf/xmlwin32url.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/12/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/12/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/16/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/16/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/8/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/8/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/COPYRIGHT.dcmtk` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/COPYRIGHT.dcmtk`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/Jfif.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/Jfif.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/README` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/README`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/README.GDCM.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/README.GDCM.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/change.log` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/change.log`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/dcmtk.sh` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/dcmtk.sh`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/example.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/example.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/filelist.doc` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/filelist.doc`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/install.doc` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/install.doc`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcapimin.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcapimin.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcapistd.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcapistd.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jccoefct.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jccoefct.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jccolor.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jccolor.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcdctmgr.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcdctmgr.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcdiffct.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcdiffct.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jchuff.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jchuff.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jchuff.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jchuff.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcinit.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcinit.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jclhuff.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jclhuff.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jclossls.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jclossls.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jclossy.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jclossy.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcmainct.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcmainct.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcmarker.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcmarker.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcmaster.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcmaster.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcodec.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcodec.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcomapi.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcomapi.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jconfig.doc` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jconfig.doc`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jconfig.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jconfig.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcparam.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcparam.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcphuff.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcphuff.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcpred.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcpred.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcprepct.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcprepct.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcsample.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcsample.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcscale.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcscale.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jcshuff.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jcshuff.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jctrans.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jctrans.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdapimin.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdapimin.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdapistd.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdapistd.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdatadst.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdatadst.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdatasrc.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdatasrc.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdcoefct.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdcoefct.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdcolor.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdcolor.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdct.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdct.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jddctmgr.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jddctmgr.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jddiffct.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jddiffct.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdhuff.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdhuff.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdhuff.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdhuff.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdinput.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdinput.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdlhuff.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdlhuff.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdlossls.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdlossls.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdlossy.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdlossy.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdmainct.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdmainct.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdmarker.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdmarker.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdmaster.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdmaster.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdmerge.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdmerge.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdphuff.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdphuff.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdpostct.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdpostct.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdpred.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdpred.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdsample.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdsample.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdscale.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdscale.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdshuff.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdshuff.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jdtrans.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jdtrans.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jerror.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jerror.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jerror.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jerror.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jfdctflt.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jfdctflt.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jfdctfst.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jfdctfst.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jfdctint.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jfdctint.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jidctflt.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jidctflt.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jidctfst.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jidctfst.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jidctint.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jidctint.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jidctred.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jidctred.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jinclude.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jinclude.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jlossls.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jlossls.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jlossy.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jlossy.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jmemmgr.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jmemmgr.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jmemnobs.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jmemnobs.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jmemsrc.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jmemsrc.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jmemsys.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jmemsys.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jmorecfg.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jmorecfg.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jpegcmake.h.in` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jpegcmake.h.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jpegint.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jpegint.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jpeglib.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jpeglib.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jquant1.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jquant1.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jquant2.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jquant2.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/jutils.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/jutils.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/libjpeg.doc` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/libjpeg.doc`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/mangle_jpeg.h.in` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/mangle_jpeg.h.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/structure.doc` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/structure.doc`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/usage.doc` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/usage.doc`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmjpeg/wizard.doc` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmjpeg/wizard.doc`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmmd5/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmmd5/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmmd5/COPYING` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmmd5/COPYING`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmmd5/md5.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmmd5/md5.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmmd5/md5.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmmd5/md5.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmmd5/md5_mangle.h.in` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmmd5/md5_mangle.h.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmmd5/md5cmp.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmmd5/md5cmp.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmmd5/md5main.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmmd5/md5main.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmmd5/tst2md5.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmmd5/tst2md5.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/LICENSE` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/LICENSE`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/README.GDCM.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/README.GDCM.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/CTestCustom.cmake.in` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/CTestCustom.cmake.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/EnsureFileInclude.cmake` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/EnsureFileInclude.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/FindFCGI.cmake` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/FindFCGI.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/FindLCMS.cmake` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/FindLCMS.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/FindLCMS2.cmake` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/FindLCMS2.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/OpenJPEGCPack.cmake` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/OpenJPEGCPack.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/OpenJPEGConfig.cmake.in` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/OpenJPEGConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/TestLargeFiles.c.cmake.in` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/TestLargeFiles.c.cmake.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/TestLargeFiles.cmake` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/TestLargeFiles.cmake`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/cmake/openjpeg_valgrind.supp` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/cmake/openjpeg_valgrind.supp`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/bio.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/bio.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/bio.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/bio.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/cidx_manager.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/cidx_manager.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/cidx_manager.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/cidx_manager.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/cio.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/cio.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/cio.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/cio.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/dwt.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/dwt.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/dwt.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/dwt.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/event.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/event.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/event.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/event.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/function_list.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/function_list.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/function_list.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/function_list.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/image.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/image.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/image.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/image.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/indexbox_manager.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/indexbox_manager.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/invert.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/invert.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/invert.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/invert.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/j2k.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/j2k.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/j2k.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/j2k.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/jp2.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/jp2.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/jp2.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/jp2.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/mct.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/mct.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/mct.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/mct.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/mqc.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/mqc.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/mqc.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/mqc.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/mqc_inl.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/mqc_inl.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/openjpeg.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/openjpeg.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/openjpeg.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/openjpeg.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/openjpeg_mangle.h.in` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/openjpeg_mangle.h.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_clock.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_clock.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_clock.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_clock.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_codec.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_codec.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_common.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_common.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_config_private.h.cmake.in` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_config_private.h.cmake.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_includes.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_includes.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_intmath.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_intmath.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_inttypes.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_inttypes.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_malloc.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_malloc.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_malloc.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_malloc.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_stdint.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/opj_stdint.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/phix_manager.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/phix_manager.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/pi.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/pi.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/pi.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/pi.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/ppix_manager.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/ppix_manager.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/sparse_array.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/sparse_array.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/sparse_array.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/sparse_array.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t1.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t1.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t1.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t1.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t1_generate_luts.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t1_generate_luts.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t1_luts.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t1_luts.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t2.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t2.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t2.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/t2.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tcd.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tcd.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tcd.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tcd.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tgt.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tgt.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tgt.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tgt.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/thix_manager.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/thix_manager.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/thread.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/thread.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/thread.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/thread.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tls_keys.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tls_keys.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tpix_manager.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmopenjpeg/src/lib/openjp2/tpix_manager.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmrle/info.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmrle/info.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmrle/info.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmrle/info.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmrle/io.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmrle/io.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmrle/io.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmrle/io.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmrle/main.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmrle/main.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmrle/rle.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmrle/rle.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmrle/rle.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmrle/rle.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmutfcpp/utf8/checked.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmutfcpp/utf8/checked.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmutfcpp/utf8/core.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmutfcpp/utf8/core.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmutfcpp/utf8/unchecked.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmutfcpp/utf8/unchecked.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmutfcpp/utf8.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmutfcpp/utf8.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/COPYING` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/COPYING`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/compare.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/compare.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/gen_uuid.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/gen_uuid.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/pack.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/pack.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/parse.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/parse.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/unpack.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/unpack.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/unparse.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/unparse.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/uuid.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/uuid.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/uuidP.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/uuidP.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/uuid_mangle.h.in` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/uuid_mangle.h.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmuuid/uuid_time.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmuuid/uuid_time.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/COPYING` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/COPYING`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/ChangeLog` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/ChangeLog`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/FAQ` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/FAQ`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/INDEX` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/INDEX`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/README` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/README`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/adler32.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/adler32.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/algorithm.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/algorithm.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/compress.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/compress.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/crc32.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/crc32.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/crc32.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/crc32.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/deflate.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/deflate.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/deflate.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/deflate.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/example.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/example.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/README.examples` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/README.examples`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/fitblk.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/fitblk.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/gun.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/gun.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/gzappend.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/gzappend.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/gzjoin.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/gzjoin.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/gzlog.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/gzlog.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/gzlog.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/gzlog.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/zlib_how.html` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/zlib_how.html`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/zpipe.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/zpipe.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/examples/zran.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/examples/zran.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/gzio.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/gzio.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/infback.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/infback.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/inffast.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/inffast.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/inffixed.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/inffixed.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/inflate.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/inflate.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/inflate.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/inflate.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/inftrees.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/inftrees.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/inftrees.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/inftrees.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/minigzip.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/minigzip.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/trees.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/trees.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/trees.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/trees.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/uncompr.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/uncompr.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/zconf.in.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/zconf.in.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/zlib.3` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/zlib.3`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/zlib.def.in` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/zlib.def.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/zlib.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/zlib.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/zlib.rc` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/zlib.rc`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/zutil.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/zutil.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/gdcmzlib/zutil.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/gdcmzlib/zutil.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/getopt/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/getopt/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/getopt/COPYING` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/getopt/COPYING`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/getopt/ex_getopt.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/getopt/ex_getopt.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/getopt/getopt.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/getopt/getopt.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/getopt/getopt.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/getopt/getopt.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/getopt/getopt_long.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/getopt/getopt_long.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/CHANGES` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/CHANGES`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/COPYING` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/COPYING`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/README` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/README`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/SETUP` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/SETUP`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/chendct.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/chendct.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/codec.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/codec.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/csize.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/csize.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/dct.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/dct.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/globals.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/globals.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/huffman.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/huffman.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/io.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/io.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/jpeg.1` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/jpeg.1`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/jpeg.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/jpeg.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/leedct.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/leedct.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/lexer.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/lexer.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/lexer.l` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/lexer.l`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/marker.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/marker.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/marker.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/marker.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/param.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/param.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/prototypes.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/prototypes.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/pvrgjpeg.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/pvrgjpeg.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/stream.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/stream.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/stream.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/stream.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/system.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/system.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/tables.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/tables.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/pvrg/transform.c` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/pvrg/transform.c`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/config.h.in` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/config.h.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/echo.cpp` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/echo.cpp`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/echo.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/echo.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/fork.cpp` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/fork.cpp`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/fork.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/fork.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/ftp.cpp` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/ftp.cpp`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/ftp.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/ftp.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/local.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/local.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/pipestream.cpp` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/pipestream.cpp`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/pipestream.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/pipestream.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/protocol.cpp` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/protocol.cpp`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/protocol.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/protocol.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/sig.cpp` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/sig.cpp`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/sig.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/sig.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/smtp.cpp` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/smtp.cpp`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/smtp.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/smtp.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/sockinet.cpp` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/sockinet.cpp`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/sockinet.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/sockinet.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/sockstream.cpp` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/sockstream.cpp`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/sockstream.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/sockstream.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/sockunix.cpp` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/sockunix.cpp`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Utilities/socketxx/socket++/sockunix.h` & `python-gdcm-3.0.9.1/gdcm_src/Utilities/socketxx/socket++/sockunix.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Csharp/AssemblyInfo.cs.in` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Csharp/AssemblyInfo.cs.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Csharp/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Csharp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Csharp/docstrings.i` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Csharp/docstrings.i`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Csharp/doxy2swig.py` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Csharp/doxy2swig.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Csharp/gdcm.i` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Csharp/gdcm.i`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Csharp/gdcm_arrays_csharp.i` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Csharp/gdcm_arrays_csharp.i`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Csharp/key.snk` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Csharp/key.snk`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Csharp/std_set.i` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Csharp/std_set.i`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Csharp/version.rc.in` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Csharp/version.rc.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Java/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Java/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Java/gdcm.i` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Java/gdcm.i`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Java/main.java` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Java/main.java`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Java/std_set.i` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Java/std_set.i`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/PHP/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/PHP/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/PHP/gdcm.i` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/PHP/gdcm.i`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Perl/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Perl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Perl/gdcm.i` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Perl/gdcm.i`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/CMakeLists.txt` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/Python.h.in` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/Python.h.in`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/TestWrap.py` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/TestWrap.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/docstrings.i` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/docstrings.i`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/doxy2swig.py` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/doxy2swig.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/gdcm.py` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/gdcm.py`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/gdcmPythonFilter.cxx` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/gdcmPythonFilter.cxx`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/gdcmPythonFilter.h` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/gdcmPythonFilter.h`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/Python/gdcmswig.i` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/Python/gdcmswig.i`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/Wrapping/SWIGCommon/gdcmcommon.i` & `python-gdcm-3.0.9.1/gdcm_src/Wrapping/SWIGCommon/gdcmcommon.i`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/gdcm_src/appveyor.yml` & `python-gdcm-3.0.9.1/gdcm_src/appveyor.yml`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/python_gdcm.egg-info/PKG-INFO` & `python-gdcm-3.0.9.1/python_gdcm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gdcm
-Version: 3.0.9.0
+Version: 3.0.9.1
 Summary: Grassroots DICOM runtime libraries
 Home-page: https://github.com/tfmoraes/python-gdcm/
 Author: Thiago Franco de Moraes
 Author-email: totonixsame@gmail.com
 License: BSD
 Description: # Python-GDCM
         
@@ -69,14 +69,16 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
```

### Comparing `python-gdcm-3.0.9.0/python_gdcm.egg-info/SOURCES.txt` & `python-gdcm-3.0.9.1/python_gdcm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-gdcm-3.0.9.0/setup.py` & `python-gdcm-3.0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
             shutil.rmtree(BUILD_DIR)
         else:
             super().build_extension(ext)
 
 
 setuptools.setup(
     name="python-gdcm",
-    version="3.0.9.0",
+    version="3.0.9.1",
     author="Thiago Franco de Moraes",
     author_email="totonixsame@gmail.com",
     description="Grassroots DICOM runtime libraries",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tfmoraes/python-gdcm/",
     license="BSD",
@@ -213,14 +213,16 @@
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: C",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Scientific/Engineering",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "Operating System :: Unix",
         "Operating System :: MacOS",
```

