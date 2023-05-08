# Comparing `tmp/wdmtoolbox-7.9.7.5.tar.gz` & `tmp/wdmtoolbox-8.9.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wdmtoolbox-7.9.7.5.tar", last modified: Thu Jul 26 06:20:10 2018, max compression
+gzip compressed data, was "dist/wdmtoolbox-8.9.7.5.tar", last modified: Sat Aug 11 07:19:59 2018, max compression
```

## Comparing `wdmtoolbox-7.9.7.5.tar` & `wdmtoolbox-8.9.7.5.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2018-07-26 06:20:10.000000 wdmtoolbox-7.9.7.5/
--rw-r--r--   0 tim       (1000) tim       (1000)     1988 2018-07-26 05:48:49.000000 wdmtoolbox-7.9.7.5/README.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     3173 2017-07-21 14:05:12.000000 wdmtoolbox-7.9.7.5/CONTRIBUTING.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     3464 2018-07-26 05:48:49.000000 wdmtoolbox-7.9.7.5/setup.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1487 2015-10-20 13:00:40.000000 wdmtoolbox-7.9.7.5/LICENSE.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       49 2018-07-26 05:48:49.000000 wdmtoolbox-7.9.7.5/pip_requirements.txt
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2018-07-26 06:20:10.000000 wdmtoolbox-7.9.7.5/wdmtoolbox.data/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2017-08-03 23:43:07.000000 wdmtoolbox-7.9.7.5/wdmtoolbox.data/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)      173 2018-07-26 05:48:49.000000 wdmtoolbox-7.9.7.5/MANIFEST.in
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2018-07-26 06:20:10.000000 wdmtoolbox-7.9.7.5/docsrc/
--rw-rw-r--   0 tim       (1000) tim       (1000)       55 2017-07-21 14:05:12.000000 wdmtoolbox-7.9.7.5/docsrc/authors.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     5712 2015-10-20 13:00:40.000000 wdmtoolbox-7.9.7.5/docsrc/Makefile
--rw-r--r--   0 tim       (1000) tim       (1000)     2730 2018-07-26 05:48:49.000000 wdmtoolbox-7.9.7.5/docsrc/install.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     3787 2018-07-26 05:48:49.000000 wdmtoolbox-7.9.7.5/docsrc/usage.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      797 2018-07-26 05:48:49.000000 wdmtoolbox-7.9.7.5/docsrc/function_summary.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)       79 2017-07-21 14:05:12.000000 wdmtoolbox-7.9.7.5/docsrc/license.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       27 2017-07-21 14:05:12.000000 wdmtoolbox-7.9.7.5/docsrc/readme.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)       60 2017-07-21 14:05:12.000000 wdmtoolbox-7.9.7.5/docsrc/contributing.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     5104 2015-10-20 13:00:40.000000 wdmtoolbox-7.9.7.5/docsrc/make.bat
--rw-r--r--   0 tim       (1000) tim       (1000)     8073 2018-07-26 05:48:49.000000 wdmtoolbox-7.9.7.5/docsrc/conf.py
--rw-r--r--   0 tim       (1000) tim       (1000)      725 2018-07-26 05:48:49.000000 wdmtoolbox-7.9.7.5/docsrc/index.rst
--rw-r--r--   0 tim       (1000) tim       (1000)        8 2018-07-26 06:19:11.000000 wdmtoolbox-7.9.7.5/VERSION
--rw-rw-r--   0 tim       (1000) tim       (1000)       56 2017-07-21 14:05:12.000000 wdmtoolbox-7.9.7.5/AUTHORS.rst
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2018-07-26 06:20:10.000000 wdmtoolbox-7.9.7.5/wdmtoolbox.egg-info/
--rw-rw-r--   0 tim       (1000) tim       (1000)       47 2016-04-06 14:04:51.000000 wdmtoolbox-7.9.7.5/wdmtoolbox.egg-info/pbr.json
--rw-r--r--   0 tim       (1000) tim       (1000)       59 2018-07-26 06:20:09.000000 wdmtoolbox-7.9.7.5/wdmtoolbox.egg-info/entry_points.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       31 2018-07-26 06:20:09.000000 wdmtoolbox-7.9.7.5/wdmtoolbox.egg-info/requires.txt
--rw-r--r--   0 tim       (1000) tim       (1000)        1 2018-07-26 06:20:09.000000 wdmtoolbox-7.9.7.5/wdmtoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       20 2018-07-26 06:20:09.000000 wdmtoolbox-7.9.7.5/wdmtoolbox.egg-info/top_level.txt
--rw-r--r--   0 tim       (1000) tim       (1000)     1394 2018-07-26 06:20:09.000000 wdmtoolbox-7.9.7.5/wdmtoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 tim       (1000) tim       (1000)     3475 2018-07-26 06:20:09.000000 wdmtoolbox-7.9.7.5/wdmtoolbox.egg-info/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)        1 2013-09-24 20:14:38.000000 wdmtoolbox-7.9.7.5/wdmtoolbox.egg-info/not-zip-safe
--rw-r--r--   0 tim       (1000) tim       (1000)     3475 2018-07-26 06:20:10.000000 wdmtoolbox-7.9.7.5/PKG-INFO
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2018-07-26 06:20:10.000000 wdmtoolbox-7.9.7.5/wdm_support/
--rw-r--r--   0 tim       (1000) tim       (1000)    95523 2013-10-18 19:50:59.000000 wdmtoolbox-7.9.7.5/wdm_support/UTCHAR.f
--rw-r--r--   0 tim       (1000) tim       (1000)       97 2013-10-18 19:50:59.000000 wdmtoolbox-7.9.7.5/wdm_support/FVERSN.INC
--rw-r--r--   0 tim       (1000) tim       (1000)     3424 2013-10-22 02:18:05.000000 wdmtoolbox-7.9.7.5/wdm_support/WDOP.f
--rw-r--r--   0 tim       (1000) tim       (1000)    35522 2013-10-18 19:50:59.000000 wdmtoolbox-7.9.7.5/wdm_support/UTWDT1.f
--rw-r--r--   0 tim       (1000) tim       (1000)    19315 2013-10-18 19:50:59.000000 wdmtoolbox-7.9.7.5/wdm_support/UTNUMB.f
--rw-r--r--   0 tim       (1000) tim       (1000)    20908 2013-10-18 19:50:59.000000 wdmtoolbox-7.9.7.5/wdm_support/TSBUFR.f
--rw-rw-r--   0 tim       (1000) tim       (1000)    35718 2015-10-20 13:00:40.000000 wdmtoolbox-7.9.7.5/wdm_support/WDATRB.f
--rw-r--r--   0 tim       (1000) tim       (1000)      283 2013-10-18 19:50:59.000000 wdmtoolbox-7.9.7.5/wdm_support/CDRLOC.INC
--rw-r--r--   0 tim       (1000) tim       (1000)   111767 2018-07-26 05:48:49.000000 wdmtoolbox-7.9.7.5/wdm_support/wdm.pyf
--rw-r--r--   0 tim       (1000) tim       (1000)      657 2013-10-18 19:50:59.000000 wdmtoolbox-7.9.7.5/wdm_support/CTSBUF.INC
--rw-r--r--   0 tim       (1000) tim       (1000)    40938 2013-10-18 19:50:59.000000 wdmtoolbox-7.9.7.5/wdm_support/WDTMS2.f
--rw-rw-r--   0 tim       (1000) tim       (1000)     1139 2018-07-26 05:48:58.000000 wdmtoolbox-7.9.7.5/wdm_support/_wdm_lib-f2pywrappers.f
--rw-r--r--   0 tim       (1000) tim       (1000)    39146 2016-02-11 15:32:35.000000 wdmtoolbox-7.9.7.5/wdm_support/UTWDMD.f
--rw-r--r--   0 tim       (1000) tim       (1000)    17488 2013-10-18 19:50:59.000000 wdmtoolbox-7.9.7.5/wdm_support/WDMESS.f
--rw-r--r--   0 tim       (1000) tim       (1000)    10003 2013-10-18 19:50:59.000000 wdmtoolbox-7.9.7.5/wdm_support/WDATM2.f
--rw-r--r--   0 tim       (1000) tim       (1000)      282 2013-10-18 19:50:59.000000 wdmtoolbox-7.9.7.5/wdm_support/CWDMID.INC
--rw-rw-r--   0 tim       (1000) tim       (1000)    88527 2018-07-26 05:48:58.000000 wdmtoolbox-7.9.7.5/wdm_support/_wdm_libmodule.c
--rw-rw-r--   0 tim       (1000) tim       (1000)     1139 2018-07-26 05:48:20.000000 wdmtoolbox-7.9.7.5/wdm_support/wdm-f2pywrappers.f
--rw-r--r--   0 tim       (1000) tim       (1000)     3604 2013-10-18 19:50:59.000000 wdmtoolbox-7.9.7.5/wdm_support/DTTM90.f
--rw-r--r--   0 tim       (1000) tim       (1000)     4170 2013-10-18 19:50:59.000000 wdmtoolbox-7.9.7.5/wdm_support/UTCP90.f
--rw-r--r--   0 tim       (1000) tim       (1000)    14261 2013-10-21 03:41:38.000000 wdmtoolbox-7.9.7.5/wdm_support/WDBTCH.f
--rw-r--r--   0 tim       (1000) tim       (1000)    18886 2013-10-18 19:50:59.000000 wdmtoolbox-7.9.7.5/wdm_support/WDATM1.f
--rw-r--r--   0 tim       (1000) tim       (1000)    29843 2013-10-18 19:50:59.000000 wdmtoolbox-7.9.7.5/wdm_support/UTWDMF.f
--rw-r--r--   0 tim       (1000) tim       (1000)      615 2013-10-18 19:50:59.000000 wdmtoolbox-7.9.7.5/wdm_support/CFBUFF.INC
--rw-r--r--   0 tim       (1000) tim       (1000)    59699 2013-10-21 18:30:40.000000 wdmtoolbox-7.9.7.5/wdm_support/UTDATE.f
--rw-rw-r--   0 tim       (1000) tim       (1000)    87497 2018-07-26 05:48:20.000000 wdmtoolbox-7.9.7.5/wdm_support/wdmmodule.c
--rw-r--r--   0 tim       (1000) tim       (1000)    73127 2013-10-21 20:15:21.000000 wdmtoolbox-7.9.7.5/wdm_support/WDTMS1.f
--rw-r--r--   0 tim       (1000) tim       (1000)     6297 2013-10-21 18:30:32.000000 wdmtoolbox-7.9.7.5/wdm_support/WDMID.f
--rw-r--r--   0 tim       (1000) tim       (1000)      939 2013-10-18 19:50:59.000000 wdmtoolbox-7.9.7.5/wdm_support/CONST.INC
--rw-r--r--   0 tim       (1000) tim       (1000)      495 2013-10-18 19:50:59.000000 wdmtoolbox-7.9.7.5/wdm_support/CWTSDS.INC
--rw-rw-r--   0 tim       (1000) tim       (1000)      113 2018-07-26 06:20:10.000000 wdmtoolbox-7.9.7.5/setup.cfg
--rw-r--r--   0 tim       (1000) tim       (1000)      591 2018-07-26 05:48:49.000000 wdmtoolbox-7.9.7.5/BADGES.rst
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2018-07-26 06:20:10.000000 wdmtoolbox-7.9.7.5/wdmtoolbox/
--rwxr-xr-x   0 tim       (1000) tim       (1000)    25077 2018-07-26 05:48:49.000000 wdmtoolbox-7.9.7.5/wdmtoolbox/wdmutil.py
--rwxr-xr-x   0 tim       (1000) tim       (1000)    17849 2018-07-26 06:14:32.000000 wdmtoolbox-7.9.7.5/wdmtoolbox/wdmtoolbox.py
--rw-r--r--   0 tim       (1000) tim       (1000)       27 2018-07-26 05:48:49.000000 wdmtoolbox-7.9.7.5/wdmtoolbox/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)   204800 2018-07-26 05:48:49.000000 wdmtoolbox-7.9.7.5/wdmtoolbox/message.wdm
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2018-08-11 07:19:59.000000 wdmtoolbox-8.9.7.5/
+-rw-r--r--   0 tim       (1000) tim       (1000)     1988 2018-07-26 05:48:49.000000 wdmtoolbox-8.9.7.5/README.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3173 2017-07-21 14:05:12.000000 wdmtoolbox-8.9.7.5/CONTRIBUTING.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     3464 2018-08-11 00:24:54.000000 wdmtoolbox-8.9.7.5/setup.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1487 2015-10-20 13:00:40.000000 wdmtoolbox-8.9.7.5/LICENSE.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       49 2018-07-26 05:48:49.000000 wdmtoolbox-8.9.7.5/pip_requirements.txt
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2018-08-11 07:19:59.000000 wdmtoolbox-8.9.7.5/wdmtoolbox.data/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2017-08-03 23:43:07.000000 wdmtoolbox-8.9.7.5/wdmtoolbox.data/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      173 2018-07-26 05:48:49.000000 wdmtoolbox-8.9.7.5/MANIFEST.in
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2018-08-11 07:19:58.000000 wdmtoolbox-8.9.7.5/docsrc/
+-rw-rw-r--   0 tim       (1000) tim       (1000)       55 2017-07-21 14:05:12.000000 wdmtoolbox-8.9.7.5/docsrc/authors.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5712 2015-10-20 13:00:40.000000 wdmtoolbox-8.9.7.5/docsrc/Makefile
+-rw-r--r--   0 tim       (1000) tim       (1000)     2730 2018-07-26 05:48:49.000000 wdmtoolbox-8.9.7.5/docsrc/install.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     3787 2018-07-26 05:48:49.000000 wdmtoolbox-8.9.7.5/docsrc/usage.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      797 2018-07-26 05:48:49.000000 wdmtoolbox-8.9.7.5/docsrc/function_summary.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)       79 2017-07-21 14:05:12.000000 wdmtoolbox-8.9.7.5/docsrc/license.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       27 2017-07-21 14:05:12.000000 wdmtoolbox-8.9.7.5/docsrc/readme.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)       60 2017-07-21 14:05:12.000000 wdmtoolbox-8.9.7.5/docsrc/contributing.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5104 2015-10-20 13:00:40.000000 wdmtoolbox-8.9.7.5/docsrc/make.bat
+-rw-r--r--   0 tim       (1000) tim       (1000)     8073 2018-07-26 05:48:49.000000 wdmtoolbox-8.9.7.5/docsrc/conf.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      725 2018-07-26 05:48:49.000000 wdmtoolbox-8.9.7.5/docsrc/index.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)        8 2018-08-11 05:14:07.000000 wdmtoolbox-8.9.7.5/VERSION
+-rw-rw-r--   0 tim       (1000) tim       (1000)       56 2017-07-21 14:05:12.000000 wdmtoolbox-8.9.7.5/AUTHORS.rst
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2018-08-11 07:19:59.000000 wdmtoolbox-8.9.7.5/wdmtoolbox.egg-info/
+-rw-rw-r--   0 tim       (1000) tim       (1000)       47 2016-04-06 14:04:51.000000 wdmtoolbox-8.9.7.5/wdmtoolbox.egg-info/pbr.json
+-rw-r--r--   0 tim       (1000) tim       (1000)       59 2018-08-11 07:19:57.000000 wdmtoolbox-8.9.7.5/wdmtoolbox.egg-info/entry_points.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       31 2018-08-11 07:19:57.000000 wdmtoolbox-8.9.7.5/wdmtoolbox.egg-info/requires.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)        1 2018-08-11 07:19:57.000000 wdmtoolbox-8.9.7.5/wdmtoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       20 2018-08-11 07:19:57.000000 wdmtoolbox-8.9.7.5/wdmtoolbox.egg-info/top_level.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)     1394 2018-08-11 07:19:57.000000 wdmtoolbox-8.9.7.5/wdmtoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)     3475 2018-08-11 07:19:57.000000 wdmtoolbox-8.9.7.5/wdmtoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)        1 2013-09-24 20:14:38.000000 wdmtoolbox-8.9.7.5/wdmtoolbox.egg-info/not-zip-safe
+-rw-r--r--   0 tim       (1000) tim       (1000)     3475 2018-08-11 07:19:59.000000 wdmtoolbox-8.9.7.5/PKG-INFO
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2018-08-11 07:19:58.000000 wdmtoolbox-8.9.7.5/wdm_support/
+-rw-r--r--   0 tim       (1000) tim       (1000)    95523 2013-10-18 19:50:59.000000 wdmtoolbox-8.9.7.5/wdm_support/UTCHAR.f
+-rw-r--r--   0 tim       (1000) tim       (1000)       97 2013-10-18 19:50:59.000000 wdmtoolbox-8.9.7.5/wdm_support/FVERSN.INC
+-rw-r--r--   0 tim       (1000) tim       (1000)     3424 2013-10-22 02:18:05.000000 wdmtoolbox-8.9.7.5/wdm_support/WDOP.f
+-rw-r--r--   0 tim       (1000) tim       (1000)    35522 2013-10-18 19:50:59.000000 wdmtoolbox-8.9.7.5/wdm_support/UTWDT1.f
+-rw-r--r--   0 tim       (1000) tim       (1000)    19315 2013-10-18 19:50:59.000000 wdmtoolbox-8.9.7.5/wdm_support/UTNUMB.f
+-rw-r--r--   0 tim       (1000) tim       (1000)    20908 2013-10-18 19:50:59.000000 wdmtoolbox-8.9.7.5/wdm_support/TSBUFR.f
+-rw-rw-r--   0 tim       (1000) tim       (1000)    35718 2015-10-20 13:00:40.000000 wdmtoolbox-8.9.7.5/wdm_support/WDATRB.f
+-rw-r--r--   0 tim       (1000) tim       (1000)      283 2013-10-18 19:50:59.000000 wdmtoolbox-8.9.7.5/wdm_support/CDRLOC.INC
+-rw-r--r--   0 tim       (1000) tim       (1000)   111767 2018-07-26 05:48:49.000000 wdmtoolbox-8.9.7.5/wdm_support/wdm.pyf
+-rw-r--r--   0 tim       (1000) tim       (1000)      657 2013-10-18 19:50:59.000000 wdmtoolbox-8.9.7.5/wdm_support/CTSBUF.INC
+-rw-r--r--   0 tim       (1000) tim       (1000)    40938 2013-10-18 19:50:59.000000 wdmtoolbox-8.9.7.5/wdm_support/WDTMS2.f
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1139 2018-07-26 05:48:58.000000 wdmtoolbox-8.9.7.5/wdm_support/_wdm_lib-f2pywrappers.f
+-rw-r--r--   0 tim       (1000) tim       (1000)    39146 2016-02-11 15:32:35.000000 wdmtoolbox-8.9.7.5/wdm_support/UTWDMD.f
+-rw-r--r--   0 tim       (1000) tim       (1000)    17488 2013-10-18 19:50:59.000000 wdmtoolbox-8.9.7.5/wdm_support/WDMESS.f
+-rw-r--r--   0 tim       (1000) tim       (1000)    10003 2013-10-18 19:50:59.000000 wdmtoolbox-8.9.7.5/wdm_support/WDATM2.f
+-rw-r--r--   0 tim       (1000) tim       (1000)      282 2013-10-18 19:50:59.000000 wdmtoolbox-8.9.7.5/wdm_support/CWDMID.INC
+-rw-rw-r--   0 tim       (1000) tim       (1000)    88527 2018-07-26 05:48:58.000000 wdmtoolbox-8.9.7.5/wdm_support/_wdm_libmodule.c
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1139 2018-07-26 05:48:20.000000 wdmtoolbox-8.9.7.5/wdm_support/wdm-f2pywrappers.f
+-rw-r--r--   0 tim       (1000) tim       (1000)     3604 2013-10-18 19:50:59.000000 wdmtoolbox-8.9.7.5/wdm_support/DTTM90.f
+-rw-r--r--   0 tim       (1000) tim       (1000)     4170 2013-10-18 19:50:59.000000 wdmtoolbox-8.9.7.5/wdm_support/UTCP90.f
+-rw-r--r--   0 tim       (1000) tim       (1000)    14261 2013-10-21 03:41:38.000000 wdmtoolbox-8.9.7.5/wdm_support/WDBTCH.f
+-rw-r--r--   0 tim       (1000) tim       (1000)    18886 2013-10-18 19:50:59.000000 wdmtoolbox-8.9.7.5/wdm_support/WDATM1.f
+-rw-r--r--   0 tim       (1000) tim       (1000)    29843 2013-10-18 19:50:59.000000 wdmtoolbox-8.9.7.5/wdm_support/UTWDMF.f
+-rw-r--r--   0 tim       (1000) tim       (1000)      615 2013-10-18 19:50:59.000000 wdmtoolbox-8.9.7.5/wdm_support/CFBUFF.INC
+-rw-r--r--   0 tim       (1000) tim       (1000)    59699 2013-10-21 18:30:40.000000 wdmtoolbox-8.9.7.5/wdm_support/UTDATE.f
+-rw-rw-r--   0 tim       (1000) tim       (1000)    87497 2018-07-26 05:48:20.000000 wdmtoolbox-8.9.7.5/wdm_support/wdmmodule.c
+-rw-r--r--   0 tim       (1000) tim       (1000)    73127 2013-10-21 20:15:21.000000 wdmtoolbox-8.9.7.5/wdm_support/WDTMS1.f
+-rw-r--r--   0 tim       (1000) tim       (1000)     6297 2013-10-21 18:30:32.000000 wdmtoolbox-8.9.7.5/wdm_support/WDMID.f
+-rw-r--r--   0 tim       (1000) tim       (1000)      939 2013-10-18 19:50:59.000000 wdmtoolbox-8.9.7.5/wdm_support/CONST.INC
+-rw-r--r--   0 tim       (1000) tim       (1000)      495 2013-10-18 19:50:59.000000 wdmtoolbox-8.9.7.5/wdm_support/CWTSDS.INC
+-rw-rw-r--   0 tim       (1000) tim       (1000)      113 2018-08-11 07:19:59.000000 wdmtoolbox-8.9.7.5/setup.cfg
+-rw-r--r--   0 tim       (1000) tim       (1000)      591 2018-07-26 05:48:49.000000 wdmtoolbox-8.9.7.5/BADGES.rst
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2018-08-11 07:19:59.000000 wdmtoolbox-8.9.7.5/wdmtoolbox/
+-rwxr-xr-x   0 tim       (1000) tim       (1000)    25424 2018-08-11 03:57:16.000000 wdmtoolbox-8.9.7.5/wdmtoolbox/wdmutil.py
+-rwxr-xr-x   0 tim       (1000) tim       (1000)    17595 2018-08-11 03:57:53.000000 wdmtoolbox-8.9.7.5/wdmtoolbox/wdmtoolbox.py
+-rw-r--r--   0 tim       (1000) tim       (1000)       27 2018-07-26 05:48:49.000000 wdmtoolbox-8.9.7.5/wdmtoolbox/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)   204800 2018-07-26 05:48:49.000000 wdmtoolbox-8.9.7.5/wdmtoolbox/message.wdm
```

### Comparing `wdmtoolbox-7.9.7.5/README.rst` & `wdmtoolbox-8.9.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/CONTRIBUTING.rst` & `wdmtoolbox-8.9.7.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/setup.py` & `wdmtoolbox-8.9.7.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 README = open(os.path.join(here, 'README.rst')).read()
 
 install_requires = [
     # List your project dependencies here.
     # For more details, see:
     # http://packages.python.org/distribute/setuptools.html#declaring-dependencies
     'tstoolbox >= 9.26.17.13',
-    'lockfile',
+    'filelock',
 ]
 
 libraries = []
 if sys.platform.startswith('win'):
     libraries = ['quadmath']
 
 wdm_support = Extension('_wdm_lib', [
```

### Comparing `wdmtoolbox-7.9.7.5/LICENSE.txt` & `wdmtoolbox-8.9.7.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/docsrc/Makefile` & `wdmtoolbox-8.9.7.5/docsrc/Makefile`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/docsrc/install.rst` & `wdmtoolbox-8.9.7.5/docsrc/install.rst`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/docsrc/usage.rst` & `wdmtoolbox-8.9.7.5/docsrc/usage.rst`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/docsrc/function_summary.rst` & `wdmtoolbox-8.9.7.5/docsrc/function_summary.rst`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/docsrc/make.bat` & `wdmtoolbox-8.9.7.5/docsrc/make.bat`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/docsrc/conf.py` & `wdmtoolbox-8.9.7.5/docsrc/conf.py`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/docsrc/index.rst` & `wdmtoolbox-8.9.7.5/docsrc/index.rst`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdmtoolbox.egg-info/SOURCES.txt` & `wdmtoolbox-8.9.7.5/wdmtoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdmtoolbox.egg-info/PKG-INFO` & `wdmtoolbox-8.9.7.5/wdmtoolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: wdmtoolbox
-Version: 7.9.7.5
+Version: 8.9.7.5
 Summary: Read and write Watershed Data Management (WDM) files
 Home-page: http://timcera.bitbucket.io/wdmtoolbox/docsrc/index.html
 Author: Tim Cera, P.E.
 Author-email: tim@cerazone.net
 License: UNKNOWN
 Description: .. image:: https://travis-ci.org/timcera/wdmtoolbox.svg?branch=master
             :target: https://travis-ci.org/timcera/wdmtoolbox
```

### Comparing `wdmtoolbox-7.9.7.5/PKG-INFO` & `wdmtoolbox-8.9.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: wdmtoolbox
-Version: 7.9.7.5
+Version: 8.9.7.5
 Summary: Read and write Watershed Data Management (WDM) files
 Home-page: http://timcera.bitbucket.io/wdmtoolbox/docsrc/index.html
 Author: Tim Cera, P.E.
 Author-email: tim@cerazone.net
 License: UNKNOWN
 Description: .. image:: https://travis-ci.org/timcera/wdmtoolbox.svg?branch=master
             :target: https://travis-ci.org/timcera/wdmtoolbox
```

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/UTCHAR.f` & `wdmtoolbox-8.9.7.5/wdm_support/UTCHAR.f`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/WDOP.f` & `wdmtoolbox-8.9.7.5/wdm_support/WDOP.f`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/UTWDT1.f` & `wdmtoolbox-8.9.7.5/wdm_support/UTWDT1.f`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/UTNUMB.f` & `wdmtoolbox-8.9.7.5/wdm_support/UTNUMB.f`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/TSBUFR.f` & `wdmtoolbox-8.9.7.5/wdm_support/TSBUFR.f`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/WDATRB.f` & `wdmtoolbox-8.9.7.5/wdm_support/WDATRB.f`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/wdm.pyf` & `wdmtoolbox-8.9.7.5/wdm_support/wdm.pyf`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/CTSBUF.INC` & `wdmtoolbox-8.9.7.5/wdm_support/CTSBUF.INC`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/WDTMS2.f` & `wdmtoolbox-8.9.7.5/wdm_support/WDTMS2.f`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/_wdm_lib-f2pywrappers.f` & `wdmtoolbox-8.9.7.5/wdm_support/_wdm_lib-f2pywrappers.f`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/UTWDMD.f` & `wdmtoolbox-8.9.7.5/wdm_support/UTWDMD.f`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/WDMESS.f` & `wdmtoolbox-8.9.7.5/wdm_support/WDMESS.f`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/WDATM2.f` & `wdmtoolbox-8.9.7.5/wdm_support/WDATM2.f`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/_wdm_libmodule.c` & `wdmtoolbox-8.9.7.5/wdm_support/_wdm_libmodule.c`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/wdm-f2pywrappers.f` & `wdmtoolbox-8.9.7.5/wdm_support/wdm-f2pywrappers.f`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/DTTM90.f` & `wdmtoolbox-8.9.7.5/wdm_support/DTTM90.f`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/UTCP90.f` & `wdmtoolbox-8.9.7.5/wdm_support/UTCP90.f`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/WDBTCH.f` & `wdmtoolbox-8.9.7.5/wdm_support/WDBTCH.f`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/WDATM1.f` & `wdmtoolbox-8.9.7.5/wdm_support/WDATM1.f`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/UTWDMF.f` & `wdmtoolbox-8.9.7.5/wdm_support/UTWDMF.f`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/CFBUFF.INC` & `wdmtoolbox-8.9.7.5/wdm_support/CFBUFF.INC`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/UTDATE.f` & `wdmtoolbox-8.9.7.5/wdm_support/UTDATE.f`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/wdmmodule.c` & `wdmtoolbox-8.9.7.5/wdm_support/wdmmodule.c`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/WDTMS1.f` & `wdmtoolbox-8.9.7.5/wdm_support/WDTMS1.f`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/WDMID.f` & `wdmtoolbox-8.9.7.5/wdm_support/WDMID.f`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdm_support/CONST.INC` & `wdmtoolbox-8.9.7.5/wdm_support/CONST.INC`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/BADGES.rst` & `wdmtoolbox-8.9.7.5/BADGES.rst`

 * *Files identical despite different names*

### Comparing `wdmtoolbox-7.9.7.5/wdmtoolbox/wdmutil.py` & `wdmtoolbox-8.9.7.5/wdmtoolbox/wdmutil.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,26 @@
 The WDM class supplies a series of utilities for working with WDM files
 with Python.  The class uses f2py to wrap the minimally necessary WDM
 routines.
 """
 
 from __future__ import print_function
 
-from builtins import str
-from builtins import object
 import datetime
 import os
 import os.path
 import re
 
+from builtins import object
+from builtins import str
+from filelock import SoftFileLock
 import pandas as pd
 
-from lockfile import LockFile
-
-import _wdm_lib
 from tstoolbox import tsutils
-
-# Load in WDM subroutines
+import _wdm_lib
 
 # Mapping between WDM TCODE and pandas interval code
 MAPTCODE = {
     1: 'S',
     2: 'T',
     3: 'H',
     4: 'D',
@@ -281,61 +278,58 @@
 """.format(retcode, additional_info))
 
     def renumber_dsn(self, wdmpath, odsn, ndsn):
         """Will renumber the odsn to the ndsn."""
         odsn = int(odsn)
         ndsn = int(ndsn)
 
-        lock = LockFile(wdmpath)
-        lock.acquire()
-        wdmfp = self._open(wdmpath, 51)
-        retcode = self.wddsrn(
-            wdmfp,
-            odsn,
-            ndsn)
-        lock.release()
-        self._close(wdmpath)
+        lock = SoftFileLock(wdmpath + '.lock', timeout=30)
+        with lock:
+            wdmfp = self._open(wdmpath, 51)
+            retcode = self.wddsrn(
+                wdmfp,
+                odsn,
+                ndsn)
+            self._close(wdmpath)
         self._retcode_check(retcode, additional_info='wddsrn')
 
     def delete_dsn(self, wdmpath, dsn):
-        """Function to delete a DSN."""
+        """Delete a DSN."""
         dsn = int(dsn)
 
-        lock = LockFile(wdmpath)
-        lock.acquire()
-        wdmfp = self._open(wdmpath, 52)
-        testreturn = self.wdckdt(wdmfp, dsn)
-        self._close(wdmpath)
-        if testreturn != 0:
+        lock = SoftFileLock(wdmpath + '.lock', timeout=30)
+        with lock:
             wdmfp = self._open(wdmpath, 52)
-            retcode = self.wddsdl(wdmfp,
-                                  dsn)
+            testreturn = self.wdckdt(wdmfp, dsn)
+            self._close(wdmpath)
+            if testreturn != 0:
+                wdmfp = self._open(wdmpath, 52)
+                retcode = self.wddsdl(wdmfp,
+                                      dsn)
+                self._close(wdmpath)
+                self._retcode_check(retcode, additional_info='wddsdl')
             self._close(wdmpath)
-            self._retcode_check(retcode, additional_info='wddsdl')
-        lock.release()
-        self._close(wdmpath)
 
     def copydsnlabel(self, inwdmpath, indsn, outwdmpath, outdsn):
         """Will copy a complete DSN label from one DSN to another."""
         assert inwdmpath != outwdmpath
         indsn = int(indsn)
         outdsn = int(outdsn)
         dsntype = 0
         inwdmfp = self._open(inwdmpath, 53, ronwfg=1)
-        lock = LockFile(outwdmpath)
-        lock.acquire()
-        outwdmfp = self._open(outwdmpath, 54)
-        retcode = self.wddscl(inwdmfp,
-                              indsn,
-                              outwdmfp,
-                              outdsn,
-                              dsntype)
+        lock = SoftFileLock(outwdmpath + '.lock', timeout=30)
+        with lock:
+            outwdmfp = self._open(outwdmpath, 54)
+            retcode = self.wddscl(inwdmfp,
+                                  indsn,
+                                  outwdmfp,
+                                  outdsn,
+                                  dsntype)
+            self._close(outwdmpath)
         self._close(inwdmpath)
-        lock.release()
-        self._close(outwdmpath)
         self._retcode_check(retcode, additional_info='wddscl')
 
     def describe_dsn(self, wdmpath, dsn):
         """Will collect some metadata about the DSN."""
         wdmfp = self._open(wdmpath, 55, ronwfg=1)
         _, llsdat, lledat, retcode = self.wtfndt(
             wdmfp,
@@ -458,34 +452,34 @@
         except ValueError:
             sdate = None
         try:
             edate = datetime.datetime(*lledat).date()
         except ValueError:
             edate = None
 
-        dateFormat_dict = {1: "S",
-                           2: "T",
-                           3: "H",
-                           4: "D",
-                           5: "M",
-                           6: "A"}
+        dateformat_dict = {1: 'S',
+                           2: 'T',
+                           3: 'H',
+                           4: 'D',
+                           5: 'M',
+                           6: 'A'}
 
         tstep = tstep[0]
         tcode = tcode[0]
         base_year = base_year[0]
 
         ostr = b''.join(ostr).strip()
         scen_ostr = b''.join(scen_ostr).strip()
         con_ostr = b''.join(con_ostr).strip()
         desc_ostr = b''.join(desc_ostr).strip()
         tstype = b''.join(tstype).strip()
 
         return {'dsn':         dsn,
-                'start_date':  pd.Period(sdate, freq=dateFormat_dict[tcode]),
-                'end_date':    pd.Period(edate, freq=dateFormat_dict[tcode]),
+                'start_date':  pd.Period(sdate, freq=dateformat_dict[tcode]),
+                'end_date':    pd.Period(edate, freq=dateformat_dict[tcode]),
                 'llsdat':      llsdat,
                 'lledat':      lledat,
                 'tstep':       tstep,
                 'tcode':       tcode,
                 'tcode_name':  MAPTCODE[tcode],
                 'location':    ostr.strip(),
                 'scenario':    scen_ostr.strip(),
@@ -510,91 +504,90 @@
         """Set DSN attributes."""
         pass
 
     def create_new_dsn(self, wdmpath, dsn, tstype='', base_year=1900, tcode=4,
                        tsstep=1, statid=' ', scenario='', location='',
                        description='', constituent='', tsfill=-999.0):
         """Create self.wdmfp/dsn."""
-        lock = LockFile(wdmpath)
-        lock.acquire()
-        wdmfp = self._open(wdmpath, 57)
-        messfp = self.wmsgop()
-
-        if self.wdckdt(wdmfp, dsn) == 1:
-            self._close(wdmpath)
-            raise DSNExistsError(dsn)
+        lock = SoftFileLock(wdmpath + '.lock', timeout=30)
+        with lock:
+            wdmfp = self._open(wdmpath, 57)
+            messfp = self.wmsgop()
+
+            if self.wdckdt(wdmfp, dsn) == 1:
+                self._close(wdmpath)
+                raise DSNExistsError(dsn)
 
-        # Parameters for wdlbax taken from ATCTSfile/clsTSerWDM.cls
-        self.wdlbax(
-            wdmfp,
-            dsn,
-            1,     # DSTYPE - always 1 for time series
-            10,    # NDN    - number of down pointers
-            10,    # NUP    - number of up pointers
-            30,    # NSA    - number of search attributes
-            100,   # NSASP  - amount of search attribute space
-            300,   # NDP    - number of data pointers
-        )      # PSA    - pointer to search attribute space
-
-        for saind, salen, saval in [(34, 1, 6),  # tgroup
-                                    (83, 1, 1),  # compfg
-                                    (84, 1, 1),  # tsform
-                                    (85, 1, 1),  # vbtime
-                                    (17, 1, int(tcode)),  # tcode
-                                    (33, 1, int(tsstep)),  # tsstep
-                                    (27, 1, int(base_year)),  # tsbyr
-                                    ]:
-            retcode = self.wdbsai(
-                wdmfp,
-                dsn,
-                messfp,
-                saind,
-                salen,
-                saval)
-            self._retcode_check(retcode, additional_info='wdbsai')
-
-        for saind, salen, saval in [(32, 1, tsfill)]:  # tsfill
-            retcode = self.wdbsar(
+            # Parameters for wdlbax taken from ATCTSfile/clsTSerWDM.cls
+            self.wdlbax(
                 wdmfp,
                 dsn,
-                messfp,
-                saind,
-                salen,
-                saval)
-            self._retcode_check(retcode, additional_info='wdbsar')
-
-        for saind, salen, saval, error_name in [
-                (2, 16, statid, 'Station ID'),
-                (1, 4, tstype.upper(), 'Time series type - tstype'),
-                (45, 48, description.upper(), 'Description'),
-                (288, 8, scenario.upper(), 'Scenario'),
-                (289, 8, constituent.upper(), 'Constituent'),
-                (290, 8, location.upper(), 'Location'),
-        ]:
-            saval = saval.strip()
-            if len(saval) > salen:
-                raise ValueError("""
+                1,     # DSTYPE - always 1 for time series
+                10,    # NDN    - number of down pointers
+                10,    # NUP    - number of up pointers
+                30,    # NSA    - number of search attributes
+                100,   # NSASP  - amount of search attribute space
+                300,   # NDP    - number of data pointers
+            )      # PSA    - pointer to search attribute space
+
+            for saind, salen, saval in [(34, 1, 6),  # tgroup
+                                        (83, 1, 1),  # compfg
+                                        (84, 1, 1),  # tsform
+                                        (85, 1, 1),  # vbtime
+                                        (17, 1, int(tcode)),  # tcode
+                                        (33, 1, int(tsstep)),  # tsstep
+                                        (27, 1, int(base_year)),  # tsbyr
+                                        ]:
+                retcode = self.wdbsai(
+                    wdmfp,
+                    dsn,
+                    messfp,
+                    saind,
+                    salen,
+                    saval)
+                self._retcode_check(retcode, additional_info='wdbsai')
+
+            for saind, salen, saval in [(32, 1, tsfill)]:  # tsfill
+                retcode = self.wdbsar(
+                    wdmfp,
+                    dsn,
+                    messfp,
+                    saind,
+                    salen,
+                    saval)
+                self._retcode_check(retcode, additional_info='wdbsar')
+
+            for saind, salen, saval, error_name in [
+                    (2, 16, statid, 'Station ID'),
+                    (1, 4, tstype.upper(), 'Time series type - tstype'),
+                    (45, 48, description.upper(), 'Description'),
+                    (288, 8, scenario.upper(), 'Scenario'),
+                    (289, 8, constituent.upper(), 'Constituent'),
+                    (290, 8, location.upper(), 'Location'),
+            ]:
+                saval = saval.strip()
+                if len(saval) > salen:
+                    raise ValueError("""
 *
 *   String "{0}" is too long for {1}.  Must
 *   have a length equal or less than {2}.
 *
 """.format(saval, error_name, salen))
 
-            saval = '{0: <{1}}'.format(saval, salen)
+                saval = '{0: <{1}}'.format(saval, salen)
 
-            retcode = self.wdbsac(
-                wdmfp,
-                dsn,
-                messfp,
-                saind,
-                salen,
-                saval)
-            self._retcode_check(retcode, additional_info='wdbsac')
-        lock.release()
-        self._close(wdmpath)
+                retcode = self.wdbsac(
+                    wdmfp,
+                    dsn,
+                    messfp,
+                    saind,
+                    salen,
+                    saval)
+                self._retcode_check(retcode, additional_info='wdbsac')
+            self._close(wdmpath)
 
     def _tcode_date(self, tcode, date):
         """Use tcode to set the significant parts of the date tuple."""
         rdate = [1, 1, 1, 0, 0, 0]
         if tcode <= 6:
             rdate[0] = date[0]
         if tcode <= 5:
@@ -626,29 +619,28 @@
 *
 *   The base year for this DSN is {0}.  All data to insert must be after the
 *   base year.  Instead the first year of the series is {1}.
 *
 """.format(dsn_desc['base_year'], llsdat[0]))
 
         nval = len(data)
-        lock = LockFile(wdmpath)
-        lock.acquire()
-        wdmfp = self._open(wdmpath, 58)
-        retcode = self.wdtput(
-            wdmfp,
-            dsn,
-            tstep,
-            llsdat,
-            nval,
-            1,
-            0,
-            tcode,
-            data)
-        lock.release()
-        self._close(wdmpath)
+        lock = SoftFileLock(wdmpath + '.lock', timeout=30)
+        with lock:
+            wdmfp = self._open(wdmpath, 58)
+            retcode = self.wdtput(
+                wdmfp,
+                dsn,
+                tstep,
+                llsdat,
+                nval,
+                1,
+                0,
+                tcode,
+                data)
+            self._close(wdmpath)
         self._retcode_check(retcode, additional_info='wdtput')
 
     def read_dsn(self, wdmpath, dsn, start_date=None, end_date=None):
         """Read from a DSN."""
         if not os.path.exists(wdmpath):
             raise ValueError("""
 ***
```

### Comparing `wdmtoolbox-7.9.7.5/wdmtoolbox/wdmtoolbox.py` & `wdmtoolbox-8.9.7.5/wdmtoolbox/wdmtoolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python
 """The component functions of the wdmtoolbox.
 
 Used to manipulate Watershed Data Management files for time-series.
 """
 from __future__ import print_function
 
-# Python batteries included imports
-from builtins import str
-from builtins import range
+from collections import OrderedDict
+import datetime
 import os
 import sys
-import datetime
-from collections import OrderedDict
 
 # Third party imports
+from builtins import range
+from builtins import str
+from dateutil.parser import parse as dateparser
 import mando
 from mando.rst_text_formatter import RSTHelpFormatter
-from dateutil.parser import parse as dateparser
 
 # Local imports
 # Load in WDM subroutines
 from tstoolbox import tsutils
 from . import wdmutil
 
 WDM = wdmutil.WDM()
@@ -28,15 +27,15 @@
 
 def _describedsn(wdmpath, dsn):
     """Private function used by routines that need a description of DSN."""
     return WDM.describe_dsn(wdmpath, int(dsn))
 
 
 def _copy_dsn(inwdmpath, indsn, outwdmpath, outdsn):
-    """The local underlying function to copy a DSN."""
+    """Copy a DSN."""
     WDM.copydsnlabel(inwdmpath, indsn, outwdmpath, outdsn)
     nts = WDM.read_dsn(inwdmpath, indsn)
     WDM.write_dsn(outwdmpath, int(outdsn), nts)
 
 
 @mando.command(formatter_class=RSTHelpFormatter, doctype='numpy')
 @tsutils.doc(tsutils.docstrings)
@@ -275,15 +274,15 @@
                            start_date=start_date,
                            end_date=end_date)
         if index == 0:
             result = nts
         else:
             try:
                 result = result.join(nts, how='outer')
-            except:
+            except ValueError:
                 raise ValueError("""
 *
 *   The column {0} is duplicated.  Dataset names must be unique.
 *
 """.format(nts.columns[0]))
     return tsutils.printiso(result)
 
@@ -518,15 +517,15 @@
 def stdtowdm(wdmpath, dsn, infile='-'):
     """DEPRECATED: Use 'csvtowdm'."""
     csvtowdm(wdmpath, dsn, input_ts=infile)
 
 
 @mando.command(formatter_class=RSTHelpFormatter, doctype='numpy')
 @tsutils.doc(tsutils.docstrings)
-def csvtowdm(wdmpath, dsn, input=None, start_date=None,
+def csvtowdm(wdmpath, dsn, start_date=None,
              end_date=None, columns=None, input_ts='-'):
     """Write data from a CSV file to a DSN.
 
     File can have comma separated
     'year', 'month', 'day', 'hour', 'minute', 'second', 'value'
     OR
     'date/time string', 'value'
@@ -535,29 +534,20 @@
     ----------
     wdmpath
         Path and WDM
         filename.
     dsn
         The Data Set Number in the WDM
         file.
-    input
-        DEPRECATED - use input_ts instead.
     {input_ts}
     {start_date}
     {end_date}
     {columns}
 
     """
-    if input is not None:
-        raise ValueError("""
-*
-*   The '--input' option has been deprecated.  Please use '--input_ts'
-*   instead.
-*
-""")
     tsd = tsutils.common_kwds(tsutils.read_iso_ts(input_ts),
                               start_date=start_date,
                               end_date=end_date,
                               pick=columns)
 
     if len(tsd.columns) > 1:
         raise ValueError("""
@@ -590,15 +580,15 @@
         'D':     4,  # day
         'H':     3,  # hour
         'T':     2,  # minute
         'S':     1   # second
     }
     try:
         finterval = mapcode[pandacode]
-    except:
+    except KeyError:
         raise KeyError("""
 *
 *   wdmtoolbox only understands PANDAS time intervals of :
 *   'A', 'AS', 'A-DEC' for annual,
 *   'M', 'MS' for monthly,
 *   'D', 'H', 'T', 'S' for day, hour, minute, and second.
 *   wdmtoolbox thinks this series is {0}.
@@ -627,15 +617,15 @@
 *
 """.format(dsntstep, tstep))
 
     WDM.write_dsn(wdmpath, dsn, data)
 
 
 def main():
-    """Main function."""
+    """Run the main function."""
     if not os.path.exists('debug_wdmtoolbox'):
         sys.tracebacklimit = 0
     mando.main()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `wdmtoolbox-7.9.7.5/wdmtoolbox/message.wdm` & `wdmtoolbox-8.9.7.5/wdmtoolbox/message.wdm`

 * *Files identical despite different names*

