# Comparing `tmp/xrootd-5.5.4.tar.gz` & `tmp/xrootd-5.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/dss/xrootd/dist/tmpywna6bsr/xrootd-5.5.4.tar", last modified: Fri Mar 24 08:34:00 2023, max compression
+gzip compressed data, was "/builds/dss/xrootd/dist/tmprpatuqqq/xrootd-5.5.5.tar", last modified: Mon May  8 08:46:34 2023, max compression
```

## Comparing `xrootd-5.5.4.tar` & `xrootd-5.5.5.tar`

### file list

```diff
@@ -1,1663 +1,1663 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/bindings/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/bindings/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/bindings/python/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/bindings/python/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/bindings/python/docs/source/.static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/bindings/python/docs/source/.static/css/
--rwxrwxrwx   0 root         (0) root         (0)    15713 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/source/.static/css/custom.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/bindings/python/docs/source/.templates/
--rwxrwxrwx   0 root         (0) root         (0)       89 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/source/.templates/layout.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/bindings/python/docs/source/examples/
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/source/examples/copyprocess.rst
--rw-rw-rw-   0 root         (0) root         (0)     2842 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/source/examples/file.rst
--rw-rw-rw-   0 root         (0) root         (0)     3243 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/source/examples/filesystem.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/bindings/python/docs/source/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/bindings/python/docs/source/modules/client/
--rw-rw-rw-   0 root         (0) root         (0)      423 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/source/modules/client/copyprocess.rst
--rw-rw-rw-   0 root         (0) root         (0)     1385 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/source/modules/client/file.rst
--rw-rw-rw-   0 root         (0) root         (0)     1293 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/source/modules/client/filesystem.rst
--rw-rw-rw-   0 root         (0) root         (0)     5238 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/source/modules/client/flags.rst
--rw-rw-rw-   0 root         (0) root         (0)      944 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/source/modules/client/responses.rst
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/source/modules/client/url.rst
--rw-rw-rw-   0 root         (0) root         (0)      304 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/source/modules/client/utils.rst
--rw-rw-rw-   0 root         (0) root         (0)     8013 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/source/examples.rst
--rw-rw-rw-   0 root         (0) root         (0)     4286 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/source/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     3673 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/source/gettingstarted.rst
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/source/install.rst
--rw-rw-rw-   0 root         (0) root         (0)    14979 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/source/xrootd-200x68.png
--rw-rw-rw-   0 root         (0) root         (0)     5581 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     1225 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/docs/ReleaseNotes.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/bindings/python/examples/
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/copy.py
--rw-rw-rw-   0 root         (0) root         (0)     1655 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/copyprocess.py
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/dirlist.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/fcntl.py
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/fcntl_async.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/fileproperties.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/filesystemproperties.py
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/iterate.py
--rw-rw-rw-   0 root         (0) root         (0)      388 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/locate.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/mkdir.py
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/mv.py
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/query.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/read.py
--rw-rw-rw-   0 root         (0) root         (0)      349 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/readchunks.py
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/readlines.py
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/rm.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/rmdir.py
--rw-rw-rw-   0 root         (0) root         (0)      850 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/vector_read.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/visa.py
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/visa_async.py
--rw-rw-rw-   0 root         (0) root         (0)      356 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/examples/write.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/bindings/python/libs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/bindings/python/libs/client/
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/libs/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1313 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/libs/client/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     7054 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/libs/client/copyprocess.py
--rw-rw-rw-   0 root         (0) root         (0)     2426 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/libs/client/env.py
--rw-rw-rw-   0 root         (0) root         (0)    13367 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/libs/client/file.py
--rw-rw-rw-   0 root         (0) root         (0)    17398 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/libs/client/filesystem.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/libs/client/finalize.py
--rw-rw-rw-   0 root         (0) root         (0)     2892 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/libs/client/flags.py
--rw-rw-rw-   0 root         (0) root         (0)     4357 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/libs/client/glob_funcs.py
--rw-rw-rw-   0 root         (0) root         (0)    11449 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/libs/client/responses.py
--rw-rw-rw-   0 root         (0) root         (0)     2842 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/libs/client/url.py
--rw-rw-rw-   0 root         (0) root         (0)     3926 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/libs/client/utils.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/bindings/python/src/
--rw-rw-rw-   0 root         (0) root         (0)    12167 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/src/AsyncResponseHandler.hh
--rw-rw-rw-   0 root         (0) root         (0)     6731 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/src/ChunkIterator.hh
--rw-rw-rw-   0 root         (0) root         (0)    13695 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/src/Conversions.hh
--rw-rw-rw-   0 root         (0) root         (0)     1904 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/src/PyXRootD.hh
--rw-rw-rw-   0 root         (0) root         (0)     8623 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/src/PyXRootDCopyProcess.cc
--rw-rw-rw-   0 root         (0) root         (0)     6663 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/src/PyXRootDCopyProcess.hh
--rw-rw-rw-   0 root         (0) root         (0)     4415 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/src/PyXRootDCopyProgressHandler.cc
--rw-rw-rw-   0 root         (0) root         (0)     3562 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/src/PyXRootDCopyProgressHandler.hh
--rw-rw-rw-   0 root         (0) root         (0)     5119 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/src/PyXRootDEnv.hh
--rw-rw-rw-   0 root         (0) root         (0)    35727 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/src/PyXRootDFile.cc
--rw-rw-rw-   0 root         (0) root         (0)    12231 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/src/PyXRootDFile.hh
--rw-rw-rw-   0 root         (0) root         (0)    37416 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/src/PyXRootDFileSystem.cc
--rw-rw-rw-   0 root         (0) root         (0)    10740 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/src/PyXRootDFileSystem.hh
--rw-rw-rw-   0 root         (0) root         (0)     2135 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/src/PyXRootDFinalize.hh
--rw-rw-rw-   0 root         (0) root         (0)     5199 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/src/PyXRootDModule.cc
--rw-rw-rw-   0 root         (0) root         (0)     7612 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/src/PyXRootDURL.cc
--rw-rw-rw-   0 root         (0) root         (0)     8015 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/src/PyXRootDURL.hh
--rw-rw-rw-   0 root         (0) root         (0)     6144 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/src/Utils.cc
--rw-rw-rw-   0 root         (0) root         (0)     4293 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/src/Utils.hh
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/bindings/python/tests/
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/tests/env.py
--rw-rw-rw-   0 root         (0) root         (0)     1839 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/tests/test_copy.py
--rw-rw-rw-   0 root         (0) root         (0)    11797 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/tests/test_file.py
--rw-rw-rw-   0 root         (0) root         (0)     5387 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/tests/test_filesystem.py
--rw-rw-rw-   0 root         (0) root         (0)     1728 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/tests/test_glob.py
--rw-rw-rw-   0 root         (0) root         (0)      785 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/tests/test_threads.py
--rw-rw-rw-   0 root         (0) root         (0)     1340 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/tests/test_url.py
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/.gitattributes
--rwxrwxrwx   0 root         (0) root         (0)       70 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     4286 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      688 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/README.rst
--rw-r--r--   0 root         (0) root         (0)        6 2023-03-24 08:34:00.000000 xrootd-5.5.4/bindings/python/VERSION
--rw-rw-rw-   0 root         (0) root         (0)     4611 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/python/setup.py.in
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-03-24 08:33:03.000000 xrootd-5.5.4/bindings/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/cmake/
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/FindAutoConf.cmake
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/FindAutoMake.cmake
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/FindCppUnit.cmake
--rw-rw-rw-   0 root         (0) root         (0)      407 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/FindDavix.cmake
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/FindKerberos5.cmake
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/FindLibTool.cmake
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/FindMacaroons.cmake
--rw-rw-rw-   0 root         (0) root         (0)     1699 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/FindReadline.cmake
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/FindSciTokensCpp.cmake
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/FindTinyXml.cmake
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/FindVOMS.cmake
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/FindYasm.cmake
--rw-rw-rw-   0 root         (0) root         (0)      740 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/Findfuse.cmake
--rw-rw-rw-   0 root         (0) root         (0)     1505 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/Findlibuuid.cmake
--rw-rw-rw-   0 root         (0) root         (0)      683 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/Findsystemd.cmake
--rw-rw-rw-   0 root         (0) root         (0)     7023 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/GNUInstallDirs.cmake
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/XRootDCommon.cmake
--rw-rw-rw-   0 root         (0) root         (0)     7570 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/XRootDConfig.cmake.in
--rw-rw-rw-   0 root         (0) root         (0)     2561 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/XRootDDefaults.cmake
--rw-rw-rw-   0 root         (0) root         (0)     4939 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/XRootDFindLibs.cmake
--rw-rw-rw-   0 root         (0) root         (0)     6893 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/XRootDOSDefs.cmake
--rw-rw-rw-   0 root         (0) root         (0)     2473 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/XRootDSummary.cmake
--rw-rw-rw-   0 root         (0) root         (0)     6716 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/XRootDSystemCheck.cmake
--rw-rw-rw-   0 root         (0) root         (0)     2565 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake/XRootDUtils.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/docs/man/
--rw-rw-rw-   0 root         (0) root         (0)      938 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/man/cmsd.8
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/man/frm_admin.8
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/man/frm_purged.8
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/man/frm_xfragent.8
--rw-rw-rw-   0 root         (0) root         (0)     1016 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/man/frm_xfrd.8
--rw-rw-rw-   0 root         (0) root         (0)     4438 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/man/libXrdVoms.1
--rw-rw-rw-   0 root         (0) root         (0)     1046 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/man/mpxstats.8
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/man/xrdadler32.1
--rw-rw-rw-   0 root         (0) root         (0)    17298 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/man/xrdcp.1
--rw-rw-rw-   0 root         (0) root         (0)     6354 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/man/xrdfs.1
--rw-rw-rw-   0 root         (0) root         (0)     1792 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/man/xrdgsiproxy.1
--rw-rw-rw-   0 root         (0) root         (0)     6823 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/man/xrdgsitest.1
--rw-rw-rw-   0 root         (0) root         (0)     1322 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/man/xrdmapc.1
--rw-rw-rw-   0 root         (0) root         (0)     2071 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/man/xrdpfc_print.8
--rw-rw-rw-   0 root         (0) root         (0)      872 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/man/xrdpwdadmin.8
--rw-rw-rw-   0 root         (0) root         (0)      850 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/man/xrdsssadmin.8
--rw-rw-rw-   0 root         (0) root         (0)      993 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/man/xrootd.8
--rw-rw-rw-   0 root         (0) root         (0)     3745 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/man/xrootdfs.1
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/PreReleaseNotes.txt
--rw-rw-rw-   0 root         (0) root         (0)     4415 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/README_IPV4_To_IPV6
--rw-rw-rw-   0 root         (0) root         (0)   169296 2023-03-24 08:33:03.000000 xrootd-5.5.4/docs/ReleaseNotes.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/packaging/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/packaging/common/
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/common/client-plugin.conf.example
--rw-rw-rw-   0 root         (0) root         (0)     6149 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/common/client.conf
--rw-rw-rw-   0 root         (0) root         (0)      494 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/common/cmsd@.service
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/common/frm_purged@.service
--rw-rw-rw-   0 root         (0) root         (0)      479 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/common/frm_xfrd@.service
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/common/http.client.conf.example
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/common/recorder.conf
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/common/xrdhttp@.socket
--rw-rw-rw-   0 root         (0) root         (0)     3006 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/common/xrootd-clustered.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3342 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/common/xrootd-filecache-clustered.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1666 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/common/xrootd-filecache-standalone.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1986 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/common/xrootd-http.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1590 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/common/xrootd-standalone.cfg
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/common/xrootd.logrotate
--rw-rw-rw-   0 root         (0) root         (0)      680 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/common/xrootd.te
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/common/xrootd@.service
--rw-rw-rw-   0 root         (0) root         (0)      122 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/common/xrootd@.socket
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/packaging/debian/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/packaging/debian/source/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/source/format
--rw-rw-rw-   0 root         (0) root         (0)        3 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/compat
--rw-rw-rw-   0 root         (0) root         (0)    16401 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/control
--rw-rw-rw-   0 root         (0) root         (0)     1328 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/copyright
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/libxrdapputils1.install
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/libxrdcl2.install
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/libxrdcrypto1.install
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/libxrdcryptolite1.install
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/libxrdffs2.install
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/libxrdhttputils1.install
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/libxrdposix2.install
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/libxrdserver2.install
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/libxrdssilib1.install
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/libxrdssishmap1.install
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/libxrdutils2.install
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/libxrdxml2.install
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/libxrootd-client-dev.install
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/libxrootd-dev.install
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/libxrootd-private-dev.install
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/libxrootd-server-dev.install
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/python3-xrootd.install
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/python3-xrootd.install.new
--rwxrwxrwx   0 root         (0) root         (0)      820 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/rules
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/xrootd-client-devel.install
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/xrootd-client-libs.install
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/xrootd-client-plugins.install
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/xrootd-client.install
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/xrootd-clients.install
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/xrootd-devel.install
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/xrootd-fuse.install
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/xrootd-libs.install
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/xrootd-plugins.install
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/xrootd-private-devel.install
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/xrootd-server-devel.install
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/xrootd-server-libs.install
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/xrootd-server-plugins.install
--rw-rw-rw-   0 root         (0) root         (0)      542 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian/xrootd-server.install
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/packaging/debian_scripts/
--rwxrwxrwx   0 root         (0) root         (0)     1745 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/debian_scripts/publish_debian_cern.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/packaging/rhel/
--rw-rw-rw-   0 root         (0) root         (0)      809 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/rhel/cmsd.init
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/rhel/frm_purged.init
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/rhel/frm_xfrd.init
--rw-rw-rw-   0 root         (0) root         (0)     8866 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/rhel/xrootd.functions
--rw-rw-rw-   0 root         (0) root         (0)     8451 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/rhel/xrootd.functions-slc4
--rw-rw-rw-   0 root         (0) root         (0)      861 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/rhel/xrootd.init
--rw-rw-rw-   0 root         (0) root         (0)    36694 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/rhel/xrootd.spec.in
--rw-rw-rw-   0 root         (0) root         (0)     3489 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/rhel/xrootd.sysconfig
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/rhel/xrootd.tmpfiles
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/packaging/tgz/
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/tgz/README
--rwxrwxrwx   0 root         (0) root         (0)     4590 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/tgz/StartCMS
--rwxrwxrwx   0 root         (0) root         (0)     4388 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/tgz/StartFRM
--rwxrwxrwx   0 root         (0) root         (0)     5420 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/tgz/StartOLB
--rw-rw-rw-   0 root         (0) root         (0)     2063 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/tgz/StartOLB.cf.example
--rwxrwxrwx   0 root         (0) root         (0)     4767 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/tgz/StartXRD
--rw-rw-rw-   0 root         (0) root         (0)     3842 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/tgz/StartXRD.cf.example
--rwxrwxrwx   0 root         (0) root         (0)     3039 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/tgz/StopCMS
--rwxrwxrwx   0 root         (0) root         (0)     3735 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/tgz/StopFRM
--rwxrwxrwx   0 root         (0) root         (0)     2910 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/tgz/StopOLB
--rwxrwxrwx   0 root         (0) root         (0)     2615 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/tgz/StopXRD
--rw-rw-rw-   0 root         (0) root         (0)     1988 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/tgz/xrootd.cf.example
--rw-rw-rw-   0 root         (0) root         (0)     3914 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/tgz/xrootd.cf.example2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/packaging/wheel/
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/wheel/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     2632 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/wheel/TestCXX14.txt
--rwxrwxrwx   0 root         (0) root         (0)      201 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/wheel/has_c++14.sh
--rwxrwxrwx   0 root         (0) root         (0)     1407 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/wheel/install.sh
--rwxrwxrwx   0 root         (0) root         (0)     1240 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/wheel/publish.sh
--rw-rw-rw-   0 root         (0) root         (0)     7310 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/wheel/setup.py
--rwxrwxrwx   0 root         (0) root         (0)    10336 2023-03-24 08:33:03.000000 xrootd-5.5.4/packaging/makesrpm.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XProtocol/
--rw-rw-rw-   0 root         (0) root         (0)      947 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XProtocol/README
--rw-rw-rw-   0 root         (0) root         (0)    11295 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XProtocol/XProtocol.cc
--rw-rw-rw-   0 root         (0) root         (0)    50827 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XProtocol/XProtocol.hh
--rw-rw-rw-   0 root         (0) root         (0)     5574 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XProtocol/XPtypes.hh
--rw-rw-rw-   0 root         (0) root         (0)    25337 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XProtocol/YProtocol.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/Xrd/
--rw-rw-rw-   0 root         (0) root         (0)     9005 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdBuffXL.cc
--rw-rw-rw-   0 root         (0) root         (0)     3279 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdBuffXL.hh
--rw-rw-rw-   0 root         (0) root         (0)    11819 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdBuffer.cc
--rw-rw-rw-   0 root         (0) root         (0)     4299 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdBuffer.hh
--rw-rw-rw-   0 root         (0) root         (0)    91975 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdConfig.cc
--rw-rw-rw-   0 root         (0) root         (0)     5523 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdConfig.hh
--rw-rw-rw-   0 root         (0) root         (0)     2900 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdGlobals.cc
--rw-rw-rw-   0 root         (0) root         (0)     9400 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdInet.cc
--rw-rw-rw-   0 root         (0) root         (0)     3445 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdInet.hh
--rw-rw-rw-   0 root         (0) root         (0)     2840 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdInfo.cc
--rw-rw-rw-   0 root         (0) root         (0)     2489 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdInfo.hh
--rw-rw-rw-   0 root         (0) root         (0)     3099 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdJob.hh
--rw-rw-rw-   0 root         (0) root         (0)    25173 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdLink.cc
--rw-rw-rw-   0 root         (0) root         (0)    26923 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdLink.hh
--rw-rw-rw-   0 root         (0) root         (0)    14522 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdLinkCtl.cc
--rw-rw-rw-   0 root         (0) root         (0)     9846 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdLinkCtl.hh
--rw-rw-rw-   0 root         (0) root         (0)     3499 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdLinkInfo.hh
--rw-rw-rw-   0 root         (0) root         (0)     5054 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdLinkMatch.cc
--rw-rw-rw-   0 root         (0) root         (0)     3288 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdLinkMatch.hh
--rw-rw-rw-   0 root         (0) root         (0)    46764 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdLinkXeq.cc
--rw-rw-rw-   0 root         (0) root         (0)     7101 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdLinkXeq.hh
--rw-rw-rw-   0 root         (0) root         (0)     8748 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdMain.cc
--rw-rw-rw-   0 root         (0) root         (0)     5456 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdObject.hh
--rw-rw-rw-   0 root         (0) root         (0)     4407 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdObject.icc
--rw-rw-rw-   0 root         (0) root         (0)    12682 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdPoll.cc
--rw-rw-rw-   0 root         (0) root         (0)     5648 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdPoll.hh
--rw-rw-rw-   0 root         (0) root         (0)     3601 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdPollE.hh
--rw-rw-rw-   0 root         (0) root         (0)    14457 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdPollE.icc
--rw-rw-rw-   0 root         (0) root         (0)     3308 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdPollInfo.hh
--rw-rw-rw-   0 root         (0) root         (0)     3207 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdPollPoll.hh
--rw-rw-rw-   0 root         (0) root         (0)    17863 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdPollPoll.icc
--rw-rw-rw-   0 root         (0) root         (0)    12456 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdProtLoad.cc
--rw-rw-rw-   0 root         (0) root         (0)     3854 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdProtLoad.hh
--rw-rw-rw-   0 root         (0) root         (0)    10727 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdProtocol.hh
--rw-rw-rw-   0 root         (0) root         (0)    24210 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdScheduler.cc
--rw-rw-rw-   0 root         (0) root         (0)     5635 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdScheduler.hh
--rw-rw-rw-   0 root         (0) root         (0)    13605 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdSendQ.cc
--rw-rw-rw-   0 root         (0) root         (0)     3735 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdSendQ.hh
--rw-rw-rw-   0 root         (0) root         (0)    12208 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdStats.cc
--rw-rw-rw-   0 root         (0) root         (0)     3836 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdStats.hh
--rw-rw-rw-   0 root         (0) root         (0)     4914 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdTcpMonPin.hh
--rw-rw-rw-   0 root         (0) root         (0)     3291 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/Xrd/XrdTrace.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdAcc/
--rw-rw-rw-   0 root         (0) root         (0)    18177 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdAcc/XrdAccAccess.cc
--rw-rw-rw-   0 root         (0) root         (0)     8058 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdAcc/XrdAccAccess.hh
--rw-rw-rw-   0 root         (0) root         (0)     4734 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdAcc/XrdAccAudit.cc
--rw-rw-rw-   0 root         (0) root         (0)     5263 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdAcc/XrdAccAudit.hh
--rw-rw-rw-   0 root         (0) root         (0)     5258 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdAcc/XrdAccAuthDB.hh
--rw-rw-rw-   0 root         (0) root         (0)    12972 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdAcc/XrdAccAuthFile.cc
--rw-rw-rw-   0 root         (0) root         (0)     3587 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdAcc/XrdAccAuthFile.hh
--rw-rw-rw-   0 root         (0) root         (0)    12043 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdAcc/XrdAccAuthorize.hh
--rw-rw-rw-   0 root         (0) root         (0)     7602 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdAcc/XrdAccCapability.cc
--rw-rw-rw-   0 root         (0) root         (0)     5914 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdAcc/XrdAccCapability.hh
--rw-rw-rw-   0 root         (0) root         (0)    34347 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdAcc/XrdAccConfig.cc
--rw-rw-rw-   0 root         (0) root         (0)     5754 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdAcc/XrdAccConfig.hh
--rw-rw-rw-   0 root         (0) root         (0)     8327 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdAcc/XrdAccEntity.cc
--rw-rw-rw-   0 root         (0) root         (0)     5422 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdAcc/XrdAccEntity.hh
--rw-rw-rw-   0 root         (0) root         (0)    15372 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdAcc/XrdAccGroups.cc
--rw-rw-rw-   0 root         (0) root         (0)     7392 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdAcc/XrdAccGroups.hh
--rw-rw-rw-   0 root         (0) root         (0)     4791 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdAcc/XrdAccPrivs.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdApps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdApps/XrdClProxyPlugin/
--rw-rw-rw-   0 root         (0) root         (0)     7035 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdClProxyPlugin/ProxyPrefixFile.cc
--rw-rw-rw-   0 root         (0) root         (0)     8962 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdClProxyPlugin/ProxyPrefixFile.hh
--rw-rw-rw-   0 root         (0) root         (0)     4214 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdClProxyPlugin/ProxyPrefixPlugin.cc
--rw-rw-rw-   0 root         (0) root         (0)     2721 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdClProxyPlugin/ProxyPrefixPlugin.hh
--rw-rw-rw-   0 root         (0) root         (0)     1822 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdClProxyPlugin/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdApps/XrdClRecordPlugin/
--rw-rw-rw-   0 root         (0) root         (0)    14346 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdClRecordPlugin/README.md
--rw-rw-rw-   0 root         (0) root         (0)    13235 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdClRecordPlugin/XrdClAction.hh
--rw-rw-rw-   0 root         (0) root         (0)     9856 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdClRecordPlugin/XrdClActionMetrics.hh
--rw-rw-rw-   0 root         (0) root         (0)    18873 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdClRecordPlugin/XrdClRecorder.hh
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdClRecordPlugin/XrdClRecorderPlugin.cc
--rw-rw-rw-   0 root         (0) root         (0)     3178 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdClRecordPlugin/XrdClRecorderPlugin.hh
--rw-rw-rw-   0 root         (0) root         (0)    53534 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdClRecordPlugin/XrdClReplay.cc
--rw-rw-rw-   0 root         (0) root         (0)     7563 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdClRecordPlugin/XrdClReplayArgs.hh
--rw-rw-rw-   0 root         (0) root         (0)    14497 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdAccTest.cc
--rw-rw-rw-   0 root         (0) root         (0)     7192 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdAppsCconfig.cc
--rw-rw-rw-   0 root         (0) root         (0)     6428 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdCks.cc
--rw-rw-rw-   0 root         (0) root         (0)    40600 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdCpConfig.cc
--rw-rw-rw-   0 root         (0) root         (0)    13017 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdCpConfig.hh
--rw-rw-rw-   0 root         (0) root         (0)     7118 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdCpFile.cc
--rw-rw-rw-   0 root         (0) root         (0)     3726 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdCpFile.hh
--rw-rw-rw-   0 root         (0) root         (0)     6172 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdCrc32c.cc
--rw-rw-rw-   0 root         (0) root         (0)    19828 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdMapCluster.cc
--rw-rw-rw-   0 root         (0) root         (0)    10453 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdMpxStats.cc
--rw-rw-rw-   0 root         (0) root         (0)    15755 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdMpxXml.cc
--rw-rw-rw-   0 root         (0) root         (0)     3279 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdMpxXml.hh
--rw-rw-rw-   0 root         (0) root         (0)     5291 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdPinls.cc
--rw-rw-rw-   0 root         (0) root         (0)    10301 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdPrep.cc
--rw-rw-rw-   0 root         (0) root         (0)     8375 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdQStats.cc
--rw-rw-rw-   0 root         (0) root         (0)    10351 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/XrdWait41.cc
--rw-rw-rw-   0 root         (0) root         (0)     9299 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps/Xrdadler32.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdBwm/
--rw-rw-rw-   0 root         (0) root         (0)    38144 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdBwm/XrdBwm.cc
--rw-rw-rw-   0 root         (0) root         (0)    12819 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdBwm/XrdBwm.hh
--rw-rw-rw-   0 root         (0) root         (0)    15615 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdBwm/XrdBwmConfig.cc
--rw-rw-rw-   0 root         (0) root         (0)    14111 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdBwm/XrdBwmHandle.cc
--rw-rw-rw-   0 root         (0) root         (0)     4374 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdBwm/XrdBwmHandle.hh
--rw-rw-rw-   0 root         (0) root         (0)    11034 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdBwm/XrdBwmLogger.cc
--rw-rw-rw-   0 root         (0) root         (0)     3761 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdBwm/XrdBwmLogger.hh
--rw-rw-rw-   0 root         (0) root         (0)     8624 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdBwm/XrdBwmPolicy.hh
--rw-rw-rw-   0 root         (0) root         (0)     6036 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdBwm/XrdBwmPolicy1.cc
--rw-rw-rw-   0 root         (0) root         (0)     4429 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdBwm/XrdBwmPolicy1.hh
--rw-rw-rw-   0 root         (0) root         (0)     3388 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdBwm/XrdBwmTrace.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdCks/
--rw-rw-rw-   0 root         (0) root         (0)    16444 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCks.hh
--rw-rw-rw-   0 root         (0) root         (0)     7765 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksAssist.cc
--rw-rw-rw-   0 root         (0) root         (0)     6718 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksAssist.hh
--rw-rw-rw-   0 root         (0) root         (0)     8525 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksCalc.hh
--rw-rw-rw-   0 root         (0) root         (0)     5687 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksCalcadler32.hh
--rw-rw-rw-   0 root         (0) root         (0)     8639 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksCalccrc32.cc
--rw-rw-rw-   0 root         (0) root         (0)     3654 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksCalccrc32.hh
--rw-rw-rw-   0 root         (0) root         (0)     1003 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksCalccrc32C.cc
--rw-rw-rw-   0 root         (0) root         (0)     2986 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksCalccrc32C.hh
--rw-rw-rw-   0 root         (0) root         (0)    12260 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksCalcmd5.cc
--rw-rw-rw-   0 root         (0) root         (0)     3564 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksCalcmd5.hh
--rw-rw-rw-   0 root         (0) root         (0)     5036 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksCalczcrc32.cc
--rw-rw-rw-   0 root         (0) root         (0)    10222 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksConfig.cc
--rw-rw-rw-   0 root         (0) root         (0)     3663 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksConfig.hh
--rw-rw-rw-   0 root         (0) root         (0)     5671 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksData.hh
--rw-rw-rw-   0 root         (0) root         (0)     7928 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksLoader.cc
--rw-rw-rw-   0 root         (0) root         (0)     6105 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksLoader.hh
--rw-rw-rw-   0 root         (0) root         (0)     9341 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksManOss.cc
--rw-rw-rw-   0 root         (0) root         (0)     3480 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksManOss.hh
--rw-rw-rw-   0 root         (0) root         (0)    21161 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksManager.cc
--rw-rw-rw-   0 root         (0) root         (0)     5041 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksManager.hh
--rw-rw-rw-   0 root         (0) root         (0)    14952 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksWrapper.hh
--rw-rw-rw-   0 root         (0) root         (0)     4283 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCks/XrdCksXAttr.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdCl/
--rw-rw-rw-   0 root         (0) root         (0)     8580 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)     5609 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClAnyObject.hh
--rw-rw-rw-   0 root         (0) root         (0)     3364 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClApply.hh
--rw-rw-rw-   0 root         (0) root         (0)    13157 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClArg.hh
--rw-rw-rw-   0 root         (0) root         (0)     3439 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClAsyncDiscardReader.hh
--rw-rw-rw-   0 root         (0) root         (0)     7661 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClAsyncHSReader.hh
--rw-rw-rw-   0 root         (0) root         (0)     5998 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClAsyncHSWriter.hh
--rw-rw-rw-   0 root         (0) root         (0)    17225 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClAsyncMsgReader.hh
--rw-rw-rw-   0 root         (0) root         (0)    10892 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClAsyncMsgWriter.hh
--rw-rw-rw-   0 root         (0) root         (0)    12785 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClAsyncPageReader.hh
--rw-rw-rw-   0 root         (0) root         (0)     8622 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClAsyncRawReader.hh
--rw-rw-rw-   0 root         (0) root         (0)     7097 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClAsyncRawReaderIntfc.hh
--rw-rw-rw-   0 root         (0) root         (0)    33331 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClAsyncSocketHandler.cc
--rw-rw-rw-   0 root         (0) root         (0)    12769 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClAsyncSocketHandler.hh
--rw-rw-rw-   0 root         (0) root         (0)    11781 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClAsyncVectorReader.hh
--rw-rw-rw-   0 root         (0) root         (0)     9115 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClBuffer.hh
--rw-rw-rw-   0 root         (0) root         (0)     8775 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClChannel.cc
--rw-rw-rw-   0 root         (0) root         (0)     7235 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClChannel.hh
--rw-rw-rw-   0 root         (0) root         (0)     2701 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClChannelHandlerList.cc
--rw-rw-rw-   0 root         (0) root         (0)     2547 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClChannelHandlerList.hh
--rw-rw-rw-   0 root         (0) root         (0)     5702 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClCheckSumHelper.hh
--rw-rw-rw-   0 root         (0) root         (0)     5843 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClCheckSumManager.cc
--rw-rw-rw-   0 root         (0) root         (0)     3367 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClCheckSumManager.hh
--rw-rw-rw-   0 root         (0) root         (0)     8890 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClCheckpointOperation.hh
--rw-rw-rw-   0 root         (0) root         (0)   109531 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClClassicCopyJob.cc
--rw-rw-rw-   0 root         (0) root         (0)     3921 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClClassicCopyJob.hh
--rw-rw-rw-   0 root         (0) root         (0)     9839 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClConstants.hh
--rw-rw-rw-   0 root         (0) root         (0)    33054 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClCopy.cc
--rw-rw-rw-   0 root         (0) root         (0)     4256 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClCopyJob.hh
--rw-rw-rw-   0 root         (0) root         (0)    21403 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClCopyProcess.cc
--rw-rw-rw-   0 root         (0) root         (0)     9463 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClCopyProcess.hh
--rw-rw-rw-   0 root         (0) root         (0)     4723 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClCtx.hh
--rw-rw-rw-   0 root         (0) root         (0)    34739 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClDefaultEnv.cc
--rw-rw-rw-   0 root         (0) root         (0)     8248 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClDefaultEnv.hh
--rw-rw-rw-   0 root         (0) root         (0)     2452 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClDlgEnv.hh
--rw-rw-rw-   0 root         (0) root         (0)     7058 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClEcHandler.cc
--rw-rw-rw-   0 root         (0) root         (0)    17872 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClEcHandler.hh
--rw-rw-rw-   0 root         (0) root         (0)     8264 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClEnv.cc
--rw-rw-rw-   0 root         (0) root         (0)     7930 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClEnv.hh
--rw-rw-rw-   0 root         (0) root         (0)    75852 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClFS.cc
--rw-rw-rw-   0 root         (0) root         (0)     3598 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClFSExecutor.cc
--rw-rw-rw-   0 root         (0) root         (0)     4052 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClFSExecutor.hh
--rw-rw-rw-   0 root         (0) root         (0)    35374 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClFile.cc
--rw-rw-rw-   0 root         (0) root         (0)    43555 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClFile.hh
--rw-rw-rw-   0 root         (0) root         (0)    61991 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClFileOperations.hh
--rw-rw-rw-   0 root         (0) root         (0)   134550 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClFileStateHandler.cc
--rw-rw-rw-   0 root         (0) root         (0)    49325 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClFileStateHandler.hh
--rw-rw-rw-   0 root         (0) root         (0)    81086 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClFileSystem.cc
--rw-rw-rw-   0 root         (0) root         (0)    44722 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClFileSystem.hh
--rw-rw-rw-   0 root         (0) root         (0)    58105 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClFileSystemOperations.hh
--rw-rw-rw-   0 root         (0) root         (0)     7347 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClFileSystemUtils.cc
--rw-rw-rw-   0 root         (0) root         (0)     3917 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClFileSystemUtils.hh
--rw-rw-rw-   0 root         (0) root         (0)     1775 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClFileTimer.cc
--rw-rw-rw-   0 root         (0) root         (0)     3561 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClFileTimer.hh
--rw-rw-rw-   0 root         (0) root         (0)     2754 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClFinalOperation.hh
--rw-rw-rw-   0 root         (0) root         (0)     4753 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClForkHandler.cc
--rw-rw-rw-   0 root         (0) root         (0)     4421 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClForkHandler.hh
--rw-rw-rw-   0 root         (0) root         (0)     9899 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClFwd.hh
--rw-rw-rw-   0 root         (0) root         (0)     6373 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClInQueue.cc
--rw-rw-rw-   0 root         (0) root         (0)     4732 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClInQueue.hh
--rw-rw-rw-   0 root         (0) root         (0)     5126 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClJobManager.cc
--rw-rw-rw-   0 root         (0) root         (0)     4860 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClJobManager.hh
--rw-rw-rw-   0 root         (0) root         (0)    36455 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClLocalFileHandler.cc
--rw-rw-rw-   0 root         (0) root         (0)    17612 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClLocalFileHandler.hh
--rw-rw-rw-   0 root         (0) root         (0)     1604 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClLocalFileTask.cc
--rw-rw-rw-   0 root         (0) root         (0)     1608 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClLocalFileTask.hh
--rw-rw-rw-   0 root         (0) root         (0)     9775 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClLog.cc
--rw-rw-rw-   0 root         (0) root         (0)    10484 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClLog.hh
--rw-rw-rw-   0 root         (0) root         (0)     5392 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClMessage.hh
--rw-rw-rw-   0 root         (0) root         (0)    20035 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClMessageUtils.cc
--rw-rw-rw-   0 root         (0) root         (0)    12633 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClMessageUtils.hh
--rw-rw-rw-   0 root         (0) root         (0)    18515 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClMetalinkRedirector.cc
--rw-rw-rw-   0 root         (0) root         (0)     8397 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClMetalinkRedirector.hh
--rw-rw-rw-   0 root         (0) root         (0)    10519 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClMonitor.hh
--rw-rw-rw-   0 root         (0) root         (0)    29362 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClOperationHandlers.hh
--rw-rw-rw-   0 root         (0) root         (0)     1066 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClOperationTimeout.hh
--rw-rw-rw-   0 root         (0) root         (0)     8987 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClOperations.cc
--rw-rw-rw-   0 root         (0) root         (0)    30811 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClOperations.hh
--rw-rw-rw-   0 root         (0) root         (0)     1295 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClOptimizers.hh
--rw-rw-rw-   0 root         (0) root         (0)     6499 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClOptional.hh
--rw-rw-rw-   0 root         (0) root         (0)     5396 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClOutQueue.cc
--rw-rw-rw-   0 root         (0) root         (0)     6707 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClOutQueue.hh
--rw-rw-rw-   0 root         (0) root         (0)    22041 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClParallelOperation.hh
--rw-rw-rw-   0 root         (0) root         (0)    26771 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClPlugInInterface.hh
--rw-rw-rw-   0 root         (0) root         (0)    18005 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClPlugInManager.cc
--rw-rw-rw-   0 root         (0) root         (0)     7482 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClPlugInManager.hh
--rw-rw-rw-   0 root         (0) root         (0)     7217 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClPoller.hh
--rw-rw-rw-   0 root         (0) root         (0)    20602 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClPollerBuiltIn.cc
--rw-rw-rw-   0 root         (0) root         (0)     7251 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClPollerBuiltIn.hh
--rw-rw-rw-   0 root         (0) root         (0)     3701 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClPollerFactory.cc
--rw-rw-rw-   0 root         (0) root         (0)     2014 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClPollerFactory.hh
--rw-rw-rw-   0 root         (0) root         (0)    17515 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClPostMaster.cc
--rw-rw-rw-   0 root         (0) root         (0)     9638 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClPostMaster.hh
--rw-rw-rw-   0 root         (0) root         (0)    23531 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClPostMasterInterfaces.hh
--rw-rw-rw-   0 root         (0) root         (0)    11305 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClPropertyList.hh
--rw-rw-rw-   0 root         (0) root         (0)     4552 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClRedirectorRegistry.cc
--rw-rw-rw-   0 root         (0) root         (0)     8258 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClRedirectorRegistry.hh
--rw-rw-rw-   0 root         (0) root         (0)     4186 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClRequestSync.hh
--rw-rw-rw-   0 root         (0) root         (0)     2659 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClResponseJob.hh
--rw-rw-rw-   0 root         (0) root         (0)     7016 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClSIDManager.cc
--rw-rw-rw-   0 root         (0) root         (0)     8209 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClSIDManager.hh
--rw-rw-rw-   0 root         (0) root         (0)    30690 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClSocket.cc
--rw-rw-rw-   0 root         (0) root         (0)    15672 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClSocket.hh
--rw-rw-rw-   0 root         (0) root         (0)     5694 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClStatus.cc
--rw-rw-rw-   0 root         (0) root         (0)     7140 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClStatus.hh
--rw-rw-rw-   0 root         (0) root         (0)    47913 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClStream.cc
--rw-rw-rw-   0 root         (0) root         (0)    16793 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClStream.hh
--rw-rw-rw-   0 root         (0) root         (0)     3611 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClSyncQueue.hh
--rw-rw-rw-   0 root         (0) root         (0)     3609 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClTPFallBackCopyJob.cc
--rw-rw-rw-   0 root         (0) root         (0)     2541 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClTPFallBackCopyJob.hh
--rw-rw-rw-   0 root         (0) root         (0)     8986 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClTaskManager.cc
--rw-rw-rw-   0 root         (0) root         (0)     6199 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClTaskManager.hh
--rw-rw-rw-   0 root         (0) root         (0)    34437 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClThirdPartyCopyJob.cc
--rw-rw-rw-   0 root         (0) root         (0)     3740 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClThirdPartyCopyJob.hh
--rw-rw-rw-   0 root         (0) root         (0)    15805 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClTls.cc
--rw-rw-rw-   0 root         (0) root         (0)     6552 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClTls.hh
--rw-rw-rw-   0 root         (0) root         (0)     3056 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClTransportManager.cc
--rw-rw-rw-   0 root         (0) root         (0)     2786 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClTransportManager.hh
--rw-rw-rw-   0 root         (0) root         (0)    17135 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClURL.cc
--rw-rw-rw-   0 root         (0) root         (0)    11760 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClURL.hh
--rw-rw-rw-   0 root         (0) root         (0)    31534 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClUtils.cc
--rw-rw-rw-   0 root         (0) root         (0)    17285 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClUtils.hh
--rw-rw-rw-   0 root         (0) root         (0)     5297 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClXCpCtx.cc
--rw-rw-rw-   0 root         (0) root         (0)     8289 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClXCpCtx.hh
--rw-rw-rw-   0 root         (0) root         (0)    17327 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClXCpSrc.cc
--rw-rw-rw-   0 root         (0) root         (0)     9459 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClXCpSrc.hh
--rw-rw-rw-   0 root         (0) root         (0)    95732 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClXRootDMsgHandler.cc
--rw-rw-rw-   0 root         (0) root         (0)    29197 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClXRootDMsgHandler.hh
--rw-rw-rw-   0 root         (0) root         (0)    26744 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClXRootDResponses.cc
--rw-rw-rw-   0 root         (0) root         (0)    45771 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClXRootDResponses.hh
--rw-rw-rw-   0 root         (0) root         (0)   128533 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClXRootDTransport.cc
--rw-rw-rw-   0 root         (0) root         (0)    21967 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClXRootDTransport.hh
--rw-rw-rw-   0 root         (0) root         (0)    42877 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClZipArchive.cc
--rw-rw-rw-   0 root         (0) root         (0)    28344 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClZipArchive.hh
--rw-rw-rw-   0 root         (0) root         (0)     8602 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClZipCache.hh
--rw-rw-rw-   0 root         (0) root         (0)     4065 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClZipListHandler.cc
--rw-rw-rw-   0 root         (0) root         (0)     5224 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClZipListHandler.hh
--rw-rw-rw-   0 root         (0) root         (0)    27700 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCl/XrdClZipOperations.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdClHttp/
--rw-rw-rw-   0 root         (0) root         (0)      463 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdClHttp/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)    13948 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdClHttp/XrdClHttpFilePlugIn.cc
--rw-rw-rw-   0 root         (0) root         (0)     5602 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdClHttp/XrdClHttpFilePlugIn.hh
--rw-rw-rw-   0 root         (0) root         (0)     7554 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdClHttp/XrdClHttpFileSystemPlugIn.cc
--rw-rw-rw-   0 root         (0) root         (0)     1885 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdClHttp/XrdClHttpFileSystemPlugIn.hh
--rw-rw-rw-   0 root         (0) root         (0)      692 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdClHttp/XrdClHttpPlugInFactory.cc
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdClHttp/XrdClHttpPlugInFactory.hh
--rw-rw-rw-   0 root         (0) root         (0)      422 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdClHttp/XrdClHttpPlugInUtil.cc
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdClHttp/XrdClHttpPlugInUtil.hh
--rw-rw-rw-   0 root         (0) root         (0)    16027 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdClHttp/XrdClHttpPosix.cc
--rw-rw-rw-   0 root         (0) root         (0)     2617 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdClHttp/XrdClHttpPosix.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdCms/
--rw-rw-rw-   0 root         (0) root         (0)    29034 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsAdmin.cc
--rw-rw-rw-   0 root         (0) root         (0)     3908 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsAdmin.hh
--rw-rw-rw-   0 root         (0) root         (0)    15730 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsBaseFS.cc
--rw-rw-rw-   0 root         (0) root         (0)     8998 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsBaseFS.hh
--rw-rw-rw-   0 root         (0) root         (0)    19325 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsBlackList.cc
--rw-rw-rw-   0 root         (0) root         (0)     5380 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsBlackList.hh
--rw-rw-rw-   0 root         (0) root         (0)    21145 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsCache.cc
--rw-rw-rw-   0 root         (0) root         (0)     5021 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsCache.hh
--rw-rw-rw-   0 root         (0) root         (0)     3239 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsClient.cc
--rw-rw-rw-   0 root         (0) root         (0)    22441 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsClient.hh
--rw-rw-rw-   0 root         (0) root         (0)    25549 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsClientConfig.cc
--rw-rw-rw-   0 root         (0) root         (0)     5371 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsClientConfig.hh
--rw-rw-rw-   0 root         (0) root         (0)    17324 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsClientMan.cc
--rw-rw-rw-   0 root         (0) root         (0)     5101 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsClientMan.hh
--rw-rw-rw-   0 root         (0) root         (0)     7117 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsClientMsg.cc
--rw-rw-rw-   0 root         (0) root         (0)     3740 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsClientMsg.hh
--rw-rw-rw-   0 root         (0) root         (0)     8243 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsClustID.cc
--rw-rw-rw-   0 root         (0) root         (0)     3382 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsClustID.hh
--rw-rw-rw-   0 root         (0) root         (0)    77195 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsCluster.cc
--rw-rw-rw-   0 root         (0) root         (0)    10458 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsCluster.hh
--rw-rw-rw-   0 root         (0) root         (0)   109417 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsConfig.cc
--rw-rw-rw-   0 root         (0) root         (0)    12336 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsConfig.hh
--rw-rw-rw-   0 root         (0) root         (0)    49369 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsFinder.cc
--rw-rw-rw-   0 root         (0) root         (0)     6835 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsFinder.hh
--rw-rw-rw-   0 root         (0) root         (0)     5106 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsJob.cc
--rw-rw-rw-   0 root         (0) root         (0)     3058 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsJob.hh
--rw-rw-rw-   0 root         (0) root         (0)     8643 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsKey.cc
--rw-rw-rw-   0 root         (0) root         (0)     6829 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsKey.hh
--rw-rw-rw-   0 root         (0) root         (0)    10887 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsLogin.cc
--rw-rw-rw-   0 root         (0) root         (0)     3223 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsLogin.hh
--rw-rw-rw-   0 root         (0) root         (0)     8263 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsManList.cc
--rw-rw-rw-   0 root         (0) root         (0)     3563 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsManList.hh
--rw-rw-rw-   0 root         (0) root         (0)     9115 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsManTree.cc
--rw-rw-rw-   0 root         (0) root         (0)     3708 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsManTree.hh
--rw-rw-rw-   0 root         (0) root         (0)    20171 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsManager.cc
--rw-rw-rw-   0 root         (0) root         (0)     4549 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsManager.hh
--rw-rw-rw-   0 root         (0) root         (0)    21971 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsMeter.cc
--rw-rw-rw-   0 root         (0) root         (0)     4787 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsMeter.hh
--rw-rw-rw-   0 root         (0) root         (0)     6578 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsNash.cc
--rw-rw-rw-   0 root         (0) root         (0)     3101 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsNash.hh
--rw-rw-rw-   0 root         (0) root         (0)    68022 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsNode.cc
--rw-rw-rw-   0 root         (0) root         (0)    11829 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsNode.hh
--rw-rw-rw-   0 root         (0) root         (0)     7875 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsPList.cc
--rw-rw-rw-   0 root         (0) root         (0)     5436 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsPList.hh
--rw-rw-rw-   0 root         (0) root         (0)    18983 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsParser.cc
--rw-rw-rw-   0 root         (0) root         (0)     4888 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsParser.hh
--rw-rw-rw-   0 root         (0) root         (0)     7886 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsPerfMon.hh
--rw-rw-rw-   0 root         (0) root         (0)     6042 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsPrepArgs.cc
--rw-rw-rw-   0 root         (0) root         (0)     3669 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsPrepArgs.hh
--rw-rw-rw-   0 root         (0) root         (0)    18512 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsPrepare.cc
--rw-rw-rw-   0 root         (0) root         (0)     4068 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsPrepare.hh
--rw-rw-rw-   0 root         (0) root         (0)    46734 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsProtocol.cc
--rw-rw-rw-   0 root         (0) root         (0)     5039 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsProtocol.hh
--rw-rw-rw-   0 root         (0) root         (0)     3945 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsRRData.cc
--rw-rw-rw-   0 root         (0) root         (0)     4633 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsRRData.hh
--rw-rw-rw-   0 root         (0) root         (0)    17719 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsRRQ.cc
--rw-rw-rw-   0 root         (0) root         (0)     7590 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsRRQ.hh
--rw-rw-rw-   0 root         (0) root         (0)     5228 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsRTable.cc
--rw-rw-rw-   0 root         (0) root         (0)     3076 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsRTable.hh
--rw-rw-rw-   0 root         (0) root         (0)     9888 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsRedirLocal.cc
--rw-rw-rw-   0 root         (0) root         (0)     3519 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsRedirLocal.hh
--rw-rw-rw-   0 root         (0) root         (0)    11036 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsResp.cc
--rw-rw-rw-   0 root         (0) root         (0)     5382 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsResp.hh
--rw-rw-rw-   0 root         (0) root         (0)     5917 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsRole.hh
--rw-rw-rw-   0 root         (0) root         (0)    11602 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsRouting.cc
--rw-rw-rw-   0 root         (0) root         (0)     4838 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsRouting.hh
--rw-rw-rw-   0 root         (0) root         (0)    14804 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsSecurity.cc
--rw-rw-rw-   0 root         (0) root         (0)     3468 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsSecurity.hh
--rw-rw-rw-   0 root         (0) root         (0)     7463 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsSelect.hh
--rw-rw-rw-   0 root         (0) root         (0)    11542 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsState.cc
--rw-rw-rw-   0 root         (0) root         (0)     3997 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsState.hh
--rw-rw-rw-   0 root         (0) root         (0)     5187 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsSupervisor.cc
--rw-rw-rw-   0 root         (0) root         (0)     2750 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsSupervisor.hh
--rw-rw-rw-   0 root         (0) root         (0)     5637 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsTalk.cc
--rw-rw-rw-   0 root         (0) root         (0)     3034 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsTalk.hh
--rw-rw-rw-   0 root         (0) root         (0)     3426 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsTrace.hh
--rw-rw-rw-   0 root         (0) root         (0)     2782 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsTypes.hh
--rw-rw-rw-   0 root         (0) root         (0)    11723 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsUtils.cc
--rw-rw-rw-   0 root         (0) root         (0)     6365 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsUtils.hh
--rw-rw-rw-   0 root         (0) root         (0)     5656 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCms/XrdCmsVnId.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdCrypto/
--rw-rw-rw-   0 root         (0) root         (0)     4302 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoAux.cc
--rw-rw-rw-   0 root         (0) root         (0)     5048 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoAux.hh
--rw-rw-rw-   0 root         (0) root         (0)     7678 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoBasic.cc
--rw-rw-rw-   0 root         (0) root         (0)     3869 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoBasic.hh
--rw-rw-rw-   0 root         (0) root         (0)     7405 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoCipher.cc
--rw-rw-rw-   0 root         (0) root         (0)     4214 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoCipher.hh
--rw-rw-rw-   0 root         (0) root         (0)    17653 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoFactory.cc
--rw-rw-rw-   0 root         (0) root         (0)     9138 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoFactory.hh
--rw-rw-rw-   0 root         (0) root         (0)     3500 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoLite.cc
--rw-rw-rw-   0 root         (0) root         (0)     5355 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoLite.hh
--rw-rw-rw-   0 root         (0) root         (0)     8734 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoLite_bf32.cc
--rw-rw-rw-   0 root         (0) root         (0)     4136 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoMsgDigest.cc
--rw-rw-rw-   0 root         (0) root         (0)     3452 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoMsgDigest.hh
--rw-rw-rw-   0 root         (0) root         (0)     9058 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoRSA.cc
--rw-rw-rw-   0 root         (0) root         (0)     4804 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoRSA.hh
--rw-rw-rw-   0 root         (0) root         (0)     2989 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoTrace.hh
--rw-rw-rw-   0 root         (0) root         (0)    10639 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoX509.cc
--rw-rw-rw-   0 root         (0) root         (0)     5644 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoX509.hh
--rw-rw-rw-   0 root         (0) root         (0)    27263 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoX509Chain.cc
--rw-rw-rw-   0 root         (0) root         (0)     7661 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoX509Chain.hh
--rw-rw-rw-   0 root         (0) root         (0)     5674 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoX509Crl.cc
--rw-rw-rw-   0 root         (0) root         (0)     4052 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoX509Crl.hh
--rw-rw-rw-   0 root         (0) root         (0)     5256 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoX509Req.cc
--rw-rw-rw-   0 root         (0) root         (0)     4177 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptoX509Req.hh
--rw-rw-rw-   0 root         (0) root         (0)    10162 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptogsiX509Chain.cc
--rw-rw-rw-   0 root         (0) root         (0)     3952 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptogsiX509Chain.hh
--rw-rw-rw-   0 root         (0) root         (0)    25131 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptosslAux.cc
--rw-rw-rw-   0 root         (0) root         (0)     7231 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptosslAux.hh
--rw-rw-rw-   0 root         (0) root         (0)    41488 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptosslCipher.cc
--rw-rw-rw-   0 root         (0) root         (0)     4573 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptosslCipher.hh
--rw-rw-rw-   0 root         (0) root         (0)    16817 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptosslFactory.cc
--rw-rw-rw-   0 root         (0) root         (0)     5208 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptosslFactory.hh
--rw-rw-rw-   0 root         (0) root         (0)     6084 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptosslMsgDigest.cc
--rw-rw-rw-   0 root         (0) root         (0)     3376 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptosslMsgDigest.hh
--rw-rw-rw-   0 root         (0) root         (0)    20903 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptosslRSA.cc
--rw-rw-rw-   0 root         (0) root         (0)     4241 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptosslRSA.hh
--rw-rw-rw-   0 root         (0) root         (0)     2896 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptosslTrace.hh
--rw-rw-rw-   0 root         (0) root         (0)    36214 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptosslX509.cc
--rw-rw-rw-   0 root         (0) root         (0)     5787 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptosslX509.hh
--rw-rw-rw-   0 root         (0) root         (0)    20566 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptosslX509Crl.cc
--rw-rw-rw-   0 root         (0) root         (0)     5006 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptosslX509Crl.hh
--rw-rw-rw-   0 root         (0) root         (0)    12043 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptosslX509Req.cc
--rw-rw-rw-   0 root         (0) root         (0)     4113 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptosslX509Req.hh
--rw-rw-rw-   0 root         (0) root         (0)    49317 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptosslgsiAux.cc
--rw-rw-rw-   0 root         (0) root         (0)     5668 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptosslgsiAux.hh
--rw-rw-rw-   0 root         (0) root         (0)    18858 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto/XrdCryptotest.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdDig/
--rw-rw-rw-   0 root         (0) root         (0)    14689 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdDig/XrdDigAuth.cc
--rw-rw-rw-   0 root         (0) root         (0)     4337 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdDig/XrdDigAuth.hh
--rw-rw-rw-   0 root         (0) root         (0)    21474 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdDig/XrdDigConfig.cc
--rw-rw-rw-   0 root         (0) root         (0)     3831 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdDig/XrdDigConfig.hh
--rw-rw-rw-   0 root         (0) root         (0)    28757 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdDig/XrdDigFS.cc
--rw-rw-rw-   0 root         (0) root         (0)    11645 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdDig/XrdDigFS.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdEc/
--rw-rw-rw-   0 root         (0) root         (0)     1708 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdEc/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)     2020 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdEc/README
--rw-rw-rw-   0 root         (0) root         (0)     3708 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdEc/XrdEcConfig.hh
--rw-rw-rw-   0 root         (0) root         (0)     3424 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdEc/XrdEcObjCfg.hh
--rw-rw-rw-   0 root         (0) root         (0)    47577 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdEc/XrdEcReader.cc
--rw-rw-rw-   0 root         (0) root         (0)     8804 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdEc/XrdEcReader.hh
--rw-rw-rw-   0 root         (0) root         (0)     9785 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdEc/XrdEcRedundancyProvider.cc
--rw-rw-rw-   0 root         (0) root         (0)     5127 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdEc/XrdEcRedundancyProvider.hh
--rw-rw-rw-   0 root         (0) root         (0)    17345 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdEc/XrdEcStrmWriter.cc
--rw-rw-rw-   0 root         (0) root         (0)    13309 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdEc/XrdEcStrmWriter.hh
--rw-rw-rw-   0 root         (0) root         (0)     7256 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdEc/XrdEcThreadPool.hh
--rw-rw-rw-   0 root         (0) root         (0)     3689 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdEc/XrdEcUtilities.cc
--rw-rw-rw-   0 root         (0) root         (0)     9976 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdEc/XrdEcUtilities.hh
--rw-rw-rw-   0 root         (0) root         (0)    12505 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdEc/XrdEcWrtBuff.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdFfs/
--rw-rw-rw-   0 root         (0) root         (0)     6405 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFfs/README
--rw-rw-rw-   0 root         (0) root         (0)    10875 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFfs/XrdFfsDent.cc
--rw-rw-rw-   0 root         (0) root         (0)     2975 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFfs/XrdFfsDent.hh
--rw-rw-rw-   0 root         (0) root         (0)     5321 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFfs/XrdFfsFsinfo.cc
--rw-rw-rw-   0 root         (0) root         (0)     2539 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFfs/XrdFfsFsinfo.hh
--rw-rw-rw-   0 root         (0) root         (0)    13902 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFfs/XrdFfsMisc.cc
--rw-rw-rw-   0 root         (0) root         (0)     3054 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFfs/XrdFfsMisc.hh
--rw-rw-rw-   0 root         (0) root         (0)    26410 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFfs/XrdFfsPosix.cc
--rw-rw-rw-   0 root         (0) root         (0)     4855 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFfs/XrdFfsPosix.hh
--rw-rw-rw-   0 root         (0) root         (0)    10077 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFfs/XrdFfsQueue.cc
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFfs/XrdFfsQueue.hh
--rw-rw-rw-   0 root         (0) root         (0)    11980 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFfs/XrdFfsWcache.cc
--rw-rw-rw-   0 root         (0) root         (0)     2664 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFfs/XrdFfsWcache.hh
--rw-rw-rw-   0 root         (0) root         (0)    48045 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFfs/XrdFfsXrootdfs.cc
--rwxrwxrwx   0 root         (0) root         (0)     1608 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFfs/xrootdfs.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdFrc/
--rw-rw-rw-   0 root         (0) root         (0)    11084 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrc/XrdFrcCID.cc
--rw-rw-rw-   0 root         (0) root         (0)     3950 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrc/XrdFrcCID.hh
--rw-rw-rw-   0 root         (0) root         (0)    11618 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrc/XrdFrcProxy.cc
--rw-rw-rw-   0 root         (0) root         (0)     3742 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrc/XrdFrcProxy.hh
--rw-rw-rw-   0 root         (0) root         (0)     8742 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrc/XrdFrcReqAgent.cc
--rw-rw-rw-   0 root         (0) root         (0)     3073 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrc/XrdFrcReqAgent.hh
--rw-rw-rw-   0 root         (0) root         (0)    21187 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrc/XrdFrcReqFile.cc
--rw-rw-rw-   0 root         (0) root         (0)     4017 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrc/XrdFrcReqFile.hh
--rw-rw-rw-   0 root         (0) root         (0)     4547 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrc/XrdFrcRequest.hh
--rw-rw-rw-   0 root         (0) root         (0)     2728 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrc/XrdFrcTrace.cc
--rw-rw-rw-   0 root         (0) root         (0)     3396 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrc/XrdFrcTrace.hh
--rw-rw-rw-   0 root         (0) root         (0)    11378 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrc/XrdFrcUtils.cc
--rw-rw-rw-   0 root         (0) root         (0)     3289 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrc/XrdFrcUtils.hh
--rw-rw-rw-   0 root         (0) root         (0)     8162 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrc/XrdFrcXAttr.hh
--rw-rw-rw-   0 root         (0) root         (0)     2863 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrc/XrdFrcXLock.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdFrm/
--rw-rw-rw-   0 root         (0) root         (0)    36149 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmAdmin.cc
--rw-rw-rw-   0 root         (0) root         (0)     7410 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmAdmin.hh
--rw-rw-rw-   0 root         (0) root         (0)    24369 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmAdminAudit.cc
--rw-rw-rw-   0 root         (0) root         (0)    13623 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmAdminFiles.cc
--rw-rw-rw-   0 root         (0) root         (0)    11144 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmAdminFind.cc
--rw-rw-rw-   0 root         (0) root         (0)     6815 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmAdminMain.cc
--rw-rw-rw-   0 root         (0) root         (0)    10240 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmAdminQuery.cc
--rw-rw-rw-   0 root         (0) root         (0)     9903 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmAdminReloc.cc
--rw-rw-rw-   0 root         (0) root         (0)     9421 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmAdminUnlink.cc
--rw-rw-rw-   0 root         (0) root         (0)    10117 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmCns.cc
--rw-rw-rw-   0 root         (0) root         (0)     3675 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmCns.hh
--rw-rw-rw-   0 root         (0) root         (0)    71607 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmConfig.cc
--rw-rw-rw-   0 root         (0) root         (0)     8419 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmConfig.hh
--rw-rw-rw-   0 root         (0) root         (0)    17426 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmFiles.cc
--rw-rw-rw-   0 root         (0) root         (0)     6386 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmFiles.hh
--rw-rw-rw-   0 root         (0) root         (0)    11087 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmMigrate.cc
--rw-rw-rw-   0 root         (0) root         (0)     3078 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmMigrate.hh
--rw-rw-rw-   0 root         (0) root         (0)    11518 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmMonitor.cc
--rw-rw-rw-   0 root         (0) root         (0)     3912 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmMonitor.hh
--rw-rw-rw-   0 root         (0) root         (0)     9482 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmPurgMain.cc
--rw-rw-rw-   0 root         (0) root         (0)    32604 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmPurge.cc
--rw-rw-rw-   0 root         (0) root         (0)     5353 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmPurge.hh
--rw-rw-rw-   0 root         (0) root         (0)     7763 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmReqBoss.cc
--rw-rw-rw-   0 root         (0) root         (0)     3059 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmReqBoss.hh
--rw-rw-rw-   0 root         (0) root         (0)     7011 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmTSort.cc
--rw-rw-rw-   0 root         (0) root         (0)     3315 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmTSort.hh
--rw-rw-rw-   0 root         (0) root         (0)    30228 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmTransfer.cc
--rw-rw-rw-   0 root         (0) root         (0)     3349 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmTransfer.hh
--rw-rw-rw-   0 root         (0) root         (0)    10404 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmXfrAgent.cc
--rw-rw-rw-   0 root         (0) root         (0)     3098 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmXfrAgent.hh
--rw-rw-rw-   0 root         (0) root         (0)     7971 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmXfrDaemon.cc
--rw-rw-rw-   0 root         (0) root         (0)     2782 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmXfrDaemon.hh
--rw-rw-rw-   0 root         (0) root         (0)     2832 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmXfrJob.hh
--rw-rw-rw-   0 root         (0) root         (0)     6343 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmXfrMain.cc
--rw-rw-rw-   0 root         (0) root         (0)    17722 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmXfrQueue.cc
--rw-rw-rw-   0 root         (0) root         (0)     4118 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm/XrdFrmXfrQueue.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdHttp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdHttp/static/
--rw-rw-rw-   0 root         (0) root         (0)     1400 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/static/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     1274 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/static/xrdhttp.css
--rw-rw-rw-   0 root         (0) root         (0)     7951 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/static/xrdhttp_css.h
--rw-rw-rw-   0 root         (0) root         (0)     8705 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/static/xrdhttp_favicon_ico.h
--rw-rw-rw-   0 root         (0) root         (0)     1909 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/XrdHttpChecksum.cc
--rw-rw-rw-   0 root         (0) root         (0)     2097 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/XrdHttpChecksum.hh
--rw-rw-rw-   0 root         (0) root         (0)     5702 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/XrdHttpChecksumHandler.cc
--rw-rw-rw-   0 root         (0) root         (0)     5188 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/XrdHttpChecksumHandler.hh
--rw-rw-rw-   0 root         (0) root         (0)     3718 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/XrdHttpExtHandler.cc
--rw-rw-rw-   0 root         (0) root         (0)     6073 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/XrdHttpExtHandler.hh
--rw-rw-rw-   0 root         (0) root         (0)     2306 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/XrdHttpModule.cc
--rw-rw-rw-   0 root         (0) root         (0)    86119 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/XrdHttpProtocol.cc
--rw-rw-rw-   0 root         (0) root         (0)    13770 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/XrdHttpProtocol.hh
--rw-rw-rw-   0 root         (0) root         (0)    84937 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/XrdHttpReq.cc
--rw-rw-rw-   0 root         (0) root         (0)    14229 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/XrdHttpReq.hh
--rw-rw-rw-   0 root         (0) root         (0)     4252 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/XrdHttpSecXtractor.hh
--rw-rw-rw-   0 root         (0) root         (0)     8841 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/XrdHttpSecurity.cc
--rw-rw-rw-   0 root         (0) root         (0)     1661 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/XrdHttpStatic.hh
--rw-rw-rw-   0 root         (0) root         (0)     2175 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/XrdHttpTrace.hh
--rw-rw-rw-   0 root         (0) root         (0)     9413 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/XrdHttpUtils.cc
--rw-rw-rw-   0 root         (0) root         (0)     2321 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/XrdHttpUtils.hh
--rw-rw-rw-   0 root         (0) root         (0)     2784 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/xrootd-http-rdr.cf
--rw-rw-rw-   0 root         (0) root         (0)      941 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp/xrootd-http.cf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdMacaroons/
--rw-rw-rw-   0 root         (0) root         (0)     2798 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdMacaroons/README.md
--rw-rw-rw-   0 root         (0) root         (0)     4922 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdMacaroons/XrdMacaroons.cc
--rw-rw-rw-   0 root         (0) root         (0)    18196 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdMacaroons/XrdMacaroonsAuthz.cc
--rw-rw-rw-   0 root         (0) root         (0)     1780 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdMacaroons/XrdMacaroonsAuthz.hh
--rw-rw-rw-   0 root         (0) root         (0)     6883 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdMacaroons/XrdMacaroonsConfigure.cc
--rw-rw-rw-   0 root         (0) root         (0)    21521 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdMacaroons/XrdMacaroonsHandler.cc
--rw-rw-rw-   0 root         (0) root         (0)     2784 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdMacaroons/XrdMacaroonsHandler.hh
--rw-rw-rw-   0 root         (0) root         (0)      122 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdMacaroons/export-lib-symbols
--rwxrwxrwx   0 root         (0) root         (0)     5269 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdMacaroons/macaroon-init
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdNet/
--rw-rw-rw-   0 root         (0) root         (0)    17923 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNet.cc
--rw-rw-rw-   0 root         (0) root         (0)    14669 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNet.hh
--rw-rw-rw-   0 root         (0) root         (0)    21048 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetAddr.cc
--rw-rw-rw-   0 root         (0) root         (0)    15050 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetAddr.hh
--rw-rw-rw-   0 root         (0) root         (0)    17181 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetAddrInfo.cc
--rw-rw-rw-   0 root         (0) root         (0)    17695 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetAddrInfo.hh
--rw-rw-rw-   0 root         (0) root         (0)     5823 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetBuffer.cc
--rw-rw-rw-   0 root         (0) root         (0)     3948 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetBuffer.hh
--rw-rw-rw-   0 root         (0) root         (0)     8210 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetCache.cc
--rw-rw-rw-   0 root         (0) root         (0)     5934 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetCache.hh
--rw-rw-rw-   0 root         (0) root         (0)     5742 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetCmsNotify.cc
--rw-rw-rw-   0 root         (0) root         (0)     2929 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetCmsNotify.hh
--rw-rw-rw-   0 root         (0) root         (0)     4246 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetConnect.cc
--rw-rw-rw-   0 root         (0) root         (0)     3196 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetConnect.hh
--rw-rw-rw-   0 root         (0) root         (0)    31959 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetIF.cc
--rw-rw-rw-   0 root         (0) root         (0)    20067 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetIF.hh
--rw-rw-rw-   0 root         (0) root         (0)     6326 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetIdentity.cc
--rw-rw-rw-   0 root         (0) root         (0)     2701 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetIdentity.hh
--rw-rw-rw-   0 root         (0) root         (0)     7246 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetMsg.cc
--rw-rw-rw-   0 root         (0) root         (0)     7458 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetMsg.hh
--rw-rw-rw-   0 root         (0) root         (0)     4955 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetOpts.hh
--rw-rw-rw-   0 root         (0) root         (0)     3294 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetPMark.cc
--rw-rw-rw-   0 root         (0) root         (0)     3824 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetPMark.hh
--rw-rw-rw-   0 root         (0) root         (0)    39260 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetPMarkCfg.cc
--rw-rw-rw-   0 root         (0) root         (0)     3755 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetPMarkCfg.hh
--rw-rw-rw-   0 root         (0) root         (0)    13957 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetPMarkFF.cc
--rw-rw-rw-   0 root         (0) root         (0)     3475 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetPMarkFF.hh
--rw-rw-rw-   0 root         (0) root         (0)     2952 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetPeer.hh
--rw-rw-rw-   0 root         (0) root         (0)     9640 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetRegistry.cc
--rw-rw-rw-   0 root         (0) root         (0)     6279 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetRegistry.hh
--rw-rw-rw-   0 root         (0) root         (0)     9552 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetSecurity.cc
--rw-rw-rw-   0 root         (0) root         (0)     3339 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetSecurity.hh
--rw-rw-rw-   0 root         (0) root         (0)     3106 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetSockAddr.hh
--rw-rw-rw-   0 root         (0) root         (0)    18472 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetSocket.cc
--rw-rw-rw-   0 root         (0) root         (0)     7647 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetSocket.hh
--rw-rw-rw-   0 root         (0) root         (0)    31024 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetUtils.cc
--rw-rw-rw-   0 root         (0) root         (0)    24210 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdNet/XrdNetUtils.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdOfs/
--rw-rw-rw-   0 root         (0) root         (0)    98478 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfs.cc
--rw-rw-rw-   0 root         (0) root         (0)    21329 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfs.hh
--rw-rw-rw-   0 root         (0) root         (0)    19274 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsCPFile.cc
--rw-rw-rw-   0 root         (0) root         (0)     8379 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsCPFile.hh
--rw-rw-rw-   0 root         (0) root         (0)    11781 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsChkPnt.cc
--rw-rw-rw-   0 root         (0) root         (0)     6193 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsChkPnt.hh
--rw-rw-rw-   0 root         (0) root         (0)    71659 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsConfig.cc
--rw-rw-rw-   0 root         (0) root         (0)    10806 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsConfigCP.cc
--rw-rw-rw-   0 root         (0) root         (0)     3117 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsConfigCP.hh
--rw-rw-rw-   0 root         (0) root         (0)    33128 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsConfigPI.cc
--rw-rw-rw-   0 root         (0) root         (0)    14532 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsConfigPI.hh
--rw-rw-rw-   0 root         (0) root         (0)    12955 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsEvr.cc
--rw-rw-rw-   0 root         (0) root         (0)     4771 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsEvr.hh
--rw-rw-rw-   0 root         (0) root         (0)    19534 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsEvs.cc
--rw-rw-rw-   0 root         (0) root         (0)     7231 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsEvs.hh
--rw-rw-rw-   0 root         (0) root         (0)    16520 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsFAttr.cc
--rw-rw-rw-   0 root         (0) root         (0)     4073 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsFS.cc
--rw-rw-rw-   0 root         (0) root         (0)    12589 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsFSctl.cc
--rw-rw-rw-   0 root         (0) root         (0)     8921 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsFSctl_PI.hh
--rw-rw-rw-   0 root         (0) root         (0)    30836 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsHandle.cc
--rw-rw-rw-   0 root         (0) root         (0)     8197 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsHandle.hh
--rw-rw-rw-   0 root         (0) root         (0)    13105 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsPoscq.cc
--rw-rw-rw-   0 root         (0) root         (0)     4134 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsPoscq.hh
--rw-rw-rw-   0 root         (0) root         (0)    28856 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsPrepGPI.cc
--rw-rw-rw-   0 root         (0) root         (0)    11518 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsPrepare.hh
--rw-rw-rw-   0 root         (0) root         (0)     3061 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsSecurity.hh
--rw-rw-rw-   0 root         (0) root         (0)     3814 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsStats.cc
--rw-rw-rw-   0 root         (0) root         (0)     3285 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsStats.hh
--rw-rw-rw-   0 root         (0) root         (0)    23537 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsTPC.cc
--rw-rw-rw-   0 root         (0) root         (0)     5117 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsTPC.hh
--rw-rw-rw-   0 root         (0) root         (0)    10359 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsTPCAuth.cc
--rw-rw-rw-   0 root         (0) root         (0)     3086 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsTPCAuth.hh
--rw-rw-rw-   0 root         (0) root         (0)     3108 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsTPCConfig.hh
--rw-rw-rw-   0 root         (0) root         (0)     7573 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsTPCInfo.cc
--rw-rw-rw-   0 root         (0) root         (0)     5241 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsTPCInfo.hh
--rw-rw-rw-   0 root         (0) root         (0)     7941 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsTPCJob.cc
--rw-rw-rw-   0 root         (0) root         (0)     3295 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsTPCJob.hh
--rw-rw-rw-   0 root         (0) root         (0)    13429 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsTPCProg.cc
--rw-rw-rw-   0 root         (0) root         (0)     3209 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsTPCProg.hh
--rw-rw-rw-   0 root         (0) root         (0)     4158 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOfs/XrdOfsTrace.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdOss/
--rw-rw-rw-   0 root         (0) root         (0)    11649 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOss.cc
--rw-rw-rw-   0 root         (0) root         (0)    46028 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOss.hh
--rw-rw-rw-   0 root         (0) root         (0)    18122 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssAio.cc
--rw-rw-rw-   0 root         (0) root         (0)    45753 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssApi.cc
--rw-rw-rw-   0 root         (0) root         (0)    17573 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssApi.hh
--rw-rw-rw-   0 root         (0) root         (0)     8491 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssAt.cc
--rw-rw-rw-   0 root         (0) root         (0)     7394 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssAt.hh
--rw-rw-rw-   0 root         (0) root         (0)    31708 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssCache.cc
--rw-rw-rw-   0 root         (0) root         (0)    11024 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssCache.hh
--rw-rw-rw-   0 root         (0) root         (0)    73786 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssConfig.cc
--rw-rw-rw-   0 root         (0) root         (0)     3327 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssConfig.hh
--rw-rw-rw-   0 root         (0) root         (0)     7753 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssCopy.cc
--rw-rw-rw-   0 root         (0) root         (0)     2632 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssCopy.hh
--rw-rw-rw-   0 root         (0) root         (0)    13674 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssCreate.cc
--rw-rw-rw-   0 root         (0) root         (0)     3641 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssDefaultSS.hh
--rw-rw-rw-   0 root         (0) root         (0)     4810 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssError.hh
--rw-rw-rw-   0 root         (0) root         (0)    16583 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssMSS.cc
--rw-rw-rw-   0 root         (0) root         (0)    11917 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssMio.cc
--rw-rw-rw-   0 root         (0) root         (0)     3591 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssMio.hh
--rw-rw-rw-   0 root         (0) root         (0)     2931 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssMioFile.hh
--rw-rw-rw-   0 root         (0) root         (0)     2987 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssOpaque.hh
--rw-rw-rw-   0 root         (0) root         (0)    13731 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssPath.cc
--rw-rw-rw-   0 root         (0) root         (0)     3880 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssPath.hh
--rw-rw-rw-   0 root         (0) root         (0)     8574 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssReloc.cc
--rw-rw-rw-   0 root         (0) root         (0)     9890 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssRename.cc
--rw-rw-rw-   0 root         (0) root         (0)     9051 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssSIgpfsT.cc
--rw-rw-rw-   0 root         (0) root         (0)    19495 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssSpace.cc
--rw-rw-rw-   0 root         (0) root         (0)     4240 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssSpace.hh
--rw-rw-rw-   0 root         (0) root         (0)    18820 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssStage.cc
--rw-rw-rw-   0 root         (0) root         (0)     4090 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssStage.hh
--rw-rw-rw-   0 root         (0) root         (0)    21165 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssStat.cc
--rw-rw-rw-   0 root         (0) root         (0)    10195 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssStatInfo.hh
--rw-rw-rw-   0 root         (0) root         (0)     3186 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssTrace.hh
--rw-rw-rw-   0 root         (0) root         (0)     8528 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssUnlink.cc
--rw-rw-rw-   0 root         (0) root         (0)     6673 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssVS.hh
--rw-rw-rw-   0 root         (0) root         (0)    41503 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOss/XrdOssWrapper.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdOssCsi/
--rw-rw-rw-   0 root         (0) root         (0)     3167 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi/README.md
--rw-rw-rw-   0 root         (0) root         (0)    15159 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi/XrdOssCsi.cc
--rw-rw-rw-   0 root         (0) root         (0)     9618 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi/XrdOssCsi.hh
--rw-rw-rw-   0 root         (0) root         (0)     7059 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiConfig.cc
--rw-rw-rw-   0 root         (0) root         (0)     6756 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiConfig.hh
--rw-rw-rw-   0 root         (0) root         (0)     2527 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiCrcUtils.cc
--rw-rw-rw-   0 root         (0) root         (0)     4781 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiCrcUtils.hh
--rw-rw-rw-   0 root         (0) root         (0)    16745 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiFile.cc
--rw-rw-rw-   0 root         (0) root         (0)     4448 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiFileAio.cc
--rw-rw-rw-   0 root         (0) root         (0)    11301 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiFileAio.hh
--rw-rw-rw-   0 root         (0) root         (0)    29563 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiPages.cc
--rw-rw-rw-   0 root         (0) root         (0)     9019 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiPages.hh
--rw-rw-rw-   0 root         (0) root         (0)    34154 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiPagesUnaligned.cc
--rw-rw-rw-   0 root         (0) root         (0)     3049 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiRanges.cc
--rw-rw-rw-   0 root         (0) root         (0)     6143 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiRanges.hh
--rw-rw-rw-   0 root         (0) root         (0)     3346 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiTagstore.hh
--rw-rw-rw-   0 root         (0) root         (0)     8697 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiTagstoreFile.cc
--rw-rw-rw-   0 root         (0) root         (0)     6957 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiTagstoreFile.hh
--rw-rw-rw-   0 root         (0) root         (0)     3315 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiTrace.hh
--rw-rw-rw-   0 root         (0) root         (0)    10382 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi/XrdOssHandler.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdOuc/
--rw-rw-rw-   0 root         (0) root         (0)     1179 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/README.bonjour
--rw-rw-rw-   0 root         (0) root         (0)     8818 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucArgs.cc
--rw-rw-rw-   0 root         (0) root         (0)     5805 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucArgs.hh
--rw-rw-rw-   0 root         (0) root         (0)    17653 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucBackTrace.cc
--rw-rw-rw-   0 root         (0) root         (0)    10560 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucBackTrace.hh
--rw-rw-rw-   0 root         (0) root         (0)     9481 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucBuffer.cc
--rw-rw-rw-   0 root         (0) root         (0)    12583 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucBuffer.hh
--rw-rw-rw-   0 root         (0) root         (0)    12756 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucCRC.cc
--rw-rw-rw-   0 root         (0) root         (0)     8087 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucCRC.hh
--rw-rw-rw-   0 root         (0) root         (0)    17087 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucCRC32C.cc
--rw-rw-rw-   0 root         (0) root         (0)      735 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucCRC32C.hh
--rw-rw-rw-   0 root         (0) root         (0)     5325 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucCache.cc
--rw-rw-rw-   0 root         (0) root         (0)    37675 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucCache.hh
--rw-rw-rw-   0 root         (0) root         (0)     5220 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucCacheCM.hh
--rw-rw-rw-   0 root         (0) root         (0)     7071 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucCacheStats.hh
--rw-rw-rw-   0 root         (0) root         (0)     4673 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucCallBack.cc
--rw-rw-rw-   0 root         (0) root         (0)     5820 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucCallBack.hh
--rw-rw-rw-   0 root         (0) root         (0)     3807 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucChain.hh
--rw-rw-rw-   0 root         (0) root         (0)     5655 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucChkPnt.hh
--rw-rw-rw-   0 root         (0) root         (0)     1514 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucCompiler.hh
--rw-rw-rw-   0 root         (0) root         (0)     5019 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucDLlist.hh
--rw-rw-rw-   0 root         (0) root         (0)     4334 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucERoute.cc
--rw-rw-rw-   0 root         (0) root         (0)     4301 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucERoute.hh
--rw-rw-rw-   0 root         (0) root         (0)     1693 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucEnum.hh
--rw-rw-rw-   0 root         (0) root         (0)     9097 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucEnv.cc
--rw-rw-rw-   0 root         (0) root         (0)     5341 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucEnv.hh
--rw-rw-rw-   0 root         (0) root         (0)    23619 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucErrInfo.hh
--rw-rw-rw-   0 root         (0) root         (0)    10829 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucExport.cc
--rw-rw-rw-   0 root         (0) root         (0)     5760 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucExport.hh
--rw-rw-rw-   0 root         (0) root         (0)     9215 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucFileInfo.cc
--rw-rw-rw-   0 root         (0) root         (0)     9566 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucFileInfo.hh
--rw-rw-rw-   0 root         (0) root         (0)    11284 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucGMap.cc
--rw-rw-rw-   0 root         (0) root         (0)     8302 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucGMap.hh
--rw-rw-rw-   0 root         (0) root         (0)     8116 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucGatherConf.cc
--rw-rw-rw-   0 root         (0) root         (0)     6689 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucGatherConf.hh
--rw-rw-rw-   0 root         (0) root         (0)     9301 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucHash.hh
--rw-rw-rw-   0 root         (0) root         (0)    11511 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucHash.icc
--rw-rw-rw-   0 root         (0) root         (0)     3214 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucHashVal.cc
--rw-rw-rw-   0 root         (0) root         (0)     3665 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucIOVec.hh
--rw-rw-rw-   0 root         (0) root         (0)   978532 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucJson.hh
--rw-rw-rw-   0 root         (0) root         (0)     2676 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucLock.hh
--rw-rw-rw-   0 root         (0) root         (0)    10867 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucLogging.cc
--rw-rw-rw-   0 root         (0) root         (0)     3153 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucLogging.hh
--rw-rw-rw-   0 root         (0) root         (0)     4695 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucMapP2X.hh
--rw-rw-rw-   0 root         (0) root         (0)    10179 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucMsubs.cc
--rw-rw-rw-   0 root         (0) root         (0)     5592 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucMsubs.hh
--rw-rw-rw-   0 root         (0) root         (0)     4780 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucN2NLoader.cc
--rw-rw-rw-   0 root         (0) root         (0)     3053 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucN2NLoader.hh
--rw-rw-rw-   0 root         (0) root         (0)    10498 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucN2No2p.cc
--rw-rw-rw-   0 root         (0) root         (0)     5458 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucNList.cc
--rw-rw-rw-   0 root         (0) root         (0)     5100 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucNList.hh
--rw-rw-rw-   0 root         (0) root         (0)    14506 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucNSWalk.cc
--rw-rw-rw-   0 root         (0) root         (0)     7383 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucNSWalk.hh
--rw-rw-rw-   0 root         (0) root         (0)     8596 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucName2Name.cc
--rw-rw-rw-   0 root         (0) root         (0)    12097 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucName2Name.hh
--rw-rw-rw-   0 root         (0) root         (0)     6417 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucPList.hh
--rw-rw-rw-   0 root         (0) root         (0)    12474 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucPgrwUtils.cc
--rw-rw-rw-   0 root         (0) root         (0)     7990 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucPgrwUtils.hh
--rw-rw-rw-   0 root         (0) root         (0)     6245 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucPinKing.hh
--rw-rw-rw-   0 root         (0) root         (0)    10383 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucPinLoader.cc
--rw-rw-rw-   0 root         (0) root         (0)     9351 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucPinLoader.hh
--rw-rw-rw-   0 root         (0) root         (0)     3859 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucPinObject.hh
--rw-rw-rw-   0 root         (0) root         (0)     2488 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucPinPath.cc
--rw-rw-rw-   0 root         (0) root         (0)     3769 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucPinPath.hh
--rw-rw-rw-   0 root         (0) root         (0)     3334 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucPreload.cc
--rw-rw-rw-   0 root         (0) root         (0)     3993 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucPreload.hh
--rw-rw-rw-   0 root         (0) root         (0)    12229 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucProg.cc
--rw-rw-rw-   0 root         (0) root         (0)     6185 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucProg.hh
--rw-rw-rw-   0 root         (0) root         (0)    30926 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucPsx.cc
--rw-rw-rw-   0 root         (0) root         (0)     6045 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucPsx.hh
--rw-rw-rw-   0 root         (0) root         (0)    13929 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucPup.cc
--rw-rw-rw-   0 root         (0) root         (0)     8053 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucPup.hh
--rw-rw-rw-   0 root         (0) root         (0)     7879 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucRash.hh
--rw-rw-rw-   0 root         (0) root         (0)     9416 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucRash.icc
--rw-rw-rw-   0 root         (0) root         (0)     6087 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucReqID.cc
--rw-rw-rw-   0 root         (0) root         (0)     3008 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucReqID.hh
--rw-rw-rw-   0 root         (0) root         (0)     3219 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucSFVec.hh
--rw-rw-rw-   0 root         (0) root         (0)     9442 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucSHA3.cc
--rw-rw-rw-   0 root         (0) root         (0)     6968 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucSHA3.hh
--rw-rw-rw-   0 root         (0) root         (0)     6346 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucSid.cc
--rw-rw-rw-   0 root         (0) root         (0)     6332 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucSid.hh
--rw-rw-rw-   0 root         (0) root         (0)     2968 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucSiteName.cc
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucSiteName.hh
--rw-rw-rw-   0 root         (0) root         (0)     3074 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucStats.hh
--rw-rw-rw-   0 root         (0) root         (0)    47398 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucStream.cc
--rw-rw-rw-   0 root         (0) root         (0)    11689 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucStream.hh
--rw-rw-rw-   0 root         (0) root         (0)    35608 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucString.cc
--rw-rw-rw-   0 root         (0) root         (0)    25266 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucString.hh
--rw-rw-rw-   0 root         (0) root         (0)     7049 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucSxeq.cc
--rw-rw-rw-   0 root         (0) root         (0)     3039 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucSxeq.hh
--rw-rw-rw-   0 root         (0) root         (0)     5248 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucTList.hh
--rw-rw-rw-   0 root         (0) root         (0)     9887 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucTPC.cc
--rw-rw-rw-   0 root         (0) root         (0)     3801 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucTPC.hh
--rw-rw-rw-   0 root         (0) root         (0)     3390 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucTUtils.hh
--rw-rw-rw-   0 root         (0) root         (0)     7032 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucTable.hh
--rw-rw-rw-   0 root         (0) root         (0)     5093 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucTokenizer.cc
--rw-rw-rw-   0 root         (0) root         (0)     3588 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucTokenizer.hh
--rw-rw-rw-   0 root         (0) root         (0)     3019 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucTrace.cc
--rw-rw-rw-   0 root         (0) root         (0)     2897 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucTrace.hh
--rw-rw-rw-   0 root         (0) root         (0)     8152 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucUri.cc
--rw-rw-rw-   0 root         (0) root         (0)     4397 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucUri.hh
--rw-rw-rw-   0 root         (0) root         (0)    43429 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucUtils.cc
--rw-rw-rw-   0 root         (0) root         (0)     5639 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucUtils.hh
--rw-rw-rw-   0 root         (0) root         (0)     5319 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucVerName.cc
--rw-rw-rw-   0 root         (0) root         (0)     4226 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucVerName.hh
--rw-rw-rw-   0 root         (0) root         (0)     7043 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOucXAttr.hh
--rw-rw-rw-   0 root         (0) root         (0)    15942 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOuca2x.cc
--rw-rw-rw-   0 root         (0) root         (0)     4130 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOuc/XrdOuca2x.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdPfc/
--rw-rw-rw-   0 root         (0) root         (0)     7215 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/README
--rw-rw-rw-   0 root         (0) root         (0)    29263 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfc.cc
--rw-rw-rw-   0 root         (0) root         (0)    18171 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfc.hh
--rw-rw-rw-   0 root         (0) root         (0)     1841 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcAllowDecision.cc
--rw-rw-rw-   0 root         (0) root         (0)     3643 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcBlacklistDecision.cc
--rw-rw-rw-   0 root         (0) root         (0)    12821 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcCommand.cc
--rw-rw-rw-   0 root         (0) root         (0)    27729 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcConfiguration.cc
--rw-rw-rw-   0 root         (0) root         (0)     2444 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcDecision.hh
--rw-rw-rw-   0 root         (0) root         (0)    46138 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcFile.cc
--rw-rw-rw-   0 root         (0) root         (0)    14635 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcFile.hh
--rw-rw-rw-   0 root         (0) root         (0)     1933 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcIO.cc
--rw-rw-rw-   0 root         (0) root         (0)     2691 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcIO.hh
--rw-rw-rw-   0 root         (0) root         (0)    10962 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcIOFile.cc
--rw-rw-rw-   0 root         (0) root         (0)     3636 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcIOFile.hh
--rw-rw-rw-   0 root         (0) root         (0)    12359 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcIOFileBlock.cc
--rw-rw-rw-   0 root         (0) root         (0)     2979 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcIOFileBlock.hh
--rw-rw-rw-   0 root         (0) root         (0)    19051 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcInfo.cc
--rw-rw-rw-   0 root         (0) root         (0)    18053 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcInfo.hh
--rw-rw-rw-   0 root         (0) root         (0)    12636 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcPrint.cc
--rw-rw-rw-   0 root         (0) root         (0)     2934 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcPrint.hh
--rw-rw-rw-   0 root         (0) root         (0)    32423 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcPurge.cc
--rw-rw-rw-   0 root         (0) root         (0)     4738 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcStats.hh
--rw-rw-rw-   0 root         (0) root         (0)     2079 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcTrace.hh
--rw-rw-rw-   0 root         (0) root         (0)     1380 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc/XrdPfcTypes.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdPosix/
--rw-rw-rw-   0 root         (0) root         (0)     7201 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/README
--rw-rw-rw-   0 root         (0) root         (0)    32970 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosix.cc
--rw-rw-rw-   0 root         (0) root         (0)     4656 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosix.hh
--rw-rw-rw-   0 root         (0) root         (0)     7779 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixAdmin.cc
--rw-rw-rw-   0 root         (0) root         (0)     3383 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixAdmin.hh
--rw-rw-rw-   0 root         (0) root         (0)     5977 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixCache.cc
--rw-rw-rw-   0 root         (0) root         (0)     6942 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixCache.hh
--rw-rw-rw-   0 root         (0) root         (0)     2992 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixCallBack.cc
--rw-rw-rw-   0 root         (0) root         (0)     4732 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixCallBack.hh
--rw-rw-rw-   0 root         (0) root         (0)    23522 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixConfig.cc
--rw-rw-rw-   0 root         (0) root         (0)     3483 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixConfig.hh
--rw-rw-rw-   0 root         (0) root         (0)     5169 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixDir.cc
--rw-rw-rw-   0 root         (0) root         (0)     4117 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixDir.hh
--rw-rw-rw-   0 root         (0) root         (0)     8592 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixExtern.hh
--rw-rw-rw-   0 root         (0) root         (0)     6173 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixExtra.cc
--rw-rw-rw-   0 root         (0) root         (0)     5480 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixExtra.hh
--rw-rw-rw-   0 root         (0) root         (0)    26695 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixFile.cc
--rw-rw-rw-   0 root         (0) root         (0)     8405 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixFile.hh
--rw-rw-rw-   0 root         (0) root         (0)     7869 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixFileRH.cc
--rw-rw-rw-   0 root         (0) root         (0)     4377 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixFileRH.hh
--rw-rw-rw-   0 root         (0) root         (0)     2994 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixInfo.hh
--rw-rw-rw-   0 root         (0) root         (0)    14923 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixLinkage.cc
--rw-rw-rw-   0 root         (0) root         (0)    14552 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixLinkage.hh
--rw-rw-rw-   0 root         (0) root         (0)     8516 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixMap.cc
--rw-rw-rw-   0 root         (0) root         (0)     3065 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixMap.hh
--rw-rw-rw-   0 root         (0) root         (0)     3041 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixObjGuard.hh
--rw-rw-rw-   0 root         (0) root         (0)    11702 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixObject.cc
--rw-rw-rw-   0 root         (0) root         (0)     4655 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixObject.hh
--rw-rw-rw-   0 root         (0) root         (0)     3600 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixOsDep.hh
--rw-rw-rw-   0 root         (0) root         (0)    24220 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixPreload.cc
--rw-rw-rw-   0 root         (0) root         (0)    19202 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixPreload32.cc
--rw-rw-rw-   0 root         (0) root         (0)     5301 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixPrepIO.cc
--rw-rw-rw-   0 root         (0) root         (0)     4774 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixPrepIO.hh
--rw-rw-rw-   0 root         (0) root         (0)     3366 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixStats.hh
--rw-rw-rw-   0 root         (0) root         (0)     2880 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixTrace.hh
--rw-rw-rw-   0 root         (0) root         (0)    53317 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixXrootd.cc
--rw-rw-rw-   0 root         (0) root         (0)    18316 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixXrootd.hh
--rw-rw-rw-   0 root         (0) root         (0)    11698 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixXrootdPath.cc
--rw-rw-rw-   0 root         (0) root         (0)     3595 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix/XrdPosixXrootdPath.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdPss/
--rw-rw-rw-   0 root         (0) root         (0)    45924 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPss/XrdPss.cc
--rw-rw-rw-   0 root         (0) root         (0)     9184 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPss/XrdPss.hh
--rw-rw-rw-   0 root         (0) root         (0)     8543 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPss/XrdPssAio.cc
--rw-rw-rw-   0 root         (0) root         (0)     5049 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPss/XrdPssAioCB.cc
--rw-rw-rw-   0 root         (0) root         (0)     3188 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPss/XrdPssAioCB.hh
--rw-rw-rw-   0 root         (0) root         (0)     8402 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPss/XrdPssCks.cc
--rw-rw-rw-   0 root         (0) root         (0)     3733 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPss/XrdPssCks.hh
--rw-rw-rw-   0 root         (0) root         (0)    30386 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPss/XrdPssConfig.cc
--rw-rw-rw-   0 root         (0) root         (0)     2807 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPss/XrdPssTrace.hh
--rw-rw-rw-   0 root         (0) root         (0)     8758 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPss/XrdPssUrlInfo.cc
--rw-rw-rw-   0 root         (0) root         (0)     3611 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPss/XrdPssUrlInfo.hh
--rw-rw-rw-   0 root         (0) root         (0)     5115 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPss/XrdPssUtils.cc
--rw-rw-rw-   0 root         (0) root         (0)     3367 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPss/XrdPssUtils.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdRmc/
--rw-rw-rw-   0 root         (0) root         (0)     3076 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdRmc/XrdRmc.cc
--rw-rw-rw-   0 root         (0) root         (0)     8248 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdRmc/XrdRmc.hh
--rw-rw-rw-   0 root         (0) root         (0)    20495 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdRmc/XrdRmcData.cc
--rw-rw-rw-   0 root         (0) root         (0)     5754 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdRmc/XrdRmcData.hh
--rw-rw-rw-   0 root         (0) root         (0)    20703 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdRmc/XrdRmcReal.cc
--rw-rw-rw-   0 root         (0) root         (0)     5594 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdRmc/XrdRmcReal.hh
--rw-rw-rw-   0 root         (0) root         (0)     7041 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdRmc/XrdRmcSlot.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdSciTokens/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdSciTokens/configs/
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/configs/export-lib-symbols
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/configs/export-module-symbols
--rw-rw-rw-   0 root         (0) root         (0)      945 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/configs/scitokens.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdSciTokens/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdSciTokens/test/config/
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/test/config/override.conf
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/test/config/scitokens-aud.cfg
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/test/config/scitokens-multi-aud.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/test/config/scitokens-no-aud.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1879 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/test/config/xrootd-http.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1598 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/test/create-pubkey.py
--rw-rw-rw-   0 root         (0) root         (0)      594 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/test/openssl-selfsigned.conf
--rwxrwxrwx   0 root         (0) root         (0)      803 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/test/setup_tests.sh
--rwxrwxrwx   0 root         (0) root         (0)     5083 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/test/test_inside_docker.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/inih/
--rw-rw-rw-   0 root         (0) root         (0)       10 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/inih/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/inih/.travis.yml
--rw-rw-rw-   0 root         (0) root         (0)    13507 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/inih/INIReader.h
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/inih/INIReaderTest.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1510 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/inih/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     1574 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/inih/README.md
--rw-rw-rw-   0 root         (0) root         (0)      416 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/inih/test.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/examples/
--rw-rw-rw-   0 root         (0) root         (0)     3435 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/examples/github-issues.cc
--rw-rw-rw-   0 root         (0) root         (0)     2787 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/examples/iostream.cc
--rw-rw-rw-   0 root         (0) root         (0)     2496 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/examples/streaming.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/picotest/
--rw-rw-rw-   0 root         (0) root         (0)     2452 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/picotest/picotest.c
--rw-rw-rw-   0 root         (0) root         (0)     1519 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/picotest/picotest.h
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/.clang-format
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/.gitmodules
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/.travis.yml
--rw-rw-rw-   0 root         (0) root         (0)      903 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/Changes
--rw-rw-rw-   0 root         (0) root         (0)     1336 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     7011 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/README.mkdn
--rw-rw-rw-   0 root         (0) root         (0)    33256 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/picojson.h
--rw-rw-rw-   0 root         (0) root         (0)    12611 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/test.cc
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/vendor/README.vendor
--rw-rw-rw-   0 root         (0) root         (0)    11357 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     7684 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/README.md
--rw-rw-rw-   0 root         (0) root         (0)    48515 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/XrdSciTokensAccess.cc
--rw-rw-rw-   0 root         (0) root         (0)     2910 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens/XrdSciTokensHelper.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdSec/
--rw-rw-rw-   0 root         (0) root         (0)     4540 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecAttr.hh
--rw-rw-rw-   0 root         (0) root         (0)     5632 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecClient.cc
--rw-rw-rw-   0 root         (0) root         (0)     6046 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecEntity.cc
--rw-rw-rw-   0 root         (0) root         (0)     6747 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecEntity.hh
--rw-rw-rw-   0 root         (0) root         (0)     6459 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecEntityAttr.cc
--rw-rw-rw-   0 root         (0) root         (0)     8424 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecEntityAttr.hh
--rw-rw-rw-   0 root         (0) root         (0)     4638 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecEntityPin.hh
--rw-rw-rw-   0 root         (0) root         (0)     2945 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecEntityXtra.cc
--rw-rw-rw-   0 root         (0) root         (0)     2772 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecEntityXtra.hh
--rw-rw-rw-   0 root         (0) root         (0)    34779 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecInterface.hh
--rw-rw-rw-   0 root         (0) root         (0)    10669 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecLoadSecurity.cc
--rw-rw-rw-   0 root         (0) root         (0)     7822 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecLoadSecurity.hh
--rw-rw-rw-   0 root         (0) root         (0)    15666 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecPManager.cc
--rw-rw-rw-   0 root         (0) root         (0)     5056 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecPManager.hh
--rw-rw-rw-   0 root         (0) root         (0)    18129 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecProtect.cc
--rw-rw-rw-   0 root         (0) root         (0)     8540 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecProtect.hh
--rw-rw-rw-   0 root         (0) root         (0)    11790 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecProtector.cc
--rw-rw-rw-   0 root         (0) root         (0)     7608 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecProtector.hh
--rw-rw-rw-   0 root         (0) root         (0)     4849 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecProtocolhost.cc
--rw-rw-rw-   0 root         (0) root         (0)     3535 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecProtocolhost.hh
--rw-rw-rw-   0 root         (0) root         (0)    40467 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecServer.cc
--rw-rw-rw-   0 root         (0) root         (0)     5105 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecServer.hh
--rw-rw-rw-   0 root         (0) root         (0)    14312 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecTLayer.cc
--rw-rw-rw-   0 root         (0) root         (0)     7692 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecTLayer.hh
--rw-rw-rw-   0 root         (0) root         (0)     3066 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSecTrace.hh
--rw-rw-rw-   0 root         (0) root         (0)     7624 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSectestClient.cc
--rw-rw-rw-   0 root         (0) root         (0)    12009 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec/XrdSectestServer.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdSecgsi/
--rw-rw-rw-   0 root         (0) root         (0)   197464 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecgsi/XrdSecProtocolgsi.cc
--rw-rw-rw-   0 root         (0) root         (0)    24807 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecgsi/XrdSecProtocolgsi.hh
--rw-rw-rw-   0 root         (0) root         (0)     6777 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecgsi/XrdSecgsiAuthzFunDN.cc
--rw-rw-rw-   0 root         (0) root         (0)    11227 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecgsi/XrdSecgsiAuthzFunVO.cc
--rw-rw-rw-   0 root         (0) root         (0)     8781 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecgsi/XrdSecgsiGMAPFunDN.cc
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecgsi/XrdSecgsiGMAPFunDN.cf
--rw-rw-rw-   0 root         (0) root         (0)     9513 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecgsi/XrdSecgsiOpts.hh
--rw-rw-rw-   0 root         (0) root         (0)    26699 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecgsi/XrdSecgsiProxy.cc
--rw-rw-rw-   0 root         (0) root         (0)     3023 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecgsi/XrdSecgsiTrace.hh
--rw-rw-rw-   0 root         (0) root         (0)    17319 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecgsi/XrdSecgsitest.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdSeckrb5/
--rw-rw-rw-   0 root         (0) root         (0)    38570 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSeckrb5/XrdSecProtocolkrb5.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdSecpwd/
--rw-rw-rw-   0 root         (0) root         (0)   129049 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecpwd/XrdSecProtocolpwd.cc
--rw-rw-rw-   0 root         (0) root         (0)    19037 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecpwd/XrdSecProtocolpwd.hh
--rw-rw-rw-   0 root         (0) root         (0)     2626 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecpwd/XrdSecpwdPlatform.hh
--rw-rw-rw-   0 root         (0) root         (0)    84580 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecpwd/XrdSecpwdSrvAdmin.cc
--rw-rw-rw-   0 root         (0) root         (0)     3023 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecpwd/XrdSecpwdTrace.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdSecsss/
--rw-rw-rw-   0 root         (0) root         (0)    41443 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecsss/XrdSecProtocolsss.cc
--rw-rw-rw-   0 root         (0) root         (0)     6297 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecsss/XrdSecProtocolsss.hh
--rw-rw-rw-   0 root         (0) root         (0)    19394 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecsss/XrdSecsssAdmin.cc
--rw-rw-rw-   0 root         (0) root         (0)     3559 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecsss/XrdSecsssCon.cc
--rw-rw-rw-   0 root         (0) root         (0)     4329 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecsss/XrdSecsssCon.hh
--rw-rw-rw-   0 root         (0) root         (0)    11806 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecsss/XrdSecsssEnt.cc
--rw-rw-rw-   0 root         (0) root         (0)     5290 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecsss/XrdSecsssEnt.hh
--rw-rw-rw-   0 root         (0) root         (0)     9560 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecsss/XrdSecsssID.cc
--rw-rw-rw-   0 root         (0) root         (0)     8505 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecsss/XrdSecsssID.hh
--rw-rw-rw-   0 root         (0) root         (0)    25232 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecsss/XrdSecsssKT.cc
--rw-rw-rw-   0 root         (0) root         (0)     5358 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecsss/XrdSecsssKT.hh
--rw-rw-rw-   0 root         (0) root         (0)     2704 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecsss/XrdSecsssMap.hh
--rw-rw-rw-   0 root         (0) root         (0)     5765 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecsss/XrdSecsssRR.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdSecunix/
--rw-rw-rw-   0 root         (0) root         (0)     8575 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecunix/XrdSecProtocolunix.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdSecztn/
--rw-rw-rw-   0 root         (0) root         (0)    28393 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecztn/XrdSecProtocolztn.cc
--rw-rw-rw-   0 root         (0) root         (0)     6814 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecztn/XrdSecztn.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdSfs/
--rw-rw-rw-   0 root         (0) root         (0)     3999 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSfs/XrdSfsAio.hh
--rw-rw-rw-   0 root         (0) root         (0)     5824 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSfs/XrdSfsDio.hh
--rw-rw-rw-   0 root         (0) root         (0)     5455 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSfs/XrdSfsFAttr.hh
--rw-rw-rw-   0 root         (0) root         (0)     5100 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSfs/XrdSfsFlags.hh
--rw-rw-rw-   0 root         (0) root         (0)     5619 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSfs/XrdSfsGPFile.hh
--rw-rw-rw-   0 root         (0) root         (0)    12634 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSfs/XrdSfsInterface.cc
--rw-rw-rw-   0 root         (0) root         (0)    67119 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSfs/XrdSfsInterface.hh
--rw-rw-rw-   0 root         (0) root         (0)    38665 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSfs/XrdSfsNative.cc
--rw-rw-rw-   0 root         (0) root         (0)    10785 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSfs/XrdSfsNative.hh
--rw-rw-rw-   0 root         (0) root         (0)     3537 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSfs/XrdSfsXio.cc
--rw-rw-rw-   0 root         (0) root         (0)     7187 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSfs/XrdSfsXio.hh
--rw-rw-rw-   0 root         (0) root         (0)     4432 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSfs/XrdSfsXioImpl.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdSsi/
--rw-rw-rw-   0 root         (0) root         (0)     6178 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiAlert.cc
--rw-rw-rw-   0 root         (0) root         (0)     3366 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiAlert.hh
--rw-rw-rw-   0 root         (0) root         (0)     2661 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiAtomics.cc
--rw-rw-rw-   0 root         (0) root         (0)     7958 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiAtomics.hh
--rw-rw-rw-   0 root         (0) root         (0)     3132 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiBVec.hh
--rw-rw-rw-   0 root         (0) root         (0)    14419 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiClient.cc
--rw-rw-rw-   0 root         (0) root         (0)     7934 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiCluster.hh
--rw-rw-rw-   0 root         (0) root         (0)     4735 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiCms.cc
--rw-rw-rw-   0 root         (0) root         (0)     3752 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiCms.hh
--rw-rw-rw-   0 root         (0) root         (0)     7049 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiDir.cc
--rw-rw-rw-   0 root         (0) root         (0)     3177 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiDir.hh
--rw-rw-rw-   0 root         (0) root         (0)     4087 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiEntity.hh
--rw-rw-rw-   0 root         (0) root         (0)     2663 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiErrInfo.cc
--rw-rw-rw-   0 root         (0) root         (0)     6519 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiErrInfo.hh
--rw-rw-rw-   0 root         (0) root         (0)     7117 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiEvent.cc
--rw-rw-rw-   0 root         (0) root         (0)     4015 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiEvent.hh
--rw-rw-rw-   0 root         (0) root         (0)    18166 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiFile.cc
--rw-rw-rw-   0 root         (0) root         (0)     5424 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiFile.hh
--rw-rw-rw-   0 root         (0) root         (0)    35655 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiFileReq.cc
--rw-rw-rw-   0 root         (0) root         (0)     6776 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiFileReq.hh
--rw-rw-rw-   0 root         (0) root         (0)     3711 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiFileResource.cc
--rw-rw-rw-   0 root         (0) root         (0)     2797 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiFileResource.hh
--rw-rw-rw-   0 root         (0) root         (0)    26232 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiFileSess.cc
--rw-rw-rw-   0 root         (0) root         (0)     6023 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiFileSess.hh
--rw-rw-rw-   0 root         (0) root         (0)     7881 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiLogger.cc
--rw-rw-rw-   0 root         (0) root         (0)     8724 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiLogger.hh
--rw-rw-rw-   0 root         (0) root         (0)     6495 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiLogging.cc
--rw-rw-rw-   0 root         (0) root         (0)    17533 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiProvider.hh
--rw-rw-rw-   0 root         (0) root         (0)     3962 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiRRAgent.hh
--rw-rw-rw-   0 root         (0) root         (0)     4545 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiRRInfo.hh
--rw-rw-rw-   0 root         (0) root         (0)     4295 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiRRTable.hh
--rw-rw-rw-   0 root         (0) root         (0)     8144 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiRequest.cc
--rw-rw-rw-   0 root         (0) root         (0)    15740 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiRequest.hh
--rw-rw-rw-   0 root         (0) root         (0)     5790 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiResource.hh
--rw-rw-rw-   0 root         (0) root         (0)     7000 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiRespInfo.hh
--rw-rw-rw-   0 root         (0) root         (0)    12144 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiResponder.cc
--rw-rw-rw-   0 root         (0) root         (0)    13431 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiResponder.hh
--rw-rw-rw-   0 root         (0) root         (0)     8986 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiScale.cc
--rw-rw-rw-   0 root         (0) root         (0)     3515 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiScale.hh
--rw-rw-rw-   0 root         (0) root         (0)    12168 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiServReal.cc
--rw-rw-rw-   0 root         (0) root         (0)     3574 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiServReal.hh
--rw-rw-rw-   0 root         (0) root         (0)     3281 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiService.cc
--rw-rw-rw-   0 root         (0) root         (0)     9866 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiService.hh
--rw-rw-rw-   0 root         (0) root         (0)    17845 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiSessReal.cc
--rw-rw-rw-   0 root         (0) root         (0)     4784 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiSessReal.hh
--rw-rw-rw-   0 root         (0) root         (0)    20137 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiSfs.cc
--rw-rw-rw-   0 root         (0) root         (0)     7069 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiSfs.hh
--rw-rw-rw-   0 root         (0) root         (0)    25133 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiSfsConfig.cc
--rw-rw-rw-   0 root         (0) root         (0)     3556 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiSfsConfig.hh
--rw-rw-rw-   0 root         (0) root         (0)    45526 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiShMam.cc
--rw-rw-rw-   0 root         (0) root         (0)     5508 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiShMam.hh
--rw-rw-rw-   0 root         (0) root         (0)    22363 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiShMap.hh
--rw-rw-rw-   0 root         (0) root         (0)    12380 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiShMap.icc
--rw-rw-rw-   0 root         (0) root         (0)     3048 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiShMat.cc
--rw-rw-rw-   0 root         (0) root         (0)    19625 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiShMat.hh
--rw-rw-rw-   0 root         (0) root         (0)     6168 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiStat.cc
--rw-rw-rw-   0 root         (0) root         (0)     6883 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiStats.cc
--rw-rw-rw-   0 root         (0) root         (0)     4527 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiStats.hh
--rw-rw-rw-   0 root         (0) root         (0)     8580 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiStream.hh
--rw-rw-rw-   0 root         (0) root         (0)    24852 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiTaskReal.cc
--rw-rw-rw-   0 root         (0) root         (0)     4845 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiTaskReal.hh
--rw-rw-rw-   0 root         (0) root         (0)     2865 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiTrace.hh
--rw-rw-rw-   0 root         (0) root         (0)     9000 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiUtils.cc
--rw-rw-rw-   0 root         (0) root         (0)     3203 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi/XrdSsiUtils.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdSut/
--rw-rw-rw-   0 root         (0) root         (0)    22213 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSut/XrdSutAux.cc
--rw-rw-rw-   0 root         (0) root         (0)    15145 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSut/XrdSutAux.hh
--rw-rw-rw-   0 root         (0) root         (0)     5926 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSut/XrdSutBuckList.cc
--rw-rw-rw-   0 root         (0) root         (0)     3963 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSut/XrdSutBuckList.hh
--rw-rw-rw-   0 root         (0) root         (0)     8236 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSut/XrdSutBucket.cc
--rw-rw-rw-   0 root         (0) root         (0)     3458 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSut/XrdSutBucket.hh
--rw-rw-rw-   0 root         (0) root         (0)    16276 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSut/XrdSutBuffer.cc
--rw-rw-rw-   0 root         (0) root         (0)     4872 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSut/XrdSutBuffer.hh
--rw-rw-rw-   0 root         (0) root         (0)     6430 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSut/XrdSutCache.hh
--rw-rw-rw-   0 root         (0) root         (0)     5618 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSut/XrdSutCacheEntry.cc
--rw-rw-rw-   0 root         (0) root         (0)     5456 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSut/XrdSutCacheEntry.hh
--rw-rw-rw-   0 root         (0) root         (0)    21841 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSut/XrdSutPFCache.cc
--rw-rw-rw-   0 root         (0) root         (0)     5757 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSut/XrdSutPFCache.hh
--rw-rw-rw-   0 root         (0) root         (0)     5549 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSut/XrdSutPFEntry.cc
--rw-rw-rw-   0 root         (0) root         (0)     4790 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSut/XrdSutPFEntry.hh
--rw-rw-rw-   0 root         (0) root         (0)    64583 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSut/XrdSutPFile.cc
--rw-rw-rw-   0 root         (0) root         (0)     7738 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSut/XrdSutPFile.hh
--rw-rw-rw-   0 root         (0) root         (0)     8759 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSut/XrdSutRndm.cc
--rw-rw-rw-   0 root         (0) root         (0)     3293 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSut/XrdSutRndm.hh
--rw-rw-rw-   0 root         (0) root         (0)     2936 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSut/XrdSutTrace.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdSys/
--rw-rw-rw-   0 root         (0) root         (0)     5249 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysAtomics.hh
--rw-rw-rw-   0 root         (0) root         (0)     4979 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysDir.cc
--rw-rw-rw-   0 root         (0) root         (0)     3341 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysDir.hh
--rw-rw-rw-   0 root         (0) root         (0)     4790 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysE2T.cc
--rw-rw-rw-   0 root         (0) root         (0)     2750 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysE2T.hh
--rw-rw-rw-   0 root         (0) root         (0)     8454 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysError.cc
--rw-rw-rw-   0 root         (0) root         (0)     7349 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysError.hh
--rw-rw-rw-   0 root         (0) root         (0)     6923 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysFAttr.cc
--rw-rw-rw-   0 root         (0) root         (0)     4996 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysFAttr.hh
--rw-rw-rw-   0 root         (0) root         (0)     7106 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysFAttrBsd.icc
--rw-rw-rw-   0 root         (0) root         (0)     6632 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysFAttrLnx.icc
--rw-rw-rw-   0 root         (0) root         (0)     6063 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysFAttrMac.icc
--rw-rw-rw-   0 root         (0) root         (0)     7705 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysFAttrSun.icc
--rw-rw-rw-   0 root         (0) root         (0)     7575 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysFD.hh
--rw-rw-rw-   0 root         (0) root         (0)     4783 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysFallocate.cc
--rw-rw-rw-   0 root         (0) root         (0)     1578 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysFallocate.hh
--rw-rw-rw-   0 root         (0) root         (0)     2714 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysHeaders.hh
--rw-rw-rw-   0 root         (0) root         (0)    43245 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysIOEvents.cc
--rw-rw-rw-   0 root         (0) root         (0)    26713 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysIOEvents.hh
--rw-rw-rw-   0 root         (0) root         (0)    16042 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysIOEventsPollE.icc
--rw-rw-rw-   0 root         (0) root         (0)    17035 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysIOEventsPollKQ.icc
--rw-rw-rw-   0 root         (0) root         (0)    18696 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysIOEventsPollPoll.icc
--rw-rw-rw-   0 root         (0) root         (0)    14965 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysIOEventsPollPort.icc
--rw-rw-rw-   0 root         (0) root         (0)    16419 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysKernelBuffer.hh
--rw-rw-rw-   0 root         (0) root         (0)     5437 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysLogPI.hh
--rw-rw-rw-   0 root         (0) root         (0)    26549 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysLogger.cc
--rw-rw-rw-   0 root         (0) root         (0)    11736 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysLogger.hh
--rw-rw-rw-   0 root         (0) root         (0)    12120 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysLogging.cc
--rw-rw-rw-   0 root         (0) root         (0)     5811 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysLogging.hh
--rw-rw-rw-   0 root         (0) root         (0)     2511 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysPageSize.hh
--rw-rw-rw-   0 root         (0) root         (0)     3233 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysPlatform.cc
--rw-rw-rw-   0 root         (0) root         (0)     8249 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysPlatform.hh
--rw-rw-rw-   0 root         (0) root         (0)    17839 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysPlugin.cc
--rw-rw-rw-   0 root         (0) root         (0)    13621 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysPlugin.hh
--rw-rw-rw-   0 root         (0) root         (0)    12930 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysPriv.cc
--rw-rw-rw-   0 root         (0) root         (0)     4228 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysPriv.hh
--rw-rw-rw-   0 root         (0) root         (0)    13657 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysPthread.cc
--rw-rw-rw-   0 root         (0) root         (0)    19415 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysPthread.hh
--rw-rw-rw-   0 root         (0) root         (0)     3245 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysPwd.hh
--rw-rw-rw-   0 root         (0) root         (0)    11994 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysRAtomic.hh
--rw-rw-rw-   0 root         (0) root         (0)     3952 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysSemWait.hh
--rw-rw-rw-   0 root         (0) root         (0)     9460 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysTimer.cc
--rw-rw-rw-   0 root         (0) root         (0)     3814 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysTimer.hh
--rw-rw-rw-   0 root         (0) root         (0)    15639 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysTrace.cc
--rw-rw-rw-   0 root         (0) root         (0)     4739 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysTrace.hh
--rw-rw-rw-   0 root         (0) root         (0)     8298 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysUtils.cc
--rw-rw-rw-   0 root         (0) root         (0)     4798 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysUtils.hh
--rw-rw-rw-   0 root         (0) root         (0)     4735 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysXAttr.cc
--rw-rw-rw-   0 root         (0) root         (0)    15063 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysXAttr.hh
--rw-rw-rw-   0 root         (0) root         (0)     5688 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysXSLock.cc
--rw-rw-rw-   0 root         (0) root         (0)     3311 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSys/XrdSysXSLock.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdThrottle/
--rw-rw-rw-   0 root         (0) root         (0)     3577 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdThrottle/README
--rw-rw-rw-   0 root         (0) root         (0)     7487 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdThrottle/XrdThrottle.hh
--rw-rw-rw-   0 root         (0) root         (0)     6658 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdThrottle/XrdThrottleFile.cc
--rw-rw-rw-   0 root         (0) root         (0)     5731 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdThrottle/XrdThrottleFileSystem.cc
--rw-rw-rw-   0 root         (0) root         (0)    12897 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdThrottle/XrdThrottleFileSystemConfig.cc
--rw-rw-rw-   0 root         (0) root         (0)    18584 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdThrottle/XrdThrottleManager.cc
--rw-rw-rw-   0 root         (0) root         (0)     5403 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdThrottle/XrdThrottleManager.hh
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdThrottle/XrdThrottleTrace.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdTls/
--rw-rw-rw-   0 root         (0) root         (0)    10417 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTls/XrdTls.cc
--rw-rw-rw-   0 root         (0) root         (0)     6921 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTls/XrdTls.hh
--rw-rw-rw-   0 root         (0) root         (0)    37652 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTls/XrdTlsContext.cc
--rw-rw-rw-   0 root         (0) root         (0)    14507 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTls/XrdTlsContext.hh
--rw-rw-rw-   0 root         (0) root         (0)     1259 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTls/XrdTlsHostcheck.hh
--rw-rw-rw-   0 root         (0) root         (0)     6628 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTls/XrdTlsHostcheck.icc
--rw-rw-rw-   0 root         (0) root         (0)     5275 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTls/XrdTlsNotary.cc
--rw-rw-rw-   0 root         (0) root         (0)     5222 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTls/XrdTlsNotary.hh
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTls/XrdTlsNotaryUtils.hh
--rw-rw-rw-   0 root         (0) root         (0)     7142 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTls/XrdTlsNotaryUtils.icc
--rw-rw-rw-   0 root         (0) root         (0)     3969 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTls/XrdTlsPeerCerts.cc
--rw-rw-rw-   0 root         (0) root         (0)     4951 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTls/XrdTlsPeerCerts.hh
--rw-rw-rw-   0 root         (0) root         (0)    33590 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTls/XrdTlsSocket.cc
--rw-rw-rw-   0 root         (0) root         (0)    11845 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTls/XrdTlsSocket.hh
--rw-rw-rw-   0 root         (0) root         (0)    16134 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTls/XrdTlsTempCA.cc
--rw-rw-rw-   0 root         (0) root         (0)     5462 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTls/XrdTlsTempCA.hh
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTls/XrdTlsTrace.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdTpc/
--rw-rw-rw-   0 root         (0) root         (0)     4032 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTpc/README.md
--rw-rw-rw-   0 root         (0) root         (0)     5387 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTpc/XrdTpcConfigure.cc
--rw-rw-rw-   0 root         (0) root         (0)     1663 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTpc/XrdTpcCurlMulti.cc
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTpc/XrdTpcCurlMulti.hh
--rw-rw-rw-   0 root         (0) root         (0)    19456 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTpc/XrdTpcMultistream.cc
--rw-rw-rw-   0 root         (0) root         (0)    10532 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTpc/XrdTpcState.cc
--rw-rw-rw-   0 root         (0) root         (0)     5794 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTpc/XrdTpcState.hh
--rw-rw-rw-   0 root         (0) root         (0)     7210 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTpc/XrdTpcStream.cc
--rw-rw-rw-   0 root         (0) root         (0)     5499 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTpc/XrdTpcStream.hh
--rw-rw-rw-   0 root         (0) root         (0)    44035 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTpc/XrdTpcTPC.cc
--rw-rw-rw-   0 root         (0) root         (0)     5994 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTpc/XrdTpcTPC.hh
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTpc/export-lib-symbols
--rwxrwxrwx   0 root         (0) root         (0)     3709 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTpc/xrootd-test-tpc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdVoms/
--rw-rw-rw-   0 root         (0) root         (0)     2917 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdVoms/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2590 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdVoms/XrdVoms.hh
--rw-rw-rw-   0 root         (0) root         (0)    22180 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdVoms/XrdVomsFun.cc
--rw-rw-rw-   0 root         (0) root         (0)     3835 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdVoms/XrdVomsFun.hh
--rw-rw-rw-   0 root         (0) root         (0)     6174 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdVoms/XrdVomsHttp.cc
--rw-rw-rw-   0 root         (0) root         (0)    15232 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdVoms/XrdVomsMapfile.cc
--rw-rw-rw-   0 root         (0) root         (0)     4249 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdVoms/XrdVomsMapfile.hh
--rw-rw-rw-   0 root         (0) root         (0)     2680 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdVoms/XrdVomsTrace.hh
--rw-rw-rw-   0 root         (0) root         (0)     4105 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdVoms/XrdVomsgsi.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdXml/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdXml/tinyxml/
--rw-rw-rw-   0 root         (0) root         (0)     2507 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXml/tinyxml/tinystr.cpp
--rw-rw-rw-   0 root         (0) root         (0)     8197 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXml/tinyxml/tinystr.h
--rw-rw-rw-   0 root         (0) root         (0)    37588 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXml/tinyxml/tinyxml.cpp
--rw-rw-rw-   0 root         (0) root         (0)    64835 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXml/tinyxml/tinyxml.h
--rw-rw-rw-   0 root         (0) root         (0)     1791 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXml/tinyxml/tinyxmlerror.cpp
--rw-rw-rw-   0 root         (0) root         (0)    37439 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXml/tinyxml/tinyxmlparser.cpp
--rw-rw-rw-   0 root         (0) root         (0)    18501 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXml/XrdXmlMetaLink.cc
--rw-rw-rw-   0 root         (0) root         (0)     9497 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXml/XrdXmlMetaLink.hh
--rw-rw-rw-   0 root         (0) root         (0)    10670 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXml/XrdXmlRdrTiny.cc
--rw-rw-rw-   0 root         (0) root         (0)     3590 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXml/XrdXmlRdrTiny.hh
--rw-rw-rw-   0 root         (0) root         (0)    11751 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXml/XrdXmlRdrXml2.cc
--rw-rw-rw-   0 root         (0) root         (0)     3585 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXml/XrdXmlRdrXml2.hh
--rw-rw-rw-   0 root         (0) root         (0)     4195 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXml/XrdXmlReader.cc
--rw-rw-rw-   0 root         (0) root         (0)     9010 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXml/XrdXmlReader.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdXrootd/
--rw-rw-rw-   0 root         (0) root         (0)    21688 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdAdmin.cc
--rw-rw-rw-   0 root         (0) root         (0)     3927 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdAdmin.hh
--rw-rw-rw-   0 root         (0) root         (0)     6106 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdAioBuff.cc
--rw-rw-rw-   0 root         (0) root         (0)     3387 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdAioBuff.hh
--rw-rw-rw-   0 root         (0) root         (0)     6164 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdAioFob.cc
--rw-rw-rw-   0 root         (0) root         (0)     3140 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdAioFob.hh
--rw-rw-rw-   0 root         (0) root         (0)    10852 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdAioPgrw.cc
--rw-rw-rw-   0 root         (0) root         (0)     4017 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdAioPgrw.hh
--rw-rw-rw-   0 root         (0) root         (0)    16842 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdAioTask.cc
--rw-rw-rw-   0 root         (0) root         (0)     5932 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdAioTask.hh
--rw-rw-rw-   0 root         (0) root         (0)     3257 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdBridge.cc
--rw-rw-rw-   0 root         (0) root         (0)    25502 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdBridge.hh
--rw-rw-rw-   0 root         (0) root         (0)    17339 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdCallBack.cc
--rw-rw-rw-   0 root         (0) root         (0)     3955 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdCallBack.hh
--rw-rw-rw-   0 root         (0) root         (0)    71797 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdConfig.cc
--rw-rw-rw-   0 root         (0) root         (0)    25761 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdConfigMon.cc
--rw-rw-rw-   0 root         (0) root         (0)    14752 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdFile.cc
--rw-rw-rw-   0 root         (0) root         (0)     8211 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdFile.hh
--rw-rw-rw-   0 root         (0) root         (0)     2629 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdFileLock.hh
--rw-rw-rw-   0 root         (0) root         (0)     6072 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdFileLock1.cc
--rw-rw-rw-   0 root         (0) root         (0)     2959 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdFileLock1.hh
--rw-rw-rw-   0 root         (0) root         (0)     7522 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdFileStats.hh
--rw-rw-rw-   0 root         (0) root         (0)    10638 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdGPFile.hh
--rw-rw-rw-   0 root         (0) root         (0)    19666 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdGSReal.cc
--rw-rw-rw-   0 root         (0) root         (0)     6593 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdGSReal.hh
--rw-rw-rw-   0 root         (0) root         (0)     5076 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdGStream.cc
--rw-rw-rw-   0 root         (0) root         (0)     8514 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdGStream.hh
--rw-rw-rw-   0 root         (0) root         (0)    26130 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdJob.cc
--rw-rw-rw-   0 root         (0) root         (0)     4224 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdJob.hh
--rw-rw-rw-   0 root         (0) root         (0)     3858 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdLoadLib.cc
--rw-rw-rw-   0 root         (0) root         (0)    14081 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdMonData.hh
--rw-rw-rw-   0 root         (0) root         (0)     5374 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdMonFMap.cc
--rw-rw-rw-   0 root         (0) root         (0)     3118 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdMonFMap.hh
--rw-rw-rw-   0 root         (0) root         (0)    18282 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdMonFile.cc
--rw-rw-rw-   0 root         (0) root         (0)     4376 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdMonFile.hh
--rw-rw-rw-   0 root         (0) root         (0)    42910 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdMonitor.cc
--rw-rw-rw-   0 root         (0) root         (0)    12097 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdMonitor.hh
--rw-rw-rw-   0 root         (0) root         (0)    17436 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdNormAio.cc
--rw-rw-rw-   0 root         (0) root         (0)     3758 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdNormAio.hh
--rw-rw-rw-   0 root         (0) root         (0)    19524 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdPgrwAio.cc
--rw-rw-rw-   0 root         (0) root         (0)     3708 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdPgrwAio.hh
--rw-rw-rw-   0 root         (0) root         (0)     4934 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdPgwBadCS.cc
--rw-rw-rw-   0 root         (0) root         (0)     2979 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdPgwBadCS.hh
--rw-rw-rw-   0 root         (0) root         (0)     7262 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdPgwCtl.cc
--rw-rw-rw-   0 root         (0) root         (0)     4842 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdPgwCtl.hh
--rw-rw-rw-   0 root         (0) root         (0)     4520 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdPgwFob.cc
--rw-rw-rw-   0 root         (0) root         (0)     4321 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdPgwFob.hh
--rw-rw-rw-   0 root         (0) root         (0)     3973 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdPio.cc
--rw-rw-rw-   0 root         (0) root         (0)     3751 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdPio.hh
--rw-rw-rw-   0 root         (0) root         (0)     4685 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdPlugin.cc
--rw-rw-rw-   0 root         (0) root         (0)    12615 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdPrepare.cc
--rw-rw-rw-   0 root         (0) root         (0)     4956 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdPrepare.hh
--rw-rw-rw-   0 root         (0) root         (0)    53957 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdProtocol.cc
--rw-rw-rw-   0 root         (0) root         (0)    23887 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdProtocol.hh
--rw-rw-rw-   0 root         (0) root         (0)     3955 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdReqID.hh
--rw-rw-rw-   0 root         (0) root         (0)    17733 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdResponse.cc
--rw-rw-rw-   0 root         (0) root         (0)     5450 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdResponse.hh
--rw-rw-rw-   0 root         (0) root         (0)     7898 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdStats.cc
--rw-rw-rw-   0 root         (0) root         (0)     4653 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdStats.hh
--rw-rw-rw-   0 root         (0) root         (0)     6456 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdTpcMon.cc
--rw-rw-rw-   0 root         (0) root         (0)     4899 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdTpcMon.hh
--rw-rw-rw-   0 root         (0) root         (0)     3605 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdTrace.hh
--rw-rw-rw-   0 root         (0) root         (0)     4806 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdTransPend.cc
--rw-rw-rw-   0 root         (0) root         (0)     3394 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdTransPend.hh
--rw-rw-rw-   0 root         (0) root         (0)     3978 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdTransSend.cc
--rw-rw-rw-   0 root         (0) root         (0)     3662 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdTransSend.hh
--rw-rw-rw-   0 root         (0) root         (0)    27246 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdTransit.cc
--rw-rw-rw-   0 root         (0) root         (0)     9705 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdTransit.hh
--rw-rw-rw-   0 root         (0) root         (0)     2783 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdWVInfo.hh
--rw-rw-rw-   0 root         (0) root         (0)     5092 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdXPath.hh
--rw-rw-rw-   0 root         (0) root         (0)   147048 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdXeq.cc
--rw-rw-rw-   0 root         (0) root         (0)     3317 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdXeq.hh
--rw-rw-rw-   0 root         (0) root         (0)    12437 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdXeqChkPnt.cc
--rw-rw-rw-   0 root         (0) root         (0)    20041 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdXeqFAttr.cc
--rw-rw-rw-   0 root         (0) root         (0)    22344 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXrootd/XrdXrootdXeqPgrw.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/src/XrdZip/
--rw-rw-rw-   0 root         (0) root         (0)    14675 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdZip/XrdZipCDFH.hh
--rw-rw-rw-   0 root         (0) root         (0)     1960 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdZip/XrdZipDataDescriptor.hh
--rw-rw-rw-   0 root         (0) root         (0)     6301 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdZip/XrdZipEOCD.hh
--rw-rw-rw-   0 root         (0) root         (0)     6223 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdZip/XrdZipExtra.hh
--rw-rw-rw-   0 root         (0) root         (0)     7291 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdZip/XrdZipLFH.hh
--rw-rw-rw-   0 root         (0) root         (0)     6734 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdZip/XrdZipUtils.hh
--rw-rw-rw-   0 root         (0) root         (0)     5265 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdZip/XrdZipZIP64EOCD.hh
--rw-rw-rw-   0 root         (0) root         (0)     3227 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdZip/XrdZipZIP64EOCDL.hh
--rw-rw-rw-   0 root         (0) root         (0)     3848 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)     6828 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdApps.cmake
--rw-rw-rw-   0 root         (0) root         (0)     4556 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdCrypto.cmake
--rw-rw-rw-   0 root         (0) root         (0)     2928 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdDaemons.cmake
--rw-rw-rw-   0 root         (0) root         (0)     1913 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFfs.cmake
--rw-rw-rw-   0 root         (0) root         (0)     3214 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdFrm.cmake
--rw-rw-rw-   0 root         (0) root         (0)     4699 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHeaders.cmake
--rw-rw-rw-   0 root         (0) root         (0)     2679 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdHttp.cmake
--rw-rw-rw-   0 root         (0) root         (0)     2084 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdIsal.cmake
--rw-rw-rw-   0 root         (0) root         (0)     1724 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdMacaroons.cmake
--rw-rw-rw-   0 root         (0) root         (0)     1934 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdOssCsi.cmake
--rw-rw-rw-   0 root         (0) root         (0)     3134 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPfc.cmake
--rw-rw-rw-   0 root         (0) root         (0)     5719 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPlugins.cmake
--rw-rw-rw-   0 root         (0) root         (0)     2958 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdPosix.cmake
--rw-rw-rw-   0 root         (0) root         (0)     1349 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSciTokens.cmake
--rw-rw-rw-   0 root         (0) root         (0)     5294 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSec.cmake
--rw-rw-rw-   0 root         (0) root         (0)     3489 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecgsi.cmake
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSeckrb5.cmake
--rw-rw-rw-   0 root         (0) root         (0)      853 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSecztn.cmake
--rw-rw-rw-   0 root         (0) root         (0)    10870 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdServer.cmake
--rw-rw-rw-   0 root         (0) root         (0)     4916 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdSsi.cmake
--rw-rw-rw-   0 root         (0) root         (0)     2328 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdTpc.cmake
--rw-rw-rw-   0 root         (0) root         (0)    14635 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdUtils.cmake
--rw-r--r--   0 root         (0) root         (0)     5171 2023-03-24 08:33:47.000000 xrootd-5.5.4/src/XrdVersion.hh
--rw-rw-rw-   0 root         (0) root         (0)     5174 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdVersion.hh.in
--rw-rw-rw-   0 root         (0) root         (0)    15666 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdVersionPlugin.hh
--rw-rw-rw-   0 root         (0) root         (0)     1877 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdVoms.cmake
--rw-rw-rw-   0 root         (0) root         (0)     2222 2023-03-24 08:33:03.000000 xrootd-5.5.4/src/XrdXml.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/tests/XrdCephTests/
--rw-rw-rw-   0 root         (0) root         (0)      556 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdCephTests/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)     6661 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdCephTests/CephParsingTest.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/tests/XrdClHttp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/tests/XrdClHttp/cases/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/tests/XrdClHttp/cases/000-simple-download/
--rw-rw-rw-   0 root         (0) root         (0)      960 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClHttp/cases/000-simple-download/main.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/tests/XrdClHttp/cases/001-deep-path-download/
--rw-rw-rw-   0 root         (0) root         (0)     1044 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClHttp/cases/001-deep-path-download/main.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/tests/XrdClHttp/cases/002-simple-upload/
--rw-rw-rw-   0 root         (0) root         (0)     1028 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClHttp/cases/002-simple-upload/main.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/tests/XrdClHttp/cases/003-deep-path-upload/
--rw-rw-rw-   0 root         (0) root         (0)     1157 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClHttp/cases/003-deep-path-upload/main.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/tests/XrdClHttp/config/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/tests/XrdClHttp/config/client/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClHttp/config/client/http.conf
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClHttp/config/caddyfile
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClHttp/config/caddyfile-webdav
--rw-rw-rw-   0 root         (0) root         (0)     1919 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClHttp/common.sh
--rwxrwxrwx   0 root         (0) root         (0)     1571 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClHttp/run_test.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/tests/XrdClTests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/tests/XrdClTests/tls/
--rw-rw-rw-   0 root         (0) root         (0)      561 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/tls/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/tls/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1861 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/tls/xrdcl-tls.cc
--rw-rw-rw-   0 root         (0) root         (0)    16273 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/tls/xrdsrv-tls.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/tests/XrdClTests/wrt/
--rw-rw-rw-   0 root         (0) root         (0)    14962 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/wrt/xrdsrv-dio.cc
--rw-rw-rw-   0 root         (0) root         (0)    14168 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/wrt/xrdsrv-wrt.cc
--rw-rw-rw-   0 root         (0) root         (0)     1082 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)    27179 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/FileCopyTest.cc
--rw-rw-rw-   0 root         (0) root         (0)    22807 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/FileSystemTest.cc
--rw-rw-rw-   0 root         (0) root         (0)    30512 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/FileTest.cc
--rw-rw-rw-   0 root         (0) root         (0)    21399 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/IdentityPlugIn.cc
--rw-rw-rw-   0 root         (0) root         (0)     2516 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/IdentityPlugIn.hh
--rw-rw-rw-   0 root         (0) root         (0)    22565 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/LocalFileHandlerTest.cc
--rw-rw-rw-   0 root         (0) root         (0)     9085 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/MonitorTestLib.cc
--rw-rw-rw-   0 root         (0) root         (0)    36161 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/OperationsWorkflowTest.cc
--rw-rw-rw-   0 root         (0) root         (0)    10184 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/PollerTest.cc
--rw-rw-rw-   0 root         (0) root         (0)    20524 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/PostMasterTest.cc
--rw-rw-rw-   0 root         (0) root         (0)    11141 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/SocketTest.cc
--rw-rw-rw-   0 root         (0) root         (0)    12152 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/ThreadingTest.cc
--rw-rw-rw-   0 root         (0) root         (0)    17858 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/UtilsTest.cc
--rw-rw-rw-   0 root         (0) root         (0)     4848 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/XRootDProtocolHelper.cc
--rw-rw-rw-   0 root         (0) root         (0)     1982 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/XRootDProtocolHelper.hh
--rw-rw-rw-   0 root         (0) root         (0)      419 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/cppunit.supp
--rwxrwxrwx   0 root         (0) root         (0)      430 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdClTests/printenv.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/tests/XrdEcTests/
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdEcTests/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)    19453 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdEcTests/MicroTest.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/tests/XrdSsiTests/
--rw-rw-rw-   0 root         (0) root         (0)      435 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdSsiTests/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)    36471 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/XrdSsiTests/XrdShMap.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/tests/common/
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/common/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)     2483 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/common/CppUnitXrdHelpers.hh
--rw-rw-rw-   0 root         (0) root         (0)     3148 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/common/PathProcessor.hh
--rw-rw-rw-   0 root         (0) root         (0)    12734 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/common/Server.cc
--rw-rw-rw-   0 root         (0) root         (0)     7796 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/common/Server.hh
--rw-rw-rw-   0 root         (0) root         (0)     4264 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/common/TestEnv.cc
--rw-rw-rw-   0 root         (0) root         (0)     2456 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/common/TestEnv.hh
--rw-rw-rw-   0 root         (0) root         (0)     5571 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/common/TextRunner.cc
--rw-rw-rw-   0 root         (0) root         (0)     3461 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/common/Utils.cc
--rw-rw-rw-   0 root         (0) root         (0)     4485 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/common/Utils.hh
--rw-rw-rw-   0 root         (0) root         (0)      212 2023-03-24 08:33:03.000000 xrootd-5.5.4/tests/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/ups/
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-03-24 08:33:03.000000 xrootd-5.5.4/ups/eupspkg.cfg.sh
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-03-24 08:33:03.000000 xrootd-5.5.4/ups/xrootd.table
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/utils/
--rwxrwxrwx   0 root         (0) root         (0)     6678 2023-03-24 08:33:03.000000 xrootd-5.5.4/utils/XrdCmsNotify.pm
--rwxrwxrwx   0 root         (0) root         (0)     7851 2023-03-24 08:33:03.000000 xrootd-5.5.4/utils/XrdOlbMonPerf
--rwxrwxrwx   0 root         (0) root         (0)     3789 2023-03-24 08:33:03.000000 xrootd-5.5.4/utils/cms_monPerf
--rwxrwxrwx   0 root         (0) root         (0)    29321 2023-03-24 08:33:03.000000 xrootd-5.5.4/utils/hpsscp
--rwxrwxrwx   0 root         (0) root         (0)     4187 2023-03-24 08:33:03.000000 xrootd-5.5.4/utils/netchk
--rwxrwxrwx   0 root         (0) root         (0)     2181 2023-03-24 08:33:03.000000 xrootd-5.5.4/utils/xrootd-config
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 08:34:00.000000 xrootd-5.5.4/xrootd.egg-info/
--rw-r--r--   0 root         (0) root         (0)      347 2023-03-24 08:34:00.000000 xrootd-5.5.4/xrootd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    46123 2023-03-24 08:34:00.000000 xrootd-5.5.4/xrootd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 08:34:00.000000 xrootd-5.5.4/xrootd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 08:34:00.000000 xrootd-5.5.4/xrootd.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     3695 2023-03-24 08:33:03.000000 xrootd-5.5.4/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)    35147 2023-03-24 08:33:03.000000 xrootd-5.5.4/COPYING
--rw-rw-rw-   0 root         (0) root         (0)     2811 2023-03-24 08:33:03.000000 xrootd-5.5.4/COPYING.BSD
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-03-24 08:33:03.000000 xrootd-5.5.4/COPYING.LGPL
--rw-rw-rw-   0 root         (0) root         (0)     1432 2023-03-24 08:33:03.000000 xrootd-5.5.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      294 2023-03-24 08:33:47.000000 xrootd-5.5.4/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     3287 2023-03-24 08:33:03.000000 xrootd-5.5.4/README
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-03-24 08:33:03.000000 xrootd-5.5.4/VERSION_INFO
--rw-rw-rw-   0 root         (0) root         (0)      941 2023-03-24 08:33:03.000000 xrootd-5.5.4/cmake_uninstall.cmake.in
--rwxrwxrwx   0 root         (0) root         (0)      991 2023-03-24 08:33:03.000000 xrootd-5.5.4/gen-tarball.sh
--rwxrwxrwx   0 root         (0) root         (0)     8485 2023-03-24 08:33:03.000000 xrootd-5.5.4/genversion.sh
--rwxr-xr-x   0 root         (0) root         (0)      201 2023-03-24 08:33:47.000000 xrootd-5.5.4/has_c++14.sh
--rwxr-xr-x   0 root         (0) root         (0)     1407 2023-03-24 08:33:47.000000 xrootd-5.5.4/install.sh
--rwxr-xr-x   0 root         (0) root         (0)     1240 2023-03-24 08:33:47.000000 xrootd-5.5.4/publish.sh
--rw-r--r--   0 root         (0) root         (0)     7310 2023-03-24 08:33:47.000000 xrootd-5.5.4/setup.py
--rw-r--r--   0 root         (0) root         (0)      347 2023-03-24 08:34:00.000000 xrootd-5.5.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-24 08:34:00.000000 xrootd-5.5.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/bindings/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/bindings/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/bindings/python/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/bindings/python/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/bindings/python/docs/source/.static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/bindings/python/docs/source/.static/css/
+-rwxrwxrwx   0 root         (0) root         (0)    15713 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/source/.static/css/custom.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/bindings/python/docs/source/.templates/
+-rwxrwxrwx   0 root         (0) root         (0)       89 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/source/.templates/layout.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/bindings/python/docs/source/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/source/examples/copyprocess.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2842 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/source/examples/file.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3243 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/source/examples/filesystem.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/bindings/python/docs/source/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/bindings/python/docs/source/modules/client/
+-rw-rw-rw-   0 root         (0) root         (0)      423 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/source/modules/client/copyprocess.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/source/modules/client/file.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/source/modules/client/filesystem.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5238 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/source/modules/client/flags.rst
+-rw-rw-rw-   0 root         (0) root         (0)      944 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/source/modules/client/responses.rst
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/source/modules/client/url.rst
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/source/modules/client/utils.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8013 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/source/examples.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4286 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/source/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     3673 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/source/gettingstarted.rst
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/source/install.rst
+-rw-rw-rw-   0 root         (0) root         (0)    14979 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/source/xrootd-200x68.png
+-rw-rw-rw-   0 root         (0) root         (0)     5581 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/docs/ReleaseNotes.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/bindings/python/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/copy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1655 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/copyprocess.py
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/dirlist.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/fcntl.py
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/fcntl_async.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/fileproperties.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/filesystemproperties.py
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/iterate.py
+-rw-rw-rw-   0 root         (0) root         (0)      388 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/locate.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/mkdir.py
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/mv.py
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/query.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/read.py
+-rw-rw-rw-   0 root         (0) root         (0)      349 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/readchunks.py
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/readlines.py
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/rm.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/rmdir.py
+-rw-rw-rw-   0 root         (0) root         (0)      850 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/vector_read.py
+-rw-rw-rw-   0 root         (0) root         (0)      226 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/visa.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/visa_async.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/examples/write.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/bindings/python/libs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/bindings/python/libs/client/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/libs/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1313 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/libs/client/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     7054 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/libs/client/copyprocess.py
+-rw-rw-rw-   0 root         (0) root         (0)     2426 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/libs/client/env.py
+-rw-rw-rw-   0 root         (0) root         (0)    13367 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/libs/client/file.py
+-rw-rw-rw-   0 root         (0) root         (0)    17398 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/libs/client/filesystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/libs/client/finalize.py
+-rw-rw-rw-   0 root         (0) root         (0)     2892 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/libs/client/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)     4357 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/libs/client/glob_funcs.py
+-rw-rw-rw-   0 root         (0) root         (0)    11449 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/libs/client/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)     2842 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/libs/client/url.py
+-rw-rw-rw-   0 root         (0) root         (0)     3926 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/libs/client/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 08:45:39.000000 xrootd-5.5.5/bindings/python/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/bindings/python/src/
+-rw-rw-rw-   0 root         (0) root         (0)    12167 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/src/AsyncResponseHandler.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6731 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/src/ChunkIterator.hh
+-rw-rw-rw-   0 root         (0) root         (0)    13695 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/src/Conversions.hh
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/src/PyXRootD.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8623 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/src/PyXRootDCopyProcess.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6663 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/src/PyXRootDCopyProcess.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4415 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/src/PyXRootDCopyProgressHandler.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3562 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/src/PyXRootDCopyProgressHandler.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5119 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/src/PyXRootDEnv.hh
+-rw-rw-rw-   0 root         (0) root         (0)    35727 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/src/PyXRootDFile.cc
+-rw-rw-rw-   0 root         (0) root         (0)    12231 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/src/PyXRootDFile.hh
+-rw-rw-rw-   0 root         (0) root         (0)    37416 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/src/PyXRootDFileSystem.cc
+-rw-rw-rw-   0 root         (0) root         (0)    10740 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/src/PyXRootDFileSystem.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2135 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/src/PyXRootDFinalize.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5199 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/src/PyXRootDModule.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7612 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/src/PyXRootDURL.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8015 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/src/PyXRootDURL.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6144 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/src/Utils.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/src/Utils.hh
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 08:45:39.000000 xrootd-5.5.5/bindings/python/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/bindings/python/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/tests/env.py
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/tests/test_copy.py
+-rw-rw-rw-   0 root         (0) root         (0)    11797 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/tests/test_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     5387 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/tests/test_filesystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1728 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/tests/test_glob.py
+-rw-rw-rw-   0 root         (0) root         (0)      785 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/tests/test_threads.py
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/tests/test_url.py
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/.gitattributes
+-rwxrwxrwx   0 root         (0) root         (0)       70 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     4286 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      688 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/README.rst
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-08 08:46:33.000000 xrootd-5.5.5/bindings/python/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)     4611 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/python/setup.py.in
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-08 08:45:38.000000 xrootd-5.5.5/bindings/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/cmake/
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/FindAutoConf.cmake
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/FindAutoMake.cmake
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/FindCppUnit.cmake
+-rw-rw-rw-   0 root         (0) root         (0)      407 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/FindDavix.cmake
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/FindKerberos5.cmake
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/FindLibTool.cmake
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/FindMacaroons.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     1699 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/FindReadline.cmake
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/FindSciTokensCpp.cmake
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/FindTinyXml.cmake
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/FindVOMS.cmake
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/FindYasm.cmake
+-rw-rw-rw-   0 root         (0) root         (0)      740 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/Findfuse.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/Findlibuuid.cmake
+-rw-rw-rw-   0 root         (0) root         (0)      683 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/Findsystemd.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     7023 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/GNUInstallDirs.cmake
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/XRootDCommon.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     7570 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/XRootDConfig.cmake.in
+-rw-rw-rw-   0 root         (0) root         (0)     2561 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/XRootDDefaults.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     4939 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/XRootDFindLibs.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     6893 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/XRootDOSDefs.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     2473 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/XRootDSummary.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     6716 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/XRootDSystemCheck.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     2565 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake/XRootDUtils.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/docs/man/
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/man/cmsd.8
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/man/frm_admin.8
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/man/frm_purged.8
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/man/frm_xfragent.8
+-rw-rw-rw-   0 root         (0) root         (0)     1016 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/man/frm_xfrd.8
+-rw-rw-rw-   0 root         (0) root         (0)     4438 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/man/libXrdVoms.1
+-rw-rw-rw-   0 root         (0) root         (0)     1046 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/man/mpxstats.8
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/man/xrdadler32.1
+-rw-rw-rw-   0 root         (0) root         (0)    17298 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/man/xrdcp.1
+-rw-rw-rw-   0 root         (0) root         (0)     6354 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/man/xrdfs.1
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/man/xrdgsiproxy.1
+-rw-rw-rw-   0 root         (0) root         (0)     6823 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/man/xrdgsitest.1
+-rw-rw-rw-   0 root         (0) root         (0)     1322 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/man/xrdmapc.1
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/man/xrdpfc_print.8
+-rw-rw-rw-   0 root         (0) root         (0)      872 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/man/xrdpwdadmin.8
+-rw-rw-rw-   0 root         (0) root         (0)      850 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/man/xrdsssadmin.8
+-rw-rw-rw-   0 root         (0) root         (0)      993 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/man/xrootd.8
+-rw-rw-rw-   0 root         (0) root         (0)     3745 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/man/xrootdfs.1
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/PreReleaseNotes.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4415 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/README_IPV4_To_IPV6
+-rw-rw-rw-   0 root         (0) root         (0)   170357 2023-05-08 08:45:38.000000 xrootd-5.5.5/docs/ReleaseNotes.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/packaging/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/packaging/common/
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/common/client-plugin.conf.example
+-rw-rw-rw-   0 root         (0) root         (0)     6149 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/common/client.conf
+-rw-rw-rw-   0 root         (0) root         (0)      494 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/common/cmsd@.service
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/common/frm_purged@.service
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/common/frm_xfrd@.service
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/common/http.client.conf.example
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/common/recorder.conf
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/common/xrdhttp@.socket
+-rw-rw-rw-   0 root         (0) root         (0)     3006 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/common/xrootd-clustered.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3342 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/common/xrootd-filecache-clustered.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1666 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/common/xrootd-filecache-standalone.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1986 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/common/xrootd-http.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/common/xrootd-standalone.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/common/xrootd.logrotate
+-rw-rw-rw-   0 root         (0) root         (0)      680 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/common/xrootd.te
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/common/xrootd@.service
+-rw-rw-rw-   0 root         (0) root         (0)      122 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/common/xrootd@.socket
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/packaging/debian/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/packaging/debian/source/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/source/format
+-rw-rw-rw-   0 root         (0) root         (0)        3 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/compat
+-rw-rw-rw-   0 root         (0) root         (0)    16401 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/control
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/copyright
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/libxrdapputils1.install
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/libxrdcl2.install
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/libxrdcrypto1.install
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/libxrdcryptolite1.install
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/libxrdffs2.install
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/libxrdhttputils1.install
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/libxrdposix2.install
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/libxrdserver2.install
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/libxrdssilib1.install
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/libxrdssishmap1.install
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/libxrdutils2.install
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/libxrdxml2.install
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/libxrootd-client-dev.install
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/libxrootd-dev.install
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/libxrootd-private-dev.install
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/libxrootd-server-dev.install
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/python3-xrootd.install
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/python3-xrootd.install.new
+-rwxrwxrwx   0 root         (0) root         (0)      820 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/rules
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 08:45:39.000000 xrootd-5.5.5/packaging/debian/xrootd-client-devel.install
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 08:45:39.000000 xrootd-5.5.5/packaging/debian/xrootd-client-libs.install
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/xrootd-client-plugins.install
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 08:45:39.000000 xrootd-5.5.5/packaging/debian/xrootd-client.install
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/xrootd-clients.install
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 08:45:39.000000 xrootd-5.5.5/packaging/debian/xrootd-devel.install
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/xrootd-fuse.install
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 08:45:39.000000 xrootd-5.5.5/packaging/debian/xrootd-libs.install
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/xrootd-plugins.install
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 08:45:39.000000 xrootd-5.5.5/packaging/debian/xrootd-private-devel.install
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 08:45:39.000000 xrootd-5.5.5/packaging/debian/xrootd-server-devel.install
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 08:45:39.000000 xrootd-5.5.5/packaging/debian/xrootd-server-libs.install
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/xrootd-server-plugins.install
+-rw-rw-rw-   0 root         (0) root         (0)      542 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian/xrootd-server.install
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/packaging/debian_scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     1745 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/debian_scripts/publish_debian_cern.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/packaging/rhel/
+-rw-rw-rw-   0 root         (0) root         (0)      809 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/rhel/cmsd.init
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/rhel/frm_purged.init
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/rhel/frm_xfrd.init
+-rw-rw-rw-   0 root         (0) root         (0)     8866 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/rhel/xrootd.functions
+-rw-rw-rw-   0 root         (0) root         (0)     8451 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/rhel/xrootd.functions-slc4
+-rw-rw-rw-   0 root         (0) root         (0)      861 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/rhel/xrootd.init
+-rw-rw-rw-   0 root         (0) root         (0)    36694 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/rhel/xrootd.spec.in
+-rw-rw-rw-   0 root         (0) root         (0)     3489 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/rhel/xrootd.sysconfig
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/rhel/xrootd.tmpfiles
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/packaging/tgz/
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/tgz/README
+-rwxrwxrwx   0 root         (0) root         (0)     4590 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/tgz/StartCMS
+-rwxrwxrwx   0 root         (0) root         (0)     4388 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/tgz/StartFRM
+-rwxrwxrwx   0 root         (0) root         (0)     5420 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/tgz/StartOLB
+-rw-rw-rw-   0 root         (0) root         (0)     2063 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/tgz/StartOLB.cf.example
+-rwxrwxrwx   0 root         (0) root         (0)     4767 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/tgz/StartXRD
+-rw-rw-rw-   0 root         (0) root         (0)     3842 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/tgz/StartXRD.cf.example
+-rwxrwxrwx   0 root         (0) root         (0)     3039 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/tgz/StopCMS
+-rwxrwxrwx   0 root         (0) root         (0)     3735 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/tgz/StopFRM
+-rwxrwxrwx   0 root         (0) root         (0)     2910 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/tgz/StopOLB
+-rwxrwxrwx   0 root         (0) root         (0)     2615 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/tgz/StopXRD
+-rw-rw-rw-   0 root         (0) root         (0)     1988 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/tgz/xrootd.cf.example
+-rw-rw-rw-   0 root         (0) root         (0)     3914 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/tgz/xrootd.cf.example2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/packaging/wheel/
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/wheel/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     2632 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/wheel/TestCXX14.txt
+-rwxrwxrwx   0 root         (0) root         (0)      201 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/wheel/has_c++14.sh
+-rwxrwxrwx   0 root         (0) root         (0)     1407 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/wheel/install.sh
+-rwxrwxrwx   0 root         (0) root         (0)     1240 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/wheel/publish.sh
+-rw-rw-rw-   0 root         (0) root         (0)     7310 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/wheel/setup.py
+-rwxrwxrwx   0 root         (0) root         (0)    10336 2023-05-08 08:45:38.000000 xrootd-5.5.5/packaging/makesrpm.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/src/XProtocol/
+-rw-rw-rw-   0 root         (0) root         (0)      947 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XProtocol/README
+-rw-rw-rw-   0 root         (0) root         (0)    11295 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XProtocol/XProtocol.cc
+-rw-rw-rw-   0 root         (0) root         (0)    50827 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XProtocol/XProtocol.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5574 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XProtocol/XPtypes.hh
+-rw-rw-rw-   0 root         (0) root         (0)    25337 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XProtocol/YProtocol.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/src/Xrd/
+-rw-rw-rw-   0 root         (0) root         (0)     9005 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdBuffXL.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3279 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdBuffXL.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11819 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdBuffer.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4299 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdBuffer.hh
+-rw-rw-rw-   0 root         (0) root         (0)    91975 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdConfig.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5523 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdConfig.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2900 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdGlobals.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9400 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdInet.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3445 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdInet.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2840 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdInfo.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2489 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdInfo.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3099 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdJob.hh
+-rw-rw-rw-   0 root         (0) root         (0)    25173 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdLink.cc
+-rw-rw-rw-   0 root         (0) root         (0)    26923 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdLink.hh
+-rw-rw-rw-   0 root         (0) root         (0)    14522 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdLinkCtl.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9846 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdLinkCtl.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3499 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdLinkInfo.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5054 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdLinkMatch.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3288 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdLinkMatch.hh
+-rw-rw-rw-   0 root         (0) root         (0)    46764 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdLinkXeq.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7101 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdLinkXeq.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8748 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdMain.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5456 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdObject.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4407 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdObject.icc
+-rw-rw-rw-   0 root         (0) root         (0)    12682 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdPoll.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5648 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdPoll.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3601 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdPollE.hh
+-rw-rw-rw-   0 root         (0) root         (0)    14457 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdPollE.icc
+-rw-rw-rw-   0 root         (0) root         (0)     3308 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdPollInfo.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3207 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdPollPoll.hh
+-rw-rw-rw-   0 root         (0) root         (0)    17863 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdPollPoll.icc
+-rw-rw-rw-   0 root         (0) root         (0)    12456 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdProtLoad.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3854 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdProtLoad.hh
+-rw-rw-rw-   0 root         (0) root         (0)    10727 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdProtocol.hh
+-rw-rw-rw-   0 root         (0) root         (0)    24210 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdScheduler.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5635 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdScheduler.hh
+-rw-rw-rw-   0 root         (0) root         (0)    13605 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdSendQ.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3735 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdSendQ.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12208 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdStats.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3836 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdStats.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4914 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdTcpMonPin.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3291 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/Xrd/XrdTrace.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/src/XrdAcc/
+-rw-rw-rw-   0 root         (0) root         (0)    18177 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdAcc/XrdAccAccess.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8058 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdAcc/XrdAccAccess.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4734 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdAcc/XrdAccAudit.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5263 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdAcc/XrdAccAudit.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5258 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdAcc/XrdAccAuthDB.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12972 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdAcc/XrdAccAuthFile.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3587 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdAcc/XrdAccAuthFile.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12043 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdAcc/XrdAccAuthorize.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7602 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdAcc/XrdAccCapability.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5914 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdAcc/XrdAccCapability.hh
+-rw-rw-rw-   0 root         (0) root         (0)    34347 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdAcc/XrdAccConfig.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5754 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdAcc/XrdAccConfig.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8327 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdAcc/XrdAccEntity.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5422 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdAcc/XrdAccEntity.hh
+-rw-rw-rw-   0 root         (0) root         (0)    15372 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdAcc/XrdAccGroups.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7392 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdAcc/XrdAccGroups.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4791 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdAcc/XrdAccPrivs.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/src/XrdApps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/src/XrdApps/XrdClProxyPlugin/
+-rw-rw-rw-   0 root         (0) root         (0)     7035 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdClProxyPlugin/ProxyPrefixFile.cc
+-rw-rw-rw-   0 root         (0) root         (0)    12371 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdClProxyPlugin/ProxyPrefixFile.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4214 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdClProxyPlugin/ProxyPrefixPlugin.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2721 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdClProxyPlugin/ProxyPrefixPlugin.hh
+-rw-rw-rw-   0 root         (0) root         (0)     1822 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdClProxyPlugin/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/src/XrdApps/XrdClRecordPlugin/
+-rw-rw-rw-   0 root         (0) root         (0)    14346 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdClRecordPlugin/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    13235 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdClRecordPlugin/XrdClAction.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9856 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdClRecordPlugin/XrdClActionMetrics.hh
+-rw-rw-rw-   0 root         (0) root         (0)    18873 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdClRecordPlugin/XrdClRecorder.hh
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdClRecordPlugin/XrdClRecorderPlugin.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3178 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdClRecordPlugin/XrdClRecorderPlugin.hh
+-rw-rw-rw-   0 root         (0) root         (0)    53534 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdClRecordPlugin/XrdClReplay.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7563 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdClRecordPlugin/XrdClReplayArgs.hh
+-rw-rw-rw-   0 root         (0) root         (0)    14497 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdAccTest.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7192 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdAppsCconfig.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6428 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdCks.cc
+-rw-rw-rw-   0 root         (0) root         (0)    40600 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdCpConfig.cc
+-rw-rw-rw-   0 root         (0) root         (0)    13017 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdCpConfig.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7118 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdCpFile.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3726 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdCpFile.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6172 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdCrc32c.cc
+-rw-rw-rw-   0 root         (0) root         (0)    19828 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdMapCluster.cc
+-rw-rw-rw-   0 root         (0) root         (0)    10453 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdMpxStats.cc
+-rw-rw-rw-   0 root         (0) root         (0)    15755 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdMpxXml.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3279 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdMpxXml.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5291 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdPinls.cc
+-rw-rw-rw-   0 root         (0) root         (0)    10301 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdPrep.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8375 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdQStats.cc
+-rw-rw-rw-   0 root         (0) root         (0)    10351 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/XrdWait41.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9299 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps/Xrdadler32.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/src/XrdBwm/
+-rw-rw-rw-   0 root         (0) root         (0)    38144 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdBwm/XrdBwm.cc
+-rw-rw-rw-   0 root         (0) root         (0)    12819 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdBwm/XrdBwm.hh
+-rw-rw-rw-   0 root         (0) root         (0)    15615 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdBwm/XrdBwmConfig.cc
+-rw-rw-rw-   0 root         (0) root         (0)    14111 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdBwm/XrdBwmHandle.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4374 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdBwm/XrdBwmHandle.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11034 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdBwm/XrdBwmLogger.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3761 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdBwm/XrdBwmLogger.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8624 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdBwm/XrdBwmPolicy.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6036 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdBwm/XrdBwmPolicy1.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4429 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdBwm/XrdBwmPolicy1.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3388 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdBwm/XrdBwmTrace.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/src/XrdCks/
+-rw-rw-rw-   0 root         (0) root         (0)    16444 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCks.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7765 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksAssist.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6718 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksAssist.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8525 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksCalc.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5687 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksCalcadler32.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8639 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksCalccrc32.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3654 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksCalccrc32.hh
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksCalccrc32C.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2986 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksCalccrc32C.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12260 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksCalcmd5.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3564 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksCalcmd5.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5036 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksCalczcrc32.cc
+-rw-rw-rw-   0 root         (0) root         (0)    10222 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksConfig.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3663 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksConfig.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5671 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksData.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7928 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksLoader.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6105 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksLoader.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9341 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksManOss.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3480 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksManOss.hh
+-rw-rw-rw-   0 root         (0) root         (0)    21161 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksManager.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5041 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksManager.hh
+-rw-rw-rw-   0 root         (0) root         (0)    14952 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksWrapper.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4283 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCks/XrdCksXAttr.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/src/XrdCl/
+-rw-rw-rw-   0 root         (0) root         (0)     8580 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5609 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClAnyObject.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3364 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClApply.hh
+-rw-rw-rw-   0 root         (0) root         (0)    13157 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClArg.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3439 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClAsyncDiscardReader.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7661 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClAsyncHSReader.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5998 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClAsyncHSWriter.hh
+-rw-rw-rw-   0 root         (0) root         (0)    17225 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClAsyncMsgReader.hh
+-rw-rw-rw-   0 root         (0) root         (0)    10892 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClAsyncMsgWriter.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12785 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClAsyncPageReader.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8622 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClAsyncRawReader.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7097 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClAsyncRawReaderIntfc.hh
+-rw-rw-rw-   0 root         (0) root         (0)    35077 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClAsyncSocketHandler.cc
+-rw-rw-rw-   0 root         (0) root         (0)    13692 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClAsyncSocketHandler.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11781 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClAsyncVectorReader.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9115 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClBuffer.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8723 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClChannel.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7235 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClChannel.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2701 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClChannelHandlerList.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2547 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClChannelHandlerList.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5702 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClCheckSumHelper.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5843 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClCheckSumManager.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClCheckSumManager.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8890 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClCheckpointOperation.hh
+-rw-rw-rw-   0 root         (0) root         (0)   109531 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClClassicCopyJob.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClClassicCopyJob.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9839 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClConstants.hh
+-rw-rw-rw-   0 root         (0) root         (0)    33054 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClCopy.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4256 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClCopyJob.hh
+-rw-rw-rw-   0 root         (0) root         (0)    21403 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClCopyProcess.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9463 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClCopyProcess.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4723 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClCtx.hh
+-rw-rw-rw-   0 root         (0) root         (0)    34739 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClDefaultEnv.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8248 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClDefaultEnv.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2452 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClDlgEnv.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7058 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClEcHandler.cc
+-rw-rw-rw-   0 root         (0) root         (0)    17872 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClEcHandler.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8264 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClEnv.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7930 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClEnv.hh
+-rw-rw-rw-   0 root         (0) root         (0)    75852 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClFS.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3598 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClFSExecutor.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4052 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClFSExecutor.hh
+-rw-rw-rw-   0 root         (0) root         (0)    35374 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClFile.cc
+-rw-rw-rw-   0 root         (0) root         (0)    43555 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClFile.hh
+-rw-rw-rw-   0 root         (0) root         (0)    61991 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClFileOperations.hh
+-rw-rw-rw-   0 root         (0) root         (0)   134550 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClFileStateHandler.cc
+-rw-rw-rw-   0 root         (0) root         (0)    49325 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClFileStateHandler.hh
+-rw-rw-rw-   0 root         (0) root         (0)    81086 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClFileSystem.cc
+-rw-rw-rw-   0 root         (0) root         (0)    44722 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClFileSystem.hh
+-rw-rw-rw-   0 root         (0) root         (0)    58105 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClFileSystemOperations.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7347 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClFileSystemUtils.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3917 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClFileSystemUtils.hh
+-rw-rw-rw-   0 root         (0) root         (0)     1775 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClFileTimer.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3561 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClFileTimer.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2754 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClFinalOperation.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4753 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClForkHandler.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4421 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClForkHandler.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9899 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClFwd.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6373 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClInQueue.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4732 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClInQueue.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5126 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClJobManager.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4860 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClJobManager.hh
+-rw-rw-rw-   0 root         (0) root         (0)    36455 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClLocalFileHandler.cc
+-rw-rw-rw-   0 root         (0) root         (0)    17612 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClLocalFileHandler.hh
+-rw-rw-rw-   0 root         (0) root         (0)     1604 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClLocalFileTask.cc
+-rw-rw-rw-   0 root         (0) root         (0)     1608 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClLocalFileTask.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9775 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClLog.cc
+-rw-rw-rw-   0 root         (0) root         (0)    10484 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClLog.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5392 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClMessage.hh
+-rw-rw-rw-   0 root         (0) root         (0)    20035 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClMessageUtils.cc
+-rw-rw-rw-   0 root         (0) root         (0)    12633 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClMessageUtils.hh
+-rw-rw-rw-   0 root         (0) root         (0)    18515 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClMetalinkRedirector.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8397 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClMetalinkRedirector.hh
+-rw-rw-rw-   0 root         (0) root         (0)    10519 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClMonitor.hh
+-rw-rw-rw-   0 root         (0) root         (0)    29362 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClOperationHandlers.hh
+-rw-rw-rw-   0 root         (0) root         (0)     1066 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClOperationTimeout.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8987 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClOperations.cc
+-rw-rw-rw-   0 root         (0) root         (0)    30811 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClOperations.hh
+-rw-rw-rw-   0 root         (0) root         (0)     1295 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClOptimizers.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6499 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClOptional.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5396 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClOutQueue.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6707 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClOutQueue.hh
+-rw-rw-rw-   0 root         (0) root         (0)    22041 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClParallelOperation.hh
+-rw-rw-rw-   0 root         (0) root         (0)    26771 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClPlugInInterface.hh
+-rw-rw-rw-   0 root         (0) root         (0)    18005 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClPlugInManager.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7482 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClPlugInManager.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7217 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClPoller.hh
+-rw-rw-rw-   0 root         (0) root         (0)    20602 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClPollerBuiltIn.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7251 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClPollerBuiltIn.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3701 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClPollerFactory.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2014 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClPollerFactory.hh
+-rw-rw-rw-   0 root         (0) root         (0)    17515 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClPostMaster.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9638 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClPostMaster.hh
+-rw-rw-rw-   0 root         (0) root         (0)    23531 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClPostMasterInterfaces.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11305 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClPropertyList.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4552 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClRedirectorRegistry.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8258 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClRedirectorRegistry.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4186 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClRequestSync.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2659 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClResponseJob.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7016 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClSIDManager.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8209 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClSIDManager.hh
+-rw-rw-rw-   0 root         (0) root         (0)    30690 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClSocket.cc
+-rw-rw-rw-   0 root         (0) root         (0)    15672 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClSocket.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5694 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClStatus.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7140 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClStatus.hh
+-rw-rw-rw-   0 root         (0) root         (0)    47978 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClStream.cc
+-rw-rw-rw-   0 root         (0) root         (0)    16875 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClStream.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3611 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClSyncQueue.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3609 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClTPFallBackCopyJob.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2541 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClTPFallBackCopyJob.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8986 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClTaskManager.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6199 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClTaskManager.hh
+-rw-rw-rw-   0 root         (0) root         (0)    34437 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClThirdPartyCopyJob.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3740 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClThirdPartyCopyJob.hh
+-rw-rw-rw-   0 root         (0) root         (0)    15805 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClTls.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6552 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClTls.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3056 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClTransportManager.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2786 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClTransportManager.hh
+-rw-rw-rw-   0 root         (0) root         (0)    17135 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClURL.cc
+-rw-rw-rw-   0 root         (0) root         (0)    11760 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClURL.hh
+-rw-rw-rw-   0 root         (0) root         (0)    32898 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClUtils.cc
+-rw-rw-rw-   0 root         (0) root         (0)    18037 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClUtils.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5297 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClXCpCtx.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8289 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClXCpCtx.hh
+-rw-rw-rw-   0 root         (0) root         (0)    17327 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClXCpSrc.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9459 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClXCpSrc.hh
+-rw-rw-rw-   0 root         (0) root         (0)    95732 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClXRootDMsgHandler.cc
+-rw-rw-rw-   0 root         (0) root         (0)    29197 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClXRootDMsgHandler.hh
+-rw-rw-rw-   0 root         (0) root         (0)    26744 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClXRootDResponses.cc
+-rw-rw-rw-   0 root         (0) root         (0)    45771 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClXRootDResponses.hh
+-rw-rw-rw-   0 root         (0) root         (0)   128533 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClXRootDTransport.cc
+-rw-rw-rw-   0 root         (0) root         (0)    21967 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClXRootDTransport.hh
+-rw-rw-rw-   0 root         (0) root         (0)    43178 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClZipArchive.cc
+-rw-rw-rw-   0 root         (0) root         (0)    28344 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClZipArchive.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8602 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClZipCache.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4065 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClZipListHandler.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5224 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClZipListHandler.hh
+-rw-rw-rw-   0 root         (0) root         (0)    27700 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCl/XrdClZipOperations.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/src/XrdClHttp/
+-rw-rw-rw-   0 root         (0) root         (0)      463 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdClHttp/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)    13948 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdClHttp/XrdClHttpFilePlugIn.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5602 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdClHttp/XrdClHttpFilePlugIn.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7554 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdClHttp/XrdClHttpFileSystemPlugIn.cc
+-rw-rw-rw-   0 root         (0) root         (0)     1885 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdClHttp/XrdClHttpFileSystemPlugIn.hh
+-rw-rw-rw-   0 root         (0) root         (0)      692 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdClHttp/XrdClHttpPlugInFactory.cc
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdClHttp/XrdClHttpPlugInFactory.hh
+-rw-rw-rw-   0 root         (0) root         (0)      422 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdClHttp/XrdClHttpPlugInUtil.cc
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdClHttp/XrdClHttpPlugInUtil.hh
+-rw-rw-rw-   0 root         (0) root         (0)    16027 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdClHttp/XrdClHttpPosix.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2617 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdClHttp/XrdClHttpPosix.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/src/XrdCms/
+-rw-rw-rw-   0 root         (0) root         (0)    29034 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsAdmin.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3908 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsAdmin.hh
+-rw-rw-rw-   0 root         (0) root         (0)    15730 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsBaseFS.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8998 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsBaseFS.hh
+-rw-rw-rw-   0 root         (0) root         (0)    19325 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsBlackList.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5380 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsBlackList.hh
+-rw-rw-rw-   0 root         (0) root         (0)    21145 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsCache.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5021 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsCache.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3239 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsClient.cc
+-rw-rw-rw-   0 root         (0) root         (0)    22441 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsClient.hh
+-rw-rw-rw-   0 root         (0) root         (0)    25549 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsClientConfig.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5371 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsClientConfig.hh
+-rw-rw-rw-   0 root         (0) root         (0)    17324 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsClientMan.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5101 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsClientMan.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7117 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsClientMsg.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3740 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsClientMsg.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8243 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsClustID.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3382 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsClustID.hh
+-rw-rw-rw-   0 root         (0) root         (0)    77195 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsCluster.cc
+-rw-rw-rw-   0 root         (0) root         (0)    10458 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsCluster.hh
+-rw-rw-rw-   0 root         (0) root         (0)   109417 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsConfig.cc
+-rw-rw-rw-   0 root         (0) root         (0)    12336 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsConfig.hh
+-rw-rw-rw-   0 root         (0) root         (0)    49369 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsFinder.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6835 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsFinder.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5106 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsJob.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3058 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsJob.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8643 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsKey.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6829 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsKey.hh
+-rw-rw-rw-   0 root         (0) root         (0)    10887 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsLogin.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3223 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsLogin.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8263 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsManList.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3563 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsManList.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9115 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsManTree.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3708 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsManTree.hh
+-rw-rw-rw-   0 root         (0) root         (0)    20171 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsManager.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4549 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsManager.hh
+-rw-rw-rw-   0 root         (0) root         (0)    21971 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsMeter.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4787 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsMeter.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6578 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsNash.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3101 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsNash.hh
+-rw-rw-rw-   0 root         (0) root         (0)    68022 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsNode.cc
+-rw-rw-rw-   0 root         (0) root         (0)    11829 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsNode.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7875 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsPList.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5436 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsPList.hh
+-rw-rw-rw-   0 root         (0) root         (0)    18983 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsParser.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4888 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsParser.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7886 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsPerfMon.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6042 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsPrepArgs.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3669 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsPrepArgs.hh
+-rw-rw-rw-   0 root         (0) root         (0)    18512 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsPrepare.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4068 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsPrepare.hh
+-rw-rw-rw-   0 root         (0) root         (0)    46734 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsProtocol.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5039 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsProtocol.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3945 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsRRData.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4633 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsRRData.hh
+-rw-rw-rw-   0 root         (0) root         (0)    17719 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsRRQ.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7590 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsRRQ.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5228 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsRTable.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3076 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsRTable.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9888 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsRedirLocal.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3519 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsRedirLocal.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11036 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsResp.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5382 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsResp.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5917 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsRole.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11602 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsRouting.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4838 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsRouting.hh
+-rw-rw-rw-   0 root         (0) root         (0)    14804 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsSecurity.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3468 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsSecurity.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7463 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsSelect.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11542 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsState.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3997 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsState.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5187 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsSupervisor.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2750 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsSupervisor.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5637 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsTalk.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3034 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsTalk.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3426 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsTrace.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2782 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsTypes.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11723 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsUtils.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6365 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsUtils.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5656 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCms/XrdCmsVnId.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdCrypto/
+-rw-rw-rw-   0 root         (0) root         (0)     4302 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoAux.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5048 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoAux.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7678 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoBasic.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3869 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoBasic.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7405 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoCipher.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4214 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoCipher.hh
+-rw-rw-rw-   0 root         (0) root         (0)    17653 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoFactory.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9138 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoFactory.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3500 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoLite.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5355 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoLite.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8734 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoLite_bf32.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4136 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoMsgDigest.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3452 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoMsgDigest.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9058 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoRSA.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4804 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoRSA.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2989 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoTrace.hh
+-rw-rw-rw-   0 root         (0) root         (0)    10639 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoX509.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5644 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoX509.hh
+-rw-rw-rw-   0 root         (0) root         (0)    27263 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoX509Chain.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7661 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoX509Chain.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5674 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoX509Crl.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4052 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoX509Crl.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5256 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoX509Req.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4177 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptoX509Req.hh
+-rw-rw-rw-   0 root         (0) root         (0)    10162 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptogsiX509Chain.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3952 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptogsiX509Chain.hh
+-rw-rw-rw-   0 root         (0) root         (0)    25131 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptosslAux.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7231 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptosslAux.hh
+-rw-rw-rw-   0 root         (0) root         (0)    41488 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptosslCipher.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4573 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptosslCipher.hh
+-rw-rw-rw-   0 root         (0) root         (0)    16817 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptosslFactory.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5208 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptosslFactory.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6084 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptosslMsgDigest.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3376 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptosslMsgDigest.hh
+-rw-rw-rw-   0 root         (0) root         (0)    20903 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptosslRSA.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4241 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptosslRSA.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2896 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptosslTrace.hh
+-rw-rw-rw-   0 root         (0) root         (0)    36214 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptosslX509.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5787 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptosslX509.hh
+-rw-rw-rw-   0 root         (0) root         (0)    20566 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptosslX509Crl.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5006 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptosslX509Crl.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12043 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptosslX509Req.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4113 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptosslX509Req.hh
+-rw-rw-rw-   0 root         (0) root         (0)    49317 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptosslgsiAux.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5668 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptosslgsiAux.hh
+-rw-rw-rw-   0 root         (0) root         (0)    18858 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto/XrdCryptotest.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdDig/
+-rw-rw-rw-   0 root         (0) root         (0)    14689 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdDig/XrdDigAuth.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4337 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdDig/XrdDigAuth.hh
+-rw-rw-rw-   0 root         (0) root         (0)    21474 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdDig/XrdDigConfig.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3831 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdDig/XrdDigConfig.hh
+-rw-rw-rw-   0 root         (0) root         (0)    28757 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdDig/XrdDigFS.cc
+-rw-rw-rw-   0 root         (0) root         (0)    11645 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdDig/XrdDigFS.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdEc/
+-rw-rw-rw-   0 root         (0) root         (0)     1708 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdEc/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2020 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdEc/README
+-rw-rw-rw-   0 root         (0) root         (0)     3708 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdEc/XrdEcConfig.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3424 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdEc/XrdEcObjCfg.hh
+-rw-rw-rw-   0 root         (0) root         (0)    47577 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdEc/XrdEcReader.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8804 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdEc/XrdEcReader.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9785 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdEc/XrdEcRedundancyProvider.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5127 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdEc/XrdEcRedundancyProvider.hh
+-rw-rw-rw-   0 root         (0) root         (0)    17345 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdEc/XrdEcStrmWriter.cc
+-rw-rw-rw-   0 root         (0) root         (0)    13309 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdEc/XrdEcStrmWriter.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7256 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdEc/XrdEcThreadPool.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3689 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdEc/XrdEcUtilities.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9976 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdEc/XrdEcUtilities.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12505 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdEc/XrdEcWrtBuff.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdFfs/
+-rw-rw-rw-   0 root         (0) root         (0)     6405 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFfs/README
+-rw-rw-rw-   0 root         (0) root         (0)    10875 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFfs/XrdFfsDent.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2975 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFfs/XrdFfsDent.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5321 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFfs/XrdFfsFsinfo.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFfs/XrdFfsFsinfo.hh
+-rw-rw-rw-   0 root         (0) root         (0)    13902 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFfs/XrdFfsMisc.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3054 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFfs/XrdFfsMisc.hh
+-rw-rw-rw-   0 root         (0) root         (0)    26410 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFfs/XrdFfsPosix.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4855 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFfs/XrdFfsPosix.hh
+-rw-rw-rw-   0 root         (0) root         (0)    10077 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFfs/XrdFfsQueue.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFfs/XrdFfsQueue.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11980 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFfs/XrdFfsWcache.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2664 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFfs/XrdFfsWcache.hh
+-rw-rw-rw-   0 root         (0) root         (0)    48045 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFfs/XrdFfsXrootdfs.cc
+-rwxrwxrwx   0 root         (0) root         (0)     1608 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFfs/xrootdfs.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdFrc/
+-rw-rw-rw-   0 root         (0) root         (0)    11084 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrc/XrdFrcCID.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3950 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrc/XrdFrcCID.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11618 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrc/XrdFrcProxy.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3742 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrc/XrdFrcProxy.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8742 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrc/XrdFrcReqAgent.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3073 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrc/XrdFrcReqAgent.hh
+-rw-rw-rw-   0 root         (0) root         (0)    21187 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrc/XrdFrcReqFile.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4017 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrc/XrdFrcReqFile.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4547 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrc/XrdFrcRequest.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2728 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrc/XrdFrcTrace.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3396 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrc/XrdFrcTrace.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11378 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrc/XrdFrcUtils.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3289 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrc/XrdFrcUtils.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8162 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrc/XrdFrcXAttr.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2863 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrc/XrdFrcXLock.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdFrm/
+-rw-rw-rw-   0 root         (0) root         (0)    36149 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmAdmin.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7410 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmAdmin.hh
+-rw-rw-rw-   0 root         (0) root         (0)    24369 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmAdminAudit.cc
+-rw-rw-rw-   0 root         (0) root         (0)    13623 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmAdminFiles.cc
+-rw-rw-rw-   0 root         (0) root         (0)    11144 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmAdminFind.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6815 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmAdminMain.cc
+-rw-rw-rw-   0 root         (0) root         (0)    10240 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmAdminQuery.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9903 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmAdminReloc.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9421 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmAdminUnlink.cc
+-rw-rw-rw-   0 root         (0) root         (0)    10117 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmCns.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3675 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmCns.hh
+-rw-rw-rw-   0 root         (0) root         (0)    71607 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmConfig.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8419 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmConfig.hh
+-rw-rw-rw-   0 root         (0) root         (0)    17426 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmFiles.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6386 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmFiles.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11087 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmMigrate.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3078 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmMigrate.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11518 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmMonitor.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3912 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmMonitor.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9482 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmPurgMain.cc
+-rw-rw-rw-   0 root         (0) root         (0)    32604 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmPurge.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5353 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmPurge.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7763 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmReqBoss.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3059 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmReqBoss.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7011 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmTSort.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3315 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmTSort.hh
+-rw-rw-rw-   0 root         (0) root         (0)    30228 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmTransfer.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3349 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmTransfer.hh
+-rw-rw-rw-   0 root         (0) root         (0)    10404 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmXfrAgent.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3098 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmXfrAgent.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7971 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmXfrDaemon.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2782 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmXfrDaemon.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2832 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmXfrJob.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6343 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmXfrMain.cc
+-rw-rw-rw-   0 root         (0) root         (0)    17722 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmXfrQueue.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4118 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm/XrdFrmXfrQueue.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdHttp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdHttp/static/
+-rw-rw-rw-   0 root         (0) root         (0)     1400 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/static/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     1274 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/static/xrdhttp.css
+-rw-rw-rw-   0 root         (0) root         (0)     7951 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/static/xrdhttp_css.h
+-rw-rw-rw-   0 root         (0) root         (0)     8705 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/static/xrdhttp_favicon_ico.h
+-rw-rw-rw-   0 root         (0) root         (0)     1909 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/XrdHttpChecksum.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2097 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/XrdHttpChecksum.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5702 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/XrdHttpChecksumHandler.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5188 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/XrdHttpChecksumHandler.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3718 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/XrdHttpExtHandler.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6073 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/XrdHttpExtHandler.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/XrdHttpModule.cc
+-rw-rw-rw-   0 root         (0) root         (0)    86158 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/XrdHttpProtocol.cc
+-rw-rw-rw-   0 root         (0) root         (0)    13770 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/XrdHttpProtocol.hh
+-rw-rw-rw-   0 root         (0) root         (0)    84937 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/XrdHttpReq.cc
+-rw-rw-rw-   0 root         (0) root         (0)    14229 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/XrdHttpReq.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4252 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/XrdHttpSecXtractor.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8841 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/XrdHttpSecurity.cc
+-rw-rw-rw-   0 root         (0) root         (0)     1661 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/XrdHttpStatic.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2175 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/XrdHttpTrace.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9413 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/XrdHttpUtils.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/XrdHttpUtils.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2784 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/xrootd-http-rdr.cf
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp/xrootd-http.cf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdMacaroons/
+-rw-rw-rw-   0 root         (0) root         (0)     2798 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdMacaroons/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     4922 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdMacaroons/XrdMacaroons.cc
+-rw-rw-rw-   0 root         (0) root         (0)    18196 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdMacaroons/XrdMacaroonsAuthz.cc
+-rw-rw-rw-   0 root         (0) root         (0)     1789 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdMacaroons/XrdMacaroonsAuthz.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6883 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdMacaroons/XrdMacaroonsConfigure.cc
+-rw-rw-rw-   0 root         (0) root         (0)    21521 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdMacaroons/XrdMacaroonsHandler.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2784 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdMacaroons/XrdMacaroonsHandler.hh
+-rw-rw-rw-   0 root         (0) root         (0)      122 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdMacaroons/export-lib-symbols
+-rwxrwxrwx   0 root         (0) root         (0)     5269 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdMacaroons/macaroon-init
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdNet/
+-rw-rw-rw-   0 root         (0) root         (0)    17923 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNet.cc
+-rw-rw-rw-   0 root         (0) root         (0)    14669 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNet.hh
+-rw-rw-rw-   0 root         (0) root         (0)    21048 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetAddr.cc
+-rw-rw-rw-   0 root         (0) root         (0)    15050 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetAddr.hh
+-rw-rw-rw-   0 root         (0) root         (0)    17181 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetAddrInfo.cc
+-rw-rw-rw-   0 root         (0) root         (0)    17695 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetAddrInfo.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5823 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetBuffer.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3948 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetBuffer.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8210 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetCache.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5934 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetCache.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5742 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetCmsNotify.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2929 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetCmsNotify.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4246 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetConnect.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3196 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetConnect.hh
+-rw-rw-rw-   0 root         (0) root         (0)    31959 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetIF.cc
+-rw-rw-rw-   0 root         (0) root         (0)    20067 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetIF.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6326 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetIdentity.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2701 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetIdentity.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7246 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetMsg.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7458 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetMsg.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4955 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetOpts.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3294 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetPMark.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3824 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetPMark.hh
+-rw-rw-rw-   0 root         (0) root         (0)    39260 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetPMarkCfg.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3755 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetPMarkCfg.hh
+-rw-rw-rw-   0 root         (0) root         (0)    13957 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetPMarkFF.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3475 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetPMarkFF.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2952 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetPeer.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9640 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetRegistry.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6279 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetRegistry.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9552 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetSecurity.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3339 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetSecurity.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3106 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetSockAddr.hh
+-rw-rw-rw-   0 root         (0) root         (0)    18472 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetSocket.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7647 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetSocket.hh
+-rw-rw-rw-   0 root         (0) root         (0)    31024 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetUtils.cc
+-rw-rw-rw-   0 root         (0) root         (0)    24210 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdNet/XrdNetUtils.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdOfs/
+-rw-rw-rw-   0 root         (0) root         (0)    98478 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfs.cc
+-rw-rw-rw-   0 root         (0) root         (0)    21329 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfs.hh
+-rw-rw-rw-   0 root         (0) root         (0)    19274 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsCPFile.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8379 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsCPFile.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11781 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsChkPnt.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6193 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsChkPnt.hh
+-rw-rw-rw-   0 root         (0) root         (0)    71659 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsConfig.cc
+-rw-rw-rw-   0 root         (0) root         (0)    10806 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsConfigCP.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3117 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsConfigCP.hh
+-rw-rw-rw-   0 root         (0) root         (0)    33128 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsConfigPI.cc
+-rw-rw-rw-   0 root         (0) root         (0)    14532 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsConfigPI.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12955 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsEvr.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4771 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsEvr.hh
+-rw-rw-rw-   0 root         (0) root         (0)    19534 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsEvs.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7231 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsEvs.hh
+-rw-rw-rw-   0 root         (0) root         (0)    16520 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsFAttr.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4073 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsFS.cc
+-rw-rw-rw-   0 root         (0) root         (0)    12589 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsFSctl.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8921 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsFSctl_PI.hh
+-rw-rw-rw-   0 root         (0) root         (0)    30836 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsHandle.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8197 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsHandle.hh
+-rw-rw-rw-   0 root         (0) root         (0)    13105 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsPoscq.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4134 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsPoscq.hh
+-rw-rw-rw-   0 root         (0) root         (0)    28856 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsPrepGPI.cc
+-rw-rw-rw-   0 root         (0) root         (0)    11518 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsPrepare.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3061 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsSecurity.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3814 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsStats.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3285 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsStats.hh
+-rw-rw-rw-   0 root         (0) root         (0)    23537 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsTPC.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5117 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsTPC.hh
+-rw-rw-rw-   0 root         (0) root         (0)    10359 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsTPCAuth.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3086 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsTPCAuth.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3108 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsTPCConfig.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7573 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsTPCInfo.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5241 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsTPCInfo.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7941 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsTPCJob.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3295 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsTPCJob.hh
+-rw-rw-rw-   0 root         (0) root         (0)    13429 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsTPCProg.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3209 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsTPCProg.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4158 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOfs/XrdOfsTrace.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdOss/
+-rw-rw-rw-   0 root         (0) root         (0)    11649 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOss.cc
+-rw-rw-rw-   0 root         (0) root         (0)    46028 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOss.hh
+-rw-rw-rw-   0 root         (0) root         (0)    18122 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssAio.cc
+-rw-rw-rw-   0 root         (0) root         (0)    45753 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssApi.cc
+-rw-rw-rw-   0 root         (0) root         (0)    17573 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssApi.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8491 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssAt.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7394 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssAt.hh
+-rw-rw-rw-   0 root         (0) root         (0)    31708 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssCache.cc
+-rw-rw-rw-   0 root         (0) root         (0)    11024 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssCache.hh
+-rw-rw-rw-   0 root         (0) root         (0)    73786 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssConfig.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3327 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssConfig.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7753 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssCopy.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2632 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssCopy.hh
+-rw-rw-rw-   0 root         (0) root         (0)    13674 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssCreate.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3641 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssDefaultSS.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4810 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssError.hh
+-rw-rw-rw-   0 root         (0) root         (0)    16583 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssMSS.cc
+-rw-rw-rw-   0 root         (0) root         (0)    11917 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssMio.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3591 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssMio.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssMioFile.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2987 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssOpaque.hh
+-rw-rw-rw-   0 root         (0) root         (0)    13731 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssPath.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3880 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssPath.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8574 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssReloc.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9890 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssRename.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9051 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssSIgpfsT.cc
+-rw-rw-rw-   0 root         (0) root         (0)    19495 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssSpace.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4240 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssSpace.hh
+-rw-rw-rw-   0 root         (0) root         (0)    18820 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssStage.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4090 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssStage.hh
+-rw-rw-rw-   0 root         (0) root         (0)    21165 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssStat.cc
+-rw-rw-rw-   0 root         (0) root         (0)    10195 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssStatInfo.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3186 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssTrace.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8528 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssUnlink.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6673 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssVS.hh
+-rw-rw-rw-   0 root         (0) root         (0)    41503 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOss/XrdOssWrapper.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdOssCsi/
+-rw-rw-rw-   0 root         (0) root         (0)     3167 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    15159 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi/XrdOssCsi.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9618 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi/XrdOssCsi.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7059 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiConfig.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6756 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiConfig.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2527 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiCrcUtils.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4781 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiCrcUtils.hh
+-rw-rw-rw-   0 root         (0) root         (0)    16745 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiFile.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4448 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiFileAio.cc
+-rw-rw-rw-   0 root         (0) root         (0)    11301 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiFileAio.hh
+-rw-rw-rw-   0 root         (0) root         (0)    29563 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiPages.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9019 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiPages.hh
+-rw-rw-rw-   0 root         (0) root         (0)    34154 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiPagesUnaligned.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3049 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiRanges.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6143 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiRanges.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3346 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiTagstore.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8697 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiTagstoreFile.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6957 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiTagstoreFile.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3315 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiTrace.hh
+-rw-rw-rw-   0 root         (0) root         (0)    10382 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi/XrdOssHandler.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdOuc/
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/README.bonjour
+-rw-rw-rw-   0 root         (0) root         (0)     8818 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucArgs.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5805 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucArgs.hh
+-rw-rw-rw-   0 root         (0) root         (0)    17653 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucBackTrace.cc
+-rw-rw-rw-   0 root         (0) root         (0)    10560 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucBackTrace.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9481 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucBuffer.cc
+-rw-rw-rw-   0 root         (0) root         (0)    12583 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucBuffer.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12756 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucCRC.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8087 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucCRC.hh
+-rw-rw-rw-   0 root         (0) root         (0)    17087 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucCRC32C.cc
+-rw-rw-rw-   0 root         (0) root         (0)      735 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucCRC32C.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5325 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucCache.cc
+-rw-rw-rw-   0 root         (0) root         (0)    37675 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucCache.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5220 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucCacheCM.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7071 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucCacheStats.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4673 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucCallBack.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5820 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucCallBack.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3807 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucChain.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5655 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucChkPnt.hh
+-rw-rw-rw-   0 root         (0) root         (0)     1514 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucCompiler.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5019 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucDLlist.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4334 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucERoute.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4301 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucERoute.hh
+-rw-rw-rw-   0 root         (0) root         (0)     1693 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucEnum.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9097 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucEnv.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5341 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucEnv.hh
+-rw-rw-rw-   0 root         (0) root         (0)    23619 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucErrInfo.hh
+-rw-rw-rw-   0 root         (0) root         (0)    10829 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucExport.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5760 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucExport.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9215 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucFileInfo.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9566 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucFileInfo.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11284 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucGMap.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8302 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucGMap.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8116 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucGatherConf.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6689 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucGatherConf.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9301 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucHash.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11511 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucHash.icc
+-rw-rw-rw-   0 root         (0) root         (0)     3214 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucHashVal.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3665 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucIOVec.hh
+-rw-rw-rw-   0 root         (0) root         (0)   978532 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucJson.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2676 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucLock.hh
+-rw-rw-rw-   0 root         (0) root         (0)    10867 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucLogging.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3153 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucLogging.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4695 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucMapP2X.hh
+-rw-rw-rw-   0 root         (0) root         (0)    10179 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucMsubs.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5592 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucMsubs.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4780 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucN2NLoader.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3053 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucN2NLoader.hh
+-rw-rw-rw-   0 root         (0) root         (0)    10498 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucN2No2p.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5458 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucNList.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5100 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucNList.hh
+-rw-rw-rw-   0 root         (0) root         (0)    14506 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucNSWalk.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7383 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucNSWalk.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8596 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucName2Name.cc
+-rw-rw-rw-   0 root         (0) root         (0)    12097 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucName2Name.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6417 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucPList.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12474 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucPgrwUtils.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7990 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucPgrwUtils.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6245 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucPinKing.hh
+-rw-rw-rw-   0 root         (0) root         (0)    10383 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucPinLoader.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9351 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucPinLoader.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3859 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucPinObject.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2488 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucPinPath.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3769 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucPinPath.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3334 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucPreload.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3993 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucPreload.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12229 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucProg.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6185 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucProg.hh
+-rw-rw-rw-   0 root         (0) root         (0)    30926 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucPsx.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6045 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucPsx.hh
+-rw-rw-rw-   0 root         (0) root         (0)    13929 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucPup.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8053 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucPup.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7879 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucRash.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9416 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucRash.icc
+-rw-rw-rw-   0 root         (0) root         (0)     6087 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucReqID.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3008 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucReqID.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3219 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucSFVec.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9442 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucSHA3.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6968 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucSHA3.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6346 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucSid.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6332 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucSid.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2968 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucSiteName.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucSiteName.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3074 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucStats.hh
+-rw-rw-rw-   0 root         (0) root         (0)    47398 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucStream.cc
+-rw-rw-rw-   0 root         (0) root         (0)    11689 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucStream.hh
+-rw-rw-rw-   0 root         (0) root         (0)    35608 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucString.cc
+-rw-rw-rw-   0 root         (0) root         (0)    25266 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucString.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7049 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucSxeq.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3039 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucSxeq.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5248 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucTList.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9887 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucTPC.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3801 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucTPC.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3390 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucTUtils.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7032 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucTable.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5093 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucTokenizer.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3588 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucTokenizer.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3019 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucTrace.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2897 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucTrace.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8152 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucUri.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4397 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucUri.hh
+-rw-rw-rw-   0 root         (0) root         (0)    43429 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucUtils.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5639 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucUtils.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5319 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucVerName.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4226 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucVerName.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7043 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOucXAttr.hh
+-rw-rw-rw-   0 root         (0) root         (0)    15942 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOuca2x.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4130 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOuc/XrdOuca2x.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdPfc/
+-rw-rw-rw-   0 root         (0) root         (0)     7215 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/README
+-rw-rw-rw-   0 root         (0) root         (0)    29263 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfc.cc
+-rw-rw-rw-   0 root         (0) root         (0)    18171 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfc.hh
+-rw-rw-rw-   0 root         (0) root         (0)     1841 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcAllowDecision.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3643 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcBlacklistDecision.cc
+-rw-rw-rw-   0 root         (0) root         (0)    12821 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcCommand.cc
+-rw-rw-rw-   0 root         (0) root         (0)    27729 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcConfiguration.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2444 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcDecision.hh
+-rw-rw-rw-   0 root         (0) root         (0)    46138 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcFile.cc
+-rw-rw-rw-   0 root         (0) root         (0)    14635 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcFile.hh
+-rw-rw-rw-   0 root         (0) root         (0)     1933 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcIO.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2691 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcIO.hh
+-rw-rw-rw-   0 root         (0) root         (0)    10962 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcIOFile.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3636 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcIOFile.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12359 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcIOFileBlock.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2979 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcIOFileBlock.hh
+-rw-rw-rw-   0 root         (0) root         (0)    19051 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcInfo.cc
+-rw-rw-rw-   0 root         (0) root         (0)    18053 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcInfo.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12636 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcPrint.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2934 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcPrint.hh
+-rw-rw-rw-   0 root         (0) root         (0)    32423 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcPurge.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4738 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcStats.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2079 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcTrace.hh
+-rw-rw-rw-   0 root         (0) root         (0)     1380 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc/XrdPfcTypes.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdPosix/
+-rw-rw-rw-   0 root         (0) root         (0)     7201 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/README
+-rw-rw-rw-   0 root         (0) root         (0)    32970 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosix.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4656 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosix.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7780 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixAdmin.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3383 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixAdmin.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5977 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixCache.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6942 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixCache.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2992 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixCallBack.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4732 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixCallBack.hh
+-rw-rw-rw-   0 root         (0) root         (0)    23522 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixConfig.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3483 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixConfig.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5169 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixDir.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4117 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixDir.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8592 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixExtern.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6173 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixExtra.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5480 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixExtra.hh
+-rw-rw-rw-   0 root         (0) root         (0)    26695 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixFile.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8414 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixFile.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7869 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixFileRH.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4377 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixFileRH.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2994 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixInfo.hh
+-rw-rw-rw-   0 root         (0) root         (0)    14923 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixLinkage.cc
+-rw-rw-rw-   0 root         (0) root         (0)    14552 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixLinkage.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8516 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixMap.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3065 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixMap.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3041 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixObjGuard.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11702 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixObject.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4655 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixObject.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3600 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixOsDep.hh
+-rw-rw-rw-   0 root         (0) root         (0)    24302 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixPreload.cc
+-rw-rw-rw-   0 root         (0) root         (0)    19284 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixPreload32.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5301 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixPrepIO.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4774 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixPrepIO.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3366 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixStats.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2880 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixTrace.hh
+-rw-rw-rw-   0 root         (0) root         (0)    53317 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixXrootd.cc
+-rw-rw-rw-   0 root         (0) root         (0)    18316 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixXrootd.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11698 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixXrootdPath.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3595 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix/XrdPosixXrootdPath.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdPss/
+-rw-rw-rw-   0 root         (0) root         (0)    45924 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPss/XrdPss.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9337 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPss/XrdPss.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8543 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPss/XrdPssAio.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5049 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPss/XrdPssAioCB.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3188 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPss/XrdPssAioCB.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8402 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPss/XrdPssCks.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3733 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPss/XrdPssCks.hh
+-rw-rw-rw-   0 root         (0) root         (0)    30386 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPss/XrdPssConfig.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2807 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPss/XrdPssTrace.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8758 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPss/XrdPssUrlInfo.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3611 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPss/XrdPssUrlInfo.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5115 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPss/XrdPssUtils.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPss/XrdPssUtils.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdRmc/
+-rw-rw-rw-   0 root         (0) root         (0)     3076 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdRmc/XrdRmc.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8248 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdRmc/XrdRmc.hh
+-rw-rw-rw-   0 root         (0) root         (0)    20495 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdRmc/XrdRmcData.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5754 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdRmc/XrdRmcData.hh
+-rw-rw-rw-   0 root         (0) root         (0)    20703 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdRmc/XrdRmcReal.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5594 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdRmc/XrdRmcReal.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7041 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdRmc/XrdRmcSlot.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdSciTokens/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdSciTokens/configs/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/configs/export-lib-symbols
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/configs/export-module-symbols
+-rw-rw-rw-   0 root         (0) root         (0)      945 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/configs/scitokens.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdSciTokens/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdSciTokens/test/config/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/test/config/override.conf
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/test/config/scitokens-aud.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/test/config/scitokens-multi-aud.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/test/config/scitokens-no-aud.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1879 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/test/config/xrootd-http.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1598 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/test/create-pubkey.py
+-rw-rw-rw-   0 root         (0) root         (0)      594 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/test/openssl-selfsigned.conf
+-rwxrwxrwx   0 root         (0) root         (0)      803 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/test/setup_tests.sh
+-rwxrwxrwx   0 root         (0) root         (0)     5083 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/test/test_inside_docker.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/inih/
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/inih/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/inih/.travis.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13507 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/inih/INIReader.h
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/inih/INIReaderTest.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/inih/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1574 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/inih/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      416 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/inih/test.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     3435 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/examples/github-issues.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2787 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/examples/iostream.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2496 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/examples/streaming.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/picotest/
+-rw-rw-rw-   0 root         (0) root         (0)     2452 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/picotest/picotest.c
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/picotest/picotest.h
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/.clang-format
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 08:45:39.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/.gitmodules
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/.travis.yml
+-rw-rw-rw-   0 root         (0) root         (0)      903 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/Changes
+-rw-rw-rw-   0 root         (0) root         (0)     1336 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     7011 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/README.mkdn
+-rw-rw-rw-   0 root         (0) root         (0)    33256 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/picojson.h
+-rw-rw-rw-   0 root         (0) root         (0)    12611 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/test.cc
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/vendor/README.vendor
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     7684 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    48515 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/XrdSciTokensAccess.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2910 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens/XrdSciTokensHelper.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdSec/
+-rw-rw-rw-   0 root         (0) root         (0)     4540 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecAttr.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5632 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecClient.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6046 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecEntity.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6747 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecEntity.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6459 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecEntityAttr.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8424 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecEntityAttr.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4638 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecEntityPin.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2945 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecEntityXtra.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2772 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecEntityXtra.hh
+-rw-rw-rw-   0 root         (0) root         (0)    34779 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecInterface.hh
+-rw-rw-rw-   0 root         (0) root         (0)    10669 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecLoadSecurity.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7822 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecLoadSecurity.hh
+-rw-rw-rw-   0 root         (0) root         (0)    15666 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecPManager.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5056 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecPManager.hh
+-rw-rw-rw-   0 root         (0) root         (0)    18129 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecProtect.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8540 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecProtect.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11790 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecProtector.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7608 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecProtector.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4849 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecProtocolhost.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3535 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecProtocolhost.hh
+-rw-rw-rw-   0 root         (0) root         (0)    40467 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecServer.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5105 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecServer.hh
+-rw-rw-rw-   0 root         (0) root         (0)    14312 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecTLayer.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7692 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecTLayer.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3066 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSecTrace.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7624 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSectestClient.cc
+-rw-rw-rw-   0 root         (0) root         (0)    12009 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec/XrdSectestServer.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdSecgsi/
+-rw-rw-rw-   0 root         (0) root         (0)   197464 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecgsi/XrdSecProtocolgsi.cc
+-rw-rw-rw-   0 root         (0) root         (0)    24807 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecgsi/XrdSecProtocolgsi.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6777 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecgsi/XrdSecgsiAuthzFunDN.cc
+-rw-rw-rw-   0 root         (0) root         (0)    11227 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecgsi/XrdSecgsiAuthzFunVO.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8781 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecgsi/XrdSecgsiGMAPFunDN.cc
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecgsi/XrdSecgsiGMAPFunDN.cf
+-rw-rw-rw-   0 root         (0) root         (0)     9513 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecgsi/XrdSecgsiOpts.hh
+-rw-rw-rw-   0 root         (0) root         (0)    26699 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecgsi/XrdSecgsiProxy.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecgsi/XrdSecgsiTrace.hh
+-rw-rw-rw-   0 root         (0) root         (0)    17319 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecgsi/XrdSecgsitest.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdSeckrb5/
+-rw-rw-rw-   0 root         (0) root         (0)    38570 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSeckrb5/XrdSecProtocolkrb5.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdSecpwd/
+-rw-rw-rw-   0 root         (0) root         (0)   129049 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecpwd/XrdSecProtocolpwd.cc
+-rw-rw-rw-   0 root         (0) root         (0)    19037 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecpwd/XrdSecProtocolpwd.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2626 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecpwd/XrdSecpwdPlatform.hh
+-rw-rw-rw-   0 root         (0) root         (0)    84580 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecpwd/XrdSecpwdSrvAdmin.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecpwd/XrdSecpwdTrace.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdSecsss/
+-rw-rw-rw-   0 root         (0) root         (0)    41443 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecsss/XrdSecProtocolsss.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6297 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecsss/XrdSecProtocolsss.hh
+-rw-rw-rw-   0 root         (0) root         (0)    19394 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecsss/XrdSecsssAdmin.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3559 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecsss/XrdSecsssCon.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4329 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecsss/XrdSecsssCon.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11806 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecsss/XrdSecsssEnt.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5290 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecsss/XrdSecsssEnt.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9560 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecsss/XrdSecsssID.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8505 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecsss/XrdSecsssID.hh
+-rw-rw-rw-   0 root         (0) root         (0)    25232 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecsss/XrdSecsssKT.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5358 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecsss/XrdSecsssKT.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2704 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecsss/XrdSecsssMap.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5765 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecsss/XrdSecsssRR.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdSecunix/
+-rw-rw-rw-   0 root         (0) root         (0)     8575 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecunix/XrdSecProtocolunix.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdSecztn/
+-rw-rw-rw-   0 root         (0) root         (0)    28393 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecztn/XrdSecProtocolztn.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6814 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecztn/XrdSecztn.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdSfs/
+-rw-rw-rw-   0 root         (0) root         (0)     3999 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSfs/XrdSfsAio.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5824 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSfs/XrdSfsDio.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5455 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSfs/XrdSfsFAttr.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5100 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSfs/XrdSfsFlags.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5619 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSfs/XrdSfsGPFile.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12634 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSfs/XrdSfsInterface.cc
+-rw-rw-rw-   0 root         (0) root         (0)    67119 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSfs/XrdSfsInterface.hh
+-rw-rw-rw-   0 root         (0) root         (0)    38665 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSfs/XrdSfsNative.cc
+-rw-rw-rw-   0 root         (0) root         (0)    10785 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSfs/XrdSfsNative.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSfs/XrdSfsXio.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7187 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSfs/XrdSfsXio.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4432 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSfs/XrdSfsXioImpl.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdSsi/
+-rw-rw-rw-   0 root         (0) root         (0)     6178 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiAlert.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3366 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiAlert.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2661 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiAtomics.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7958 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiAtomics.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3132 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiBVec.hh
+-rw-rw-rw-   0 root         (0) root         (0)    14419 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiClient.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7934 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiCluster.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4735 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiCms.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3752 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiCms.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7049 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiDir.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3177 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiDir.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4087 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiEntity.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2663 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiErrInfo.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6519 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiErrInfo.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7117 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiEvent.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4015 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiEvent.hh
+-rw-rw-rw-   0 root         (0) root         (0)    18166 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiFile.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5424 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiFile.hh
+-rw-rw-rw-   0 root         (0) root         (0)    35655 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiFileReq.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6776 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiFileReq.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3711 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiFileResource.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2797 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiFileResource.hh
+-rw-rw-rw-   0 root         (0) root         (0)    26232 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiFileSess.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6023 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiFileSess.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7881 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiLogger.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8724 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiLogger.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6495 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiLogging.cc
+-rw-rw-rw-   0 root         (0) root         (0)    17533 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiProvider.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3962 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiRRAgent.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4545 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiRRInfo.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4295 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiRRTable.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8144 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiRequest.cc
+-rw-rw-rw-   0 root         (0) root         (0)    15740 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiRequest.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5790 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiResource.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7000 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiRespInfo.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12144 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiResponder.cc
+-rw-rw-rw-   0 root         (0) root         (0)    13431 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiResponder.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8986 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiScale.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3515 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiScale.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12168 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiServReal.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3574 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiServReal.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3281 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiService.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9866 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiService.hh
+-rw-rw-rw-   0 root         (0) root         (0)    17845 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiSessReal.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4784 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiSessReal.hh
+-rw-rw-rw-   0 root         (0) root         (0)    20137 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiSfs.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7069 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiSfs.hh
+-rw-rw-rw-   0 root         (0) root         (0)    25133 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiSfsConfig.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3556 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiSfsConfig.hh
+-rw-rw-rw-   0 root         (0) root         (0)    45526 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiShMam.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5508 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiShMam.hh
+-rw-rw-rw-   0 root         (0) root         (0)    22363 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiShMap.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12380 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiShMap.icc
+-rw-rw-rw-   0 root         (0) root         (0)     3048 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiShMat.cc
+-rw-rw-rw-   0 root         (0) root         (0)    19625 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiShMat.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6168 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiStat.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6883 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiStats.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4527 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiStats.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8580 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiStream.hh
+-rw-rw-rw-   0 root         (0) root         (0)    24852 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiTaskReal.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4845 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiTaskReal.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2865 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiTrace.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9000 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiUtils.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3203 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi/XrdSsiUtils.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdSut/
+-rw-rw-rw-   0 root         (0) root         (0)    22213 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSut/XrdSutAux.cc
+-rw-rw-rw-   0 root         (0) root         (0)    15145 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSut/XrdSutAux.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5926 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSut/XrdSutBuckList.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3963 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSut/XrdSutBuckList.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8236 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSut/XrdSutBucket.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3458 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSut/XrdSutBucket.hh
+-rw-rw-rw-   0 root         (0) root         (0)    16276 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSut/XrdSutBuffer.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4872 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSut/XrdSutBuffer.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6430 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSut/XrdSutCache.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5618 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSut/XrdSutCacheEntry.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5456 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSut/XrdSutCacheEntry.hh
+-rw-rw-rw-   0 root         (0) root         (0)    21841 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSut/XrdSutPFCache.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5757 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSut/XrdSutPFCache.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5549 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSut/XrdSutPFEntry.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4790 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSut/XrdSutPFEntry.hh
+-rw-rw-rw-   0 root         (0) root         (0)    64583 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSut/XrdSutPFile.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7738 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSut/XrdSutPFile.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8759 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSut/XrdSutRndm.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3293 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSut/XrdSutRndm.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2936 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSut/XrdSutTrace.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdSys/
+-rw-rw-rw-   0 root         (0) root         (0)     5249 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysAtomics.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4979 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysDir.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3341 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysDir.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4872 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysE2T.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2750 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysE2T.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8454 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysError.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7349 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysError.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6923 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysFAttr.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4996 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysFAttr.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7106 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysFAttrBsd.icc
+-rw-rw-rw-   0 root         (0) root         (0)     6632 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysFAttrLnx.icc
+-rw-rw-rw-   0 root         (0) root         (0)     6063 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysFAttrMac.icc
+-rw-rw-rw-   0 root         (0) root         (0)     7705 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysFAttrSun.icc
+-rw-rw-rw-   0 root         (0) root         (0)     7575 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysFD.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4783 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysFallocate.cc
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysFallocate.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2714 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysHeaders.hh
+-rw-rw-rw-   0 root         (0) root         (0)    43245 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysIOEvents.cc
+-rw-rw-rw-   0 root         (0) root         (0)    26713 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysIOEvents.hh
+-rw-rw-rw-   0 root         (0) root         (0)    16042 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysIOEventsPollE.icc
+-rw-rw-rw-   0 root         (0) root         (0)    17035 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysIOEventsPollKQ.icc
+-rw-rw-rw-   0 root         (0) root         (0)    18696 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysIOEventsPollPoll.icc
+-rw-rw-rw-   0 root         (0) root         (0)    14965 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysIOEventsPollPort.icc
+-rw-rw-rw-   0 root         (0) root         (0)    16419 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysKernelBuffer.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5437 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysLogPI.hh
+-rw-rw-rw-   0 root         (0) root         (0)    26549 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysLogger.cc
+-rw-rw-rw-   0 root         (0) root         (0)    11736 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysLogger.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12120 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysLogging.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5811 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysLogging.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2511 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysPageSize.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3233 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysPlatform.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8249 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysPlatform.hh
+-rw-rw-rw-   0 root         (0) root         (0)    17839 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysPlugin.cc
+-rw-rw-rw-   0 root         (0) root         (0)    13621 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysPlugin.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12930 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysPriv.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4228 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysPriv.hh
+-rw-rw-rw-   0 root         (0) root         (0)    13657 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysPthread.cc
+-rw-rw-rw-   0 root         (0) root         (0)    19415 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysPthread.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3245 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysPwd.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11994 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysRAtomic.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3952 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysSemWait.hh
+-rw-rw-rw-   0 root         (0) root         (0)     9460 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysTimer.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3814 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysTimer.hh
+-rw-rw-rw-   0 root         (0) root         (0)    15639 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysTrace.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4739 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysTrace.hh
+-rw-rw-rw-   0 root         (0) root         (0)     8298 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysUtils.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4798 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysUtils.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4735 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysXAttr.cc
+-rw-rw-rw-   0 root         (0) root         (0)    15063 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysXAttr.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5688 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysXSLock.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3311 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSys/XrdSysXSLock.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdThrottle/
+-rw-rw-rw-   0 root         (0) root         (0)     3577 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdThrottle/README
+-rw-rw-rw-   0 root         (0) root         (0)     7487 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdThrottle/XrdThrottle.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6658 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdThrottle/XrdThrottleFile.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5731 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdThrottle/XrdThrottleFileSystem.cc
+-rw-rw-rw-   0 root         (0) root         (0)    12897 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdThrottle/XrdThrottleFileSystemConfig.cc
+-rw-rw-rw-   0 root         (0) root         (0)    18584 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdThrottle/XrdThrottleManager.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5403 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdThrottle/XrdThrottleManager.hh
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdThrottle/XrdThrottleTrace.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdTls/
+-rw-rw-rw-   0 root         (0) root         (0)    10417 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTls/XrdTls.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6921 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTls/XrdTls.hh
+-rw-rw-rw-   0 root         (0) root         (0)    37652 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTls/XrdTlsContext.cc
+-rw-rw-rw-   0 root         (0) root         (0)    14507 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTls/XrdTlsContext.hh
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTls/XrdTlsHostcheck.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6628 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTls/XrdTlsHostcheck.icc
+-rw-rw-rw-   0 root         (0) root         (0)     5275 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTls/XrdTlsNotary.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5222 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTls/XrdTlsNotary.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTls/XrdTlsNotaryUtils.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7142 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTls/XrdTlsNotaryUtils.icc
+-rw-rw-rw-   0 root         (0) root         (0)     3969 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTls/XrdTlsPeerCerts.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4951 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTls/XrdTlsPeerCerts.hh
+-rw-rw-rw-   0 root         (0) root         (0)    33590 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTls/XrdTlsSocket.cc
+-rw-rw-rw-   0 root         (0) root         (0)    11845 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTls/XrdTlsSocket.hh
+-rw-rw-rw-   0 root         (0) root         (0)    16134 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTls/XrdTlsTempCA.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5462 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTls/XrdTlsTempCA.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTls/XrdTlsTrace.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdTpc/
+-rw-rw-rw-   0 root         (0) root         (0)     4032 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTpc/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     5387 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTpc/XrdTpcConfigure.cc
+-rw-rw-rw-   0 root         (0) root         (0)     1663 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTpc/XrdTpcCurlMulti.cc
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTpc/XrdTpcCurlMulti.hh
+-rw-rw-rw-   0 root         (0) root         (0)    19456 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTpc/XrdTpcMultistream.cc
+-rw-rw-rw-   0 root         (0) root         (0)    10532 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTpc/XrdTpcState.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5794 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTpc/XrdTpcState.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7210 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTpc/XrdTpcStream.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5499 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTpc/XrdTpcStream.hh
+-rw-rw-rw-   0 root         (0) root         (0)    44035 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTpc/XrdTpcTPC.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5994 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTpc/XrdTpcTPC.hh
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTpc/export-lib-symbols
+-rwxrwxrwx   0 root         (0) root         (0)     3709 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTpc/xrootd-test-tpc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdVoms/
+-rw-rw-rw-   0 root         (0) root         (0)     2917 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdVoms/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2590 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdVoms/XrdVoms.hh
+-rw-rw-rw-   0 root         (0) root         (0)    22180 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdVoms/XrdVomsFun.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3835 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdVoms/XrdVomsFun.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6174 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdVoms/XrdVomsHttp.cc
+-rw-rw-rw-   0 root         (0) root         (0)    15232 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdVoms/XrdVomsMapfile.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4249 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdVoms/XrdVomsMapfile.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2680 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdVoms/XrdVomsTrace.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4105 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdVoms/XrdVomsgsi.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdXml/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdXml/tinyxml/
+-rw-rw-rw-   0 root         (0) root         (0)     2507 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXml/tinyxml/tinystr.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     8197 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXml/tinyxml/tinystr.h
+-rw-rw-rw-   0 root         (0) root         (0)    37588 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXml/tinyxml/tinyxml.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    64835 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXml/tinyxml/tinyxml.h
+-rw-rw-rw-   0 root         (0) root         (0)     1791 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXml/tinyxml/tinyxmlerror.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    37439 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXml/tinyxml/tinyxmlparser.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    18501 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXml/XrdXmlMetaLink.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9497 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXml/XrdXmlMetaLink.hh
+-rw-rw-rw-   0 root         (0) root         (0)    10670 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXml/XrdXmlRdrTiny.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3590 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXml/XrdXmlRdrTiny.hh
+-rw-rw-rw-   0 root         (0) root         (0)    11751 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXml/XrdXmlRdrXml2.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3585 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXml/XrdXmlRdrXml2.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4195 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXml/XrdXmlReader.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9010 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXml/XrdXmlReader.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdXrootd/
+-rw-rw-rw-   0 root         (0) root         (0)    21688 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdAdmin.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3927 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdAdmin.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6106 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdAioBuff.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3396 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdAioBuff.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6164 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdAioFob.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3140 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdAioFob.hh
+-rw-rw-rw-   0 root         (0) root         (0)    10852 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdAioPgrw.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4017 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdAioPgrw.hh
+-rw-rw-rw-   0 root         (0) root         (0)    16842 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdAioTask.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5932 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdAioTask.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3257 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdBridge.cc
+-rw-rw-rw-   0 root         (0) root         (0)    25502 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdBridge.hh
+-rw-rw-rw-   0 root         (0) root         (0)    17339 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdCallBack.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdCallBack.hh
+-rw-rw-rw-   0 root         (0) root         (0)    71797 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdConfig.cc
+-rw-rw-rw-   0 root         (0) root         (0)    25761 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdConfigMon.cc
+-rw-rw-rw-   0 root         (0) root         (0)    14829 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdFile.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8211 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdFile.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2629 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdFileLock.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6072 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdFileLock1.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2959 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdFileLock1.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7522 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdFileStats.hh
+-rw-rw-rw-   0 root         (0) root         (0)    10638 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdGPFile.hh
+-rw-rw-rw-   0 root         (0) root         (0)    19666 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdGSReal.cc
+-rw-rw-rw-   0 root         (0) root         (0)     6593 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdGSReal.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5076 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdGStream.cc
+-rw-rw-rw-   0 root         (0) root         (0)     8514 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdGStream.hh
+-rw-rw-rw-   0 root         (0) root         (0)    26130 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdJob.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4224 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdJob.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3858 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdLoadLib.cc
+-rw-rw-rw-   0 root         (0) root         (0)    14081 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdMonData.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5374 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdMonFMap.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3118 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdMonFMap.hh
+-rw-rw-rw-   0 root         (0) root         (0)    18282 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdMonFile.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4376 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdMonFile.hh
+-rw-rw-rw-   0 root         (0) root         (0)    42910 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdMonitor.cc
+-rw-rw-rw-   0 root         (0) root         (0)    12097 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdMonitor.hh
+-rw-rw-rw-   0 root         (0) root         (0)    17436 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdNormAio.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3758 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdNormAio.hh
+-rw-rw-rw-   0 root         (0) root         (0)    19524 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdPgrwAio.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3708 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdPgrwAio.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4934 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdPgwBadCS.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2979 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdPgwBadCS.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7262 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdPgwCtl.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4842 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdPgwCtl.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4520 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdPgwFob.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4321 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdPgwFob.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3973 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdPio.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3751 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdPio.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4685 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdPlugin.cc
+-rw-rw-rw-   0 root         (0) root         (0)    12615 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdPrepare.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4956 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdPrepare.hh
+-rw-rw-rw-   0 root         (0) root         (0)    53955 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdProtocol.cc
+-rw-rw-rw-   0 root         (0) root         (0)    23977 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdProtocol.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdReqID.hh
+-rw-rw-rw-   0 root         (0) root         (0)    17733 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdResponse.cc
+-rw-rw-rw-   0 root         (0) root         (0)     5450 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdResponse.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7898 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdStats.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4653 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdStats.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6457 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdTpcMon.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4899 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdTpcMon.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3605 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdTrace.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4806 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdTransPend.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3394 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdTransPend.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3978 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdTransSend.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3662 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdTransSend.hh
+-rw-rw-rw-   0 root         (0) root         (0)    27246 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdTransit.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9705 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdTransit.hh
+-rw-rw-rw-   0 root         (0) root         (0)     2783 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdWVInfo.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5092 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdXPath.hh
+-rw-rw-rw-   0 root         (0) root         (0)   147048 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdXeq.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3317 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdXeq.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12437 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdXeqChkPnt.cc
+-rw-rw-rw-   0 root         (0) root         (0)    20041 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdXeqFAttr.cc
+-rw-rw-rw-   0 root         (0) root         (0)    22344 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXrootd/XrdXrootdXeqPgrw.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/src/XrdZip/
+-rw-rw-rw-   0 root         (0) root         (0)    14675 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdZip/XrdZipCDFH.hh
+-rw-rw-rw-   0 root         (0) root         (0)     1960 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdZip/XrdZipDataDescriptor.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6301 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdZip/XrdZipEOCD.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6223 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdZip/XrdZipExtra.hh
+-rw-rw-rw-   0 root         (0) root         (0)     7291 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdZip/XrdZipLFH.hh
+-rw-rw-rw-   0 root         (0) root         (0)     6734 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdZip/XrdZipUtils.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5265 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdZip/XrdZipZIP64EOCD.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3227 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdZip/XrdZipZIP64EOCDL.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3848 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)     6828 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdApps.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     4556 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdCrypto.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     2928 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdDaemons.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     1913 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFfs.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     3214 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdFrm.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     4699 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHeaders.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     2679 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdHttp.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     2084 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdIsal.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdMacaroons.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdOssCsi.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     3134 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPfc.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     5719 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPlugins.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     2958 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdPosix.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSciTokens.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     5294 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSec.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     3489 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecgsi.cmake
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSeckrb5.cmake
+-rw-rw-rw-   0 root         (0) root         (0)      853 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSecztn.cmake
+-rw-rw-rw-   0 root         (0) root         (0)    10870 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdServer.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     4916 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdSsi.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdTpc.cmake
+-rw-rw-rw-   0 root         (0) root         (0)    14635 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdUtils.cmake
+-rw-r--r--   0 root         (0) root         (0)     5171 2023-05-08 08:46:21.000000 xrootd-5.5.5/src/XrdVersion.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5174 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdVersion.hh.in
+-rw-rw-rw-   0 root         (0) root         (0)    15666 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdVersionPlugin.hh
+-rw-rw-rw-   0 root         (0) root         (0)     1877 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdVoms.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     2222 2023-05-08 08:45:38.000000 xrootd-5.5.5/src/XrdXml.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/tests/XrdCephTests/
+-rw-rw-rw-   0 root         (0) root         (0)      556 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdCephTests/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)     6661 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdCephTests/CephParsingTest.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/tests/XrdClHttp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:33.000000 xrootd-5.5.5/tests/XrdClHttp/cases/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/tests/XrdClHttp/cases/000-simple-download/
+-rw-rw-rw-   0 root         (0) root         (0)      960 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClHttp/cases/000-simple-download/main.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/tests/XrdClHttp/cases/001-deep-path-download/
+-rw-rw-rw-   0 root         (0) root         (0)     1044 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClHttp/cases/001-deep-path-download/main.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/tests/XrdClHttp/cases/002-simple-upload/
+-rw-rw-rw-   0 root         (0) root         (0)     1028 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClHttp/cases/002-simple-upload/main.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/tests/XrdClHttp/cases/003-deep-path-upload/
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClHttp/cases/003-deep-path-upload/main.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/tests/XrdClHttp/config/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/tests/XrdClHttp/config/client/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClHttp/config/client/http.conf
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClHttp/config/caddyfile
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClHttp/config/caddyfile-webdav
+-rw-rw-rw-   0 root         (0) root         (0)     1919 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClHttp/common.sh
+-rwxrwxrwx   0 root         (0) root         (0)     1571 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClHttp/run_test.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/tests/XrdClTests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/tests/XrdClTests/tls/
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/tls/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/tls/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/tls/xrdcl-tls.cc
+-rw-rw-rw-   0 root         (0) root         (0)    16273 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/tls/xrdsrv-tls.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/tests/XrdClTests/wrt/
+-rw-rw-rw-   0 root         (0) root         (0)    14962 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/wrt/xrdsrv-dio.cc
+-rw-rw-rw-   0 root         (0) root         (0)    14168 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/wrt/xrdsrv-wrt.cc
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)    27183 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/FileCopyTest.cc
+-rw-rw-rw-   0 root         (0) root         (0)    22807 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/FileSystemTest.cc
+-rw-rw-rw-   0 root         (0) root         (0)    30512 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/FileTest.cc
+-rw-rw-rw-   0 root         (0) root         (0)    21399 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/IdentityPlugIn.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2516 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/IdentityPlugIn.hh
+-rw-rw-rw-   0 root         (0) root         (0)    22565 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/LocalFileHandlerTest.cc
+-rw-rw-rw-   0 root         (0) root         (0)     9085 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/MonitorTestLib.cc
+-rw-rw-rw-   0 root         (0) root         (0)    36161 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/OperationsWorkflowTest.cc
+-rw-rw-rw-   0 root         (0) root         (0)    10184 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/PollerTest.cc
+-rw-rw-rw-   0 root         (0) root         (0)    20524 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/PostMasterTest.cc
+-rw-rw-rw-   0 root         (0) root         (0)    11141 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/SocketTest.cc
+-rw-rw-rw-   0 root         (0) root         (0)    12152 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/ThreadingTest.cc
+-rw-rw-rw-   0 root         (0) root         (0)    17858 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/UtilsTest.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4848 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/XRootDProtocolHelper.cc
+-rw-rw-rw-   0 root         (0) root         (0)     1982 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/XRootDProtocolHelper.hh
+-rw-rw-rw-   0 root         (0) root         (0)      419 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/cppunit.supp
+-rwxrwxrwx   0 root         (0) root         (0)      430 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdClTests/printenv.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/tests/XrdEcTests/
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdEcTests/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)    19453 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdEcTests/MicroTest.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/tests/XrdSsiTests/
+-rw-rw-rw-   0 root         (0) root         (0)      435 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdSsiTests/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)    36471 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/XrdSsiTests/XrdShMap.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/tests/common/
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/common/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2485 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/common/CppUnitXrdHelpers.hh
+-rw-rw-rw-   0 root         (0) root         (0)     3148 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/common/PathProcessor.hh
+-rw-rw-rw-   0 root         (0) root         (0)    12734 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/common/Server.cc
+-rw-rw-rw-   0 root         (0) root         (0)     7796 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/common/Server.hh
+-rw-rw-rw-   0 root         (0) root         (0)     4264 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/common/TestEnv.cc
+-rw-rw-rw-   0 root         (0) root         (0)     2456 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/common/TestEnv.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5571 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/common/TextRunner.cc
+-rw-rw-rw-   0 root         (0) root         (0)     3461 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/common/Utils.cc
+-rw-rw-rw-   0 root         (0) root         (0)     4485 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/common/Utils.hh
+-rw-rw-rw-   0 root         (0) root         (0)      212 2023-05-08 08:45:38.000000 xrootd-5.5.5/tests/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/ups/
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-05-08 08:45:38.000000 xrootd-5.5.5/ups/eupspkg.cfg.sh
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-05-08 08:45:38.000000 xrootd-5.5.5/ups/xrootd.table
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/utils/
+-rwxrwxrwx   0 root         (0) root         (0)     6678 2023-05-08 08:45:38.000000 xrootd-5.5.5/utils/XrdCmsNotify.pm
+-rwxrwxrwx   0 root         (0) root         (0)     7851 2023-05-08 08:45:38.000000 xrootd-5.5.5/utils/XrdOlbMonPerf
+-rwxrwxrwx   0 root         (0) root         (0)     3789 2023-05-08 08:45:38.000000 xrootd-5.5.5/utils/cms_monPerf
+-rwxrwxrwx   0 root         (0) root         (0)    29321 2023-05-08 08:45:38.000000 xrootd-5.5.5/utils/hpsscp
+-rwxrwxrwx   0 root         (0) root         (0)     4187 2023-05-08 08:45:38.000000 xrootd-5.5.5/utils/netchk
+-rwxrwxrwx   0 root         (0) root         (0)     2181 2023-05-08 08:45:38.000000 xrootd-5.5.5/utils/xrootd-config
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:46:34.000000 xrootd-5.5.5/xrootd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-05-08 08:46:33.000000 xrootd-5.5.5/xrootd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    46123 2023-05-08 08:46:33.000000 xrootd-5.5.5/xrootd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 08:46:33.000000 xrootd-5.5.5/xrootd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 08:46:33.000000 xrootd-5.5.5/xrootd.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3695 2023-05-08 08:45:38.000000 xrootd-5.5.5/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2023-05-08 08:45:38.000000 xrootd-5.5.5/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)     2811 2023-05-08 08:45:38.000000 xrootd-5.5.5/COPYING.BSD
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-05-08 08:45:38.000000 xrootd-5.5.5/COPYING.LGPL
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2023-05-08 08:45:38.000000 xrootd-5.5.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      294 2023-05-08 08:46:21.000000 xrootd-5.5.5/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     3287 2023-05-08 08:45:38.000000 xrootd-5.5.5/README
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-05-08 08:45:38.000000 xrootd-5.5.5/VERSION_INFO
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-05-08 08:45:38.000000 xrootd-5.5.5/cmake_uninstall.cmake.in
+-rwxrwxrwx   0 root         (0) root         (0)      991 2023-05-08 08:45:38.000000 xrootd-5.5.5/gen-tarball.sh
+-rwxrwxrwx   0 root         (0) root         (0)     8485 2023-05-08 08:45:38.000000 xrootd-5.5.5/genversion.sh
+-rwxr-xr-x   0 root         (0) root         (0)      201 2023-05-08 08:46:21.000000 xrootd-5.5.5/has_c++14.sh
+-rwxr-xr-x   0 root         (0) root         (0)     1407 2023-05-08 08:46:21.000000 xrootd-5.5.5/install.sh
+-rwxr-xr-x   0 root         (0) root         (0)     1240 2023-05-08 08:46:21.000000 xrootd-5.5.5/publish.sh
+-rw-r--r--   0 root         (0) root         (0)     7310 2023-05-08 08:46:21.000000 xrootd-5.5.5/setup.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-05-08 08:46:34.000000 xrootd-5.5.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 08:46:34.000000 xrootd-5.5.5/setup.cfg
```

### Comparing `xrootd-5.5.4/bindings/python/docs/source/.static/css/custom.css` & `xrootd-5.5.5/bindings/python/docs/source/.static/css/custom.css`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/docs/source/examples/file.rst` & `xrootd-5.5.5/bindings/python/docs/source/examples/file.rst`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/docs/source/examples/filesystem.rst` & `xrootd-5.5.5/bindings/python/docs/source/examples/filesystem.rst`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/docs/source/modules/client/file.rst` & `xrootd-5.5.5/bindings/python/docs/source/modules/client/file.rst`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/docs/source/modules/client/filesystem.rst` & `xrootd-5.5.5/bindings/python/docs/source/modules/client/filesystem.rst`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/docs/source/modules/client/flags.rst` & `xrootd-5.5.5/bindings/python/docs/source/modules/client/flags.rst`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/docs/source/modules/client/responses.rst` & `xrootd-5.5.5/bindings/python/docs/source/modules/client/responses.rst`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/docs/source/conf.py` & `xrootd-5.5.5/bindings/python/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/docs/source/favicon.ico` & `xrootd-5.5.5/bindings/python/docs/source/favicon.ico`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/docs/source/gettingstarted.rst` & `xrootd-5.5.5/bindings/python/docs/source/gettingstarted.rst`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/docs/source/index.rst` & `xrootd-5.5.5/bindings/python/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/docs/source/xrootd-200x68.png` & `xrootd-5.5.5/bindings/python/docs/source/xrootd-200x68.png`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/docs/Makefile` & `xrootd-5.5.5/bindings/python/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/docs/ReleaseNotes.txt` & `xrootd-5.5.5/bindings/python/docs/ReleaseNotes.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/examples/copyprocess.py` & `xrootd-5.5.5/bindings/python/examples/copyprocess.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/examples/dirlist.py` & `xrootd-5.5.5/bindings/python/examples/dirlist.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/examples/fileproperties.py` & `xrootd-5.5.5/bindings/python/examples/fileproperties.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/examples/filesystemproperties.py` & `xrootd-5.5.5/bindings/python/examples/filesystemproperties.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/examples/query.py` & `xrootd-5.5.5/bindings/python/examples/query.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/examples/read.py` & `xrootd-5.5.5/bindings/python/examples/read.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/examples/vector_read.py` & `xrootd-5.5.5/bindings/python/examples/vector_read.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/libs/client/__init__.py` & `xrootd-5.5.5/bindings/python/libs/client/__init__.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/libs/client/_version.py` & `xrootd-5.5.5/bindings/python/libs/client/_version.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/libs/client/copyprocess.py` & `xrootd-5.5.5/bindings/python/libs/client/copyprocess.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/libs/client/env.py` & `xrootd-5.5.5/bindings/python/libs/client/env.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/libs/client/file.py` & `xrootd-5.5.5/bindings/python/libs/client/file.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/libs/client/filesystem.py` & `xrootd-5.5.5/bindings/python/libs/client/filesystem.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/libs/client/finalize.py` & `xrootd-5.5.5/bindings/python/libs/client/finalize.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/libs/client/flags.py` & `xrootd-5.5.5/bindings/python/libs/client/flags.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/libs/client/glob_funcs.py` & `xrootd-5.5.5/bindings/python/libs/client/glob_funcs.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/libs/client/responses.py` & `xrootd-5.5.5/bindings/python/libs/client/responses.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/libs/client/url.py` & `xrootd-5.5.5/bindings/python/libs/client/url.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/libs/client/utils.py` & `xrootd-5.5.5/bindings/python/libs/client/utils.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/src/AsyncResponseHandler.hh` & `xrootd-5.5.5/bindings/python/src/AsyncResponseHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/src/ChunkIterator.hh` & `xrootd-5.5.5/bindings/python/src/ChunkIterator.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/src/Conversions.hh` & `xrootd-5.5.5/bindings/python/src/Conversions.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/src/PyXRootD.hh` & `xrootd-5.5.5/bindings/python/src/PyXRootD.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/src/PyXRootDCopyProcess.cc` & `xrootd-5.5.5/bindings/python/src/PyXRootDCopyProcess.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/src/PyXRootDCopyProcess.hh` & `xrootd-5.5.5/bindings/python/src/PyXRootDCopyProcess.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/src/PyXRootDCopyProgressHandler.cc` & `xrootd-5.5.5/bindings/python/src/PyXRootDCopyProgressHandler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/src/PyXRootDCopyProgressHandler.hh` & `xrootd-5.5.5/bindings/python/src/PyXRootDCopyProgressHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/src/PyXRootDEnv.hh` & `xrootd-5.5.5/bindings/python/src/PyXRootDEnv.hh`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,14 @@
   }
 
   //----------------------------------------------------------------------------
   //! @return : client version, e.g.: v4.10.0
   //----------------------------------------------------------------------------
   PyObject* XrdVersion_cpp( PyObject *self, PyObject *args )
   {
-    static std::string verstr( XrdVERSION[0] == 'v' ? XrdVERSION + 1 : XrdVERSION );
+    static std::string verstr( XrdVERSION[0] == 'v' ? &XrdVERSION[1] : XrdVERSION );
     return Py_BuildValue( "s", verstr.c_str() );
   }
 
 }
 
 #endif /* PYENV_HH_ */
```

### Comparing `xrootd-5.5.4/bindings/python/src/PyXRootDFile.cc` & `xrootd-5.5.5/bindings/python/src/PyXRootDFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/src/PyXRootDFile.hh` & `xrootd-5.5.5/bindings/python/src/PyXRootDFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/src/PyXRootDFileSystem.cc` & `xrootd-5.5.5/bindings/python/src/PyXRootDFileSystem.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/src/PyXRootDFileSystem.hh` & `xrootd-5.5.5/bindings/python/src/PyXRootDFileSystem.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/src/PyXRootDFinalize.hh` & `xrootd-5.5.5/bindings/python/src/PyXRootDFinalize.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/src/PyXRootDModule.cc` & `xrootd-5.5.5/bindings/python/src/PyXRootDModule.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/src/PyXRootDURL.cc` & `xrootd-5.5.5/bindings/python/src/PyXRootDURL.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/src/PyXRootDURL.hh` & `xrootd-5.5.5/bindings/python/src/PyXRootDURL.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/src/Utils.cc` & `xrootd-5.5.5/bindings/python/src/Utils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/src/Utils.hh` & `xrootd-5.5.5/bindings/python/src/Utils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/tests/test_copy.py` & `xrootd-5.5.5/bindings/python/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/tests/test_file.py` & `xrootd-5.5.5/bindings/python/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/tests/test_filesystem.py` & `xrootd-5.5.5/bindings/python/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/tests/test_glob.py` & `xrootd-5.5.5/bindings/python/tests/test_glob.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/tests/test_threads.py` & `xrootd-5.5.5/bindings/python/tests/test_threads.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/tests/test_url.py` & `xrootd-5.5.5/bindings/python/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/CMakeLists.txt` & `xrootd-5.5.5/bindings/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/README.rst` & `xrootd-5.5.5/bindings/python/README.rst`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/bindings/python/setup.py.in` & `xrootd-5.5.5/bindings/python/setup.py.in`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/cmake/FindCppUnit.cmake` & `xrootd-5.5.5/cmake/FindCppUnit.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/cmake/FindKerberos5.cmake` & `xrootd-5.5.5/cmake/FindKerberos5.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/cmake/FindReadline.cmake` & `xrootd-5.5.5/cmake/FindReadline.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/cmake/FindVOMS.cmake` & `xrootd-5.5.5/cmake/FindVOMS.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/cmake/Findfuse.cmake` & `xrootd-5.5.5/cmake/Findfuse.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/cmake/Findlibuuid.cmake` & `xrootd-5.5.5/cmake/Findlibuuid.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/cmake/Findsystemd.cmake` & `xrootd-5.5.5/cmake/Findsystemd.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/cmake/GNUInstallDirs.cmake` & `xrootd-5.5.5/cmake/GNUInstallDirs.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/cmake/XRootDConfig.cmake.in` & `xrootd-5.5.5/cmake/XRootDConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/cmake/XRootDDefaults.cmake` & `xrootd-5.5.5/cmake/XRootDDefaults.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/cmake/XRootDFindLibs.cmake` & `xrootd-5.5.5/cmake/XRootDFindLibs.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/cmake/XRootDOSDefs.cmake` & `xrootd-5.5.5/cmake/XRootDOSDefs.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/cmake/XRootDSummary.cmake` & `xrootd-5.5.5/cmake/XRootDSummary.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/cmake/XRootDSystemCheck.cmake` & `xrootd-5.5.5/cmake/XRootDSystemCheck.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/cmake/XRootDUtils.cmake` & `xrootd-5.5.5/cmake/XRootDUtils.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/docs/man/cmsd.8` & `xrootd-5.5.5/docs/man/cmsd.8`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/docs/man/frm_admin.8` & `xrootd-5.5.5/docs/man/frm_admin.8`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/docs/man/frm_purged.8` & `xrootd-5.5.5/docs/man/frm_purged.8`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/docs/man/frm_xfragent.8` & `xrootd-5.5.5/docs/man/frm_xfragent.8`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/docs/man/frm_xfrd.8` & `xrootd-5.5.5/docs/man/frm_xfrd.8`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/docs/man/libXrdVoms.1` & `xrootd-5.5.5/docs/man/libXrdVoms.1`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/docs/man/mpxstats.8` & `xrootd-5.5.5/docs/man/mpxstats.8`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/docs/man/xrdadler32.1` & `xrootd-5.5.5/docs/man/xrdadler32.1`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/docs/man/xrdcp.1` & `xrootd-5.5.5/docs/man/xrdcp.1`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/docs/man/xrdfs.1` & `xrootd-5.5.5/docs/man/xrdfs.1`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/docs/man/xrdgsiproxy.1` & `xrootd-5.5.5/docs/man/xrdgsiproxy.1`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/docs/man/xrdgsitest.1` & `xrootd-5.5.5/docs/man/xrdgsitest.1`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/docs/man/xrdmapc.1` & `xrootd-5.5.5/docs/man/xrdmapc.1`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/docs/man/xrdpfc_print.8` & `xrootd-5.5.5/docs/man/xrdpfc_print.8`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/docs/man/xrdpwdadmin.8` & `xrootd-5.5.5/docs/man/xrdpwdadmin.8`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/docs/man/xrdsssadmin.8` & `xrootd-5.5.5/docs/man/xrdsssadmin.8`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/docs/man/xrootd.8` & `xrootd-5.5.5/docs/man/xrootd.8`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/docs/man/xrootdfs.1` & `xrootd-5.5.5/docs/man/xrootdfs.1`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/docs/README_IPV4_To_IPV6` & `xrootd-5.5.5/docs/README_IPV4_To_IPV6`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/docs/ReleaseNotes.txt` & `xrootd-5.5.5/docs/ReleaseNotes.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,36 @@
 XRootD
 ======
 
 Release Notes
 =============
 
 -------------
+Version 5.5.5
+-------------
+
++ **Major bug fixes**
+  **[HTTP]** Initialize SecEntity.addrInfo to avoid SEGV (issue 1986)
+  **[Server]** Allow XrdXrootdFile::Serialize() to be used to wait more than once (issue 1995)
+  **[Server]** Correct file handle returned when reusing it from external table
+  **[XrdCl]** Fix client crash on early closed connection (issue 1934)
+
++ **Minor bug fixes**
+  **[Server]** Use correct format to print size_t (issue 1989)
+  **[XrdApps]** Let XrdClProxyPlugin work with PgRead (issue 1993)
+  **[XrdCl]** Avoid possibility of Channel unregistering the wrong task (issue 1883)
+  **[XrdCl]** Fix ZipArchive issuing VectorWrite which is too large during CloseArchive (issue 2004)
+  **[XrdSys]** Avoid memory leak when overwriting the default message for EBADE
+
++ **Miscellaneous**
+  **[CMake]** Adjust build rules to not depend on scitokenscpp to build libXrdSecztn
+  **[Server,XrdPosix,XrdSecgsi]** Fix compile warnings with Clang compiler
+  **[XrdPosix]** Fix build with Clang and _FORTIFY_SOURCE enabled (issue 1975)
+
+-------------
 Version 5.5.4
 -------------
 
 + **Minor bug fixes**
  **[SSI]** Avoid file system+SSI feature interference that caused problems
  **[Server]** Fix dropped connections when link is reused (issue 1928)
  **[Server]** Limit max number of sockets in poller (issue 1962)
```

### Comparing `xrootd-5.5.4/packaging/common/client-plugin.conf.example` & `xrootd-5.5.5/packaging/common/client-plugin.conf.example`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/common/client.conf` & `xrootd-5.5.5/packaging/common/client.conf`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/common/xrootd-clustered.cfg` & `xrootd-5.5.5/packaging/common/xrootd-clustered.cfg`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/common/xrootd-filecache-clustered.cfg` & `xrootd-5.5.5/packaging/common/xrootd-filecache-clustered.cfg`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/common/xrootd-filecache-standalone.cfg` & `xrootd-5.5.5/packaging/common/xrootd-filecache-standalone.cfg`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/common/xrootd-http.cfg` & `xrootd-5.5.5/packaging/common/xrootd-http.cfg`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/common/xrootd-standalone.cfg` & `xrootd-5.5.5/packaging/common/xrootd-standalone.cfg`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/common/xrootd.logrotate` & `xrootd-5.5.5/packaging/common/xrootd.logrotate`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/common/xrootd.te` & `xrootd-5.5.5/packaging/common/xrootd.te`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/debian/control` & `xrootd-5.5.5/packaging/debian/control`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/debian/copyright` & `xrootd-5.5.5/packaging/debian/copyright`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/debian/rules` & `xrootd-5.5.5/packaging/debian/rules`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/debian/xrootd-server.install` & `xrootd-5.5.5/packaging/debian/xrootd-server.install`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/debian_scripts/publish_debian_cern.sh` & `xrootd-5.5.5/packaging/debian_scripts/publish_debian_cern.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/rhel/cmsd.init` & `xrootd-5.5.5/packaging/rhel/cmsd.init`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/rhel/frm_purged.init` & `xrootd-5.5.5/packaging/rhel/frm_purged.init`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/rhel/frm_xfrd.init` & `xrootd-5.5.5/packaging/rhel/frm_xfrd.init`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/rhel/xrootd.functions` & `xrootd-5.5.5/packaging/rhel/xrootd.functions`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/rhel/xrootd.functions-slc4` & `xrootd-5.5.5/packaging/rhel/xrootd.functions-slc4`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/rhel/xrootd.init` & `xrootd-5.5.5/packaging/rhel/xrootd.init`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/rhel/xrootd.spec.in` & `xrootd-5.5.5/packaging/rhel/xrootd.spec.in`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/rhel/xrootd.sysconfig` & `xrootd-5.5.5/packaging/rhel/xrootd.sysconfig`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/tgz/README` & `xrootd-5.5.5/packaging/tgz/README`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/tgz/StartCMS` & `xrootd-5.5.5/packaging/tgz/StartCMS`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/tgz/StartFRM` & `xrootd-5.5.5/packaging/tgz/StartFRM`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/tgz/StartOLB` & `xrootd-5.5.5/packaging/tgz/StartOLB`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/tgz/StartOLB.cf.example` & `xrootd-5.5.5/packaging/tgz/StartOLB.cf.example`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/tgz/StartXRD` & `xrootd-5.5.5/packaging/tgz/StartXRD`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/tgz/StartXRD.cf.example` & `xrootd-5.5.5/packaging/tgz/StartXRD.cf.example`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/tgz/StopCMS` & `xrootd-5.5.5/packaging/tgz/StopCMS`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/tgz/StopFRM` & `xrootd-5.5.5/packaging/tgz/StopFRM`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/tgz/StopOLB` & `xrootd-5.5.5/packaging/tgz/StopOLB`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/tgz/StopXRD` & `xrootd-5.5.5/packaging/tgz/StopXRD`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/tgz/xrootd.cf.example` & `xrootd-5.5.5/packaging/tgz/xrootd.cf.example`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/tgz/xrootd.cf.example2` & `xrootd-5.5.5/packaging/tgz/xrootd.cf.example2`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/wheel/TestCXX14.txt` & `xrootd-5.5.5/packaging/wheel/TestCXX14.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/wheel/install.sh` & `xrootd-5.5.5/packaging/wheel/install.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/wheel/publish.sh` & `xrootd-5.5.5/packaging/wheel/publish.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/wheel/setup.py` & `xrootd-5.5.5/packaging/wheel/setup.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/packaging/makesrpm.sh` & `xrootd-5.5.5/packaging/makesrpm.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XProtocol/README` & `xrootd-5.5.5/src/XProtocol/README`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XProtocol/XProtocol.cc` & `xrootd-5.5.5/src/XProtocol/XProtocol.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XProtocol/XProtocol.hh` & `xrootd-5.5.5/src/XProtocol/XProtocol.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XProtocol/XPtypes.hh` & `xrootd-5.5.5/src/XProtocol/XPtypes.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XProtocol/YProtocol.hh` & `xrootd-5.5.5/src/XProtocol/YProtocol.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdBuffXL.cc` & `xrootd-5.5.5/src/Xrd/XrdBuffXL.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdBuffXL.hh` & `xrootd-5.5.5/src/Xrd/XrdBuffXL.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdBuffer.cc` & `xrootd-5.5.5/src/Xrd/XrdBuffer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdBuffer.hh` & `xrootd-5.5.5/src/Xrd/XrdBuffer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdConfig.cc` & `xrootd-5.5.5/src/Xrd/XrdConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdConfig.hh` & `xrootd-5.5.5/src/Xrd/XrdConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdGlobals.cc` & `xrootd-5.5.5/src/Xrd/XrdGlobals.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdInet.cc` & `xrootd-5.5.5/src/Xrd/XrdInet.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdInet.hh` & `xrootd-5.5.5/src/Xrd/XrdInet.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdInfo.cc` & `xrootd-5.5.5/src/Xrd/XrdInfo.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdInfo.hh` & `xrootd-5.5.5/src/Xrd/XrdInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdJob.hh` & `xrootd-5.5.5/src/Xrd/XrdJob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdLink.cc` & `xrootd-5.5.5/src/Xrd/XrdLink.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdLink.hh` & `xrootd-5.5.5/src/Xrd/XrdLink.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdLinkCtl.cc` & `xrootd-5.5.5/src/Xrd/XrdLinkCtl.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdLinkCtl.hh` & `xrootd-5.5.5/src/Xrd/XrdLinkCtl.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdLinkInfo.hh` & `xrootd-5.5.5/src/Xrd/XrdLinkInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdLinkMatch.cc` & `xrootd-5.5.5/src/Xrd/XrdLinkMatch.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdLinkMatch.hh` & `xrootd-5.5.5/src/Xrd/XrdLinkMatch.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdLinkXeq.cc` & `xrootd-5.5.5/src/Xrd/XrdLinkXeq.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdLinkXeq.hh` & `xrootd-5.5.5/src/Xrd/XrdLinkXeq.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdMain.cc` & `xrootd-5.5.5/src/Xrd/XrdMain.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdObject.hh` & `xrootd-5.5.5/src/Xrd/XrdObject.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdObject.icc` & `xrootd-5.5.5/src/Xrd/XrdObject.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdPoll.cc` & `xrootd-5.5.5/src/Xrd/XrdPoll.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdPoll.hh` & `xrootd-5.5.5/src/Xrd/XrdPoll.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdPollE.hh` & `xrootd-5.5.5/src/Xrd/XrdPollE.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdPollE.icc` & `xrootd-5.5.5/src/Xrd/XrdPollE.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdPollInfo.hh` & `xrootd-5.5.5/src/Xrd/XrdPollInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdPollPoll.hh` & `xrootd-5.5.5/src/Xrd/XrdPollPoll.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdPollPoll.icc` & `xrootd-5.5.5/src/Xrd/XrdPollPoll.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdProtLoad.cc` & `xrootd-5.5.5/src/Xrd/XrdProtLoad.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdProtLoad.hh` & `xrootd-5.5.5/src/Xrd/XrdProtLoad.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdProtocol.hh` & `xrootd-5.5.5/src/Xrd/XrdProtocol.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdScheduler.cc` & `xrootd-5.5.5/src/Xrd/XrdScheduler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdScheduler.hh` & `xrootd-5.5.5/src/Xrd/XrdScheduler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdSendQ.cc` & `xrootd-5.5.5/src/Xrd/XrdSendQ.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdSendQ.hh` & `xrootd-5.5.5/src/Xrd/XrdSendQ.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdStats.cc` & `xrootd-5.5.5/src/Xrd/XrdStats.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdStats.hh` & `xrootd-5.5.5/src/Xrd/XrdStats.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdTcpMonPin.hh` & `xrootd-5.5.5/src/Xrd/XrdTcpMonPin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/Xrd/XrdTrace.hh` & `xrootd-5.5.5/src/Xrd/XrdTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdAcc/XrdAccAccess.cc` & `xrootd-5.5.5/src/XrdAcc/XrdAccAccess.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdAcc/XrdAccAccess.hh` & `xrootd-5.5.5/src/XrdAcc/XrdAccAccess.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdAcc/XrdAccAudit.cc` & `xrootd-5.5.5/src/XrdAcc/XrdAccAudit.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdAcc/XrdAccAudit.hh` & `xrootd-5.5.5/src/XrdAcc/XrdAccAudit.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdAcc/XrdAccAuthDB.hh` & `xrootd-5.5.5/src/XrdAcc/XrdAccAuthDB.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdAcc/XrdAccAuthFile.cc` & `xrootd-5.5.5/src/XrdAcc/XrdAccAuthFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdAcc/XrdAccAuthFile.hh` & `xrootd-5.5.5/src/XrdAcc/XrdAccAuthFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdAcc/XrdAccAuthorize.hh` & `xrootd-5.5.5/src/XrdAcc/XrdAccAuthorize.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdAcc/XrdAccCapability.cc` & `xrootd-5.5.5/src/XrdAcc/XrdAccCapability.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdAcc/XrdAccCapability.hh` & `xrootd-5.5.5/src/XrdAcc/XrdAccCapability.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdAcc/XrdAccConfig.cc` & `xrootd-5.5.5/src/XrdAcc/XrdAccConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdAcc/XrdAccConfig.hh` & `xrootd-5.5.5/src/XrdAcc/XrdAccConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdAcc/XrdAccEntity.cc` & `xrootd-5.5.5/src/XrdAcc/XrdAccEntity.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdAcc/XrdAccEntity.hh` & `xrootd-5.5.5/src/XrdAcc/XrdAccEntity.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdAcc/XrdAccGroups.cc` & `xrootd-5.5.5/src/XrdAcc/XrdAccGroups.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdAcc/XrdAccGroups.hh` & `xrootd-5.5.5/src/XrdAcc/XrdAccGroups.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdAcc/XrdAccPrivs.hh` & `xrootd-5.5.5/src/XrdAcc/XrdAccPrivs.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdClProxyPlugin/ProxyPrefixFile.cc` & `xrootd-5.5.5/src/XrdApps/XrdClProxyPlugin/ProxyPrefixFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdClProxyPlugin/ProxyPrefixFile.hh` & `xrootd-5.5.5/src/XrdApps/XrdClProxyPlugin/ProxyPrefixFile.hh`

 * *Files 20% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 // or submit itself to any jurisdiction.
 //------------------------------------------------------------------------------
 
 #pragma once
 #include "XrdCl/XrdClDefaultEnv.hh"
 #include "XrdCl/XrdClPlugInInterface.hh"
 
+#include <utility>
+
 using namespace XrdCl;
 
 namespace xrdcl_proxy
 {
 //------------------------------------------------------------------------------
 //! XrdClFile plugin that appends an URL prefix to the given URL. The URL
 //! prefix is set as an environment variable XRD_URL_PREFIX.
@@ -41,140 +43,211 @@
   //! Constructor
   //----------------------------------------------------------------------------
   ProxyPrefixFile();
 
   //----------------------------------------------------------------------------
   //! Destructor
   //----------------------------------------------------------------------------
-  virtual ~ProxyPrefixFile();
+  virtual ~ProxyPrefixFile() override;
 
   //----------------------------------------------------------------------------
   //! Open
   //----------------------------------------------------------------------------
   virtual XRootDStatus Open(const std::string& url,
                             OpenFlags::Flags flags,
                             Access::Mode mode,
                             ResponseHandler* handler,
-                            uint16_t timeout);
+                            uint16_t timeout) override;
 
   //----------------------------------------------------------------------------
   //! Close
   //----------------------------------------------------------------------------
   virtual XRootDStatus Close(ResponseHandler* handler,
-                             uint16_t         timeout)
+                             uint16_t         timeout) override
   {
     return pFile->Close(handler, timeout);
   }
 
   //----------------------------------------------------------------------------
   //! Stat
   //----------------------------------------------------------------------------
   virtual XRootDStatus Stat(bool             force,
                             ResponseHandler* handler,
-                            uint16_t         timeout)
+                            uint16_t         timeout) override
   {
     return pFile->Stat(force, handler, timeout);
   }
 
 
   //----------------------------------------------------------------------------
   //! Read
   //----------------------------------------------------------------------------
   virtual XRootDStatus Read(uint64_t         offset,
                             uint32_t         size,
                             void*            buffer,
                             ResponseHandler* handler,
-                            uint16_t         timeout)
+                            uint16_t         timeout) override
   {
     return pFile->Read(offset, size, buffer, handler, timeout);
   }
 
+  //------------------------------------------------------------------------
+  //! PgRead
+  //------------------------------------------------------------------------
+  virtual XRootDStatus PgRead( uint64_t         offset,
+                               uint32_t         size,
+                               void            *buffer,
+                               ResponseHandler *handler,
+                               uint16_t         timeout ) override
+  {
+    return pFile->PgRead(offset, size, buffer, handler, timeout);
+  }
+
   //----------------------------------------------------------------------------
   //! Write
   //----------------------------------------------------------------------------
   virtual XRootDStatus Write(uint64_t         offset,
                              uint32_t         size,
                              const void*      buffer,
                              ResponseHandler* handler,
-                             uint16_t         timeout)
+                             uint16_t         timeout) override
   {
     return pFile->Write(offset, size, buffer, handler, timeout);
   }
 
+  //------------------------------------------------------------------------
+  //! Write
+  //------------------------------------------------------------------------
+  virtual XRootDStatus Write( uint64_t          offset,
+                              Buffer          &&buffer,
+                              ResponseHandler  *handler,
+                              uint16_t          timeout = 0 ) override
+  {
+    return pFile->Write(offset, std::move(buffer), handler, timeout);
+  }
+
+  //------------------------------------------------------------------------
+  //! Write
+  //------------------------------------------------------------------------
+  virtual XRootDStatus Write( uint64_t            offset,
+                              uint32_t            size,
+                              Optional<uint64_t>  fdoff,
+                              int                 fd,
+                              ResponseHandler    *handler,
+                              uint16_t            timeout = 0 ) override
+  {
+    return pFile->Write(offset, size, fdoff, fd, handler, timeout);
+  }
+
+  //------------------------------------------------------------------------
+  //! PgWrite
+  //------------------------------------------------------------------------
+  virtual XRootDStatus PgWrite( uint64_t               offset,
+                                uint32_t               nbpgs,
+                                const void            *buffer,
+                                std::vector<uint32_t> &cksums,
+                                ResponseHandler       *handler,
+                                uint16_t               timeout ) override
+  {
+    return pFile->PgWrite(offset, nbpgs, buffer, cksums, handler, timeout);
+  }
+
   //----------------------------------------------------------------------------
   //! Sync
   //----------------------------------------------------------------------------
   virtual XRootDStatus Sync(ResponseHandler* handler,
-                            uint16_t         timeout)
+                            uint16_t         timeout) override
   {
     return pFile->Sync(handler, timeout);
   }
 
   //----------------------------------------------------------------------------
   //! Truncate
   //----------------------------------------------------------------------------
   virtual XRootDStatus Truncate(uint64_t         size,
                                 ResponseHandler* handler,
-                                uint16_t         timeout)
+                                uint16_t         timeout) override
   {
     return pFile->Truncate(size, handler, timeout);
   }
 
   //----------------------------------------------------------------------------
   //! VectorRead
   //----------------------------------------------------------------------------
   virtual XRootDStatus VectorRead(const ChunkList& chunks,
                                   void*            buffer,
                                   ResponseHandler* handler,
-                                  uint16_t         timeout)
+                                  uint16_t         timeout) override
   {
     return pFile->VectorRead(chunks, buffer, handler, timeout);
   }
 
+  //------------------------------------------------------------------------
+  //! VectorWrite
+  //------------------------------------------------------------------------
+  virtual XRootDStatus VectorWrite( const ChunkList &chunks,
+                                    ResponseHandler *handler,
+                                    uint16_t         timeout = 0 ) override
+  {
+    return pFile->VectorWrite(chunks, handler, timeout);
+  }
+
+  //------------------------------------------------------------------------
+  //! @see XrdCl::File::WriteV
+  //------------------------------------------------------------------------
+  virtual XRootDStatus WriteV( uint64_t            offset,
+                               const struct iovec *iov,
+                               int                 iovcnt,
+                               ResponseHandler    *handler,
+                               uint16_t            timeout = 0 ) override
+  {
+    return pFile->WriteV(offset, iov, iovcnt, handler, timeout);
+  }
+
   //----------------------------------------------------------------------------
   //! Fcntl
   //----------------------------------------------------------------------------
   virtual XRootDStatus Fcntl(const Buffer&    arg,
                              ResponseHandler* handler,
-                             uint16_t         timeout)
+                             uint16_t         timeout) override
   {
     return pFile->Fcntl(arg, handler, timeout);
   }
 
   //----------------------------------------------------------------------------
   //! Visa
   //----------------------------------------------------------------------------
   virtual XRootDStatus Visa(ResponseHandler* handler,
-                            uint16_t         timeout)
+                            uint16_t         timeout) override
   {
     return pFile->Visa(handler, timeout);
   }
 
   //----------------------------------------------------------------------------
   //! IsOpen
   //----------------------------------------------------------------------------
-  virtual bool IsOpen() const
+  virtual bool IsOpen() const override
   {
     return pFile->IsOpen();
   }
 
   //----------------------------------------------------------------------------
   //! SetProperty
   //----------------------------------------------------------------------------
   virtual bool SetProperty(const std::string& name,
-                           const std::string& value)
+                           const std::string& value) override
   {
     return pFile->SetProperty(name, value);
   }
 
   //----------------------------------------------------------------------------
   //! GetProperty
   //----------------------------------------------------------------------------
   virtual bool GetProperty(const std::string& name,
-                           std::string& value) const
+                           std::string& value) const override
   {
     return pFile->GetProperty(name, value);
   }
 
 private:
 
   //----------------------------------------------------------------------------
```

### Comparing `xrootd-5.5.4/src/XrdApps/XrdClProxyPlugin/ProxyPrefixPlugin.cc` & `xrootd-5.5.5/src/XrdApps/XrdClProxyPlugin/ProxyPrefixPlugin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdClProxyPlugin/ProxyPrefixPlugin.hh` & `xrootd-5.5.5/src/XrdApps/XrdClProxyPlugin/ProxyPrefixPlugin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdClProxyPlugin/README.md` & `xrootd-5.5.5/src/XrdApps/XrdClProxyPlugin/README.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdClRecordPlugin/README.md` & `xrootd-5.5.5/src/XrdApps/XrdClRecordPlugin/README.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdClRecordPlugin/XrdClAction.hh` & `xrootd-5.5.5/src/XrdApps/XrdClRecordPlugin/XrdClAction.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdClRecordPlugin/XrdClActionMetrics.hh` & `xrootd-5.5.5/src/XrdApps/XrdClRecordPlugin/XrdClActionMetrics.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdClRecordPlugin/XrdClRecorder.hh` & `xrootd-5.5.5/src/XrdApps/XrdClRecordPlugin/XrdClRecorder.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdClRecordPlugin/XrdClRecorderPlugin.cc` & `xrootd-5.5.5/src/XrdApps/XrdClRecordPlugin/XrdClRecorderPlugin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdClRecordPlugin/XrdClRecorderPlugin.hh` & `xrootd-5.5.5/src/XrdApps/XrdClRecordPlugin/XrdClRecorderPlugin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdClRecordPlugin/XrdClReplay.cc` & `xrootd-5.5.5/src/XrdApps/XrdClRecordPlugin/XrdClReplay.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdClRecordPlugin/XrdClReplayArgs.hh` & `xrootd-5.5.5/src/XrdApps/XrdClRecordPlugin/XrdClReplayArgs.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdAccTest.cc` & `xrootd-5.5.5/src/XrdApps/XrdAccTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdAppsCconfig.cc` & `xrootd-5.5.5/src/XrdApps/XrdAppsCconfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdCks.cc` & `xrootd-5.5.5/src/XrdApps/XrdCks.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdCpConfig.cc` & `xrootd-5.5.5/src/XrdApps/XrdCpConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdCpConfig.hh` & `xrootd-5.5.5/src/XrdApps/XrdCpConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdCpFile.cc` & `xrootd-5.5.5/src/XrdApps/XrdCpFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdCpFile.hh` & `xrootd-5.5.5/src/XrdApps/XrdCpFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdCrc32c.cc` & `xrootd-5.5.5/src/XrdApps/XrdCrc32c.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdMapCluster.cc` & `xrootd-5.5.5/src/XrdApps/XrdMapCluster.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdMpxStats.cc` & `xrootd-5.5.5/src/XrdApps/XrdMpxStats.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdMpxXml.cc` & `xrootd-5.5.5/src/XrdApps/XrdMpxXml.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdMpxXml.hh` & `xrootd-5.5.5/src/XrdApps/XrdMpxXml.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdPinls.cc` & `xrootd-5.5.5/src/XrdApps/XrdPinls.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdPrep.cc` & `xrootd-5.5.5/src/XrdApps/XrdPrep.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdQStats.cc` & `xrootd-5.5.5/src/XrdApps/XrdQStats.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/XrdWait41.cc` & `xrootd-5.5.5/src/XrdApps/XrdWait41.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps/Xrdadler32.cc` & `xrootd-5.5.5/src/XrdApps/Xrdadler32.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdBwm/XrdBwm.cc` & `xrootd-5.5.5/src/XrdBwm/XrdBwm.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdBwm/XrdBwm.hh` & `xrootd-5.5.5/src/XrdBwm/XrdBwm.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdBwm/XrdBwmConfig.cc` & `xrootd-5.5.5/src/XrdBwm/XrdBwmConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdBwm/XrdBwmHandle.cc` & `xrootd-5.5.5/src/XrdBwm/XrdBwmHandle.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdBwm/XrdBwmHandle.hh` & `xrootd-5.5.5/src/XrdBwm/XrdBwmHandle.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdBwm/XrdBwmLogger.cc` & `xrootd-5.5.5/src/XrdBwm/XrdBwmLogger.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdBwm/XrdBwmLogger.hh` & `xrootd-5.5.5/src/XrdBwm/XrdBwmLogger.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdBwm/XrdBwmPolicy.hh` & `xrootd-5.5.5/src/XrdBwm/XrdBwmPolicy.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdBwm/XrdBwmPolicy1.cc` & `xrootd-5.5.5/src/XrdBwm/XrdBwmPolicy1.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdBwm/XrdBwmPolicy1.hh` & `xrootd-5.5.5/src/XrdBwm/XrdBwmPolicy1.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdBwm/XrdBwmTrace.hh` & `xrootd-5.5.5/src/XrdBwm/XrdBwmTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCks.hh` & `xrootd-5.5.5/src/XrdCks/XrdCks.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksAssist.cc` & `xrootd-5.5.5/src/XrdCks/XrdCksAssist.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksAssist.hh` & `xrootd-5.5.5/src/XrdCks/XrdCksAssist.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksCalc.hh` & `xrootd-5.5.5/src/XrdCks/XrdCksCalc.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksCalcadler32.hh` & `xrootd-5.5.5/src/XrdCks/XrdCksCalcadler32.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksCalccrc32.cc` & `xrootd-5.5.5/src/XrdCks/XrdCksCalccrc32.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksCalccrc32.hh` & `xrootd-5.5.5/src/XrdCks/XrdCksCalccrc32.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksCalccrc32C.cc` & `xrootd-5.5.5/src/XrdCks/XrdCksCalccrc32C.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksCalccrc32C.hh` & `xrootd-5.5.5/src/XrdCks/XrdCksCalccrc32C.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksCalcmd5.cc` & `xrootd-5.5.5/src/XrdCks/XrdCksCalcmd5.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksCalcmd5.hh` & `xrootd-5.5.5/src/XrdCks/XrdCksCalcmd5.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksCalczcrc32.cc` & `xrootd-5.5.5/src/XrdCks/XrdCksCalczcrc32.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksConfig.cc` & `xrootd-5.5.5/src/XrdCks/XrdCksConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksConfig.hh` & `xrootd-5.5.5/src/XrdCks/XrdCksConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksData.hh` & `xrootd-5.5.5/src/XrdCks/XrdCksData.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksLoader.cc` & `xrootd-5.5.5/src/XrdCks/XrdCksLoader.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksLoader.hh` & `xrootd-5.5.5/src/XrdCks/XrdCksLoader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksManOss.cc` & `xrootd-5.5.5/src/XrdCks/XrdCksManOss.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksManOss.hh` & `xrootd-5.5.5/src/XrdCks/XrdCksManOss.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksManager.cc` & `xrootd-5.5.5/src/XrdCks/XrdCksManager.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksManager.hh` & `xrootd-5.5.5/src/XrdCks/XrdCksManager.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksWrapper.hh` & `xrootd-5.5.5/src/XrdCks/XrdCksWrapper.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCks/XrdCksXAttr.hh` & `xrootd-5.5.5/src/XrdCks/XrdCksXAttr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/CMakeLists.txt` & `xrootd-5.5.5/src/XrdCl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClAnyObject.hh` & `xrootd-5.5.5/src/XrdCl/XrdClAnyObject.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClApply.hh` & `xrootd-5.5.5/src/XrdCl/XrdClApply.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClArg.hh` & `xrootd-5.5.5/src/XrdCl/XrdClArg.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClAsyncDiscardReader.hh` & `xrootd-5.5.5/src/XrdCl/XrdClAsyncDiscardReader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClAsyncHSReader.hh` & `xrootd-5.5.5/src/XrdCl/XrdClAsyncHSReader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClAsyncHSWriter.hh` & `xrootd-5.5.5/src/XrdCl/XrdClAsyncHSWriter.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClAsyncMsgReader.hh` & `xrootd-5.5.5/src/XrdCl/XrdClAsyncMsgReader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClAsyncMsgWriter.hh` & `xrootd-5.5.5/src/XrdCl/XrdClAsyncMsgWriter.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClAsyncPageReader.hh` & `xrootd-5.5.5/src/XrdCl/XrdClAsyncPageReader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClAsyncRawReader.hh` & `xrootd-5.5.5/src/XrdCl/XrdClAsyncRawReader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClAsyncRawReaderIntfc.hh` & `xrootd-5.5.5/src/XrdCl/XrdClAsyncRawReaderIntfc.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClAsyncSocketHandler.cc` & `xrootd-5.5.5/src/XrdCl/XrdClAsyncSocketHandler.cc`

 * *Files 10% similar despite different names*

```diff
@@ -132,14 +132,17 @@
       if( !st.IsOK() )
         log->Error( AsyncSockMsg, "[%s] Unable to set keepalive probes: %s",
                     st.ToString().c_str() );
 #endif
     }
 
     pHandShakeDone = false;
+    pTlsHandShakeOngoing = false;
+    pHSWaitStarted = 0;
+    pHSWaitSeconds = 0;
 
     //--------------------------------------------------------------------------
     // Initiate async connection to the address
     //--------------------------------------------------------------------------
     char nameBuff[256];
     pSockAddr.Format( nameBuff, sizeof(nameBuff), XrdNetAddrInfo::fmtAdv6 );
     log->Debug( AsyncSockMsg, "[%s] Attempting connection to %s",
@@ -210,79 +213,112 @@
     // First check if the socket itself wants to apply some mapping on the
     // event. E.g. in case of TLS socket it might want to map read events to
     // write events and vice-versa.
     //--------------------------------------------------------------------------
     type = pSocket->MapEvent( type );
 
     //--------------------------------------------------------------------------
+    // Handle any read or write events. If any of the handlers indicate an error
+    // we will have been disconnected. A disconnection may cause the current
+    // object to be asynchronously reused or deleted, so we return immediately.
+    //--------------------------------------------------------------------------
+    if( !EventRead( type ) )
+      return;
+
+    if( !EventWrite( type ) )
+      return;
+  }
+
+  //----------------------------------------------------------------------------
+  // Handler for read related socket events
+  //----------------------------------------------------------------------------
+  bool AsyncSocketHandler::EventRead( uint8_t type )
+  {
+    //--------------------------------------------------------------------------
     // Read event
     //--------------------------------------------------------------------------
     if( type & ReadyToRead )
     {
       pLastActivity = time(0);
       if( unlikely( pTlsHandShakeOngoing ) )
-        OnTLSHandShake();
-      else if( likely( pHandShakeDone ) )
-        OnRead();
-      else
-        OnReadWhileHandshaking();
+        return OnTLSHandShake();
+
+      if( likely( pHandShakeDone ) )
+        return OnRead();
+
+      return OnReadWhileHandshaking();
     }
 
     //--------------------------------------------------------------------------
     // Read timeout
     //--------------------------------------------------------------------------
     else if( type & ReadTimeOut )
     {
       if( pHSWaitSeconds )
-        CheckHSWait();
+      {
+        if( !CheckHSWait() )
+          return false;
+      }
 
       if( likely( pHandShakeDone ) )
-        OnReadTimeout();
-      else
-        OnTimeoutWhileHandshaking();
+        return OnReadTimeout();
+
+      return OnTimeoutWhileHandshaking();
     }
 
+    return true;
+  }
+
+  //----------------------------------------------------------------------------
+  // Handler for write related socket events
+  //----------------------------------------------------------------------------
+  bool AsyncSocketHandler::EventWrite( uint8_t type )
+  {
     //--------------------------------------------------------------------------
     // Write event
     //--------------------------------------------------------------------------
     if( type & ReadyToWrite )
     {
       pLastActivity = time(0);
       if( unlikely( pSocket->GetStatus() == Socket::Connecting ) )
-        OnConnectionReturn();
+        return OnConnectionReturn();
+
       //------------------------------------------------------------------------
       // Make sure we are not writing anything if we have been told to wait.
       //------------------------------------------------------------------------
-      else if( pHSWaitSeconds == 0 )
-      {
-        if( unlikely( pTlsHandShakeOngoing ) )
-          OnTLSHandShake();
-        else if( likely( pHandShakeDone ) )
-          OnWrite();
-        else
-          OnWriteWhileHandshaking();
-      }
+      if( pHSWaitSeconds != 0 )
+        return true;
+
+      if( unlikely( pTlsHandShakeOngoing ) )
+        return OnTLSHandShake();
+
+      if( likely( pHandShakeDone ) )
+        return OnWrite();
+
+      return OnWriteWhileHandshaking();
     }
 
     //--------------------------------------------------------------------------
     // Write timeout
     //--------------------------------------------------------------------------
     else if( type & WriteTimeOut )
     {
       if( likely( pHandShakeDone ) )
-        OnWriteTimeout();
-      else
-        OnTimeoutWhileHandshaking();
+        return OnWriteTimeout();
+
+      return OnTimeoutWhileHandshaking();
     }
+
+    return true;
   }
 
   //----------------------------------------------------------------------------
   // Connect returned
   //----------------------------------------------------------------------------
-  void AsyncSocketHandler::OnConnectionReturn()
+  bool AsyncSocketHandler::OnConnectionReturn()
   {
     //--------------------------------------------------------------------------
     // Check whether we were able to connect
     //--------------------------------------------------------------------------
     Log *log = DefaultEnv::GetLog();
     log->Debug( AsyncSockMsg, "[%s] Async connection call returned",
                 pStreamName.c_str() );
@@ -299,38 +335,38 @@
     if( !st.IsOK() )
     {
       log->Error( AsyncSockMsg, "[%s] Unable to get the status of the "
                   "connect operation: %s", pStreamName.c_str(),
                   XrdSysE2T( errno ) );
       pStream->OnConnectError( pSubStreamNum,
                                XRootDStatus( stFatal, errSocketOptError, errno ) );
-      return;
+      return false;
     }
 
     //--------------------------------------------------------------------------
     // We were unable to connect
     //--------------------------------------------------------------------------
     if( errorCode )
     {
       log->Error( AsyncSockMsg, "[%s] Unable to connect: %s",
                   pStreamName.c_str(), XrdSysE2T( errorCode ) );
       pStream->OnConnectError( pSubStreamNum,
                                XRootDStatus( stError, errConnectionError ) );
-      return;
+      return false;
     }
     pSocket->SetStatus( Socket::Connected );
 
     //--------------------------------------------------------------------------
     // Cork the socket
     //--------------------------------------------------------------------------
     st = pSocket->Cork();
     if( !st.IsOK() )
     {
       pStream->OnConnectError( pSubStreamNum, st );
-      return;
+      return false;
     }
 
     //--------------------------------------------------------------------------
     // Initialize the handshake
     //--------------------------------------------------------------------------
     pHandShakeData.reset( new HandShakeData( pStream->GetURL(),
                                         pSubStreamNum ) );
@@ -340,15 +376,15 @@
 
     st = pTransport->HandShake( pHandShakeData.get(), *pChannelData );
     if( !st.IsOK() )
     {
       log->Error( AsyncSockMsg, "[%s] Connection negotiation failed",
                   pStreamName.c_str() );
       pStream->OnConnectError( pSubStreamNum, st );
-      return;
+      return false;
     }
 
     if( st.code != suRetry )
       ++pHandShakeData->step;
 
     //--------------------------------------------------------------------------
     // Initialize the hand-shake reader and writer
@@ -368,171 +404,181 @@
     //--------------------------------------------------------------------------
     // Listen to what the server has to say
     //--------------------------------------------------------------------------
     if( !pPoller->EnableReadNotification( pSocket, true, pTimeoutResolution ) )
     {
       pStream->OnConnectError( pSubStreamNum,
                                XRootDStatus( stFatal, errPollerError ) );
-      return;
+      return false;
     }
+    return true;
   }
 
   //----------------------------------------------------------------------------
   // Got a write readiness event
   //----------------------------------------------------------------------------
-  void AsyncSocketHandler::OnWrite()
+  bool AsyncSocketHandler::OnWrite()
   {
     if( !reqwriter )
     {
       OnFault( XRootDStatus( stError, errInternal, 0, "Request writer is null." ) );
-      return;
+      return false;
     }
     //--------------------------------------------------------------------------
     // Let's do the writing ...
     //--------------------------------------------------------------------------
     XRootDStatus st = reqwriter->Write();
     if( !st.IsOK() )
     {
       //------------------------------------------------------------------------
       // We failed
       //------------------------------------------------------------------------
       OnFault( st );
-      return;
+      return false;
     }
     //--------------------------------------------------------------------------
     // We are not done yet
     //--------------------------------------------------------------------------
-    if( st.code == suRetry) return;
+    if( st.code == suRetry) return true;
     //--------------------------------------------------------------------------
     // Disable the respective substream if empty
     //--------------------------------------------------------------------------
     reqwriter->Reset();
     pStream->DisableIfEmpty( pSubStreamNum );
+    return true;
   }
 
   //----------------------------------------------------------------------------
   // Got a write readiness event while handshaking
   //----------------------------------------------------------------------------
-  void AsyncSocketHandler::OnWriteWhileHandshaking()
+  bool AsyncSocketHandler::OnWriteWhileHandshaking()
   {
     XRootDStatus st;
     if( !hswriter || !hswriter->HasMsg() )
     {
       if( !(st = DisableUplink()).IsOK() )
+      {
         OnFaultWhileHandshaking( st );
-      return;
+        return false;
+      }
+      return true;
     }
     //--------------------------------------------------------------------------
     // Let's do the writing ...
     //--------------------------------------------------------------------------
     st = hswriter->Write();
     if( !st.IsOK() )
     {
       //------------------------------------------------------------------------
       // We failed
       //------------------------------------------------------------------------
       OnFaultWhileHandshaking( st );
-      return;
+      return false;
     }
     //--------------------------------------------------------------------------
     // We are not done yet
     //--------------------------------------------------------------------------
-    if( st.code == suRetry ) return;
+    if( st.code == suRetry ) return true;
     //--------------------------------------------------------------------------
     // Disable the uplink
     // Note: at this point we don't deallocate the HS message as we might need
     //       to re-send it in case of a kXR_wait response
     //--------------------------------------------------------------------------
     if( !(st = DisableUplink()).IsOK() )
+    {
       OnFaultWhileHandshaking( st );
+      return false;
+    }
+    return true;
   }
 
   //----------------------------------------------------------------------------
   // Got a read readiness event
   //----------------------------------------------------------------------------
-  void AsyncSocketHandler::OnRead()
+  bool AsyncSocketHandler::OnRead()
   {
     //--------------------------------------------------------------------------
     // Make sure the response reader object exists
     //--------------------------------------------------------------------------
     if( !rspreader )
     {
       OnFault( XRootDStatus( stError, errInternal, 0, "Response reader is null." ) );
-      return;
+      return false;
     }
 
     //--------------------------------------------------------------------------
     // Readout the data from the socket
     //--------------------------------------------------------------------------
     XRootDStatus st = rspreader->Read();
 
     //--------------------------------------------------------------------------
     // Handler header corruption
     //--------------------------------------------------------------------------
     if( !st.IsOK() && st.code == errCorruptedHeader )
     {
       OnHeaderCorruption();
-      return;
+      return false;
     }
 
     //--------------------------------------------------------------------------
     // Handler other errors
     //--------------------------------------------------------------------------
     if( !st.IsOK() )
     {
       OnFault( st );
-      return;
+      return false;
     }
 
     //--------------------------------------------------------------------------
     // We are not done yet
     //--------------------------------------------------------------------------
-    if( st.code == suRetry ) return;
+    if( st.code == suRetry ) return true;
 
     //--------------------------------------------------------------------------
     // We are done, reset the response reader so we can read out next message
     //--------------------------------------------------------------------------
     rspreader->Reset();
+    return true;
   }
 
   //----------------------------------------------------------------------------
   // Got a read readiness event while handshaking
   //----------------------------------------------------------------------------
-  void AsyncSocketHandler::OnReadWhileHandshaking()
+  bool AsyncSocketHandler::OnReadWhileHandshaking()
   {
     //--------------------------------------------------------------------------
     // Make sure the response reader object exists
     //--------------------------------------------------------------------------
     if( !hsreader )
     {
       OnFault( XRootDStatus( stError, errInternal, 0, "Hand-shake reader is null." ) );
-      return;
+      return false;
     }
 
     //--------------------------------------------------------------------------
     // Read the message and let the transport handler look at it when
     // reading has finished
     //--------------------------------------------------------------------------
     XRootDStatus st = hsreader->Read();
     if( !st.IsOK() )
     {
       OnFaultWhileHandshaking( st );
-      return;
+      return false;
     }
 
     if( st.code != suDone )
-      return;
+      return true;
 
-    HandleHandShake( hsreader->ReleaseMsg() );
+    return HandleHandShake( hsreader->ReleaseMsg() );
   }
 
   //------------------------------------------------------------------------
   // Handle the handshake message
   //------------------------------------------------------------------------
-  void AsyncSocketHandler::HandleHandShake( std::unique_ptr<Message> msg )
+  bool AsyncSocketHandler::HandleHandShake( std::unique_ptr<Message> msg )
   {
     //--------------------------------------------------------------------------
     // OK, we have a new message, let's deal with it;
     //--------------------------------------------------------------------------
     pHandShakeData->in = msg.release();
     XRootDStatus st = pTransport->HandShake( pHandShakeData.get(), *pChannelData );
 
@@ -543,15 +589,15 @@
 
     delete pHandShakeData->in;
     pHandShakeData->in = 0;
 
     if( !st.IsOK() )
     {
       OnFaultWhileHandshaking( st );
-      return;
+      return false;
     }
 
     if( st.code == suRetry )
     {
       //------------------------------------------------------------------------
       // We are handling a wait response and the transport handler told
       // as to retry the request
@@ -564,59 +610,62 @@
           Log *log = DefaultEnv::GetLog();
           log->Error( AsyncSockMsg,
                       "[%s] Won't retry kXR_endsess request because would"
                       "reach connection timeout.",
                       pStreamName.c_str() );
 
           OnFaultWhileHandshaking( XRootDStatus( stError, errSocketTimeout ) );
+          return false;
         }
         else
         {
           //--------------------------------------------------------------------
           // We need to wait before replaying the request
           //--------------------------------------------------------------------
           Log *log = DefaultEnv::GetLog();
           log->Debug( AsyncSockMsg, "[%s] Received a wait response to endsess request, "
                       "will wait for %d seconds before replaying the endsess request",
                       waitSeconds );
           pHSWaitStarted = time( 0 );
           pHSWaitSeconds = waitSeconds;
         }
-        return;
+        return true;
       }
       //------------------------------------------------------------------------
       // We are re-sending a protocol request
       //------------------------------------------------------------------------
       else if( pHandShakeData->out )
       {
-        SendHSMsg();
-        return;
+        return SendHSMsg();
       }
     }
 
     //--------------------------------------------------------------------------
     // If now is the time to enable encryption
     //--------------------------------------------------------------------------
     if( !pSocket->IsEncrypted() &&
          pTransport->NeedEncryption( pHandShakeData.get(), *pChannelData ) )
     {
       XRootDStatus st = DoTlsHandShake();
-      if( !st.IsOK() || st.code == suRetry ) return;
+      if( !st.IsOK() )
+        return false;
+      if ( st.code == suRetry )
+        return true;
     }
 
     //--------------------------------------------------------------------------
     // Now prepare the next step of the hand-shake procedure
     //--------------------------------------------------------------------------
-    HandShakeNextStep( st.IsOK() && st.code == suDone );
+    return HandShakeNextStep( st.IsOK() && st.code == suDone );
   }
 
   //------------------------------------------------------------------------
   // Prepare the next step of the hand-shake procedure
   //------------------------------------------------------------------------
-  void AsyncSocketHandler::HandShakeNextStep( bool done )
+  bool AsyncSocketHandler::HandShakeNextStep( bool done )
   {
     //--------------------------------------------------------------------------
     // We successfully proceeded to the next step
     //--------------------------------------------------------------------------
     ++pHandShakeData->step;
 
     //--------------------------------------------------------------------------
@@ -632,26 +681,27 @@
       //------------------------------------------------------------------------
       reqwriter.reset( new AsyncMsgWriter( *pTransport, *pSocket, pStreamName, *pStream, pSubStreamNum, *pChannelData ) );
       rspreader.reset( new AsyncMsgReader( *pTransport, *pSocket, pStreamName, *pStream, pSubStreamNum ) );
       XRootDStatus st;
       if( !(st = EnableUplink()).IsOK() )
       {
         OnFaultWhileHandshaking( st );
-        return;
+        return false;
       }
       pHandShakeDone = true;
       pStream->OnConnect( pSubStreamNum );
     }
     //--------------------------------------------------------------------------
     // The transport handler gave us something to write
     //--------------------------------------------------------------------------
     else if( pHandShakeData->out )
     {
-      SendHSMsg();
+      return SendHSMsg();
     }
+    return true;
   }
 
   //----------------------------------------------------------------------------
   // Handle fault
   //----------------------------------------------------------------------------
   void AsyncSocketHandler::OnFault( XRootDStatus st )
   {
@@ -673,35 +723,39 @@
 
     pStream->OnConnectError( pSubStreamNum, st );
   }
 
   //----------------------------------------------------------------------------
   // Handle write timeout
   //----------------------------------------------------------------------------
-  void AsyncSocketHandler::OnWriteTimeout()
+  bool AsyncSocketHandler::OnWriteTimeout()
   {
-    pStream->OnWriteTimeout( pSubStreamNum );
+    return pStream->OnWriteTimeout( pSubStreamNum );
   }
 
   //----------------------------------------------------------------------------
   // Handler read timeout
   //----------------------------------------------------------------------------
-  void AsyncSocketHandler::OnReadTimeout()
+  bool AsyncSocketHandler::OnReadTimeout()
   {
-    pStream->OnReadTimeout( pSubStreamNum );
+    return pStream->OnReadTimeout( pSubStreamNum );
   }
 
   //----------------------------------------------------------------------------
   // Handle timeout while handshaking
   //----------------------------------------------------------------------------
-  void AsyncSocketHandler::OnTimeoutWhileHandshaking()
+  bool AsyncSocketHandler::OnTimeoutWhileHandshaking()
   {
     time_t now = time(0);
     if( now > pConnectionStarted+pConnectionTimeout )
+    {
       OnFaultWhileHandshaking( XRootDStatus( stError, errSocketTimeout ) );
+      return false;
+    }
+    return true;
   }
 
   //----------------------------------------------------------------------------
   // Handle header corruption in case of kXR_status response
   //----------------------------------------------------------------------------
   void AsyncSocketHandler::OnHeaderCorruption()
   {
@@ -719,16 +773,16 @@
   {
     Log *log = DefaultEnv::GetLog();
     log->Debug( AsyncSockMsg, "[%s] TLS hand-shake exchange.", pStreamName.c_str() );
 
     XRootDStatus st;
     if( !( st = pSocket->TlsHandShake( this, pUrl.GetHostName() ) ).IsOK() )
     {
-      OnFaultWhileHandshaking( st );
       pTlsHandShakeOngoing = false;
+      OnFaultWhileHandshaking( st );
       return st;
     }
 
     if( st.code == suRetry )
     {
       pTlsHandShakeOngoing = true;
       return st;
@@ -739,33 +793,36 @@
 
     return st;
   }
 
   //----------------------------------------------------------------------------
   // Handle read/write event if we are in the middle of a TLS hand-shake
   //----------------------------------------------------------------------------
-  inline void AsyncSocketHandler::OnTLSHandShake()
+  inline bool AsyncSocketHandler::OnTLSHandShake()
   {
     XRootDStatus st = DoTlsHandShake();
-    if( !st.IsOK() || st.code == suRetry ) return;
+    if( !st.IsOK() )
+      return false;
+    if ( st.code == suRetry )
+      return true;
 
-    HandShakeNextStep( pTransport->HandShakeDone( pHandShakeData.get(),
-                                                  *pChannelData ) );
+    return HandShakeNextStep( pTransport->HandShakeDone( pHandShakeData.get(),
+                                                         *pChannelData ) );
   }
 
   //----------------------------------------------------------------------------
   // Prepare a HS writer for sending and enable uplink
   //----------------------------------------------------------------------------
-  void AsyncSocketHandler::SendHSMsg()
+  bool AsyncSocketHandler::SendHSMsg()
   {
     if( !hswriter )
     {
       OnFaultWhileHandshaking( XRootDStatus( stError, errInternal, 0,
                                              "HS writer object missing!" ) );
-      return;
+      return false;
     }
     //--------------------------------------------------------------------------
     // We only set a new HS message if this is not a replay due to kXR_wait
     //--------------------------------------------------------------------------
     if( !pHSWaitSeconds )
     {
       hswriter->Reset( pHandShakeData->out );
@@ -779,16 +836,17 @@
     //--------------------------------------------------------------------------
     // Enable writing so we can replay the HS message
     //--------------------------------------------------------------------------
     XRootDStatus st;
     if( !(st = EnableUplink()).IsOK() )
     {
       OnFaultWhileHandshaking( st );
-      return;
+      return false;
     }
+    return true;
   }
 
   kXR_int32 AsyncSocketHandler::HandleWaitRsp( Message *msg )
   {
     // It would be more coherent if this could be done in the
     // transport layer, unfortunately the API does not allow it.
     kXR_int32 waitSeconds = -1;
@@ -797,29 +855,31 @@
       waitSeconds = rsp->body.wait.seconds;
     return waitSeconds;
   }
 
   //----------------------------------------------------------------------------
   // Check if HS wait time elapsed
   //----------------------------------------------------------------------------
-  void AsyncSocketHandler::CheckHSWait()
+  bool AsyncSocketHandler::CheckHSWait()
   {
     time_t now = time( 0 );
     if( now - pHSWaitStarted >= pHSWaitSeconds )
     {
       Log *log = DefaultEnv::GetLog();
       log->Debug( AsyncSockMsg, "[%s] The hand-shake wait time elapsed, will "
                   "replay the endsess request.", pStreamName.c_str() );
-      SendHSMsg();
+      if( !SendHSMsg() )
+        return false;
       //------------------------------------------------------------------------
       // Make sure the wait state is reset
       //------------------------------------------------------------------------
       pHSWaitSeconds = 0;
       pHSWaitStarted = 0;
     }
+    return true;
   }
 
   //------------------------------------------------------------------------
   // Get the IP stack
   //------------------------------------------------------------------------
   std::string AsyncSocketHandler::GetIpStack() const
   {
```

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClAsyncSocketHandler.hh` & `xrootd-5.5.5/src/XrdCl/XrdClAsyncSocketHandler.hh`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 #include "XrdCl/XrdClTaskManager.hh"
 #include "XrdCl/XrdClXRootDResponses.hh"
 #include "XrdCl/XrdClURL.hh"
 #include "XrdCl/XrdClAsyncMsgReader.hh"
 #include "XrdCl/XrdClAsyncHSReader.hh"
 #include "XrdCl/XrdClAsyncMsgWriter.hh"
 #include "XrdCl/XrdClAsyncHSWriter.hh"
+#include "XrdOuc/XrdOucCompiler.hh"
 
 namespace XrdCl
 {
   class Stream;
 
   //----------------------------------------------------------------------------
   //! Utility class handling asynchronous socket interactions and forwarding
@@ -145,70 +146,71 @@
       //! Convert Stream object and sub-stream number to stream name
       //------------------------------------------------------------------------
       static std::string ToStreamName( const URL &url, uint16_t strmnb );
 
       //------------------------------------------------------------------------
       // Connect returned
       //------------------------------------------------------------------------
-      virtual void OnConnectionReturn();
+      virtual bool OnConnectionReturn() XRD_WARN_UNUSED_RESULT;
 
       //------------------------------------------------------------------------
       // Got a write readiness event
       //------------------------------------------------------------------------
-      void OnWrite();
+      bool OnWrite() XRD_WARN_UNUSED_RESULT;
 
       //------------------------------------------------------------------------
       // Got a write readiness event while handshaking
       //------------------------------------------------------------------------
-      void OnWriteWhileHandshaking();
+      bool OnWriteWhileHandshaking() XRD_WARN_UNUSED_RESULT;
 
       //------------------------------------------------------------------------
       // Got a read readiness event
       //------------------------------------------------------------------------
-      void OnRead();
+      bool OnRead() XRD_WARN_UNUSED_RESULT;
 
       //------------------------------------------------------------------------
       // Got a read readiness event while handshaking
       //------------------------------------------------------------------------
-      void OnReadWhileHandshaking();
+      bool OnReadWhileHandshaking() XRD_WARN_UNUSED_RESULT;
 
       //------------------------------------------------------------------------
       // Handle the handshake message
       //------------------------------------------------------------------------
-      void HandleHandShake( std::unique_ptr<Message> msg );
+      bool HandleHandShake( std::unique_ptr<Message> msg )
+                            XRD_WARN_UNUSED_RESULT;
 
       //------------------------------------------------------------------------
       // Prepare the next step of the hand-shake procedure
       //------------------------------------------------------------------------
-      void HandShakeNextStep( bool done );
+      bool HandShakeNextStep( bool done ) XRD_WARN_UNUSED_RESULT;
 
       //------------------------------------------------------------------------
       // Handle fault
       //------------------------------------------------------------------------
       void OnFault( XRootDStatus st );
 
       //------------------------------------------------------------------------
       // Handle fault while handshaking
       //------------------------------------------------------------------------
       void OnFaultWhileHandshaking( XRootDStatus st );
 
       //------------------------------------------------------------------------
       // Handle write timeout event
       //------------------------------------------------------------------------
-      void OnWriteTimeout();
+      bool OnWriteTimeout() XRD_WARN_UNUSED_RESULT;
 
       //------------------------------------------------------------------------
       // Handle read timeout event
       //------------------------------------------------------------------------
-      void OnReadTimeout();
+      bool OnReadTimeout() XRD_WARN_UNUSED_RESULT;
 
       //------------------------------------------------------------------------
       // Handle timeout event while handshaking
       //------------------------------------------------------------------------
-      void OnTimeoutWhileHandshaking();
+      bool OnTimeoutWhileHandshaking() XRD_WARN_UNUSED_RESULT;
 
       //------------------------------------------------------------------------
       // Handle header corruption in case of kXR_status response
       //------------------------------------------------------------------------
       void OnHeaderCorruption();
 
       //------------------------------------------------------------------------
@@ -225,34 +227,44 @@
       //------------------------------------------------------------------------
       XRootDStatus DoTlsHandShake();
 
       //------------------------------------------------------------------------
       // Handle read/write event if we are in the middle of a TLS hand-shake
       //------------------------------------------------------------------------
       // Handle read/write event if we are in the middle of a TLS hand-shake
-      void OnTLSHandShake();
+      bool OnTLSHandShake() XRD_WARN_UNUSED_RESULT;
 
       //------------------------------------------------------------------------
       // Prepare a HS writer for sending and enable uplink
       //------------------------------------------------------------------------
-      void SendHSMsg();
+      bool SendHSMsg() XRD_WARN_UNUSED_RESULT;
 
       //------------------------------------------------------------------------
       // Extract the value of a wait response
       //
       // @param rsp : the server response
       // @return    : if rsp is a wait response then its value
       //              otherwise -1
       //------------------------------------------------------------------------
       inline kXR_int32 HandleWaitRsp( Message *rsp );
 
       //------------------------------------------------------------------------
       // Check if HS wait time elapsed
       //------------------------------------------------------------------------
-      void CheckHSWait();
+      bool CheckHSWait() XRD_WARN_UNUSED_RESULT;
+
+      //------------------------------------------------------------------------
+      // Handler for read related socket events
+      //------------------------------------------------------------------------
+      inline bool EventRead( uint8_t type ) XRD_WARN_UNUSED_RESULT;
+
+      //------------------------------------------------------------------------
+      // Handler for write related socket events
+      //------------------------------------------------------------------------
+      inline bool EventWrite( uint8_t type ) XRD_WARN_UNUSED_RESULT;
 
       //------------------------------------------------------------------------
       // Data members
       //------------------------------------------------------------------------
       Poller                        *pPoller;
       TransportHandler              *pTransport;
       AnyObject                     *pChannelData;
```

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClAsyncVectorReader.hh` & `xrootd-5.5.5/src/XrdCl/XrdClAsyncVectorReader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClBuffer.hh` & `xrootd-5.5.5/src/XrdCl/XrdClBuffer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClChannel.cc` & `xrootd-5.5.5/src/XrdCl/XrdClChannel.cc`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,14 @@
 
   //----------------------------------------------------------------------------
   // Destructor
   //----------------------------------------------------------------------------
   Channel::~Channel()
   {
     pTickGenerator->Invalidate();
-    pTaskManager->UnregisterTask( pTickGenerator );
     delete pStream;
     pTransport->FinalizeChannel( pChannelData );
   }
 
   //----------------------------------------------------------------------------
   // Send the message asynchronously
   //----------------------------------------------------------------------------
```

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClChannel.hh` & `xrootd-5.5.5/src/XrdCl/XrdClChannel.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClChannelHandlerList.cc` & `xrootd-5.5.5/src/XrdCl/XrdClChannelHandlerList.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClChannelHandlerList.hh` & `xrootd-5.5.5/src/XrdCl/XrdClChannelHandlerList.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClCheckSumHelper.hh` & `xrootd-5.5.5/src/XrdCl/XrdClCheckSumHelper.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClCheckSumManager.cc` & `xrootd-5.5.5/src/XrdCl/XrdClCheckSumManager.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClCheckSumManager.hh` & `xrootd-5.5.5/src/XrdCl/XrdClCheckSumManager.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClCheckpointOperation.hh` & `xrootd-5.5.5/src/XrdCl/XrdClCheckpointOperation.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClClassicCopyJob.cc` & `xrootd-5.5.5/src/XrdCl/XrdClClassicCopyJob.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClClassicCopyJob.hh` & `xrootd-5.5.5/src/XrdCl/XrdClClassicCopyJob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClConstants.hh` & `xrootd-5.5.5/src/XrdCl/XrdClConstants.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClCopy.cc` & `xrootd-5.5.5/src/XrdCl/XrdClCopy.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClCopyJob.hh` & `xrootd-5.5.5/src/XrdCl/XrdClCopyJob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClCopyProcess.cc` & `xrootd-5.5.5/src/XrdCl/XrdClCopyProcess.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClCopyProcess.hh` & `xrootd-5.5.5/src/XrdCl/XrdClCopyProcess.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClCtx.hh` & `xrootd-5.5.5/src/XrdCl/XrdClCtx.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClDefaultEnv.cc` & `xrootd-5.5.5/src/XrdCl/XrdClDefaultEnv.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClDefaultEnv.hh` & `xrootd-5.5.5/src/XrdCl/XrdClDefaultEnv.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClDlgEnv.hh` & `xrootd-5.5.5/src/XrdCl/XrdClDlgEnv.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClEcHandler.cc` & `xrootd-5.5.5/src/XrdCl/XrdClEcHandler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClEcHandler.hh` & `xrootd-5.5.5/src/XrdCl/XrdClEcHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClEnv.cc` & `xrootd-5.5.5/src/XrdCl/XrdClEnv.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClEnv.hh` & `xrootd-5.5.5/src/XrdCl/XrdClEnv.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClFS.cc` & `xrootd-5.5.5/src/XrdCl/XrdClFS.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClFSExecutor.cc` & `xrootd-5.5.5/src/XrdCl/XrdClFSExecutor.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClFSExecutor.hh` & `xrootd-5.5.5/src/XrdCl/XrdClFSExecutor.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClFile.cc` & `xrootd-5.5.5/src/XrdCl/XrdClFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClFile.hh` & `xrootd-5.5.5/src/XrdCl/XrdClFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClFileOperations.hh` & `xrootd-5.5.5/src/XrdCl/XrdClFileOperations.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClFileStateHandler.cc` & `xrootd-5.5.5/src/XrdCl/XrdClFileStateHandler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClFileStateHandler.hh` & `xrootd-5.5.5/src/XrdCl/XrdClFileStateHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClFileSystem.cc` & `xrootd-5.5.5/src/XrdCl/XrdClFileSystem.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClFileSystem.hh` & `xrootd-5.5.5/src/XrdCl/XrdClFileSystem.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClFileSystemOperations.hh` & `xrootd-5.5.5/src/XrdCl/XrdClFileSystemOperations.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClFileSystemUtils.cc` & `xrootd-5.5.5/src/XrdCl/XrdClFileSystemUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClFileSystemUtils.hh` & `xrootd-5.5.5/src/XrdCl/XrdClFileSystemUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClFileTimer.cc` & `xrootd-5.5.5/src/XrdCl/XrdClFileTimer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClFileTimer.hh` & `xrootd-5.5.5/src/XrdCl/XrdClFileTimer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClFinalOperation.hh` & `xrootd-5.5.5/src/XrdCl/XrdClFinalOperation.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClForkHandler.cc` & `xrootd-5.5.5/src/XrdCl/XrdClForkHandler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClForkHandler.hh` & `xrootd-5.5.5/src/XrdCl/XrdClForkHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClFwd.hh` & `xrootd-5.5.5/src/XrdCl/XrdClFwd.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClInQueue.cc` & `xrootd-5.5.5/src/XrdCl/XrdClInQueue.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClInQueue.hh` & `xrootd-5.5.5/src/XrdCl/XrdClInQueue.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClJobManager.cc` & `xrootd-5.5.5/src/XrdCl/XrdClJobManager.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClJobManager.hh` & `xrootd-5.5.5/src/XrdCl/XrdClJobManager.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClLocalFileHandler.cc` & `xrootd-5.5.5/src/XrdCl/XrdClLocalFileHandler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClLocalFileHandler.hh` & `xrootd-5.5.5/src/XrdCl/XrdClLocalFileHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClLocalFileTask.cc` & `xrootd-5.5.5/src/XrdCl/XrdClLocalFileTask.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClLocalFileTask.hh` & `xrootd-5.5.5/src/XrdCl/XrdClLocalFileTask.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClLog.cc` & `xrootd-5.5.5/src/XrdCl/XrdClLog.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClLog.hh` & `xrootd-5.5.5/src/XrdCl/XrdClLog.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClMessage.hh` & `xrootd-5.5.5/src/XrdCl/XrdClMessage.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClMessageUtils.cc` & `xrootd-5.5.5/src/XrdCl/XrdClMessageUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClMessageUtils.hh` & `xrootd-5.5.5/src/XrdCl/XrdClMessageUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClMetalinkRedirector.cc` & `xrootd-5.5.5/src/XrdCl/XrdClMetalinkRedirector.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClMetalinkRedirector.hh` & `xrootd-5.5.5/src/XrdCl/XrdClMetalinkRedirector.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClMonitor.hh` & `xrootd-5.5.5/src/XrdCl/XrdClMonitor.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClOperationHandlers.hh` & `xrootd-5.5.5/src/XrdCl/XrdClOperationHandlers.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClOperationTimeout.hh` & `xrootd-5.5.5/src/XrdCl/XrdClOperationTimeout.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClOperations.cc` & `xrootd-5.5.5/src/XrdCl/XrdClOperations.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClOperations.hh` & `xrootd-5.5.5/src/XrdCl/XrdClOperations.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClOptimizers.hh` & `xrootd-5.5.5/src/XrdCl/XrdClOptimizers.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClOptional.hh` & `xrootd-5.5.5/src/XrdCl/XrdClOptional.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClOutQueue.cc` & `xrootd-5.5.5/src/XrdCl/XrdClOutQueue.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClOutQueue.hh` & `xrootd-5.5.5/src/XrdCl/XrdClOutQueue.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClParallelOperation.hh` & `xrootd-5.5.5/src/XrdCl/XrdClParallelOperation.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClPlugInInterface.hh` & `xrootd-5.5.5/src/XrdCl/XrdClPlugInInterface.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClPlugInManager.cc` & `xrootd-5.5.5/src/XrdCl/XrdClPlugInManager.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClPlugInManager.hh` & `xrootd-5.5.5/src/XrdCl/XrdClPlugInManager.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClPoller.hh` & `xrootd-5.5.5/src/XrdCl/XrdClPoller.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClPollerBuiltIn.cc` & `xrootd-5.5.5/src/XrdCl/XrdClPollerBuiltIn.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClPollerBuiltIn.hh` & `xrootd-5.5.5/src/XrdCl/XrdClPollerBuiltIn.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClPollerFactory.cc` & `xrootd-5.5.5/src/XrdCl/XrdClPollerFactory.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClPollerFactory.hh` & `xrootd-5.5.5/src/XrdCl/XrdClPollerFactory.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClPostMaster.cc` & `xrootd-5.5.5/src/XrdCl/XrdClPostMaster.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClPostMaster.hh` & `xrootd-5.5.5/src/XrdCl/XrdClPostMaster.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClPostMasterInterfaces.hh` & `xrootd-5.5.5/src/XrdCl/XrdClPostMasterInterfaces.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClPropertyList.hh` & `xrootd-5.5.5/src/XrdCl/XrdClPropertyList.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClRedirectorRegistry.cc` & `xrootd-5.5.5/src/XrdCl/XrdClRedirectorRegistry.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClRedirectorRegistry.hh` & `xrootd-5.5.5/src/XrdCl/XrdClRedirectorRegistry.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClRequestSync.hh` & `xrootd-5.5.5/src/XrdCl/XrdClRequestSync.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClResponseJob.hh` & `xrootd-5.5.5/src/XrdCl/XrdClResponseJob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClSIDManager.cc` & `xrootd-5.5.5/src/XrdCl/XrdClSIDManager.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClSIDManager.hh` & `xrootd-5.5.5/src/XrdCl/XrdClSIDManager.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClSocket.cc` & `xrootd-5.5.5/src/XrdCl/XrdClSocket.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClSocket.hh` & `xrootd-5.5.5/src/XrdCl/XrdClSocket.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClStatus.cc` & `xrootd-5.5.5/src/XrdCl/XrdClStatus.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClStatus.hh` & `xrootd-5.5.5/src/XrdCl/XrdClStatus.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClStream.cc` & `xrootd-5.5.5/src/XrdCl/XrdClStream.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1017,21 +1017,21 @@
       mon->Event( Monitor::EvDisconnect, &i );
     }
   }
 
   //----------------------------------------------------------------------------
   // Call back when a message has been reconstructed
   //----------------------------------------------------------------------------
-  void Stream::OnReadTimeout( uint16_t substream )
+  bool Stream::OnReadTimeout( uint16_t substream )
   {
     //--------------------------------------------------------------------------
     // We only take the main stream into account
     //--------------------------------------------------------------------------
     if( substream != 0 )
-      return;
+      return true;
 
     //--------------------------------------------------------------------------
     // Check if there is no outgoing messages and if the stream TTL is elapesed.
     // It is assumed that the underlying transport makes sure that there is no
     // pending requests that are not answered, ie. all possible virtual streams
     // are de-allocated
     //--------------------------------------------------------------------------
@@ -1063,35 +1063,38 @@
         // Important note!
         //
         // This destroys the Stream object itself, the underlined
         // AsyncSocketHandler object (that called this method) and the Channel
         // object that aggregates this Stream.
         //----------------------------------------------------------------------
         DefaultEnv::GetPostMaster()->ForceDisconnect( *pUrl );
-        return;
+        return false;
       }
     }
 
     //--------------------------------------------------------------------------
     // Check if the stream is broken
     //--------------------------------------------------------------------------
     XRootDStatus st = pTransport->IsStreamBroken( now-lastActivity,
                                             *pChannelData );
     if( !st.IsOK() )
     {
       scopedLock.UnLock();
       OnError( substream, st );
+      return false;
     }
+    return true;
   }
 
   //----------------------------------------------------------------------------
   // Call back when a message has been reconstru
   //----------------------------------------------------------------------------
-  void Stream::OnWriteTimeout( uint16_t /*substream*/ )
+  bool Stream::OnWriteTimeout( uint16_t /*substream*/ )
   {
+    return true;
   }
 
   //----------------------------------------------------------------------------
   // Register channel event handler
   //----------------------------------------------------------------------------
   void Stream::RegisterEventHandler( ChannelEventHandler *handler )
   {
```

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClStream.hh` & `xrootd-5.5.5/src/XrdCl/XrdClStream.hh`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 #include "XrdCl/XrdClJobManager.hh"
 #include "XrdCl/XrdClInQueue.hh"
 #include "XrdCl/XrdClUtils.hh"
 
 #include "XrdSys/XrdSysPthread.hh"
 #include "XrdSys/XrdSysRAtomic.hh"
 #include "XrdNet/XrdNetAddr.hh"
+#include "XrdOuc/XrdOucCompiler.hh"
 #include <list>
 #include <vector>
 #include <functional>
 #include <memory>
 
 namespace XrdCl
 {
@@ -215,20 +216,20 @@
       //! Force error
       //------------------------------------------------------------------------
       void ForceError( XRootDStatus status );
 
       //------------------------------------------------------------------------
       //! On read timeout
       //------------------------------------------------------------------------
-      void OnReadTimeout( uint16_t subStream );
+      bool OnReadTimeout( uint16_t subStream ) XRD_WARN_UNUSED_RESULT;
 
       //------------------------------------------------------------------------
       //! On write timeout
       //------------------------------------------------------------------------
-      void OnWriteTimeout( uint16_t subStream );
+      bool OnWriteTimeout( uint16_t subStream ) XRD_WARN_UNUSED_RESULT;
 
       //------------------------------------------------------------------------
       //! Register channel event handler
       //------------------------------------------------------------------------
       void RegisterEventHandler( ChannelEventHandler *handler );
 
       //------------------------------------------------------------------------
```

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClSyncQueue.hh` & `xrootd-5.5.5/src/XrdCl/XrdClSyncQueue.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClTPFallBackCopyJob.cc` & `xrootd-5.5.5/src/XrdCl/XrdClTPFallBackCopyJob.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClTPFallBackCopyJob.hh` & `xrootd-5.5.5/src/XrdCl/XrdClTPFallBackCopyJob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClTaskManager.cc` & `xrootd-5.5.5/src/XrdCl/XrdClTaskManager.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClTaskManager.hh` & `xrootd-5.5.5/src/XrdCl/XrdClTaskManager.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClThirdPartyCopyJob.cc` & `xrootd-5.5.5/src/XrdCl/XrdClThirdPartyCopyJob.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClThirdPartyCopyJob.hh` & `xrootd-5.5.5/src/XrdCl/XrdClThirdPartyCopyJob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClTls.cc` & `xrootd-5.5.5/src/XrdCl/XrdClTls.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClTls.hh` & `xrootd-5.5.5/src/XrdCl/XrdClTls.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClTransportManager.cc` & `xrootd-5.5.5/src/XrdCl/XrdClTransportManager.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClTransportManager.hh` & `xrootd-5.5.5/src/XrdCl/XrdClTransportManager.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClURL.cc` & `xrootd-5.5.5/src/XrdCl/XrdClURL.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClURL.hh` & `xrootd-5.5.5/src/XrdCl/XrdClURL.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClUtils.cc` & `xrootd-5.5.5/src/XrdCl/XrdClUtils.cc`

 * *Files 2% similar despite different names*

```diff
@@ -861,8 +861,58 @@
     //--------------------------------------------------------------------------
     std::set<std::string> dst_supported( dstcks.begin(), dstcks.end() );
     std::vector<std::string>::iterator itr = srccks.begin();
     for( ; itr != srccks.end(); ++itr )
       if( dst_supported.count( *itr ) ) return *itr;
     return std::string();
   }
+
+  //----------------------------------------------------------------------------
+  //! Split chunks in a ChunkList into one or more ChunkLists
+  //----------------------------------------------------------------------------
+  void Utils::SplitChunks( std::vector<ChunkList> &listsvec,
+                           const ChunkList        &chunks,
+                           const uint32_t          maxcs,
+                           const size_t            maxc )
+  {
+    listsvec.clear();
+    if( !chunks.size() ) return;
+
+    listsvec.emplace_back();
+    ChunkList *c    = &listsvec.back();
+    const size_t cs = chunks.size();
+    size_t idx      = 0;
+    size_t nc       = 0;
+    ChunkInfo tmpc;
+
+    c->reserve( cs );
+
+    while( idx < cs )
+    {
+      if( maxc && nc >= maxc )
+      {
+        listsvec.emplace_back();
+        c = &listsvec.back();
+        c->reserve( cs - idx );
+        nc = 0;
+      }
+
+      if( tmpc.length == 0 )
+        tmpc = chunks[idx];
+
+      if( maxcs && tmpc.length > maxcs )
+      {
+        c->emplace_back( tmpc.offset, maxcs, tmpc.buffer );
+        tmpc.offset += maxcs;
+        tmpc.length -= maxcs;
+        tmpc.buffer  = static_cast<char*>( tmpc.buffer ) + maxcs;
+      }
+      else
+      {
+        c->emplace_back( tmpc.offset, tmpc.length, tmpc.buffer );
+        tmpc.length = 0;
+        ++idx;
+      }
+      ++nc;
+    }
+  }
 }
```

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClUtils.hh` & `xrootd-5.5.5/src/XrdCl/XrdClUtils.hh`

 * *Files 6% similar despite different names*

```diff
@@ -268,14 +268,26 @@
       {
         if( url.IsLocalFile() ) return false;
         int protver = 0;
         auto st = GetProtocolVersion( url, protver );
         if( !st.IsOK() ) return false;
         return protver >= kXR_PROTPGRWVERSION;
       }
+
+      //------------------------------------------------------------------------
+      //! Split chunks in a ChunkList into one or more ChunkLists
+      //! @param listsvec        : output vector of ChunkLists
+      //! @param chunks          : input ChunkLisits
+      //! @param maxcs           : maximum size of a ChunkInfo in output
+      //! @param maxc            : maximum number of ChunkInfo in each ChunkList
+      //------------------------------------------------------------------------
+      static void SplitChunks( std::vector<ChunkList> &listsvec,
+                               const ChunkList        &chunks,
+                               const uint32_t          maxcs,
+                               const size_t            maxc );
   };
 
   //----------------------------------------------------------------------------
   //! Smart descriptor - closes the descriptor on destruction
   //----------------------------------------------------------------------------
   class ScopedDescriptor
   {
```

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClXCpCtx.cc` & `xrootd-5.5.5/src/XrdCl/XrdClXCpCtx.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClXCpCtx.hh` & `xrootd-5.5.5/src/XrdCl/XrdClXCpCtx.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClXCpSrc.cc` & `xrootd-5.5.5/src/XrdCl/XrdClXCpSrc.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClXCpSrc.hh` & `xrootd-5.5.5/src/XrdCl/XrdClXCpSrc.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClXRootDMsgHandler.cc` & `xrootd-5.5.5/src/XrdCl/XrdClXRootDMsgHandler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClXRootDMsgHandler.hh` & `xrootd-5.5.5/src/XrdCl/XrdClXRootDMsgHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClXRootDResponses.cc` & `xrootd-5.5.5/src/XrdCl/XrdClXRootDResponses.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClXRootDResponses.hh` & `xrootd-5.5.5/src/XrdCl/XrdClXRootDResponses.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClXRootDTransport.cc` & `xrootd-5.5.5/src/XrdCl/XrdClXRootDTransport.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClXRootDTransport.hh` & `xrootd-5.5.5/src/XrdCl/XrdClXRootDTransport.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClZipArchive.cc` & `xrootd-5.5.5/src/XrdCl/XrdClZipArchive.cc`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 #include "XrdCl/XrdClFileOperations.hh"
 #include "XrdCl/XrdClCheckpointOperation.hh"
 #include "XrdCl/XrdClZipArchive.hh"
 #include "XrdCl/XrdClLog.hh"
 #include "XrdCl/XrdClDefaultEnv.hh"
 #include "XrdCl/XrdClConstants.hh"
+#include "XrdCl/XrdClUtils.hh"
 #include "XrdZip/XrdZipZIP64EOCDL.hh"
 
 #include <sys/stat.h>
 
 namespace XrdCl
 {
   using namespace XrdZip;
@@ -622,18 +623,26 @@
         lfhbuf->reserve( lfhlen );
         nf.lfh->Serialize( *lfhbuf );
         chunks.emplace_back( nf.offset, lfhbuf->size(), lfhbuf->data() );
         wrtbufs.emplace_back( std::move( lfhbuf ) );
       }
 
       auto wrtbuff = std::make_shared<buffer_t>( GetCD() );
-      chunks.emplace_back( cdoff, wrtbuff->size(), wrtbuff->data() );
+      Pipeline p = XrdCl::Write( archive, cdoff,
+                                 wrtbuff->size(),
+                                 wrtbuff->data() );
       wrtbufs.emplace_back( std::move( wrtbuff ) );
 
-      Pipeline p = XrdCl::VectorWrite( archive, chunks );
+      std::vector<ChunkList> listsvec;
+      XrdCl::Utils::SplitChunks( listsvec, chunks, 262144, 1024 );
+
+      for(auto itr = listsvec.rbegin(); itr != listsvec.rend(); ++itr)
+      {
+        p = XrdCl::VectorWrite( archive, *itr ) | p;
+      }
       if( ckpinit )
         p       |= XrdCl::Checkpoint( archive, ChkPtCode::COMMIT );
       p         |= Close( archive ) >>
                      [=]( XRootDStatus &st )
                      {
                        if( st.IsOK() ) Clear();
                        else openstage = Error;
```

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClZipArchive.hh` & `xrootd-5.5.5/src/XrdCl/XrdClZipArchive.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClZipCache.hh` & `xrootd-5.5.5/src/XrdCl/XrdClZipCache.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClZipListHandler.cc` & `xrootd-5.5.5/src/XrdCl/XrdClZipListHandler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClZipListHandler.hh` & `xrootd-5.5.5/src/XrdCl/XrdClZipListHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCl/XrdClZipOperations.hh` & `xrootd-5.5.5/src/XrdCl/XrdClZipOperations.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdClHttp/XrdClHttpFilePlugIn.cc` & `xrootd-5.5.5/src/XrdClHttp/XrdClHttpFilePlugIn.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdClHttp/XrdClHttpFilePlugIn.hh` & `xrootd-5.5.5/src/XrdClHttp/XrdClHttpFilePlugIn.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdClHttp/XrdClHttpFileSystemPlugIn.cc` & `xrootd-5.5.5/src/XrdClHttp/XrdClHttpFileSystemPlugIn.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdClHttp/XrdClHttpFileSystemPlugIn.hh` & `xrootd-5.5.5/src/XrdClHttp/XrdClHttpFileSystemPlugIn.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdClHttp/XrdClHttpPlugInFactory.cc` & `xrootd-5.5.5/src/XrdClHttp/XrdClHttpPlugInFactory.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdClHttp/XrdClHttpPosix.cc` & `xrootd-5.5.5/src/XrdClHttp/XrdClHttpPosix.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdClHttp/XrdClHttpPosix.hh` & `xrootd-5.5.5/src/XrdClHttp/XrdClHttpPosix.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsAdmin.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsAdmin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsAdmin.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsAdmin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsBaseFS.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsBaseFS.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsBaseFS.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsBaseFS.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsBlackList.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsBlackList.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsBlackList.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsBlackList.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsCache.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsCache.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsCache.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsCache.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsClient.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsClient.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsClient.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsClient.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsClientConfig.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsClientConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsClientConfig.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsClientConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsClientMan.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsClientMan.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsClientMan.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsClientMan.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsClientMsg.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsClientMsg.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsClientMsg.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsClientMsg.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsClustID.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsClustID.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsClustID.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsClustID.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsCluster.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsCluster.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsCluster.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsCluster.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsConfig.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsConfig.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsFinder.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsFinder.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsFinder.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsFinder.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsJob.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsJob.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsJob.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsJob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsKey.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsKey.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsKey.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsKey.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsLogin.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsLogin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsLogin.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsLogin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsManList.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsManList.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsManList.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsManList.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsManTree.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsManTree.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsManTree.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsManTree.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsManager.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsManager.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsManager.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsManager.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsMeter.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsMeter.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsMeter.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsMeter.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsNash.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsNash.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsNash.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsNash.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsNode.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsNode.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsNode.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsNode.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsPList.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsPList.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsPList.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsPList.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsParser.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsParser.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsParser.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsParser.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsPerfMon.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsPerfMon.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsPrepArgs.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsPrepArgs.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsPrepArgs.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsPrepArgs.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsPrepare.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsPrepare.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsPrepare.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsPrepare.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsProtocol.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsProtocol.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsProtocol.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsProtocol.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsRRData.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsRRData.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsRRData.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsRRData.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsRRQ.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsRRQ.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsRRQ.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsRRQ.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsRTable.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsRTable.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsRTable.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsRTable.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsRedirLocal.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsRedirLocal.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsRedirLocal.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsRedirLocal.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsResp.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsResp.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsResp.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsResp.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsRole.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsRole.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsRouting.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsRouting.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsRouting.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsRouting.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsSecurity.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsSecurity.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsSecurity.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsSecurity.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsSelect.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsSelect.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsState.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsState.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsState.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsState.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsSupervisor.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsSupervisor.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsSupervisor.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsSupervisor.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsTalk.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsTalk.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsTalk.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsTalk.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsTrace.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsTypes.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsTypes.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsUtils.cc` & `xrootd-5.5.5/src/XrdCms/XrdCmsUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsUtils.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCms/XrdCmsVnId.hh` & `xrootd-5.5.5/src/XrdCms/XrdCmsVnId.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoAux.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoAux.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoAux.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoAux.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoBasic.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoBasic.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoBasic.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoBasic.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoCipher.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoCipher.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoCipher.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoCipher.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoFactory.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoFactory.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoFactory.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoFactory.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoLite.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoLite.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoLite.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoLite.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoLite_bf32.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoLite_bf32.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoMsgDigest.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoMsgDigest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoMsgDigest.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoMsgDigest.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoRSA.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoRSA.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoRSA.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoRSA.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoTrace.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoX509.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoX509.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoX509.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoX509.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoX509Chain.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoX509Chain.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoX509Chain.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoX509Chain.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoX509Crl.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoX509Crl.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoX509Crl.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoX509Crl.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoX509Req.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoX509Req.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptoX509Req.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptoX509Req.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptogsiX509Chain.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptogsiX509Chain.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptogsiX509Chain.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptogsiX509Chain.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptosslAux.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptosslAux.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptosslAux.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptosslAux.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptosslCipher.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptosslCipher.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptosslCipher.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptosslCipher.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptosslFactory.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptosslFactory.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptosslFactory.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptosslFactory.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptosslMsgDigest.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptosslMsgDigest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptosslMsgDigest.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptosslMsgDigest.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptosslRSA.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptosslRSA.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptosslRSA.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptosslRSA.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptosslTrace.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptosslTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptosslX509.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptosslX509.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptosslX509.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptosslX509.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptosslX509Crl.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptosslX509Crl.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptosslX509Crl.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptosslX509Crl.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptosslX509Req.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptosslX509Req.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptosslX509Req.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptosslX509Req.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptosslgsiAux.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptosslgsiAux.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptosslgsiAux.hh` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptosslgsiAux.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto/XrdCryptotest.cc` & `xrootd-5.5.5/src/XrdCrypto/XrdCryptotest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdDig/XrdDigAuth.cc` & `xrootd-5.5.5/src/XrdDig/XrdDigAuth.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdDig/XrdDigAuth.hh` & `xrootd-5.5.5/src/XrdDig/XrdDigAuth.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdDig/XrdDigConfig.cc` & `xrootd-5.5.5/src/XrdDig/XrdDigConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdDig/XrdDigConfig.hh` & `xrootd-5.5.5/src/XrdDig/XrdDigConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdDig/XrdDigFS.cc` & `xrootd-5.5.5/src/XrdDig/XrdDigFS.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdDig/XrdDigFS.hh` & `xrootd-5.5.5/src/XrdDig/XrdDigFS.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdEc/CMakeLists.txt` & `xrootd-5.5.5/src/XrdEc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdEc/README` & `xrootd-5.5.5/src/XrdEc/README`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdEc/XrdEcConfig.hh` & `xrootd-5.5.5/src/XrdEc/XrdEcConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdEc/XrdEcObjCfg.hh` & `xrootd-5.5.5/src/XrdEc/XrdEcObjCfg.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdEc/XrdEcReader.cc` & `xrootd-5.5.5/src/XrdEc/XrdEcReader.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdEc/XrdEcReader.hh` & `xrootd-5.5.5/src/XrdEc/XrdEcReader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdEc/XrdEcRedundancyProvider.cc` & `xrootd-5.5.5/src/XrdEc/XrdEcRedundancyProvider.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdEc/XrdEcRedundancyProvider.hh` & `xrootd-5.5.5/src/XrdEc/XrdEcRedundancyProvider.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdEc/XrdEcStrmWriter.cc` & `xrootd-5.5.5/src/XrdEc/XrdEcStrmWriter.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdEc/XrdEcStrmWriter.hh` & `xrootd-5.5.5/src/XrdEc/XrdEcStrmWriter.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdEc/XrdEcThreadPool.hh` & `xrootd-5.5.5/src/XrdEc/XrdEcThreadPool.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdEc/XrdEcUtilities.cc` & `xrootd-5.5.5/src/XrdEc/XrdEcUtilities.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdEc/XrdEcUtilities.hh` & `xrootd-5.5.5/src/XrdEc/XrdEcUtilities.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdEc/XrdEcWrtBuff.hh` & `xrootd-5.5.5/src/XrdEc/XrdEcWrtBuff.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFfs/README` & `xrootd-5.5.5/src/XrdFfs/README`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFfs/XrdFfsDent.cc` & `xrootd-5.5.5/src/XrdFfs/XrdFfsDent.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFfs/XrdFfsDent.hh` & `xrootd-5.5.5/src/XrdFfs/XrdFfsDent.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFfs/XrdFfsFsinfo.cc` & `xrootd-5.5.5/src/XrdFfs/XrdFfsFsinfo.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFfs/XrdFfsFsinfo.hh` & `xrootd-5.5.5/src/XrdFfs/XrdFfsFsinfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFfs/XrdFfsMisc.cc` & `xrootd-5.5.5/src/XrdFfs/XrdFfsMisc.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFfs/XrdFfsMisc.hh` & `xrootd-5.5.5/src/XrdFfs/XrdFfsMisc.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFfs/XrdFfsPosix.cc` & `xrootd-5.5.5/src/XrdFfs/XrdFfsPosix.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFfs/XrdFfsPosix.hh` & `xrootd-5.5.5/src/XrdFfs/XrdFfsPosix.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFfs/XrdFfsQueue.cc` & `xrootd-5.5.5/src/XrdFfs/XrdFfsQueue.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFfs/XrdFfsQueue.hh` & `xrootd-5.5.5/src/XrdFfs/XrdFfsQueue.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFfs/XrdFfsWcache.cc` & `xrootd-5.5.5/src/XrdFfs/XrdFfsWcache.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFfs/XrdFfsWcache.hh` & `xrootd-5.5.5/src/XrdFfs/XrdFfsWcache.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFfs/XrdFfsXrootdfs.cc` & `xrootd-5.5.5/src/XrdFfs/XrdFfsXrootdfs.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFfs/xrootdfs.template` & `xrootd-5.5.5/src/XrdFfs/xrootdfs.template`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrc/XrdFrcCID.cc` & `xrootd-5.5.5/src/XrdFrc/XrdFrcCID.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrc/XrdFrcCID.hh` & `xrootd-5.5.5/src/XrdFrc/XrdFrcCID.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrc/XrdFrcProxy.cc` & `xrootd-5.5.5/src/XrdFrc/XrdFrcProxy.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrc/XrdFrcProxy.hh` & `xrootd-5.5.5/src/XrdFrc/XrdFrcProxy.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrc/XrdFrcReqAgent.cc` & `xrootd-5.5.5/src/XrdFrc/XrdFrcReqAgent.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrc/XrdFrcReqAgent.hh` & `xrootd-5.5.5/src/XrdFrc/XrdFrcReqAgent.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrc/XrdFrcReqFile.cc` & `xrootd-5.5.5/src/XrdFrc/XrdFrcReqFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrc/XrdFrcReqFile.hh` & `xrootd-5.5.5/src/XrdFrc/XrdFrcReqFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrc/XrdFrcRequest.hh` & `xrootd-5.5.5/src/XrdFrc/XrdFrcRequest.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrc/XrdFrcTrace.cc` & `xrootd-5.5.5/src/XrdFrc/XrdFrcTrace.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrc/XrdFrcTrace.hh` & `xrootd-5.5.5/src/XrdFrc/XrdFrcTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrc/XrdFrcUtils.cc` & `xrootd-5.5.5/src/XrdFrc/XrdFrcUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrc/XrdFrcUtils.hh` & `xrootd-5.5.5/src/XrdFrc/XrdFrcUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrc/XrdFrcXAttr.hh` & `xrootd-5.5.5/src/XrdFrc/XrdFrcXAttr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrc/XrdFrcXLock.hh` & `xrootd-5.5.5/src/XrdFrc/XrdFrcXLock.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmAdmin.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmAdmin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmAdmin.hh` & `xrootd-5.5.5/src/XrdFrm/XrdFrmAdmin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmAdminAudit.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmAdminAudit.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmAdminFiles.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmAdminFiles.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmAdminFind.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmAdminFind.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmAdminMain.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmAdminMain.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmAdminQuery.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmAdminQuery.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmAdminReloc.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmAdminReloc.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmAdminUnlink.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmAdminUnlink.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmCns.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmCns.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmCns.hh` & `xrootd-5.5.5/src/XrdFrm/XrdFrmCns.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmConfig.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmConfig.hh` & `xrootd-5.5.5/src/XrdFrm/XrdFrmConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmFiles.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmFiles.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmFiles.hh` & `xrootd-5.5.5/src/XrdFrm/XrdFrmFiles.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmMigrate.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmMigrate.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmMigrate.hh` & `xrootd-5.5.5/src/XrdFrm/XrdFrmMigrate.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmMonitor.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmMonitor.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmMonitor.hh` & `xrootd-5.5.5/src/XrdFrm/XrdFrmMonitor.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmPurgMain.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmPurgMain.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmPurge.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmPurge.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmPurge.hh` & `xrootd-5.5.5/src/XrdFrm/XrdFrmPurge.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmReqBoss.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmReqBoss.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmReqBoss.hh` & `xrootd-5.5.5/src/XrdFrm/XrdFrmReqBoss.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmTSort.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmTSort.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmTSort.hh` & `xrootd-5.5.5/src/XrdFrm/XrdFrmTSort.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmTransfer.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmTransfer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmTransfer.hh` & `xrootd-5.5.5/src/XrdFrm/XrdFrmTransfer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmXfrAgent.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmXfrAgent.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmXfrAgent.hh` & `xrootd-5.5.5/src/XrdFrm/XrdFrmXfrAgent.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmXfrDaemon.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmXfrDaemon.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmXfrDaemon.hh` & `xrootd-5.5.5/src/XrdFrm/XrdFrmXfrDaemon.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmXfrJob.hh` & `xrootd-5.5.5/src/XrdFrm/XrdFrmXfrJob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmXfrMain.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmXfrMain.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmXfrQueue.cc` & `xrootd-5.5.5/src/XrdFrm/XrdFrmXfrQueue.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm/XrdFrmXfrQueue.hh` & `xrootd-5.5.5/src/XrdFrm/XrdFrmXfrQueue.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/static/favicon.ico` & `xrootd-5.5.5/src/XrdHttp/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/static/xrdhttp.css` & `xrootd-5.5.5/src/XrdHttp/static/xrdhttp.css`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/static/xrdhttp_css.h` & `xrootd-5.5.5/src/XrdHttp/static/xrdhttp_css.h`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/static/xrdhttp_favicon_ico.h` & `xrootd-5.5.5/src/XrdHttp/static/xrdhttp_favicon_ico.h`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/XrdHttpChecksum.cc` & `xrootd-5.5.5/src/XrdHttp/XrdHttpChecksum.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/XrdHttpChecksum.hh` & `xrootd-5.5.5/src/XrdHttp/XrdHttpChecksum.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/XrdHttpChecksumHandler.cc` & `xrootd-5.5.5/src/XrdHttp/XrdHttpChecksumHandler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/XrdHttpChecksumHandler.hh` & `xrootd-5.5.5/src/XrdHttp/XrdHttpChecksumHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/XrdHttpExtHandler.cc` & `xrootd-5.5.5/src/XrdHttp/XrdHttpExtHandler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/XrdHttpExtHandler.hh` & `xrootd-5.5.5/src/XrdHttp/XrdHttpExtHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/XrdHttpModule.cc` & `xrootd-5.5.5/src/XrdHttp/XrdHttpModule.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/XrdHttpProtocol.cc` & `xrootd-5.5.5/src/XrdHttp/XrdHttpProtocol.cc`

 * *Files 0% similar despite different names*

```diff
@@ -276,14 +276,15 @@
   else
     hp->ishttps = myishttps;
 
   // We now have to do some work arounds to tell the underlying framework
   // that is is https without invoking TLS on the actual link. Eventually,
   // we should just use the link's TLS native implementation.
   //
+  SecEntity.addrInfo = lp->AddrInfo();
   XrdNetAddr *netP = const_cast<XrdNetAddr*>(lp->NetAddr());
   netP->SetDialect("https");
   netP->SetTLS(true);
 
   // Allocate 1MB buffer from pool
   if (!hp->myBuff) {
     hp->myBuff = BPool->Obtain(1024 * 1024);
```

### Comparing `xrootd-5.5.4/src/XrdHttp/XrdHttpProtocol.hh` & `xrootd-5.5.5/src/XrdHttp/XrdHttpProtocol.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/XrdHttpReq.cc` & `xrootd-5.5.5/src/XrdHttp/XrdHttpReq.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/XrdHttpReq.hh` & `xrootd-5.5.5/src/XrdHttp/XrdHttpReq.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/XrdHttpSecXtractor.hh` & `xrootd-5.5.5/src/XrdHttp/XrdHttpSecXtractor.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/XrdHttpSecurity.cc` & `xrootd-5.5.5/src/XrdHttp/XrdHttpSecurity.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/XrdHttpStatic.hh` & `xrootd-5.5.5/src/XrdHttp/XrdHttpStatic.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/XrdHttpTrace.hh` & `xrootd-5.5.5/src/XrdHttp/XrdHttpTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/XrdHttpUtils.cc` & `xrootd-5.5.5/src/XrdHttp/XrdHttpUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/XrdHttpUtils.hh` & `xrootd-5.5.5/src/XrdHttp/XrdHttpUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/xrootd-http-rdr.cf` & `xrootd-5.5.5/src/XrdHttp/xrootd-http-rdr.cf`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp/xrootd-http.cf` & `xrootd-5.5.5/src/XrdHttp/xrootd-http.cf`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdMacaroons/README.md` & `xrootd-5.5.5/src/XrdMacaroons/README.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdMacaroons/XrdMacaroons.cc` & `xrootd-5.5.5/src/XrdMacaroons/XrdMacaroons.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdMacaroons/XrdMacaroonsAuthz.cc` & `xrootd-5.5.5/src/XrdMacaroons/XrdMacaroonsAuthz.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdMacaroons/XrdMacaroonsAuthz.hh` & `xrootd-5.5.5/src/XrdMacaroons/XrdMacaroonsAuthz.hh`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                      const Access_Operation oper) override
     {
         return 0;
     }
 
     // Macaroons don't have a concept off an "issuers"; return an empty
     // list.
-    virtual Issuers IssuerList() {return Issuers();}
+    virtual Issuers IssuerList() override {return Issuers();}
 
 private:
     XrdAccPrivs OnMissing(const XrdSecEntity     *Entity,
                           const char             *path,
                           const Access_Operation  oper,
                                 XrdOucEnv        *env);
```

### Comparing `xrootd-5.5.4/src/XrdMacaroons/XrdMacaroonsConfigure.cc` & `xrootd-5.5.5/src/XrdMacaroons/XrdMacaroonsConfigure.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdMacaroons/XrdMacaroonsHandler.cc` & `xrootd-5.5.5/src/XrdMacaroons/XrdMacaroonsHandler.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdMacaroons/XrdMacaroonsHandler.hh` & `xrootd-5.5.5/src/XrdMacaroons/XrdMacaroonsHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdMacaroons/macaroon-init` & `xrootd-5.5.5/src/XrdMacaroons/macaroon-init`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNet.cc` & `xrootd-5.5.5/src/XrdNet/XrdNet.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNet.hh` & `xrootd-5.5.5/src/XrdNet/XrdNet.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetAddr.cc` & `xrootd-5.5.5/src/XrdNet/XrdNetAddr.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetAddr.hh` & `xrootd-5.5.5/src/XrdNet/XrdNetAddr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetAddrInfo.cc` & `xrootd-5.5.5/src/XrdNet/XrdNetAddrInfo.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetAddrInfo.hh` & `xrootd-5.5.5/src/XrdNet/XrdNetAddrInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetBuffer.cc` & `xrootd-5.5.5/src/XrdNet/XrdNetBuffer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetBuffer.hh` & `xrootd-5.5.5/src/XrdNet/XrdNetBuffer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetCache.cc` & `xrootd-5.5.5/src/XrdNet/XrdNetCache.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetCache.hh` & `xrootd-5.5.5/src/XrdNet/XrdNetCache.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetCmsNotify.cc` & `xrootd-5.5.5/src/XrdNet/XrdNetCmsNotify.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetCmsNotify.hh` & `xrootd-5.5.5/src/XrdNet/XrdNetCmsNotify.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetConnect.cc` & `xrootd-5.5.5/src/XrdNet/XrdNetConnect.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetConnect.hh` & `xrootd-5.5.5/src/XrdNet/XrdNetConnect.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetIF.cc` & `xrootd-5.5.5/src/XrdNet/XrdNetIF.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetIF.hh` & `xrootd-5.5.5/src/XrdNet/XrdNetIF.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetIdentity.cc` & `xrootd-5.5.5/src/XrdNet/XrdNetIdentity.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetIdentity.hh` & `xrootd-5.5.5/src/XrdNet/XrdNetIdentity.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetMsg.cc` & `xrootd-5.5.5/src/XrdNet/XrdNetMsg.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetMsg.hh` & `xrootd-5.5.5/src/XrdNet/XrdNetMsg.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetOpts.hh` & `xrootd-5.5.5/src/XrdNet/XrdNetOpts.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetPMark.cc` & `xrootd-5.5.5/src/XrdNet/XrdNetPMark.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetPMark.hh` & `xrootd-5.5.5/src/XrdNet/XrdNetPMark.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetPMarkCfg.cc` & `xrootd-5.5.5/src/XrdNet/XrdNetPMarkCfg.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetPMarkCfg.hh` & `xrootd-5.5.5/src/XrdNet/XrdNetPMarkCfg.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetPMarkFF.cc` & `xrootd-5.5.5/src/XrdNet/XrdNetPMarkFF.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetPMarkFF.hh` & `xrootd-5.5.5/src/XrdNet/XrdNetPMarkFF.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetPeer.hh` & `xrootd-5.5.5/src/XrdNet/XrdNetPeer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetRegistry.cc` & `xrootd-5.5.5/src/XrdNet/XrdNetRegistry.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetRegistry.hh` & `xrootd-5.5.5/src/XrdNet/XrdNetRegistry.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetSecurity.cc` & `xrootd-5.5.5/src/XrdNet/XrdNetSecurity.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetSecurity.hh` & `xrootd-5.5.5/src/XrdNet/XrdNetSecurity.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetSockAddr.hh` & `xrootd-5.5.5/src/XrdNet/XrdNetSockAddr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetSocket.cc` & `xrootd-5.5.5/src/XrdNet/XrdNetSocket.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetSocket.hh` & `xrootd-5.5.5/src/XrdNet/XrdNetSocket.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetUtils.cc` & `xrootd-5.5.5/src/XrdNet/XrdNetUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdNet/XrdNetUtils.hh` & `xrootd-5.5.5/src/XrdNet/XrdNetUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfs.cc` & `xrootd-5.5.5/src/XrdOfs/XrdOfs.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfs.hh` & `xrootd-5.5.5/src/XrdOfs/XrdOfs.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsCPFile.cc` & `xrootd-5.5.5/src/XrdOfs/XrdOfsCPFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsCPFile.hh` & `xrootd-5.5.5/src/XrdOfs/XrdOfsCPFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsChkPnt.cc` & `xrootd-5.5.5/src/XrdOfs/XrdOfsChkPnt.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsChkPnt.hh` & `xrootd-5.5.5/src/XrdOfs/XrdOfsChkPnt.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsConfig.cc` & `xrootd-5.5.5/src/XrdOfs/XrdOfsConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsConfigCP.cc` & `xrootd-5.5.5/src/XrdOfs/XrdOfsConfigCP.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsConfigCP.hh` & `xrootd-5.5.5/src/XrdOfs/XrdOfsConfigCP.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsConfigPI.cc` & `xrootd-5.5.5/src/XrdOfs/XrdOfsConfigPI.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsConfigPI.hh` & `xrootd-5.5.5/src/XrdOfs/XrdOfsConfigPI.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsEvr.cc` & `xrootd-5.5.5/src/XrdOfs/XrdOfsEvr.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsEvr.hh` & `xrootd-5.5.5/src/XrdOfs/XrdOfsEvr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsEvs.cc` & `xrootd-5.5.5/src/XrdOfs/XrdOfsEvs.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsEvs.hh` & `xrootd-5.5.5/src/XrdOfs/XrdOfsEvs.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsFAttr.cc` & `xrootd-5.5.5/src/XrdOfs/XrdOfsFAttr.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsFS.cc` & `xrootd-5.5.5/src/XrdOfs/XrdOfsFS.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsFSctl.cc` & `xrootd-5.5.5/src/XrdOfs/XrdOfsFSctl.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsFSctl_PI.hh` & `xrootd-5.5.5/src/XrdOfs/XrdOfsFSctl_PI.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsHandle.cc` & `xrootd-5.5.5/src/XrdOfs/XrdOfsHandle.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsHandle.hh` & `xrootd-5.5.5/src/XrdOfs/XrdOfsHandle.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsPoscq.cc` & `xrootd-5.5.5/src/XrdOfs/XrdOfsPoscq.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsPoscq.hh` & `xrootd-5.5.5/src/XrdOfs/XrdOfsPoscq.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsPrepGPI.cc` & `xrootd-5.5.5/src/XrdOfs/XrdOfsPrepGPI.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsPrepare.hh` & `xrootd-5.5.5/src/XrdOfs/XrdOfsPrepare.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsSecurity.hh` & `xrootd-5.5.5/src/XrdOfs/XrdOfsSecurity.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsStats.cc` & `xrootd-5.5.5/src/XrdOfs/XrdOfsStats.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsStats.hh` & `xrootd-5.5.5/src/XrdOfs/XrdOfsStats.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsTPC.cc` & `xrootd-5.5.5/src/XrdOfs/XrdOfsTPC.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsTPC.hh` & `xrootd-5.5.5/src/XrdOfs/XrdOfsTPC.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsTPCAuth.cc` & `xrootd-5.5.5/src/XrdOfs/XrdOfsTPCAuth.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsTPCAuth.hh` & `xrootd-5.5.5/src/XrdOfs/XrdOfsTPCAuth.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsTPCConfig.hh` & `xrootd-5.5.5/src/XrdOfs/XrdOfsTPCConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsTPCInfo.cc` & `xrootd-5.5.5/src/XrdOfs/XrdOfsTPCInfo.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsTPCInfo.hh` & `xrootd-5.5.5/src/XrdOfs/XrdOfsTPCInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsTPCJob.cc` & `xrootd-5.5.5/src/XrdOfs/XrdOfsTPCJob.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsTPCJob.hh` & `xrootd-5.5.5/src/XrdOfs/XrdOfsTPCJob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsTPCProg.cc` & `xrootd-5.5.5/src/XrdOfs/XrdOfsTPCProg.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsTPCProg.hh` & `xrootd-5.5.5/src/XrdOfs/XrdOfsTPCProg.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOfs/XrdOfsTrace.hh` & `xrootd-5.5.5/src/XrdOfs/XrdOfsTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOss.cc` & `xrootd-5.5.5/src/XrdOss/XrdOss.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOss.hh` & `xrootd-5.5.5/src/XrdOss/XrdOss.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssAio.cc` & `xrootd-5.5.5/src/XrdOss/XrdOssAio.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssApi.cc` & `xrootd-5.5.5/src/XrdOss/XrdOssApi.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssApi.hh` & `xrootd-5.5.5/src/XrdOss/XrdOssApi.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssAt.cc` & `xrootd-5.5.5/src/XrdOss/XrdOssAt.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssAt.hh` & `xrootd-5.5.5/src/XrdOss/XrdOssAt.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssCache.cc` & `xrootd-5.5.5/src/XrdOss/XrdOssCache.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssCache.hh` & `xrootd-5.5.5/src/XrdOss/XrdOssCache.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssConfig.cc` & `xrootd-5.5.5/src/XrdOss/XrdOssConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssConfig.hh` & `xrootd-5.5.5/src/XrdOss/XrdOssConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssCopy.cc` & `xrootd-5.5.5/src/XrdOss/XrdOssCopy.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssCopy.hh` & `xrootd-5.5.5/src/XrdOss/XrdOssCopy.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssCreate.cc` & `xrootd-5.5.5/src/XrdOss/XrdOssCreate.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssDefaultSS.hh` & `xrootd-5.5.5/src/XrdOss/XrdOssDefaultSS.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssError.hh` & `xrootd-5.5.5/src/XrdOss/XrdOssError.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssMSS.cc` & `xrootd-5.5.5/src/XrdOss/XrdOssMSS.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssMio.cc` & `xrootd-5.5.5/src/XrdOss/XrdOssMio.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssMio.hh` & `xrootd-5.5.5/src/XrdOss/XrdOssMio.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssMioFile.hh` & `xrootd-5.5.5/src/XrdOss/XrdOssMioFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssOpaque.hh` & `xrootd-5.5.5/src/XrdOss/XrdOssOpaque.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssPath.cc` & `xrootd-5.5.5/src/XrdOss/XrdOssPath.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssPath.hh` & `xrootd-5.5.5/src/XrdOss/XrdOssPath.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssReloc.cc` & `xrootd-5.5.5/src/XrdOss/XrdOssReloc.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssRename.cc` & `xrootd-5.5.5/src/XrdOss/XrdOssRename.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssSIgpfsT.cc` & `xrootd-5.5.5/src/XrdOss/XrdOssSIgpfsT.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssSpace.cc` & `xrootd-5.5.5/src/XrdOss/XrdOssSpace.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssSpace.hh` & `xrootd-5.5.5/src/XrdOss/XrdOssSpace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssStage.cc` & `xrootd-5.5.5/src/XrdOss/XrdOssStage.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssStage.hh` & `xrootd-5.5.5/src/XrdOss/XrdOssStage.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssStat.cc` & `xrootd-5.5.5/src/XrdOss/XrdOssStat.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssStatInfo.hh` & `xrootd-5.5.5/src/XrdOss/XrdOssStatInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssTrace.hh` & `xrootd-5.5.5/src/XrdOss/XrdOssTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssUnlink.cc` & `xrootd-5.5.5/src/XrdOss/XrdOssUnlink.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssVS.hh` & `xrootd-5.5.5/src/XrdOss/XrdOssVS.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOss/XrdOssWrapper.hh` & `xrootd-5.5.5/src/XrdOss/XrdOssWrapper.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi/README.md` & `xrootd-5.5.5/src/XrdOssCsi/README.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi/XrdOssCsi.cc` & `xrootd-5.5.5/src/XrdOssCsi/XrdOssCsi.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi/XrdOssCsi.hh` & `xrootd-5.5.5/src/XrdOssCsi/XrdOssCsi.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiConfig.cc` & `xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiConfig.hh` & `xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiCrcUtils.cc` & `xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiCrcUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiCrcUtils.hh` & `xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiCrcUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiFile.cc` & `xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiFileAio.cc` & `xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiFileAio.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiFileAio.hh` & `xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiFileAio.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiPages.cc` & `xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiPages.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiPages.hh` & `xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiPages.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiPagesUnaligned.cc` & `xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiPagesUnaligned.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiRanges.cc` & `xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiRanges.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiRanges.hh` & `xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiRanges.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiTagstore.hh` & `xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiTagstore.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiTagstoreFile.cc` & `xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiTagstoreFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiTagstoreFile.hh` & `xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiTagstoreFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi/XrdOssCsiTrace.hh` & `xrootd-5.5.5/src/XrdOssCsi/XrdOssCsiTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi/XrdOssHandler.hh` & `xrootd-5.5.5/src/XrdOssCsi/XrdOssHandler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/README.bonjour` & `xrootd-5.5.5/src/XrdOuc/README.bonjour`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucArgs.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucArgs.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucArgs.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucArgs.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucBackTrace.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucBackTrace.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucBackTrace.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucBackTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucBuffer.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucBuffer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucBuffer.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucBuffer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucCRC.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucCRC.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucCRC.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucCRC.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucCRC32C.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucCRC32C.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucCRC32C.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucCRC32C.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucCache.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucCache.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucCache.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucCache.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucCacheCM.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucCacheCM.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucCacheStats.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucCacheStats.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucCallBack.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucCallBack.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucCallBack.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucCallBack.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucChain.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucChain.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucChkPnt.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucChkPnt.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucCompiler.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucCompiler.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucDLlist.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucDLlist.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucERoute.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucERoute.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucERoute.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucERoute.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucEnum.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucEnum.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucEnv.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucEnv.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucEnv.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucEnv.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucErrInfo.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucErrInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucExport.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucExport.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucExport.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucExport.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucFileInfo.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucFileInfo.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucFileInfo.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucFileInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucGMap.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucGMap.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucGMap.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucGMap.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucGatherConf.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucGatherConf.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucGatherConf.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucGatherConf.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucHash.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucHash.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucHash.icc` & `xrootd-5.5.5/src/XrdOuc/XrdOucHash.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucHashVal.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucHashVal.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucIOVec.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucIOVec.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucJson.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucJson.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucLock.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucLock.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucLogging.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucLogging.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucLogging.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucLogging.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucMapP2X.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucMapP2X.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucMsubs.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucMsubs.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucMsubs.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucMsubs.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucN2NLoader.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucN2NLoader.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucN2NLoader.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucN2NLoader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucN2No2p.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucN2No2p.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucNList.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucNList.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucNList.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucNList.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucNSWalk.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucNSWalk.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucNSWalk.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucNSWalk.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucName2Name.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucName2Name.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucName2Name.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucName2Name.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucPList.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucPList.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucPgrwUtils.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucPgrwUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucPgrwUtils.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucPgrwUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucPinKing.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucPinKing.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucPinLoader.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucPinLoader.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucPinLoader.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucPinLoader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucPinObject.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucPinObject.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucPinPath.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucPinPath.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucPinPath.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucPinPath.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucPreload.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucPreload.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucPreload.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucPreload.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucProg.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucProg.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucProg.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucProg.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucPsx.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucPsx.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucPsx.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucPsx.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucPup.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucPup.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucPup.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucPup.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucRash.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucRash.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucRash.icc` & `xrootd-5.5.5/src/XrdOuc/XrdOucRash.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucReqID.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucReqID.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucReqID.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucReqID.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucSFVec.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucSFVec.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucSHA3.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucSHA3.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucSHA3.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucSHA3.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucSid.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucSid.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucSid.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucSid.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucSiteName.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucSiteName.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucSiteName.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucSiteName.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucStats.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucStats.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucStream.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucStream.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucStream.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucStream.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucString.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucString.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucString.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucString.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucSxeq.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucSxeq.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucSxeq.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucSxeq.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucTList.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucTList.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucTPC.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucTPC.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucTPC.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucTPC.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucTUtils.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucTUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucTable.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucTable.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucTokenizer.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucTokenizer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucTokenizer.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucTokenizer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucTrace.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucTrace.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucTrace.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucUri.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucUri.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucUri.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucUri.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucUtils.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucUtils.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucVerName.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOucVerName.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucVerName.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucVerName.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOucXAttr.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOucXAttr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOuca2x.cc` & `xrootd-5.5.5/src/XrdOuc/XrdOuca2x.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOuc/XrdOuca2x.hh` & `xrootd-5.5.5/src/XrdOuc/XrdOuca2x.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/README` & `xrootd-5.5.5/src/XrdPfc/README`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfc.cc` & `xrootd-5.5.5/src/XrdPfc/XrdPfc.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfc.hh` & `xrootd-5.5.5/src/XrdPfc/XrdPfc.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcAllowDecision.cc` & `xrootd-5.5.5/src/XrdPfc/XrdPfcAllowDecision.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcBlacklistDecision.cc` & `xrootd-5.5.5/src/XrdPfc/XrdPfcBlacklistDecision.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcCommand.cc` & `xrootd-5.5.5/src/XrdPfc/XrdPfcCommand.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcConfiguration.cc` & `xrootd-5.5.5/src/XrdPfc/XrdPfcConfiguration.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcDecision.hh` & `xrootd-5.5.5/src/XrdPfc/XrdPfcDecision.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcFile.cc` & `xrootd-5.5.5/src/XrdPfc/XrdPfcFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcFile.hh` & `xrootd-5.5.5/src/XrdPfc/XrdPfcFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcIO.cc` & `xrootd-5.5.5/src/XrdPfc/XrdPfcIO.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcIO.hh` & `xrootd-5.5.5/src/XrdPfc/XrdPfcIO.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcIOFile.cc` & `xrootd-5.5.5/src/XrdPfc/XrdPfcIOFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcIOFile.hh` & `xrootd-5.5.5/src/XrdPfc/XrdPfcIOFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcIOFileBlock.cc` & `xrootd-5.5.5/src/XrdPfc/XrdPfcIOFileBlock.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcIOFileBlock.hh` & `xrootd-5.5.5/src/XrdPfc/XrdPfcIOFileBlock.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcInfo.cc` & `xrootd-5.5.5/src/XrdPfc/XrdPfcInfo.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcInfo.hh` & `xrootd-5.5.5/src/XrdPfc/XrdPfcInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcPrint.cc` & `xrootd-5.5.5/src/XrdPfc/XrdPfcPrint.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcPrint.hh` & `xrootd-5.5.5/src/XrdPfc/XrdPfcPrint.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcPurge.cc` & `xrootd-5.5.5/src/XrdPfc/XrdPfcPurge.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcStats.hh` & `xrootd-5.5.5/src/XrdPfc/XrdPfcStats.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcTrace.hh` & `xrootd-5.5.5/src/XrdPfc/XrdPfcTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc/XrdPfcTypes.hh` & `xrootd-5.5.5/src/XrdPfc/XrdPfcTypes.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/README` & `xrootd-5.5.5/src/XrdPosix/README`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosix.cc` & `xrootd-5.5.5/src/XrdPosix/XrdPosix.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosix.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosix.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixAdmin.cc` & `xrootd-5.5.5/src/XrdPosix/XrdPosixAdmin.cc`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 {
    XrdCl::XRootDStatus            xStatus;
    XrdCl::LocationInfo           *info = 0;
    XrdCl::LocationInfo::Iterator  it;
    XrdCl::URL                    *uVec;
    XrdNetAddr netLoc;
    const char *hName;
-   unsigned int i;
+   unsigned long i;
 
 // Make sure admin is ok
 //
    if (!isOK()) return 0;
 
 // Issue the deep locate and verify that all went well
 //
```

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixAdmin.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosixAdmin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixCache.cc` & `xrootd-5.5.5/src/XrdPosix/XrdPosixCache.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixCache.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosixCache.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixCallBack.cc` & `xrootd-5.5.5/src/XrdPosix/XrdPosixCallBack.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixCallBack.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosixCallBack.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixConfig.cc` & `xrootd-5.5.5/src/XrdPosix/XrdPosixConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixConfig.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosixConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixDir.cc` & `xrootd-5.5.5/src/XrdPosix/XrdPosixDir.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixDir.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosixDir.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixExtern.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosixExtern.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixExtra.cc` & `xrootd-5.5.5/src/XrdPosix/XrdPosixExtra.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixExtra.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosixExtra.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixFile.cc` & `xrootd-5.5.5/src/XrdPosix/XrdPosixFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixFile.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosixFile.hh`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
                               {updMutex.Lock();
                                if (newsz > mySize) mySize = newsz;
                                updMutex.UnLock();
                               }
 
        using         XrdPosixObject::Who;
 
-inline bool          Who(XrdPosixFile **fileP)
+inline bool          Who(XrdPosixFile **fileP) override
                           {*fileP = this; return true;}
 
        int           Write(char *Buff, long long Offs, int Len) override;
 
        void          Write(XrdOucCacheIOCB &iocb, char *buff, long long offs,
                            int wlen) override;
```

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixFileRH.cc` & `xrootd-5.5.5/src/XrdPosix/XrdPosixFileRH.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixFileRH.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosixFileRH.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixInfo.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosixInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixLinkage.cc` & `xrootd-5.5.5/src/XrdPosix/XrdPosixLinkage.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixLinkage.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosixLinkage.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixMap.cc` & `xrootd-5.5.5/src/XrdPosix/XrdPosixMap.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixMap.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosixMap.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixObjGuard.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosixObjGuard.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixObject.cc` & `xrootd-5.5.5/src/XrdPosix/XrdPosixObject.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixObject.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosixObject.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixOsDep.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosixOsDep.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixPreload.cc` & `xrootd-5.5.5/src/XrdPosix/XrdPosixPreload.cc`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 /* COPYING (GPL license).  If not, see <http://www.gnu.org/licenses/>.        */
 /*                                                                            */
 /* The copyright holder's institutional names and contributor's names may not */
 /* be used to endorse or promote products derived from this software without  */
 /* specific prior written permission of the institution or contributor.       */
 /******************************************************************************/
 
+#if defined(__clang__) && defined(_FORTIFY_SOURCE)
+#undef _FORTIFY_SOURCE
+#endif
+
 #include <sys/types.h>
 #include <cstdarg>
 #include <unistd.h>
 #include <cstdlib>
 
 #include "XrdPosix/XrdPosixLinkage.hh"
 #include "XrdPosix/XrdPosixOsDep.hh"
```

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixPreload32.cc` & `xrootd-5.5.5/src/XrdPosix/XrdPosixPreload32.cc`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 /* COPYING (GPL license).  If not, see <http://www.gnu.org/licenses/>.        */
 /*                                                                            */
 /* The copyright holder's institutional names and contributor's names may not */
 /* be used to endorse or promote products derived from this software without  */
 /* specific prior written permission of the institution or contributor.       */
 /******************************************************************************/
 
+#if defined(__clang__) && defined(_FORTIFY_SOURCE)
+#undef _FORTIFY_SOURCE
+#endif
+
 #ifdef  _LARGEFILE_SOURCE
 #undef  _LARGEFILE_SOURCE
 #endif
 
 #ifdef  _LARGEFILE64_SOURCE
 #undef  _LARGEFILE64_SOURCE
 #endif
```

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixPrepIO.cc` & `xrootd-5.5.5/src/XrdPosix/XrdPosixPrepIO.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixPrepIO.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosixPrepIO.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixStats.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosixStats.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixTrace.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosixTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixXrootd.cc` & `xrootd-5.5.5/src/XrdPosix/XrdPosixXrootd.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixXrootd.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosixXrootd.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixXrootdPath.cc` & `xrootd-5.5.5/src/XrdPosix/XrdPosixXrootdPath.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix/XrdPosixXrootdPath.hh` & `xrootd-5.5.5/src/XrdPosix/XrdPosixXrootdPath.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPss/XrdPss.cc` & `xrootd-5.5.5/src/XrdPss/XrdPss.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPss/XrdPss.hh` & `xrootd-5.5.5/src/XrdPss/XrdPss.hh`

 * *Files 21% similar despite different names*

```diff
@@ -140,42 +140,42 @@
 class XrdSysError;
 
 struct XrdVersionInfo;
 
 class XrdPssSys : public XrdOss
 {
 public:
-virtual XrdOssDF *newDir(const char *tident)
+virtual XrdOssDF *newDir(const char *tident) override
                        {return (XrdOssDF *)new XrdPssDir(tident);}
-virtual XrdOssDF *newFile(const char *tident)
+virtual XrdOssDF *newFile(const char *tident) override
                        {return (XrdOssDF *)new XrdPssFile(tident);}
 
-virtual void      Connect(XrdOucEnv &);
+virtual void      Connect(XrdOucEnv &) override;
 
-virtual void      Disc(XrdOucEnv &);
+virtual void      Disc(XrdOucEnv &) override;
 
-int       Chmod(const char *, mode_t mode, XrdOucEnv *eP=0);
+int       Chmod(const char *, mode_t mode, XrdOucEnv *eP=0) override;
 bool      ConfigMapID();
 virtual
-int       Create(const char *, const char *, mode_t, XrdOucEnv &, int opts=0);
-void      EnvInfo(XrdOucEnv *envP);
-uint64_t  Features() {return myFeatures;}
+int       Create(const char *, const char *, mode_t, XrdOucEnv &, int opts=0) override;
+void      EnvInfo(XrdOucEnv *envP) override;
+uint64_t  Features() override {return myFeatures;}
 int       Init(XrdSysLogger *, const char *) override {return -ENOTSUP;}
 int       Init(XrdSysLogger *, const char *, XrdOucEnv *envP) override;
-int       Lfn2Pfn(const char *Path, char *buff, int blen);
+int       Lfn2Pfn(const char *Path, char *buff, int blen) override;
 const
-char     *Lfn2Pfn(const char *Path, char *buff, int blen, int &rc);
-int       Mkdir(const char *, mode_t mode, int mkpath=0, XrdOucEnv *eP=0);
-int       Remdir(const char *, int Opts=0, XrdOucEnv *eP=0);
+char     *Lfn2Pfn(const char *Path, char *buff, int blen, int &rc) override;
+int       Mkdir(const char *, mode_t mode, int mkpath=0, XrdOucEnv *eP=0) override;
+int       Remdir(const char *, int Opts=0, XrdOucEnv *eP=0) override;
 int       Rename(const char *, const char *,
-                 XrdOucEnv *eP1=0, XrdOucEnv *eP2=0);
-int       Stat(const char *, struct stat *, int opts=0, XrdOucEnv *eP=0);
-int       Stats(char *bp, int bl);
-int       Truncate(const char *, unsigned long long, XrdOucEnv *eP=0);
-int       Unlink(const char *, int Opts=0, XrdOucEnv *eP=0);
+                 XrdOucEnv *eP1=0, XrdOucEnv *eP2=0) override;
+int       Stat(const char *, struct stat *, int opts=0, XrdOucEnv *eP=0) override;
+int       Stats(char *bp, int bl) override;
+int       Truncate(const char *, unsigned long long, XrdOucEnv *eP=0) override;
+int       Unlink(const char *, int Opts=0, XrdOucEnv *eP=0) override;
 
 static const int    PolNum = 2;
 enum   PolAct {PolPath = 0, PolObj = 1};
 
 static int   P2DST(int &retc, char *hBuff, int hBlen, PolAct pType,
                    const char *path);
 static int   P2OUT(char *pbuff, int pblen, XrdPssUrlInfo &uInfo);
```

### Comparing `xrootd-5.5.4/src/XrdPss/XrdPssAio.cc` & `xrootd-5.5.5/src/XrdPss/XrdPssAio.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPss/XrdPssAioCB.cc` & `xrootd-5.5.5/src/XrdPss/XrdPssAioCB.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPss/XrdPssAioCB.hh` & `xrootd-5.5.5/src/XrdPss/XrdPssAioCB.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPss/XrdPssCks.cc` & `xrootd-5.5.5/src/XrdPss/XrdPssCks.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPss/XrdPssCks.hh` & `xrootd-5.5.5/src/XrdPss/XrdPssCks.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPss/XrdPssConfig.cc` & `xrootd-5.5.5/src/XrdPss/XrdPssConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPss/XrdPssTrace.hh` & `xrootd-5.5.5/src/XrdPss/XrdPssTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPss/XrdPssUrlInfo.cc` & `xrootd-5.5.5/src/XrdPss/XrdPssUrlInfo.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPss/XrdPssUrlInfo.hh` & `xrootd-5.5.5/src/XrdPss/XrdPssUrlInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPss/XrdPssUtils.cc` & `xrootd-5.5.5/src/XrdPss/XrdPssUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPss/XrdPssUtils.hh` & `xrootd-5.5.5/src/XrdPss/XrdPssUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdRmc/XrdRmc.cc` & `xrootd-5.5.5/src/XrdRmc/XrdRmc.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdRmc/XrdRmc.hh` & `xrootd-5.5.5/src/XrdRmc/XrdRmc.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdRmc/XrdRmcData.cc` & `xrootd-5.5.5/src/XrdRmc/XrdRmcData.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdRmc/XrdRmcData.hh` & `xrootd-5.5.5/src/XrdRmc/XrdRmcData.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdRmc/XrdRmcReal.cc` & `xrootd-5.5.5/src/XrdRmc/XrdRmcReal.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdRmc/XrdRmcReal.hh` & `xrootd-5.5.5/src/XrdRmc/XrdRmcReal.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdRmc/XrdRmcSlot.hh` & `xrootd-5.5.5/src/XrdRmc/XrdRmcSlot.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/configs/scitokens.cfg` & `xrootd-5.5.5/src/XrdSciTokens/configs/scitokens.cfg`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/test/config/xrootd-http.cfg` & `xrootd-5.5.5/src/XrdSciTokens/test/config/xrootd-http.cfg`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/test/create-pubkey.py` & `xrootd-5.5.5/src/XrdSciTokens/test/create-pubkey.py`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/test/openssl-selfsigned.conf` & `xrootd-5.5.5/src/XrdSciTokens/test/openssl-selfsigned.conf`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/test/setup_tests.sh` & `xrootd-5.5.5/src/XrdSciTokens/test/setup_tests.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/test/test_inside_docker.sh` & `xrootd-5.5.5/src/XrdSciTokens/test/test_inside_docker.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/vendor/inih/INIReader.h` & `xrootd-5.5.5/src/XrdSciTokens/vendor/inih/INIReader.h`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/vendor/inih/INIReaderTest.cpp` & `xrootd-5.5.5/src/XrdSciTokens/vendor/inih/INIReaderTest.cpp`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/vendor/inih/LICENSE.txt` & `xrootd-5.5.5/src/XrdSciTokens/vendor/inih/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/vendor/inih/README.md` & `xrootd-5.5.5/src/XrdSciTokens/vendor/inih/README.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/examples/github-issues.cc` & `xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/examples/github-issues.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/examples/iostream.cc` & `xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/examples/iostream.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/examples/streaming.cc` & `xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/examples/streaming.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/picotest/picotest.c` & `xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/picotest/picotest.c`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/picotest/picotest.h` & `xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/picotest/picotest.h`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/Changes` & `xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/Changes`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/LICENSE` & `xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/LICENSE`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/README.mkdn` & `xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/README.mkdn`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/picojson.h` & `xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/picojson.h`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/vendor/picojson/test.cc` & `xrootd-5.5.5/src/XrdSciTokens/vendor/picojson/test.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/LICENSE` & `xrootd-5.5.5/src/XrdSciTokens/LICENSE`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/README.md` & `xrootd-5.5.5/src/XrdSciTokens/README.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/XrdSciTokensAccess.cc` & `xrootd-5.5.5/src/XrdSciTokens/XrdSciTokensAccess.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens/XrdSciTokensHelper.hh` & `xrootd-5.5.5/src/XrdSciTokens/XrdSciTokensHelper.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecAttr.hh` & `xrootd-5.5.5/src/XrdSec/XrdSecAttr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecClient.cc` & `xrootd-5.5.5/src/XrdSec/XrdSecClient.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecEntity.cc` & `xrootd-5.5.5/src/XrdSec/XrdSecEntity.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecEntity.hh` & `xrootd-5.5.5/src/XrdSec/XrdSecEntity.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecEntityAttr.cc` & `xrootd-5.5.5/src/XrdSec/XrdSecEntityAttr.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecEntityAttr.hh` & `xrootd-5.5.5/src/XrdSec/XrdSecEntityAttr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecEntityPin.hh` & `xrootd-5.5.5/src/XrdSec/XrdSecEntityPin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecEntityXtra.cc` & `xrootd-5.5.5/src/XrdSec/XrdSecEntityXtra.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecEntityXtra.hh` & `xrootd-5.5.5/src/XrdSec/XrdSecEntityXtra.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecInterface.hh` & `xrootd-5.5.5/src/XrdSec/XrdSecInterface.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecLoadSecurity.cc` & `xrootd-5.5.5/src/XrdSec/XrdSecLoadSecurity.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecLoadSecurity.hh` & `xrootd-5.5.5/src/XrdSec/XrdSecLoadSecurity.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecPManager.cc` & `xrootd-5.5.5/src/XrdSec/XrdSecPManager.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecPManager.hh` & `xrootd-5.5.5/src/XrdSec/XrdSecPManager.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecProtect.cc` & `xrootd-5.5.5/src/XrdSec/XrdSecProtect.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecProtect.hh` & `xrootd-5.5.5/src/XrdSec/XrdSecProtect.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecProtector.cc` & `xrootd-5.5.5/src/XrdSec/XrdSecProtector.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecProtector.hh` & `xrootd-5.5.5/src/XrdSec/XrdSecProtector.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecProtocolhost.cc` & `xrootd-5.5.5/src/XrdSec/XrdSecProtocolhost.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecProtocolhost.hh` & `xrootd-5.5.5/src/XrdSec/XrdSecProtocolhost.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecServer.cc` & `xrootd-5.5.5/src/XrdSec/XrdSecServer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecServer.hh` & `xrootd-5.5.5/src/XrdSec/XrdSecServer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecTLayer.cc` & `xrootd-5.5.5/src/XrdSec/XrdSecTLayer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecTLayer.hh` & `xrootd-5.5.5/src/XrdSec/XrdSecTLayer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSecTrace.hh` & `xrootd-5.5.5/src/XrdSec/XrdSecTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSectestClient.cc` & `xrootd-5.5.5/src/XrdSec/XrdSectestClient.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec/XrdSectestServer.cc` & `xrootd-5.5.5/src/XrdSec/XrdSectestServer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecgsi/XrdSecProtocolgsi.cc` & `xrootd-5.5.5/src/XrdSecgsi/XrdSecProtocolgsi.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecgsi/XrdSecProtocolgsi.hh` & `xrootd-5.5.5/src/XrdSecgsi/XrdSecProtocolgsi.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecgsi/XrdSecgsiAuthzFunDN.cc` & `xrootd-5.5.5/src/XrdSecgsi/XrdSecgsiAuthzFunDN.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecgsi/XrdSecgsiAuthzFunVO.cc` & `xrootd-5.5.5/src/XrdSecgsi/XrdSecgsiAuthzFunVO.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecgsi/XrdSecgsiGMAPFunDN.cc` & `xrootd-5.5.5/src/XrdSecgsi/XrdSecgsiGMAPFunDN.cc`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
    if (fcf) {
       char l[4096], val[4096], usr[256];
       while (fgets(l, sizeof(l), fcf)) {
          int len = strlen(l);
          if (len < 2) continue;
          if (l[0] == '#') continue;
          if (l[len-1] == '\n') l[len-1] = '\0';
-         if (sscanf(l, "%4096s %256s", val, usr) >= 2) {
+         if (sscanf(l, "%4095s %255s", val, usr) >= 2) {
             XrdOucString stype = "matching";
             char *p = &val[0];
             int type = kFull;
             if (val[0] == '^') {
                // Starts-with
                type = kBegins;
                p = &val[1];
```

### Comparing `xrootd-5.5.4/src/XrdSecgsi/XrdSecgsiGMAPFunDN.cf` & `xrootd-5.5.5/src/XrdSecgsi/XrdSecgsiGMAPFunDN.cf`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecgsi/XrdSecgsiOpts.hh` & `xrootd-5.5.5/src/XrdSecgsi/XrdSecgsiOpts.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecgsi/XrdSecgsiProxy.cc` & `xrootd-5.5.5/src/XrdSecgsi/XrdSecgsiProxy.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecgsi/XrdSecgsiTrace.hh` & `xrootd-5.5.5/src/XrdSecgsi/XrdSecgsiTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecgsi/XrdSecgsitest.cc` & `xrootd-5.5.5/src/XrdSecgsi/XrdSecgsitest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSeckrb5/XrdSecProtocolkrb5.cc` & `xrootd-5.5.5/src/XrdSeckrb5/XrdSecProtocolkrb5.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecpwd/XrdSecProtocolpwd.cc` & `xrootd-5.5.5/src/XrdSecpwd/XrdSecProtocolpwd.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecpwd/XrdSecProtocolpwd.hh` & `xrootd-5.5.5/src/XrdSecpwd/XrdSecProtocolpwd.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecpwd/XrdSecpwdPlatform.hh` & `xrootd-5.5.5/src/XrdSecpwd/XrdSecpwdPlatform.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecpwd/XrdSecpwdSrvAdmin.cc` & `xrootd-5.5.5/src/XrdSecpwd/XrdSecpwdSrvAdmin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecpwd/XrdSecpwdTrace.hh` & `xrootd-5.5.5/src/XrdSecpwd/XrdSecpwdTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecsss/XrdSecProtocolsss.cc` & `xrootd-5.5.5/src/XrdSecsss/XrdSecProtocolsss.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecsss/XrdSecProtocolsss.hh` & `xrootd-5.5.5/src/XrdSecsss/XrdSecProtocolsss.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecsss/XrdSecsssAdmin.cc` & `xrootd-5.5.5/src/XrdSecsss/XrdSecsssAdmin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecsss/XrdSecsssCon.cc` & `xrootd-5.5.5/src/XrdSecsss/XrdSecsssCon.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecsss/XrdSecsssCon.hh` & `xrootd-5.5.5/src/XrdSecsss/XrdSecsssCon.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecsss/XrdSecsssEnt.cc` & `xrootd-5.5.5/src/XrdSecsss/XrdSecsssEnt.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecsss/XrdSecsssEnt.hh` & `xrootd-5.5.5/src/XrdSecsss/XrdSecsssEnt.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecsss/XrdSecsssID.cc` & `xrootd-5.5.5/src/XrdSecsss/XrdSecsssID.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecsss/XrdSecsssID.hh` & `xrootd-5.5.5/src/XrdSecsss/XrdSecsssID.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecsss/XrdSecsssKT.cc` & `xrootd-5.5.5/src/XrdSecsss/XrdSecsssKT.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecsss/XrdSecsssKT.hh` & `xrootd-5.5.5/src/XrdSecsss/XrdSecsssKT.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecsss/XrdSecsssMap.hh` & `xrootd-5.5.5/src/XrdSecsss/XrdSecsssMap.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecsss/XrdSecsssRR.hh` & `xrootd-5.5.5/src/XrdSecsss/XrdSecsssRR.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecunix/XrdSecProtocolunix.cc` & `xrootd-5.5.5/src/XrdSecunix/XrdSecProtocolunix.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecztn/XrdSecProtocolztn.cc` & `xrootd-5.5.5/src/XrdSecztn/XrdSecProtocolztn.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecztn/XrdSecztn.cc` & `xrootd-5.5.5/src/XrdSecztn/XrdSecztn.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSfs/XrdSfsAio.hh` & `xrootd-5.5.5/src/XrdSfs/XrdSfsAio.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSfs/XrdSfsDio.hh` & `xrootd-5.5.5/src/XrdSfs/XrdSfsDio.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSfs/XrdSfsFAttr.hh` & `xrootd-5.5.5/src/XrdSfs/XrdSfsFAttr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSfs/XrdSfsFlags.hh` & `xrootd-5.5.5/src/XrdSfs/XrdSfsFlags.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSfs/XrdSfsGPFile.hh` & `xrootd-5.5.5/src/XrdSfs/XrdSfsGPFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSfs/XrdSfsInterface.cc` & `xrootd-5.5.5/src/XrdSfs/XrdSfsInterface.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSfs/XrdSfsInterface.hh` & `xrootd-5.5.5/src/XrdSfs/XrdSfsInterface.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSfs/XrdSfsNative.cc` & `xrootd-5.5.5/src/XrdSfs/XrdSfsNative.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSfs/XrdSfsNative.hh` & `xrootd-5.5.5/src/XrdSfs/XrdSfsNative.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSfs/XrdSfsXio.cc` & `xrootd-5.5.5/src/XrdSfs/XrdSfsXio.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSfs/XrdSfsXio.hh` & `xrootd-5.5.5/src/XrdSfs/XrdSfsXio.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSfs/XrdSfsXioImpl.hh` & `xrootd-5.5.5/src/XrdSfs/XrdSfsXioImpl.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiAlert.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiAlert.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiAlert.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiAlert.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiAtomics.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiAtomics.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiAtomics.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiAtomics.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiBVec.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiBVec.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiClient.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiClient.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiCluster.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiCluster.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiCms.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiCms.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiCms.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiCms.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiDir.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiDir.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiDir.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiDir.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiEntity.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiEntity.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiErrInfo.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiErrInfo.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiErrInfo.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiErrInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiEvent.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiEvent.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiEvent.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiEvent.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiFile.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiFile.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiFileReq.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiFileReq.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiFileReq.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiFileReq.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiFileResource.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiFileResource.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiFileResource.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiFileResource.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiFileSess.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiFileSess.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiFileSess.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiFileSess.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiLogger.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiLogger.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiLogger.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiLogger.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiLogging.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiLogging.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiProvider.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiProvider.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiRRAgent.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiRRAgent.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiRRInfo.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiRRInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiRRTable.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiRRTable.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiRequest.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiRequest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiRequest.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiRequest.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiResource.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiResource.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiRespInfo.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiRespInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiResponder.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiResponder.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiResponder.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiResponder.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiScale.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiScale.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiScale.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiScale.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiServReal.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiServReal.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiServReal.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiServReal.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiService.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiService.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiService.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiService.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiSessReal.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiSessReal.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiSessReal.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiSessReal.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiSfs.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiSfs.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiSfs.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiSfs.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiSfsConfig.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiSfsConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiSfsConfig.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiSfsConfig.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiShMam.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiShMam.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiShMam.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiShMam.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiShMap.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiShMap.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiShMap.icc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiShMap.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiShMat.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiShMat.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiShMat.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiShMat.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiStat.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiStat.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiStats.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiStats.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiStats.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiStats.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiStream.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiStream.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiTaskReal.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiTaskReal.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiTaskReal.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiTaskReal.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiTrace.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiUtils.cc` & `xrootd-5.5.5/src/XrdSsi/XrdSsiUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi/XrdSsiUtils.hh` & `xrootd-5.5.5/src/XrdSsi/XrdSsiUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSut/XrdSutAux.cc` & `xrootd-5.5.5/src/XrdSut/XrdSutAux.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSut/XrdSutAux.hh` & `xrootd-5.5.5/src/XrdSut/XrdSutAux.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSut/XrdSutBuckList.cc` & `xrootd-5.5.5/src/XrdSut/XrdSutBuckList.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSut/XrdSutBuckList.hh` & `xrootd-5.5.5/src/XrdSut/XrdSutBuckList.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSut/XrdSutBucket.cc` & `xrootd-5.5.5/src/XrdSut/XrdSutBucket.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSut/XrdSutBucket.hh` & `xrootd-5.5.5/src/XrdSut/XrdSutBucket.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSut/XrdSutBuffer.cc` & `xrootd-5.5.5/src/XrdSut/XrdSutBuffer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSut/XrdSutBuffer.hh` & `xrootd-5.5.5/src/XrdSut/XrdSutBuffer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSut/XrdSutCache.hh` & `xrootd-5.5.5/src/XrdSut/XrdSutCache.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSut/XrdSutCacheEntry.cc` & `xrootd-5.5.5/src/XrdSut/XrdSutCacheEntry.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSut/XrdSutCacheEntry.hh` & `xrootd-5.5.5/src/XrdSut/XrdSutCacheEntry.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSut/XrdSutPFCache.cc` & `xrootd-5.5.5/src/XrdSut/XrdSutPFCache.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSut/XrdSutPFCache.hh` & `xrootd-5.5.5/src/XrdSut/XrdSutPFCache.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSut/XrdSutPFEntry.cc` & `xrootd-5.5.5/src/XrdSut/XrdSutPFEntry.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSut/XrdSutPFEntry.hh` & `xrootd-5.5.5/src/XrdSut/XrdSutPFEntry.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSut/XrdSutPFile.cc` & `xrootd-5.5.5/src/XrdSut/XrdSutPFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSut/XrdSutPFile.hh` & `xrootd-5.5.5/src/XrdSut/XrdSutPFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSut/XrdSutRndm.cc` & `xrootd-5.5.5/src/XrdSut/XrdSutRndm.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSut/XrdSutRndm.hh` & `xrootd-5.5.5/src/XrdSut/XrdSutRndm.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSut/XrdSutTrace.hh` & `xrootd-5.5.5/src/XrdSut/XrdSutTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysAtomics.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysAtomics.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysDir.cc` & `xrootd-5.5.5/src/XrdSys/XrdSysDir.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysDir.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysDir.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysE2T.cc` & `xrootd-5.5.5/src/XrdSys/XrdSysE2T.cc`

 * *Files 1% similar despite different names*

```diff
@@ -50,32 +50,36 @@
 int initErrTable()
 {
    char *eTxt, eBuff[80];
    int lastGood = 0;
 
 // Premap all known error codes.
 //
-   for(int i = 1; i <errSlots; i++)
+   for(int i = 1; i < errSlots; i++)
       {eTxt = strerror(ERRNOBASE + i);
        if (eTxt)
           { eTxt = strdup(eTxt);
            *eTxt = tolower(*eTxt);
            Errno2String[i] = eTxt;
            lastGood = i;
           }
       }
    // NOTE: On systems without EAUTH (authentication error; currently all Glibc systems but GNU Hurd),
    // EAUTH is remapped to EBADE ('invalid exchange').  Given there's no current XRootD use of a
    // syscall that can return EBADE, we assume EBADE really means authentication denied.
 #if defined(EBADE)
+   if (Errno2String[EBADE]) {
+     free((char*)Errno2String[EBADE]);
+   }
+
    Errno2String[EBADE] = "authentication failed - possible invalid exchange";
 #endif
 
-// Supply generic message for missing ones
-//
+   // Supply generic message for missing ones
+   //
    for (int i = 1; i < lastGood; i++)
        {if (!Errno2String[i])
            {snprintf(eBuff, sizeof(eBuff), "unknown error %d", ERRNOBASE + i);
             Errno2String[i] = strdup(eBuff);
            }
        }
```

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysE2T.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysE2T.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysError.cc` & `xrootd-5.5.5/src/XrdSys/XrdSysError.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysError.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysError.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysFAttr.cc` & `xrootd-5.5.5/src/XrdSys/XrdSysFAttr.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysFAttr.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysFAttr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysFAttrBsd.icc` & `xrootd-5.5.5/src/XrdSys/XrdSysFAttrBsd.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysFAttrLnx.icc` & `xrootd-5.5.5/src/XrdSys/XrdSysFAttrLnx.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysFAttrMac.icc` & `xrootd-5.5.5/src/XrdSys/XrdSysFAttrMac.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysFAttrSun.icc` & `xrootd-5.5.5/src/XrdSys/XrdSysFAttrSun.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysFD.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysFD.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysFallocate.cc` & `xrootd-5.5.5/src/XrdSys/XrdSysFallocate.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysFallocate.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysFallocate.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysHeaders.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysHeaders.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysIOEvents.cc` & `xrootd-5.5.5/src/XrdSys/XrdSysIOEvents.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysIOEvents.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysIOEvents.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysIOEventsPollE.icc` & `xrootd-5.5.5/src/XrdSys/XrdSysIOEventsPollE.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysIOEventsPollKQ.icc` & `xrootd-5.5.5/src/XrdSys/XrdSysIOEventsPollKQ.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysIOEventsPollPoll.icc` & `xrootd-5.5.5/src/XrdSys/XrdSysIOEventsPollPoll.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysIOEventsPollPort.icc` & `xrootd-5.5.5/src/XrdSys/XrdSysIOEventsPollPort.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysKernelBuffer.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysKernelBuffer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysLogPI.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysLogPI.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysLogger.cc` & `xrootd-5.5.5/src/XrdSys/XrdSysLogger.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysLogger.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysLogger.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysLogging.cc` & `xrootd-5.5.5/src/XrdSys/XrdSysLogging.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysLogging.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysLogging.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysPageSize.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysPageSize.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysPlatform.cc` & `xrootd-5.5.5/src/XrdSys/XrdSysPlatform.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysPlatform.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysPlatform.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysPlugin.cc` & `xrootd-5.5.5/src/XrdSys/XrdSysPlugin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysPlugin.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysPlugin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysPriv.cc` & `xrootd-5.5.5/src/XrdSys/XrdSysPriv.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysPriv.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysPriv.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysPthread.cc` & `xrootd-5.5.5/src/XrdSys/XrdSysPthread.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysPthread.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysPthread.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysPwd.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysPwd.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysRAtomic.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysRAtomic.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysSemWait.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysSemWait.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysTimer.cc` & `xrootd-5.5.5/src/XrdSys/XrdSysTimer.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysTimer.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysTimer.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysTrace.cc` & `xrootd-5.5.5/src/XrdSys/XrdSysTrace.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysTrace.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysUtils.cc` & `xrootd-5.5.5/src/XrdSys/XrdSysUtils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysUtils.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysXAttr.cc` & `xrootd-5.5.5/src/XrdSys/XrdSysXAttr.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysXAttr.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysXAttr.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysXSLock.cc` & `xrootd-5.5.5/src/XrdSys/XrdSysXSLock.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSys/XrdSysXSLock.hh` & `xrootd-5.5.5/src/XrdSys/XrdSysXSLock.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdThrottle/README` & `xrootd-5.5.5/src/XrdThrottle/README`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdThrottle/XrdThrottle.hh` & `xrootd-5.5.5/src/XrdThrottle/XrdThrottle.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdThrottle/XrdThrottleFile.cc` & `xrootd-5.5.5/src/XrdThrottle/XrdThrottleFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdThrottle/XrdThrottleFileSystem.cc` & `xrootd-5.5.5/src/XrdThrottle/XrdThrottleFileSystem.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdThrottle/XrdThrottleFileSystemConfig.cc` & `xrootd-5.5.5/src/XrdThrottle/XrdThrottleFileSystemConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdThrottle/XrdThrottleManager.cc` & `xrootd-5.5.5/src/XrdThrottle/XrdThrottleManager.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdThrottle/XrdThrottleManager.hh` & `xrootd-5.5.5/src/XrdThrottle/XrdThrottleManager.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdThrottle/XrdThrottleTrace.hh` & `xrootd-5.5.5/src/XrdThrottle/XrdThrottleTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTls/XrdTls.cc` & `xrootd-5.5.5/src/XrdTls/XrdTls.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTls/XrdTls.hh` & `xrootd-5.5.5/src/XrdTls/XrdTls.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTls/XrdTlsContext.cc` & `xrootd-5.5.5/src/XrdTls/XrdTlsContext.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTls/XrdTlsContext.hh` & `xrootd-5.5.5/src/XrdTls/XrdTlsContext.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTls/XrdTlsHostcheck.hh` & `xrootd-5.5.5/src/XrdTls/XrdTlsHostcheck.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTls/XrdTlsHostcheck.icc` & `xrootd-5.5.5/src/XrdTls/XrdTlsHostcheck.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTls/XrdTlsNotary.cc` & `xrootd-5.5.5/src/XrdTls/XrdTlsNotary.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTls/XrdTlsNotary.hh` & `xrootd-5.5.5/src/XrdTls/XrdTlsNotary.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTls/XrdTlsNotaryUtils.hh` & `xrootd-5.5.5/src/XrdTls/XrdTlsNotaryUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTls/XrdTlsNotaryUtils.icc` & `xrootd-5.5.5/src/XrdTls/XrdTlsNotaryUtils.icc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTls/XrdTlsPeerCerts.cc` & `xrootd-5.5.5/src/XrdTls/XrdTlsPeerCerts.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTls/XrdTlsPeerCerts.hh` & `xrootd-5.5.5/src/XrdTls/XrdTlsPeerCerts.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTls/XrdTlsSocket.cc` & `xrootd-5.5.5/src/XrdTls/XrdTlsSocket.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTls/XrdTlsSocket.hh` & `xrootd-5.5.5/src/XrdTls/XrdTlsSocket.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTls/XrdTlsTempCA.cc` & `xrootd-5.5.5/src/XrdTls/XrdTlsTempCA.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTls/XrdTlsTempCA.hh` & `xrootd-5.5.5/src/XrdTls/XrdTlsTempCA.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTls/XrdTlsTrace.hh` & `xrootd-5.5.5/src/XrdTls/XrdTlsTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTpc/README.md` & `xrootd-5.5.5/src/XrdTpc/README.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTpc/XrdTpcConfigure.cc` & `xrootd-5.5.5/src/XrdTpc/XrdTpcConfigure.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTpc/XrdTpcCurlMulti.cc` & `xrootd-5.5.5/src/XrdTpc/XrdTpcCurlMulti.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTpc/XrdTpcMultistream.cc` & `xrootd-5.5.5/src/XrdTpc/XrdTpcMultistream.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTpc/XrdTpcState.cc` & `xrootd-5.5.5/src/XrdTpc/XrdTpcState.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTpc/XrdTpcState.hh` & `xrootd-5.5.5/src/XrdTpc/XrdTpcState.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTpc/XrdTpcStream.cc` & `xrootd-5.5.5/src/XrdTpc/XrdTpcStream.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTpc/XrdTpcStream.hh` & `xrootd-5.5.5/src/XrdTpc/XrdTpcStream.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTpc/XrdTpcTPC.cc` & `xrootd-5.5.5/src/XrdTpc/XrdTpcTPC.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTpc/XrdTpcTPC.hh` & `xrootd-5.5.5/src/XrdTpc/XrdTpcTPC.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTpc/xrootd-test-tpc` & `xrootd-5.5.5/src/XrdTpc/xrootd-test-tpc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdVoms/README.md` & `xrootd-5.5.5/src/XrdVoms/README.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdVoms/XrdVoms.hh` & `xrootd-5.5.5/src/XrdVoms/XrdVoms.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdVoms/XrdVomsFun.cc` & `xrootd-5.5.5/src/XrdVoms/XrdVomsFun.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdVoms/XrdVomsFun.hh` & `xrootd-5.5.5/src/XrdVoms/XrdVomsFun.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdVoms/XrdVomsHttp.cc` & `xrootd-5.5.5/src/XrdVoms/XrdVomsHttp.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdVoms/XrdVomsMapfile.cc` & `xrootd-5.5.5/src/XrdVoms/XrdVomsMapfile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdVoms/XrdVomsMapfile.hh` & `xrootd-5.5.5/src/XrdVoms/XrdVomsMapfile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdVoms/XrdVomsTrace.hh` & `xrootd-5.5.5/src/XrdVoms/XrdVomsTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdVoms/XrdVomsgsi.cc` & `xrootd-5.5.5/src/XrdVoms/XrdVomsgsi.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXml/tinyxml/tinystr.cpp` & `xrootd-5.5.5/src/XrdXml/tinyxml/tinystr.cpp`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXml/tinyxml/tinystr.h` & `xrootd-5.5.5/src/XrdXml/tinyxml/tinystr.h`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXml/tinyxml/tinyxml.cpp` & `xrootd-5.5.5/src/XrdXml/tinyxml/tinyxml.cpp`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXml/tinyxml/tinyxml.h` & `xrootd-5.5.5/src/XrdXml/tinyxml/tinyxml.h`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXml/tinyxml/tinyxmlerror.cpp` & `xrootd-5.5.5/src/XrdXml/tinyxml/tinyxmlerror.cpp`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXml/tinyxml/tinyxmlparser.cpp` & `xrootd-5.5.5/src/XrdXml/tinyxml/tinyxmlparser.cpp`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXml/XrdXmlMetaLink.cc` & `xrootd-5.5.5/src/XrdXml/XrdXmlMetaLink.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXml/XrdXmlMetaLink.hh` & `xrootd-5.5.5/src/XrdXml/XrdXmlMetaLink.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXml/XrdXmlRdrTiny.cc` & `xrootd-5.5.5/src/XrdXml/XrdXmlRdrTiny.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXml/XrdXmlRdrTiny.hh` & `xrootd-5.5.5/src/XrdXml/XrdXmlRdrTiny.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXml/XrdXmlRdrXml2.cc` & `xrootd-5.5.5/src/XrdXml/XrdXmlRdrXml2.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXml/XrdXmlRdrXml2.hh` & `xrootd-5.5.5/src/XrdXml/XrdXmlRdrXml2.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXml/XrdXmlReader.cc` & `xrootd-5.5.5/src/XrdXml/XrdXmlReader.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXml/XrdXmlReader.hh` & `xrootd-5.5.5/src/XrdXml/XrdXmlReader.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdAdmin.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdAdmin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdAdmin.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdAdmin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdAioBuff.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdAioBuff.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdAioBuff.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdAioBuff.hh`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 static
 XrdXrootdAioBuff*       Alloc(XrdXrootdAioTask *arp);
 
         void            doneRead() override;
 
         void            doneWrite() override;
 
-virtual void            Recycle();
+virtual void            Recycle() override;
 
 XrdXrootdAioBuff*       next;
 
 XrdXrootdAioPgrw* const pgrwP;  // -> Derived type is of this type or 0
 
                   XrdXrootdAioBuff(XrdXrootdAioTask* tP, XrdBuffer* bP)
                                   : pgrwP(0),     reqP(tP), buffP(bP) {}
```

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdAioFob.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdAioFob.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdAioFob.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdAioFob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdAioPgrw.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdAioPgrw.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdAioPgrw.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdAioPgrw.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdAioTask.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdAioTask.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdAioTask.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdAioTask.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdBridge.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdBridge.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdBridge.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdBridge.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdCallBack.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdCallBack.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdCallBack.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdCallBack.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdConfig.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdConfig.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdConfigMon.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdConfigMon.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdFile.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdFile.cc`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,18 @@
 {
 
 // Change the reference counter and check if anyone is waiting
 //
    fileMutex.Lock();
    refCount += num;
    TRACEI(FSAIO,"File::Ref="<<refCount<<" after +"<<num<<' '<<FileKey);
-   if (num < 0 && syncWait && refCount <= 0) syncWait->Post();
+   if (num < 0 && syncWait && refCount <= 0)
+      {syncWait->Post();
+       syncWait = nullptr;
+      }
    fileMutex.UnLock();
 }
 
 /******************************************************************************/
 /*                             S e r i a l i z e                              */
 /******************************************************************************/
   
@@ -211,14 +214,15 @@
 //
    if (fhProc && (i = fhProc->Get()) >= 0) 
       {XrdXrootdFile **fP;
        if (i < XRD_FTABSIZE)   fP = &FTab[i];
           else {i -= XRD_FTABSIZE;
                 if (XTab && i < XTnum) fP = &XTab[i];
                    else fP = 0;
+                i += XRD_FTABSIZE;
                }
        if (fP && *fP == heldSpotP)
           {*fP = fp;
            TRACEI(FS, "reusing fh " <<i <<" for " <<fp->FileKey);
            return i;
           }
        char fhn[32];
```

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdFile.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdFileLock.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdFileLock.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdFileLock1.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdFileLock1.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdFileLock1.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdFileLock1.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdFileStats.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdFileStats.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdGPFile.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdGPFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdGSReal.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdGSReal.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdGSReal.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdGSReal.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdGStream.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdGStream.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdGStream.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdGStream.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdJob.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdJob.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdJob.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdJob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdLoadLib.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdLoadLib.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdMonData.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdMonData.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdMonFMap.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdMonFMap.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdMonFMap.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdMonFMap.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdMonFile.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdMonFile.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdMonFile.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdMonFile.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdMonitor.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdMonitor.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdMonitor.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdMonitor.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdNormAio.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdNormAio.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdNormAio.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdNormAio.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdPgrwAio.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdPgrwAio.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdPgrwAio.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdPgrwAio.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdPgwBadCS.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdPgwBadCS.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdPgwBadCS.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdPgwBadCS.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdPgwCtl.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdPgwCtl.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdPgwCtl.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdPgwCtl.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdPgwFob.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdPgwFob.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdPgwFob.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdPgwFob.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdPio.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdPio.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdPio.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdPio.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdPlugin.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdPlugin.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdPrepare.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdPrepare.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdPrepare.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdPrepare.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdProtocol.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdProtocol.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1497,15 +1497,15 @@
    PathID             = 0;
    newPio             = false;
    rvSeq              = 0;
    wvSeq              = 0;
    doTLS              = tlsNot; // Assume client is not capable. This will be
    ableTLS            = false;  // resolved during the kXR_protocol interchange.
    isTLS              = false;  // Made true when link converted to TLS
-   linkAioReq         = {0};
+   linkAioReq         = 0;
    pioFree = pioFirst = pioLast = 0;
    isActive = isLinkWT= isNOP = isDead = false;
    sigNeed = sigHere = sigRead = false;
    sigWarn = true;
    rdType             = 0;
    Entity.Reset(0);
    memset(Stream,  0, sizeof(Stream));
```

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdProtocol.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdProtocol.hh`

 * *Files 1% similar despite different names*

```diff
@@ -159,55 +159,55 @@
 
        void          aioUpdate(int val) {srvrAioOps += val;}
 
        void          aioUpdReq(int val) {linkAioReq += val;}
 
 static char         *Buffer(XrdSfsXioHandle h, int *bsz); // XrdSfsXio
 
-XrdSfsXioHandle      Claim(const char *buff, int datasz, int minasz=0);// XrdSfsXio
+XrdSfsXioHandle      Claim(const char *buff, int datasz, int minasz=0) override;// XrdSfsXio
 
 static int           Configure(char *parms, XrdProtocol_Config *pi);
 
-       void          DoIt() {(*this.*Resume)();}
+       void          DoIt() override {(*this.*Resume)();}
 
        int           do_WriteSpan();
 
        int           getData(gdCallBack   *gdcbP, const char *dtype,
                              char *buff, int blen);
 
        int           getData(gdCallBack   *gdcbP, const char *dtype,
                              struct iovec *iov,   int iovn);
 
        int           getDump(const char *dtype, int dlen);
 
        int           getPathID() {return PathID;}
 
-       XrdProtocol  *Match(XrdLink *lp);
+       XrdProtocol  *Match(XrdLink *lp) override;
 
-       int           Process(XrdLink *lp); //  Sync: Job->Link.DoIt->Process
+       int           Process(XrdLink *lp) override; //  Sync: Job->Link.DoIt->Process
 
        int           Process2();
 
        int           ProcSig();
 
-       void          Recycle(XrdLink *lp, int consec, const char *reason);
+       void          Recycle(XrdLink *lp, int consec, const char *reason) override;
 
 static void          Reclaim(XrdSfsXioHandle h); // XrdSfsXio
 
-       int           SendFile(int fildes); // XrdSfsDio
+       int           SendFile(int fildes) override; // XrdSfsDio
 
-       int           SendFile(XrdOucSFVec *sfvec, int sfvnum); // XrdSfsDio
+       int           SendFile(XrdOucSFVec *sfvec, int sfvnum) override; // XrdSfsDio
 
-       void          SetFD(int fildes); // XrdSfsDio
+       void          SetFD(int fildes) override; // XrdSfsDio
 
-       int           Stats(char *buff, int blen, int do_sync=0);
+       int           Stats(char *buff, int blen, int do_sync=0) override;
 
        void          StreamNOP();
 
-XrdSfsXioHandle      Swap(const char *buff, XrdSfsXioHandle h=0); // XrdSfsXio
+XrdSfsXioHandle      Swap(const char *buff, XrdSfsXioHandle h=0) override; // XrdSfsXio
 
 XrdXrootdProtocol   *VerifyStream(int &rc, int pID, bool lok=true);
 
               XrdXrootdProtocol operator =(const XrdXrootdProtocol &rhs) = delete;
               XrdXrootdProtocol();
              ~XrdXrootdProtocol() {Cleanup();}
```

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdReqID.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdReqID.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdResponse.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdResponse.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdResponse.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdResponse.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdStats.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdStats.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdStats.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdStats.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdTpcMon.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdTpcMon.cc`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 /******************************************************************************/
   
 namespace
 {
 const char *json_fmt = "{\"TPC\":\"%s\",\"Client\":\"%s\","
 "\"Xeq\":{\"Beg\":\"%s\",\"End\":\"%s\",\"RC\":%d,\"Strm\":%u,\"Type\":\"%s\","
         "\"IPv\":%c},"
-"\"Src\":\"%s\",\"Dst\":\"%s\",\"Size\":%d}";
+"\"Src\":\"%s\",\"Dst\":\"%s\",\"Size\":%zu}";
 
 const char *urlFMT = "";
 
 XrdSysError eDest(0, "Ouc");
 }
 
 /******************************************************************************/
```

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdTpcMon.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdTpcMon.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdTrace.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdTrace.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdTransPend.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdTransPend.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdTransPend.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdTransPend.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdTransSend.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdTransSend.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdTransSend.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdTransSend.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdTransit.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdTransit.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdTransit.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdTransit.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdWVInfo.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdWVInfo.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdXPath.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdXPath.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdXeq.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdXeq.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdXeq.hh` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdXeq.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdXeqChkPnt.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdXeqChkPnt.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdXeqFAttr.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdXeqFAttr.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXrootd/XrdXrootdXeqPgrw.cc` & `xrootd-5.5.5/src/XrdXrootd/XrdXrootdXeqPgrw.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdZip/XrdZipCDFH.hh` & `xrootd-5.5.5/src/XrdZip/XrdZipCDFH.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdZip/XrdZipDataDescriptor.hh` & `xrootd-5.5.5/src/XrdZip/XrdZipDataDescriptor.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdZip/XrdZipEOCD.hh` & `xrootd-5.5.5/src/XrdZip/XrdZipEOCD.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdZip/XrdZipExtra.hh` & `xrootd-5.5.5/src/XrdZip/XrdZipExtra.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdZip/XrdZipLFH.hh` & `xrootd-5.5.5/src/XrdZip/XrdZipLFH.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdZip/XrdZipUtils.hh` & `xrootd-5.5.5/src/XrdZip/XrdZipUtils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdZip/XrdZipZIP64EOCD.hh` & `xrootd-5.5.5/src/XrdZip/XrdZipZIP64EOCD.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdZip/XrdZipZIP64EOCDL.hh` & `xrootd-5.5.5/src/XrdZip/XrdZipZIP64EOCDL.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/CMakeLists.txt` & `xrootd-5.5.5/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdApps.cmake` & `xrootd-5.5.5/src/XrdApps.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdCrypto.cmake` & `xrootd-5.5.5/src/XrdCrypto.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdDaemons.cmake` & `xrootd-5.5.5/src/XrdDaemons.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFfs.cmake` & `xrootd-5.5.5/src/XrdFfs.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdFrm.cmake` & `xrootd-5.5.5/src/XrdFrm.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHeaders.cmake` & `xrootd-5.5.5/src/XrdHeaders.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdHttp.cmake` & `xrootd-5.5.5/src/XrdHttp.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdIsal.cmake` & `xrootd-5.5.5/src/XrdIsal.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdMacaroons.cmake` & `xrootd-5.5.5/src/XrdMacaroons.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdOssCsi.cmake` & `xrootd-5.5.5/src/XrdOssCsi.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPfc.cmake` & `xrootd-5.5.5/src/XrdPfc.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPlugins.cmake` & `xrootd-5.5.5/src/XrdPlugins.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdPosix.cmake` & `xrootd-5.5.5/src/XrdPosix.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSciTokens.cmake` & `xrootd-5.5.5/src/XrdSciTokens.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSec.cmake` & `xrootd-5.5.5/src/XrdSec.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecgsi.cmake` & `xrootd-5.5.5/src/XrdSecgsi.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSeckrb5.cmake` & `xrootd-5.5.5/src/XrdSeckrb5.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSecztn.cmake` & `xrootd-5.5.5/src/XrdSecztn.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdServer.cmake` & `xrootd-5.5.5/src/XrdServer.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdSsi.cmake` & `xrootd-5.5.5/src/XrdSsi.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdTpc.cmake` & `xrootd-5.5.5/src/XrdTpc.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdUtils.cmake` & `xrootd-5.5.5/src/XrdUtils.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdVersion.hh` & `xrootd-5.5.5/src/XrdVersion.hh`

 * *Files 1% similar despite different names*

```diff
@@ -27,22 +27,22 @@
 
 // this file is automatically updated by the genversion.sh script
 // if you touch anything make sure that it still works
 
 #ifndef __XRD_VERSION_H__
 #define __XRD_VERSION_H__
 
-#define XrdVERSION  "v5.5.4"
+#define XrdVERSION  "v5.5.5"
 
 // Numeric representation of the version tag
 // The format for the released code is: xyyzz, where: x is the major version,
 // y is the minor version and zz is the bugfix revision number
 // For the non-released code the value is 1000000
 #define XrdVNUMUNK  1000000
-#define XrdVNUMBER  50504
+#define XrdVNUMBER  50505
 
 #if XrdDEBUG
 #define XrdVSTRING XrdVERSION "_dbg"
 #else
 #define XrdVSTRING XrdVERSION
 #endif
```

### Comparing `xrootd-5.5.4/src/XrdVersion.hh.in` & `xrootd-5.5.5/src/XrdVersion.hh.in`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdVersionPlugin.hh` & `xrootd-5.5.5/src/XrdVersionPlugin.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdVoms.cmake` & `xrootd-5.5.5/src/XrdVoms.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/src/XrdXml.cmake` & `xrootd-5.5.5/src/XrdXml.cmake`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdCephTests/CMakeLists.txt` & `xrootd-5.5.5/tests/XrdCephTests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdCephTests/CephParsingTest.cc` & `xrootd-5.5.5/tests/XrdCephTests/CephParsingTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClHttp/cases/000-simple-download/main.sh` & `xrootd-5.5.5/tests/XrdClHttp/cases/000-simple-download/main.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClHttp/cases/001-deep-path-download/main.sh` & `xrootd-5.5.5/tests/XrdClHttp/cases/001-deep-path-download/main.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClHttp/cases/002-simple-upload/main.sh` & `xrootd-5.5.5/tests/XrdClHttp/cases/002-simple-upload/main.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClHttp/cases/003-deep-path-upload/main.sh` & `xrootd-5.5.5/tests/XrdClHttp/cases/003-deep-path-upload/main.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClHttp/common.sh` & `xrootd-5.5.5/tests/XrdClHttp/common.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClHttp/run_test.sh` & `xrootd-5.5.5/tests/XrdClHttp/run_test.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/tls/CMakeLists.txt` & `xrootd-5.5.5/tests/XrdClTests/tls/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/tls/README.md` & `xrootd-5.5.5/tests/XrdClTests/tls/README.md`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/tls/xrdcl-tls.cc` & `xrootd-5.5.5/tests/XrdClTests/tls/xrdcl-tls.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/tls/xrdsrv-tls.cc` & `xrootd-5.5.5/tests/XrdClTests/tls/xrdsrv-tls.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/wrt/xrdsrv-dio.cc` & `xrootd-5.5.5/tests/XrdClTests/wrt/xrdsrv-dio.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/wrt/xrdsrv-wrt.cc` & `xrootd-5.5.5/tests/XrdClTests/wrt/xrdsrv-wrt.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/CMakeLists.txt` & `xrootd-5.5.5/tests/XrdClTests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/FileCopyTest.cc` & `xrootd-5.5.5/tests/XrdClTests/FileCopyTest.cc`

 * *Files 0% similar despite different names*

```diff
@@ -393,15 +393,15 @@
     properties.Set( "checkSumPreset", "bad-value" ); //< provide wrong checksum value, so the check fails and the file gets removed
     properties.Set( "rmOnBadCksum",   true        );
     CPPUNIT_ASSERT_XRDST( process12.AddJob( properties, &results ) );
     CPPUNIT_ASSERT_XRDST( process12.Prepare() );
     CPPUNIT_ASSERT_XRDST_NOTOK( process12.Run(0), XrdCl::errCheckSumError );
     XrdCl::StatInfo *info = 0;
     XrdCl::XRootDStatus status = fs.Stat( targetPath, info );
-    CPPUNIT_ASSERT_XRDST( status.status == XrdCl::stError && st.code == XrdCl::errNotFound );
+    CPPUNIT_ASSERT_XRDST( status.status == XrdCl::stError && status.code == XrdCl::errNotFound );
     properties.Clear();
 
     //--------------------------------------------------------------------------
     // Copy with `--zip-mtln-cksum`
     //--------------------------------------------------------------------------
     results.Clear();
     properties.Set( "source",         metalinkURL2 );
```

### Comparing `xrootd-5.5.4/tests/XrdClTests/FileSystemTest.cc` & `xrootd-5.5.5/tests/XrdClTests/FileSystemTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/FileTest.cc` & `xrootd-5.5.5/tests/XrdClTests/FileTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/IdentityPlugIn.cc` & `xrootd-5.5.5/tests/XrdClTests/IdentityPlugIn.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/IdentityPlugIn.hh` & `xrootd-5.5.5/tests/XrdClTests/IdentityPlugIn.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/LocalFileHandlerTest.cc` & `xrootd-5.5.5/tests/XrdClTests/LocalFileHandlerTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/MonitorTestLib.cc` & `xrootd-5.5.5/tests/XrdClTests/MonitorTestLib.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/OperationsWorkflowTest.cc` & `xrootd-5.5.5/tests/XrdClTests/OperationsWorkflowTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/PollerTest.cc` & `xrootd-5.5.5/tests/XrdClTests/PollerTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/PostMasterTest.cc` & `xrootd-5.5.5/tests/XrdClTests/PostMasterTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/SocketTest.cc` & `xrootd-5.5.5/tests/XrdClTests/SocketTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/ThreadingTest.cc` & `xrootd-5.5.5/tests/XrdClTests/ThreadingTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/UtilsTest.cc` & `xrootd-5.5.5/tests/XrdClTests/UtilsTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/XRootDProtocolHelper.cc` & `xrootd-5.5.5/tests/XrdClTests/XRootDProtocolHelper.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdClTests/XRootDProtocolHelper.hh` & `xrootd-5.5.5/tests/XrdClTests/XRootDProtocolHelper.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdEcTests/MicroTest.cc` & `xrootd-5.5.5/tests/XrdEcTests/MicroTest.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/XrdSsiTests/XrdShMap.cc` & `xrootd-5.5.5/tests/XrdSsiTests/XrdShMap.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/common/CMakeLists.txt` & `xrootd-5.5.5/tests/common/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/common/CppUnitXrdHelpers.hh` & `xrootd-5.5.5/tests/common/CppUnitXrdHelpers.hh`

 * *Files 4% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 
 #include <XrdCl/XrdClXRootDResponses.hh>
 #include <cerrno>
 #include <cstring>
 
 #define CPPUNIT_ASSERT_XRDST_NOTOK( x, err )         \
 {                                                    \
-  XrdCl::XRootDStatus st = x;                        \
+  XrdCl::XRootDStatus _st = x;                       \
   std::string msg = "["; msg += #x; msg += "]: ";    \
-  msg += st.ToStr();                                 \
-  CPPUNIT_ASSERT_MESSAGE( msg, !st.IsOK() && st.code == err ); \
+  msg += _st.ToStr();                                \
+  CPPUNIT_ASSERT_MESSAGE( msg, !_st.IsOK() && _st.code == err ); \
 }
 
 #define CPPUNIT_ASSERT_XRDST( x )                    \
 {                                                    \
-  XrdCl::XRootDStatus st = x;                        \
+  XrdCl::XRootDStatus _st = x;                       \
   std::string msg = "["; msg += #x; msg += "]: ";    \
-  msg += st.ToStr();                                 \
-  CPPUNIT_ASSERT_MESSAGE( msg, st.IsOK() );          \
+  msg += _st.ToStr();                                \
+  CPPUNIT_ASSERT_MESSAGE( msg, _st.IsOK() );         \
 }
 
 #define CPPUNIT_ASSERT_ERRNO( x )                    \
 {                                                    \
   std::string msg = "["; msg += #x; msg += "]: ";    \
   msg += strerror( errno );                          \
   CPPUNIT_ASSERT_MESSAGE( msg, x );                  \
```

### Comparing `xrootd-5.5.4/tests/common/PathProcessor.hh` & `xrootd-5.5.5/tests/common/PathProcessor.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/common/Server.cc` & `xrootd-5.5.5/tests/common/Server.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/common/Server.hh` & `xrootd-5.5.5/tests/common/Server.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/common/TestEnv.cc` & `xrootd-5.5.5/tests/common/TestEnv.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/common/TestEnv.hh` & `xrootd-5.5.5/tests/common/TestEnv.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/common/TextRunner.cc` & `xrootd-5.5.5/tests/common/TextRunner.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/common/Utils.cc` & `xrootd-5.5.5/tests/common/Utils.cc`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/tests/common/Utils.hh` & `xrootd-5.5.5/tests/common/Utils.hh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/ups/eupspkg.cfg.sh` & `xrootd-5.5.5/ups/eupspkg.cfg.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/utils/XrdCmsNotify.pm` & `xrootd-5.5.5/utils/XrdCmsNotify.pm`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/utils/XrdOlbMonPerf` & `xrootd-5.5.5/utils/XrdOlbMonPerf`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/utils/cms_monPerf` & `xrootd-5.5.5/utils/cms_monPerf`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/utils/hpsscp` & `xrootd-5.5.5/utils/hpsscp`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/utils/netchk` & `xrootd-5.5.5/utils/netchk`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/utils/xrootd-config` & `xrootd-5.5.5/utils/xrootd-config`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/xrootd.egg-info/SOURCES.txt` & `xrootd-5.5.5/xrootd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/CMakeLists.txt` & `xrootd-5.5.5/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/COPYING` & `xrootd-5.5.5/COPYING`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/COPYING.BSD` & `xrootd-5.5.5/COPYING.BSD`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/COPYING.LGPL` & `xrootd-5.5.5/COPYING.LGPL`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/LICENSE` & `xrootd-5.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/README` & `xrootd-5.5.5/README`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/cmake_uninstall.cmake.in` & `xrootd-5.5.5/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/gen-tarball.sh` & `xrootd-5.5.5/gen-tarball.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/genversion.sh` & `xrootd-5.5.5/genversion.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/install.sh` & `xrootd-5.5.5/install.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/publish.sh` & `xrootd-5.5.5/publish.sh`

 * *Files identical despite different names*

### Comparing `xrootd-5.5.4/setup.py` & `xrootd-5.5.5/setup.py`

 * *Files identical despite different names*

