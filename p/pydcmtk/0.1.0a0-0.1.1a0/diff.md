# Comparing `tmp/pydcmtk-0.1.0a0.tar.gz` & `tmp/pydcmtk-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydcmtk-0.1.0a0.tar", last modified: Fri May  5 12:56:04 2023, max compression
+gzip compressed data, was "pydcmtk-0.1.1a0.tar", last modified: Mon May  8 19:05:21 2023, max compression
```

## Comparing `pydcmtk-0.1.0a0.tar` & `pydcmtk-0.1.1a0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-05-05 12:56:04.240836 pydcmtk-0.1.0a0/
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     1071 2023-05-04 17:30:52.000000 pydcmtk-0.1.0a0/LICENSE
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     1505 2023-05-05 12:56:04.240836 pydcmtk-0.1.0a0/PKG-INFO
--rw-rw-r--   0 zeus      (1000) zeus      (1000)       43 2023-05-04 17:30:52.000000 pydcmtk-0.1.0a0/README.md
--rw-rw-r--   0 zeus      (1000) zeus      (1000)      265 2023-05-04 17:48:24.000000 pydcmtk-0.1.0a0/pyproject.toml
--rw-rw-r--   0 zeus      (1000) zeus      (1000)       38 2023-05-05 12:56:04.240836 pydcmtk-0.1.0a0/setup.cfg
-drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-05-05 12:56:04.228836 pydcmtk-0.1.0a0/src/
-drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-05-05 12:56:04.240836 pydcmtk-0.1.0a0/src/pydcmtk/
--rw-rw-r--   0 zeus      (1000) zeus      (1000)       89 2023-05-04 23:08:01.000000 pydcmtk-0.1.0a0/src/pydcmtk/__init__.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:09.000000 pydcmtk-0.1.0a0/src/pydcmtk/cda2dcm.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)      330 2023-05-04 18:35:13.000000 pydcmtk-0.1.0a0/src/pydcmtk/core.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:02:05.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcm2json.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:55.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcm2pdf.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:48.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcm2pnm.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:41.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcm2xml.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:32.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmcjpeg.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:27.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmcjpls.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:20.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmconv.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:15.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmcrle.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     9091 2023-05-04 23:07:23.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmdjpeg.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:02:05.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmdjpls.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:55.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmdrle.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:48.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmdspfn.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:41.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmdump.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:32.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmftest.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:27.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmgpdir.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:20.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmicmp.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:15.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmj2pnm.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:09.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcml2pnm.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:02:05.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmmkcrv.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:55.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmmkdir.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:48.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmmklut.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:41.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmodify.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:32.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmp2pgm.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:27.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmprscp.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:20.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmprscu.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:15.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmpschk.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:09.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmpsmk.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:02:05.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmpsprt.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:55.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmpsrcv.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:48.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmpssnd.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:41.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmqridx.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:32.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmqrscp.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:27.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmqrti.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:20.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmquant.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:15.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmrecv.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:09.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmscale.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:02:05.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmsend.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:55.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcmsign.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:48.000000 pydcmtk-0.1.0a0/src/pydcmtk/dcod2lum.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:41.000000 pydcmtk-0.1.0a0/src/pydcmtk/dconvlum.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:32.000000 pydcmtk-0.1.0a0/src/pydcmtk/drtdump.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:27.000000 pydcmtk-0.1.0a0/src/pydcmtk/dsr2html.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:20.000000 pydcmtk-0.1.0a0/src/pydcmtk/dsr2xml.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:15.000000 pydcmtk-0.1.0a0/src/pydcmtk/dsrdump.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:09.000000 pydcmtk-0.1.0a0/src/pydcmtk/dump2dcm.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:02:05.000000 pydcmtk-0.1.0a0/src/pydcmtk/echoscu.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:55.000000 pydcmtk-0.1.0a0/src/pydcmtk/findscu.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:48.000000 pydcmtk-0.1.0a0/src/pydcmtk/getscu.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     4961 2023-05-04 23:06:28.000000 pydcmtk-0.1.0a0/src/pydcmtk/img2dcm.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:27.000000 pydcmtk-0.1.0a0/src/pydcmtk/mkreport.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:20.000000 pydcmtk-0.1.0a0/src/pydcmtk/movescu.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:15.000000 pydcmtk-0.1.0a0/src/pydcmtk/msgserv.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     4106 2023-05-04 21:23:19.000000 pydcmtk-0.1.0a0/src/pydcmtk/pdf2dcm.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:02:05.000000 pydcmtk-0.1.0a0/src/pydcmtk/stl2dcm.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:55.000000 pydcmtk-0.1.0a0/src/pydcmtk/storescp.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:48.000000 pydcmtk-0.1.0a0/src/pydcmtk/storescu.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:41.000000 pydcmtk-0.1.0a0/src/pydcmtk/termscu.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:27.000000 pydcmtk-0.1.0a0/src/pydcmtk/wlmscpfs.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:20.000000 pydcmtk-0.1.0a0/src/pydcmtk/xml2dcm.py
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:15.000000 pydcmtk-0.1.0a0/src/pydcmtk/xml2dsr.py
-drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-05-05 12:56:04.240836 pydcmtk-0.1.0a0/src/pydcmtk.egg-info/
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     1505 2023-05-05 12:56:04.000000 pydcmtk-0.1.0a0/src/pydcmtk.egg-info/PKG-INFO
--rw-rw-r--   0 zeus      (1000) zeus      (1000)     1651 2023-05-05 12:56:04.000000 pydcmtk-0.1.0a0/src/pydcmtk.egg-info/SOURCES.txt
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        1 2023-05-05 12:56:04.000000 pydcmtk-0.1.0a0/src/pydcmtk.egg-info/dependency_links.txt
--rw-rw-r--   0 zeus      (1000) zeus      (1000)        8 2023-05-05 12:56:04.000000 pydcmtk-0.1.0a0/src/pydcmtk.egg-info/top_level.txt
+drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-05-08 19:05:21.510841 pydcmtk-0.1.1a0/
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     1071 2023-05-04 17:30:52.000000 pydcmtk-0.1.1a0/LICENSE
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     1505 2023-05-08 19:05:21.510841 pydcmtk-0.1.1a0/PKG-INFO
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)       43 2023-05-04 17:30:52.000000 pydcmtk-0.1.1a0/README.md
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)      265 2023-05-08 19:04:25.000000 pydcmtk-0.1.1a0/pyproject.toml
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)       38 2023-05-08 19:05:21.510841 pydcmtk-0.1.1a0/setup.cfg
+drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-05-08 19:05:21.494840 pydcmtk-0.1.1a0/src/
+drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-05-08 19:05:21.506841 pydcmtk-0.1.1a0/src/pydcmtk/
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)       89 2023-05-04 23:08:01.000000 pydcmtk-0.1.1a0/src/pydcmtk/__init__.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:09.000000 pydcmtk-0.1.1a0/src/pydcmtk/cda2dcm.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)      330 2023-05-04 18:35:13.000000 pydcmtk-0.1.1a0/src/pydcmtk/core.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:02:05.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcm2json.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:55.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcm2pdf.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:48.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcm2pnm.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:41.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcm2xml.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:32.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmcjpeg.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:27.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmcjpls.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:20.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmconv.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:15.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmcrle.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     9092 2023-05-08 19:01:10.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmdjpeg.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:02:05.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmdjpls.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:55.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmdrle.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:48.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmdspfn.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:41.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmdump.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:32.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmftest.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:27.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmgpdir.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:20.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmicmp.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:15.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmj2pnm.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:09.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcml2pnm.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:02:05.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmmkcrv.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:55.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmmkdir.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:48.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmmklut.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:41.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmodify.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:32.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmp2pgm.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:27.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmprscp.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:20.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmprscu.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:15.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmpschk.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:09.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmpsmk.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:02:05.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmpsprt.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:55.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmpsrcv.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:48.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmpssnd.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:41.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmqridx.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:32.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmqrscp.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:27.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmqrti.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:20.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmquant.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:15.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmrecv.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:09.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmscale.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:02:05.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmsend.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:55.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcmsign.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:48.000000 pydcmtk-0.1.1a0/src/pydcmtk/dcod2lum.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:41.000000 pydcmtk-0.1.1a0/src/pydcmtk/dconvlum.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:32.000000 pydcmtk-0.1.1a0/src/pydcmtk/drtdump.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:27.000000 pydcmtk-0.1.1a0/src/pydcmtk/dsr2html.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:20.000000 pydcmtk-0.1.1a0/src/pydcmtk/dsr2xml.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:15.000000 pydcmtk-0.1.1a0/src/pydcmtk/dsrdump.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:09.000000 pydcmtk-0.1.1a0/src/pydcmtk/dump2dcm.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:02:05.000000 pydcmtk-0.1.1a0/src/pydcmtk/echoscu.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:55.000000 pydcmtk-0.1.1a0/src/pydcmtk/findscu.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:48.000000 pydcmtk-0.1.1a0/src/pydcmtk/getscu.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     4961 2023-05-04 23:06:28.000000 pydcmtk-0.1.1a0/src/pydcmtk/img2dcm.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:27.000000 pydcmtk-0.1.1a0/src/pydcmtk/mkreport.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:20.000000 pydcmtk-0.1.1a0/src/pydcmtk/movescu.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:15.000000 pydcmtk-0.1.1a0/src/pydcmtk/msgserv.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     4106 2023-05-04 21:23:19.000000 pydcmtk-0.1.1a0/src/pydcmtk/pdf2dcm.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:02:05.000000 pydcmtk-0.1.1a0/src/pydcmtk/stl2dcm.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:55.000000 pydcmtk-0.1.1a0/src/pydcmtk/storescp.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:48.000000 pydcmtk-0.1.1a0/src/pydcmtk/storescu.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:41.000000 pydcmtk-0.1.1a0/src/pydcmtk/termscu.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:27.000000 pydcmtk-0.1.1a0/src/pydcmtk/wlmscpfs.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:20.000000 pydcmtk-0.1.1a0/src/pydcmtk/xml2dcm.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-05-04 18:01:15.000000 pydcmtk-0.1.1a0/src/pydcmtk/xml2dsr.py
+drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-05-08 19:05:21.506841 pydcmtk-0.1.1a0/src/pydcmtk.egg-info/
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     1505 2023-05-08 19:05:21.000000 pydcmtk-0.1.1a0/src/pydcmtk.egg-info/PKG-INFO
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     1651 2023-05-08 19:05:21.000000 pydcmtk-0.1.1a0/src/pydcmtk.egg-info/SOURCES.txt
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        1 2023-05-08 19:05:21.000000 pydcmtk-0.1.1a0/src/pydcmtk.egg-info/dependency_links.txt
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        8 2023-05-08 19:05:21.000000 pydcmtk-0.1.1a0/src/pydcmtk.egg-info/top_level.txt
```

### Comparing `pydcmtk-0.1.0a0/LICENSE` & `pydcmtk-0.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydcmtk-0.1.0a0/PKG-INFO` & `pydcmtk-0.1.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydcmtk
-Version: 0.1.0a0
+Version: 0.1.1a0
 Author-email: lcscosta <lcscosta@disroot.org>
 License: MIT License
         
         Copyright (c) 2023 Lucas da Costa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pydcmtk-0.1.0a0/src/pydcmtk/dcmdjpeg.py` & `pydcmtk-0.1.1a0/src/pydcmtk/dcmdjpeg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from .core import run_binary
 
 def dcmdjpeg(
         dcmfile_in: Path = Path(),
         dcmfile_out: Path = Path(),
         options: list = []
-    )
+    ):
     """
     SYNOPSIS
 
         dcmdjpeg [options] dcmfile-in dcmfile-out
 
     DESCRIPTION
```

### Comparing `pydcmtk-0.1.0a0/src/pydcmtk/img2dcm.py` & `pydcmtk-0.1.1a0/src/pydcmtk/img2dcm.py`

 * *Files identical despite different names*

### Comparing `pydcmtk-0.1.0a0/src/pydcmtk/pdf2dcm.py` & `pydcmtk-0.1.1a0/src/pydcmtk/pdf2dcm.py`

 * *Files identical despite different names*

### Comparing `pydcmtk-0.1.0a0/src/pydcmtk.egg-info/PKG-INFO` & `pydcmtk-0.1.1a0/src/pydcmtk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydcmtk
-Version: 0.1.0a0
+Version: 0.1.1a0
 Author-email: lcscosta <lcscosta@disroot.org>
 License: MIT License
         
         Copyright (c) 2023 Lucas da Costa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pydcmtk-0.1.0a0/src/pydcmtk.egg-info/SOURCES.txt` & `pydcmtk-0.1.1a0/src/pydcmtk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

