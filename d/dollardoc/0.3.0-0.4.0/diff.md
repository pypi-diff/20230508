# Comparing `tmp/dollardoc-0.3.0.tar.gz` & `tmp/dollardoc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dollardoc-0.3.0.tar", last modified: Sat Apr  1 08:47:30 2023, max compression
+gzip compressed data, was "dist\dollardoc-0.4.0.tar", last modified: Mon May  8 16:48:38 2023, max compression
```

## Comparing `dollardoc-0.3.0.tar` & `dollardoc-0.4.0.tar`

### file list

```diff
@@ -1,86 +1,89 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 08:47:30.275985 dollardoc-0.3.0/
--rw-rw-rw-   0        0        0    35149 2023-03-18 10:28:03.000000 dollardoc-0.3.0/LICENSE
--rw-rw-rw-   0        0        0       52 2023-03-18 06:57:05.000000 dollardoc-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7774 2023-04-01 08:47:30.275985 dollardoc-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4730 2023-04-01 08:38:35.000000 dollardoc-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-01 08:47:30.275985 dollardoc-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2395 2023-04-01 08:46:19.000000 dollardoc-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-01 08:47:30.201988 dollardoc-0.3.0/src/
--rw-rw-rw-   0        0        0        0 2023-03-07 04:44:41.000000 dollardoc-0.3.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 08:47:30.221986 dollardoc-0.3.0/src/dollar/
--rw-rw-rw-   0        0        0      263 2023-03-31 08:04:47.000000 dollardoc-0.3.0/src/dollar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 08:47:30.222985 dollardoc-0.3.0/src/dollar/builder/
--rw-rw-rw-   0        0        0       42 2023-03-17 11:00:23.000000 dollardoc-0.3.0/src/dollar/builder/__init__.py
--rw-rw-rw-   0        0        0     6562 2023-04-01 07:42:37.000000 dollardoc-0.3.0/src/dollar/builder/dollarbuilder.py
-drwxrwxrwx   0        0        0        0 2023-04-01 08:47:30.224985 dollardoc-0.3.0/src/dollar/cli/
--rw-rw-rw-   0        0        0       20 2023-03-19 05:23:32.000000 dollardoc-0.3.0/src/dollar/cli/__init__.py
--rw-rw-rw-   0        0        0      441 2023-03-19 09:23:01.000000 dollardoc-0.3.0/src/dollar/cli/cli.py
--rw-rw-rw-   0        0        0      620 2023-03-31 08:00:49.000000 dollardoc-0.3.0/src/dollar/confighandler.py
--rw-rw-rw-   0        0        0     1771 2023-03-31 08:00:49.000000 dollardoc-0.3.0/src/dollar/configmap.py
--rw-rw-rw-   0        0        0      229 2023-03-31 07:54:02.000000 dollardoc-0.3.0/src/dollar/configtype.py
--rw-rw-rw-   0        0        0     1338 2023-03-19 11:30:42.000000 dollardoc-0.3.0/src/dollar/dollarcontext.py
--rw-rw-rw-   0        0        0      641 2023-03-19 13:07:58.000000 dollardoc-0.3.0/src/dollar/dollarexception.py
--rw-rw-rw-   0        0        0     1246 2023-03-18 16:46:01.000000 dollardoc-0.3.0/src/dollar/dollarobject.py
--rw-rw-rw-   0        0        0     1136 2023-03-31 06:39:56.000000 dollardoc-0.3.0/src/dollar/dollarobjectidmap.py
--rw-rw-rw-   0        0        0     1927 2023-03-19 04:34:53.000000 dollardoc-0.3.0/src/dollar/dollarobjectimpl.py
-drwxrwxrwx   0        0        0        0 2023-04-01 08:47:30.229985 dollardoc-0.3.0/src/dollar/file/
--rw-rw-rw-   0        0        0      168 2023-03-18 14:33:50.000000 dollardoc-0.3.0/src/dollar/file/__init__.py
--rw-rw-rw-   0        0        0      839 2023-03-19 11:23:16.000000 dollardoc-0.3.0/src/dollar/file/dollarfile.py
--rw-rw-rw-   0        0        0     1735 2023-03-19 11:23:16.000000 dollardoc-0.3.0/src/dollar/file/dollarfilereader.py
--rw-rw-rw-   0        0        0      748 2023-03-19 11:23:16.000000 dollardoc-0.3.0/src/dollar/file/dollarfilewriter.py
--rw-rw-rw-   0        0        0      679 2023-03-18 18:43:08.000000 dollardoc-0.3.0/src/dollar/file/filecopier.py
-drwxrwxrwx   0        0        0        0 2023-04-01 08:47:30.230985 dollardoc-0.3.0/src/dollar/format/
--rw-rw-rw-   0        0        0        0 2023-03-18 10:44:16.000000 dollardoc-0.3.0/src/dollar/format/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 08:47:30.233987 dollardoc-0.3.0/src/dollar/format/header/
--rw-rw-rw-   0        0        0       92 2023-03-18 10:44:59.000000 dollardoc-0.3.0/src/dollar/format/header/__init__.py
--rw-rw-rw-   0        0        0     1456 2023-03-19 11:23:16.000000 dollardoc-0.3.0/src/dollar/format/header/headerparser.py
--rw-rw-rw-   0        0        0      299 2023-03-18 17:22:50.000000 dollardoc-0.3.0/src/dollar/format/header/headerparserresult.py
-drwxrwxrwx   0        0        0        0 2023-04-01 08:47:30.236986 dollardoc-0.3.0/src/dollar/format/input/
--rw-rw-rw-   0        0        0      363 2023-03-18 17:24:53.000000 dollardoc-0.3.0/src/dollar/format/input/__init__.py
--rw-rw-rw-   0        0        0     4504 2023-03-19 11:23:16.000000 dollardoc-0.3.0/src/dollar/format/input/inputformat.py
--rw-rw-rw-   0        0        0      171 2023-03-18 17:22:17.000000 dollardoc-0.3.0/src/dollar/format/input/inputformattype.py
-drwxrwxrwx   0        0        0        0 2023-04-01 08:47:30.242986 dollardoc-0.3.0/src/dollar/format/output/
--rw-rw-rw-   0        0        0     1010 2023-03-19 04:42:12.000000 dollardoc-0.3.0/src/dollar/format/output/__init__.py
--rw-rw-rw-   0        0        0     1399 2023-03-18 17:21:52.000000 dollardoc-0.3.0/src/dollar/format/output/outputfactory.py
--rw-rw-rw-   0        0        0     8285 2023-03-19 11:23:16.000000 dollardoc-0.3.0/src/dollar/format/output/outputformat.py
--rw-rw-rw-   0        0        0    10051 2023-03-19 11:23:16.000000 dollardoc-0.3.0/src/dollar/format/output/outputformatter.py
--rw-rw-rw-   0        0        0      231 2023-03-18 16:14:35.000000 dollardoc-0.3.0/src/dollar/format/output/outputformatterhandler.py
--rw-rw-rw-   0        0        0      416 2023-03-16 18:18:12.000000 dollardoc-0.3.0/src/dollar/format/output/outputformattype.py
-drwxrwxrwx   0        0        0        0 2023-04-01 08:47:30.246986 dollardoc-0.3.0/src/dollar/format/raw/
--rw-rw-rw-   0        0        0      407 2023-03-18 10:44:37.000000 dollardoc-0.3.0/src/dollar/format/raw/__init__.py
--rw-rw-rw-   0        0        0     3588 2023-03-19 11:23:16.000000 dollardoc-0.3.0/src/dollar/format/raw/rawdollarformat.py
--rw-rw-rw-   0        0        0      142 2023-03-16 18:18:12.000000 dollardoc-0.3.0/src/dollar/format/raw/rawdollarformattype.py
--rw-rw-rw-   0        0        0    10043 2023-04-01 07:29:19.000000 dollardoc-0.3.0/src/dollar/format/raw/rawdollarparser.py
-drwxrwxrwx   0        0        0        0 2023-04-01 08:47:30.250989 dollardoc-0.3.0/src/dollar/format/transformer/
--rw-rw-rw-   0        0        0      166 2023-03-18 10:44:22.000000 dollardoc-0.3.0/src/dollar/format/transformer/__init__.py
--rw-rw-rw-   0        0        0     4457 2023-03-31 05:19:03.000000 dollardoc-0.3.0/src/dollar/format/transformer/headertransformer.py
--rw-rw-rw-   0        0        0     4785 2023-03-31 06:38:10.000000 dollardoc-0.3.0/src/dollar/format/transformer/inputtostrtransformer.py
--rw-rw-rw-   0        0        0     9676 2023-03-31 10:39:24.000000 dollardoc-0.3.0/src/dollar/format/transformer/rawtoinputtransformer.py
-drwxrwxrwx   0        0        0        0 2023-04-01 08:47:30.253987 dollardoc-0.3.0/src/dollar/helper/
--rw-rw-rw-   0        0        0      100 2023-03-19 07:26:09.000000 dollardoc-0.3.0/src/dollar/helper/__init__.py
--rw-rw-rw-   0        0        0     1100 2023-03-31 05:55:32.000000 dollardoc-0.3.0/src/dollar/helper/dollarobjecthelper.py
--rw-rw-rw-   0        0        0      321 2023-03-18 16:17:25.000000 dollardoc-0.3.0/src/dollar/helper/validationhelper.py
-drwxrwxrwx   0        0        0        0 2023-04-01 08:47:30.261986 dollardoc-0.3.0/src/dollar/plugin/
--rw-rw-rw-   0        0        0      340 2023-03-31 08:04:40.000000 dollardoc-0.3.0/src/dollar/plugin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 08:47:30.268986 dollardoc-0.3.0/src/dollar/plugin/builtin/
--rw-rw-rw-   0        0        0      286 2023-03-18 10:43:51.000000 dollardoc-0.3.0/src/dollar/plugin/builtin/__init__.py
--rw-rw-rw-   0        0        0     1080 2023-03-31 05:41:02.000000 dollardoc-0.3.0/src/dollar/plugin/builtin/dollarbaseextensionplugin.py
--rw-rw-rw-   0        0        0     1064 2023-03-19 06:08:15.000000 dollardoc-0.3.0/src/dollar/plugin/builtin/linkfunctionplugin.py
--rw-rw-rw-   0        0        0     1105 2023-03-19 06:08:12.000000 dollardoc-0.3.0/src/dollar/plugin/builtin/listbacklinksfunctionplugin.py
--rw-rw-rw-   0        0        0     1367 2023-03-19 06:08:12.000000 dollardoc-0.3.0/src/dollar/plugin/builtin/listfunctionplugin.py
--rw-rw-rw-   0        0        0     1122 2023-03-19 06:08:02.000000 dollardoc-0.3.0/src/dollar/plugin/builtin/listreffunctionplugin.py
--rw-rw-rw-   0        0        0     1110 2023-03-30 17:59:33.000000 dollardoc-0.3.0/src/dollar/plugin/builtin/pageextensionplugin.py
--rw-rw-rw-   0        0        0     1068 2023-03-31 08:06:23.000000 dollardoc-0.3.0/src/dollar/plugin/builtinpluginloader.py
--rw-rw-rw-   0        0        0     1560 2023-03-31 08:05:30.000000 dollardoc-0.3.0/src/dollar/plugin/dollarplugin.py
--rw-rw-rw-   0        0        0      793 2023-03-19 05:56:34.000000 dollardoc-0.3.0/src/dollar/plugin/pluginarg.py
--rw-rw-rw-   0        0        0     1684 2023-03-31 06:36:52.000000 dollardoc-0.3.0/src/dollar/plugin/pluginargvalidatior.py
--rw-rw-rw-   0        0        0     1549 2023-03-31 10:47:34.000000 dollardoc-0.3.0/src/dollar/plugin/pluginhandler.py
--rw-rw-rw-   0        0        0     3526 2023-04-01 07:36:23.000000 dollardoc-0.3.0/src/dollar/plugin/pluginmap.py
--rw-rw-rw-   0        0        0      104 2023-03-17 07:56:10.000000 dollardoc-0.3.0/src/dollar/plugin/plugintype.py
-drwxrwxrwx   0        0        0        0 2023-04-01 08:47:30.274985 dollardoc-0.3.0/src/dollardoc.egg-info/
--rw-rw-rw-   0        0        0     7774 2023-04-01 08:47:30.000000 dollardoc-0.3.0/src/dollardoc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2428 2023-04-01 08:47:30.000000 dollardoc-0.3.0/src/dollardoc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-01 08:47:30.000000 dollardoc-0.3.0/src/dollardoc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-01 08:47:30.000000 dollardoc-0.3.0/src/dollardoc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-01 08:47:30.000000 dollardoc-0.3.0/src/dollardoc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-01 08:47:30.000000 dollardoc-0.3.0/src/dollardoc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 16:48:38.704465 dollardoc-0.4.0/
+-rw-rw-rw-   0        0        0    35149 2023-03-18 10:28:03.000000 dollardoc-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0       52 2023-03-18 06:57:05.000000 dollardoc-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7893 2023-05-08 16:48:38.704465 dollardoc-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4849 2023-04-01 12:41:26.000000 dollardoc-0.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 16:48:38.704465 dollardoc-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2395 2023-05-08 16:44:46.000000 dollardoc-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:48:38.634465 dollardoc-0.4.0/src/
+-rw-rw-rw-   0        0        0        0 2023-03-07 04:44:41.000000 dollardoc-0.4.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:48:38.643788 dollardoc-0.4.0/src/dollar/
+-rw-rw-rw-   0        0        0      317 2023-04-22 03:03:06.000000 dollardoc-0.4.0/src/dollar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:48:38.646788 dollardoc-0.4.0/src/dollar/builder/
+-rw-rw-rw-   0        0        0       92 2023-04-13 04:44:41.000000 dollardoc-0.4.0/src/dollar/builder/__init__.py
+-rw-rw-rw-   0        0        0     4101 2023-05-08 15:26:17.000000 dollardoc-0.4.0/src/dollar/builder/dollarbuilder.py
+-rw-rw-rw-   0        0        0     5189 2023-05-08 15:28:55.000000 dollardoc-0.4.0/src/dollar/builder/dollarlivebuilder.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:48:38.648790 dollardoc-0.4.0/src/dollar/cli/
+-rw-rw-rw-   0        0        0       20 2023-03-19 05:23:32.000000 dollardoc-0.4.0/src/dollar/cli/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-03-19 09:23:01.000000 dollardoc-0.4.0/src/dollar/cli/cli.py
+-rw-rw-rw-   0        0        0      649 2023-04-19 03:17:19.000000 dollardoc-0.4.0/src/dollar/confighandler.py
+-rw-rw-rw-   0        0        0     1771 2023-03-31 08:00:49.000000 dollardoc-0.4.0/src/dollar/configmap.py
+-rw-rw-rw-   0        0        0      229 2023-03-31 07:54:02.000000 dollardoc-0.4.0/src/dollar/configtype.py
+-rw-rw-rw-   0        0        0     1338 2023-03-19 11:30:42.000000 dollardoc-0.4.0/src/dollar/dollarcontext.py
+-rw-rw-rw-   0        0        0      641 2023-03-19 13:07:58.000000 dollardoc-0.4.0/src/dollar/dollarexception.py
+-rw-rw-rw-   0        0        0     1472 2023-04-12 17:47:09.000000 dollardoc-0.4.0/src/dollar/dollarobject.py
+-rw-rw-rw-   0        0        0     2916 2023-04-22 03:52:58.000000 dollardoc-0.4.0/src/dollar/dollarobjectidmap.py
+-rw-rw-rw-   0        0        0     2802 2023-04-22 03:28:22.000000 dollardoc-0.4.0/src/dollar/dollarobjectimpl.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:48:38.653790 dollardoc-0.4.0/src/dollar/file/
+-rw-rw-rw-   0        0        0      168 2023-03-18 14:33:50.000000 dollardoc-0.4.0/src/dollar/file/__init__.py
+-rw-rw-rw-   0        0        0     1569 2023-04-10 13:25:46.000000 dollardoc-0.4.0/src/dollar/file/dollarfile.py
+-rw-rw-rw-   0        0        0     1710 2023-04-10 12:46:05.000000 dollardoc-0.4.0/src/dollar/file/dollarfilereader.py
+-rw-rw-rw-   0        0        0      890 2023-04-22 03:05:02.000000 dollardoc-0.4.0/src/dollar/file/dollarfilewriter.py
+-rw-rw-rw-   0        0        0      679 2023-03-18 18:43:08.000000 dollardoc-0.4.0/src/dollar/file/filecopier.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:48:38.655789 dollardoc-0.4.0/src/dollar/format/
+-rw-rw-rw-   0        0        0        0 2023-03-18 10:44:16.000000 dollardoc-0.4.0/src/dollar/format/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:48:38.657788 dollardoc-0.4.0/src/dollar/format/header/
+-rw-rw-rw-   0        0        0       92 2023-03-18 10:44:59.000000 dollardoc-0.4.0/src/dollar/format/header/__init__.py
+-rw-rw-rw-   0        0        0     1456 2023-03-19 11:23:16.000000 dollardoc-0.4.0/src/dollar/format/header/headerparser.py
+-rw-rw-rw-   0        0        0      299 2023-03-18 17:22:50.000000 dollardoc-0.4.0/src/dollar/format/header/headerparserresult.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:48:38.660787 dollardoc-0.4.0/src/dollar/format/input/
+-rw-rw-rw-   0        0        0      363 2023-03-18 17:24:53.000000 dollardoc-0.4.0/src/dollar/format/input/__init__.py
+-rw-rw-rw-   0        0        0     4504 2023-03-19 11:23:16.000000 dollardoc-0.4.0/src/dollar/format/input/inputformat.py
+-rw-rw-rw-   0        0        0      171 2023-03-18 17:22:17.000000 dollardoc-0.4.0/src/dollar/format/input/inputformattype.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:48:38.669208 dollardoc-0.4.0/src/dollar/format/output/
+-rw-rw-rw-   0        0        0     1090 2023-04-23 07:51:16.000000 dollardoc-0.4.0/src/dollar/format/output/__init__.py
+-rw-rw-rw-   0        0        0     1530 2023-04-23 08:04:07.000000 dollardoc-0.4.0/src/dollar/format/output/outputfactory.py
+-rw-rw-rw-   0        0        0     8285 2023-03-19 11:23:16.000000 dollardoc-0.4.0/src/dollar/format/output/outputformat.py
+-rw-rw-rw-   0        0        0      120 2023-04-23 07:50:57.000000 dollardoc-0.4.0/src/dollar/format/output/outputformatdollarobjectlinktype.py
+-rw-rw-rw-   0        0        0    10915 2023-04-23 08:04:50.000000 dollardoc-0.4.0/src/dollar/format/output/outputformatter.py
+-rw-rw-rw-   0        0        0      437 2023-04-23 07:58:15.000000 dollardoc-0.4.0/src/dollar/format/output/outputformatterhandler.py
+-rw-rw-rw-   0        0        0      416 2023-03-16 18:18:12.000000 dollardoc-0.4.0/src/dollar/format/output/outputformattype.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:48:38.672208 dollardoc-0.4.0/src/dollar/format/raw/
+-rw-rw-rw-   0        0        0      407 2023-03-18 10:44:37.000000 dollardoc-0.4.0/src/dollar/format/raw/__init__.py
+-rw-rw-rw-   0        0        0     3588 2023-03-19 11:23:16.000000 dollardoc-0.4.0/src/dollar/format/raw/rawdollarformat.py
+-rw-rw-rw-   0        0        0      142 2023-03-16 18:18:12.000000 dollardoc-0.4.0/src/dollar/format/raw/rawdollarformattype.py
+-rw-rw-rw-   0        0        0    10074 2023-05-08 16:21:16.000000 dollardoc-0.4.0/src/dollar/format/raw/rawdollarparser.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:48:38.677204 dollardoc-0.4.0/src/dollar/format/transformer/
+-rw-rw-rw-   0        0        0      166 2023-03-18 10:44:22.000000 dollardoc-0.4.0/src/dollar/format/transformer/__init__.py
+-rw-rw-rw-   0        0        0     4457 2023-03-31 05:19:03.000000 dollardoc-0.4.0/src/dollar/format/transformer/headertransformer.py
+-rw-rw-rw-   0        0        0     5153 2023-04-23 08:07:02.000000 dollardoc-0.4.0/src/dollar/format/transformer/inputtostrtransformer.py
+-rw-rw-rw-   0        0        0     9676 2023-03-31 10:39:24.000000 dollardoc-0.4.0/src/dollar/format/transformer/rawtoinputtransformer.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:48:38.681202 dollardoc-0.4.0/src/dollar/helper/
+-rw-rw-rw-   0        0        0      100 2023-03-19 07:26:09.000000 dollardoc-0.4.0/src/dollar/helper/__init__.py
+-rw-rw-rw-   0        0        0     3976 2023-05-08 15:26:02.000000 dollardoc-0.4.0/src/dollar/helper/dollarobjectcreationhelper.py
+-rw-rw-rw-   0        0        0     1100 2023-03-31 05:55:32.000000 dollardoc-0.4.0/src/dollar/helper/dollarobjecthelper.py
+-rw-rw-rw-   0        0        0      321 2023-03-18 16:17:25.000000 dollardoc-0.4.0/src/dollar/helper/validationhelper.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:48:38.689208 dollardoc-0.4.0/src/dollar/plugin/
+-rw-rw-rw-   0        0        0      340 2023-03-31 08:04:40.000000 dollardoc-0.4.0/src/dollar/plugin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:48:38.697208 dollardoc-0.4.0/src/dollar/plugin/builtin/
+-rw-rw-rw-   0        0        0      286 2023-03-18 10:43:51.000000 dollardoc-0.4.0/src/dollar/plugin/builtin/__init__.py
+-rw-rw-rw-   0        0        0     1080 2023-03-31 05:41:02.000000 dollardoc-0.4.0/src/dollar/plugin/builtin/dollarbaseextensionplugin.py
+-rw-rw-rw-   0        0        0     1064 2023-03-19 06:08:15.000000 dollardoc-0.4.0/src/dollar/plugin/builtin/linkfunctionplugin.py
+-rw-rw-rw-   0        0        0     1105 2023-03-19 06:08:12.000000 dollardoc-0.4.0/src/dollar/plugin/builtin/listbacklinksfunctionplugin.py
+-rw-rw-rw-   0        0        0     1367 2023-03-19 06:08:12.000000 dollardoc-0.4.0/src/dollar/plugin/builtin/listfunctionplugin.py
+-rw-rw-rw-   0        0        0     1122 2023-03-19 06:08:02.000000 dollardoc-0.4.0/src/dollar/plugin/builtin/listreffunctionplugin.py
+-rw-rw-rw-   0        0        0     1110 2023-03-30 17:59:33.000000 dollardoc-0.4.0/src/dollar/plugin/builtin/pageextensionplugin.py
+-rw-rw-rw-   0        0        0     1033 2023-05-08 16:04:41.000000 dollardoc-0.4.0/src/dollar/plugin/builtinpluginloader.py
+-rw-rw-rw-   0        0        0     1560 2023-03-31 08:05:30.000000 dollardoc-0.4.0/src/dollar/plugin/dollarplugin.py
+-rw-rw-rw-   0        0        0      793 2023-03-19 05:56:34.000000 dollardoc-0.4.0/src/dollar/plugin/pluginarg.py
+-rw-rw-rw-   0        0        0     1684 2023-03-31 06:36:52.000000 dollardoc-0.4.0/src/dollar/plugin/pluginargvalidatior.py
+-rw-rw-rw-   0        0        0     1641 2023-05-08 16:18:04.000000 dollardoc-0.4.0/src/dollar/plugin/pluginhandler.py
+-rw-rw-rw-   0        0        0     3585 2023-05-08 16:40:25.000000 dollardoc-0.4.0/src/dollar/plugin/pluginmap.py
+-rw-rw-rw-   0        0        0      104 2023-03-17 07:56:10.000000 dollardoc-0.4.0/src/dollar/plugin/plugintype.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:48:38.703208 dollardoc-0.4.0/src/dollardoc.egg-info/
+-rw-rw-rw-   0        0        0     7893 2023-05-08 16:48:38.000000 dollardoc-0.4.0/src/dollardoc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2577 2023-05-08 16:48:38.000000 dollardoc-0.4.0/src/dollardoc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 16:48:38.000000 dollardoc-0.4.0/src/dollardoc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-08 16:48:38.000000 dollardoc-0.4.0/src/dollardoc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-05-08 16:48:38.000000 dollardoc-0.4.0/src/dollardoc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-08 16:48:38.000000 dollardoc-0.4.0/src/dollardoc.egg-info/top_level.txt
```

### Comparing `dollardoc-0.3.0/LICENSE` & `dollardoc-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/PKG-INFO` & `dollardoc-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dollardoc
-Version: 0.3.0
+Version: 0.4.0
 Summary: Object oriented markdown documentation
 Home-page: https://github.com/dollardoc/dollardoc
 Author: dollardoc
 Author-email: development@dollardoc.dev
 License: UNKNOWN
 Description: # DollarDoc
         
@@ -148,15 +148,15 @@
         $ python build.py
         ```
         
         Unless there is an exception, all your generated markdown files will show up in the `output/` folder.
         
         ## Dollar Syntax Specification Document
         
-        *Specification currently under development*
+        [dollar-syntax-specification-v0_1_0.pdf](https://github.com/dollardoc/dollar-syntax-specification/releases/download/v0.1.0/dollar-syntax-specification-v0_1_0.pdf)
         
         ## Outputs Supported
         
         This project only supports plain markdown files. Other alternatives has been considered, like docusaurus style markdown output, but nothing has been decided at this moment.
         
         ## Future of the Project
```

### Comparing `dollardoc-0.3.0/README.md` & `dollardoc-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 $ python build.py
 ```
 
 Unless there is an exception, all your generated markdown files will show up in the `output/` folder.
 
 ## Dollar Syntax Specification Document
 
-*Specification currently under development*
+[dollar-syntax-specification-v0_1_0.pdf](https://github.com/dollardoc/dollar-syntax-specification/releases/download/v0.1.0/dollar-syntax-specification-v0_1_0.pdf)
 
 ## Outputs Supported
 
 This project only supports plain markdown files. Other alternatives has been considered, like docusaurus style markdown output, but nothing has been decided at this moment.
 
 ## Future of the Project
```

### Comparing `dollardoc-0.3.0/setup.py` & `dollardoc-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="dollardoc",
-    version="0.3.0",
+    version="0.4.0",
     description="Object oriented markdown documentation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="dollardoc",
     author_email="development@dollardoc.dev",
     url="https://github.com/dollardoc/dollardoc",
     packages=[
```

### Comparing `dollardoc-0.3.0/src/dollar/builder/dollarbuilder.py` & `dollardoc-0.4.0/src/dollar/helper/dollarobjectcreationhelper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,145 +1,91 @@
-from dollar.confighandler import ConfigHandler
-from dollar.confighandler import ConfigType
-from dollar.dollarcontext import DollarContext
-from dollar.dollarobjectidmap import DollarObjectIdMap
+from typing import Optional
+
 from dollar.dollarobjectimpl import DollarObjectImpl
+from dollar.dollarcontext import DollarContext
 from dollar.dollarexception import DollarExecutionException
 from dollar.dollarexception import DollarException
-from dollar.file.dollarfile import DollarFile
-from dollar.file.dollarfilereader import DollarFileReader
-from dollar.file.dollarfilewriter import DollarFileWriter
-from dollar.file.filecopier import FileCopier
 from dollar.format.header.headerparser import HeaderParser
-from dollar.format.raw.rawdollarparser import RawDollarParser
 from dollar.format.transformer.headertransformer import HeaderTransformer
-from dollar.format.transformer.inputtostrtransformer import InputToStrTransformer
-from dollar.format.transformer.rawtoinputtransformer import RawToInputTransformer
-from dollar.plugin.builtinpluginloader import BuiltinPluginLoader
-from dollar.plugin.pluginhandler import PluginHandler
-
+from dollar.dollarobjectidmap import DollarObjectIdMap
+from dollar.plugin.pluginmap import PluginMap
 
-class DollarBuilder:
 
+class DollarObjectCreationHelper:
     @staticmethod
-    def build():
-        config_map = ConfigHandler.load_config_default()
-        conf_docs_path = config_map.get(ConfigType.DOCS_PATH)
-        conf_target_path = config_map.get(ConfigType.TARGET_PATH)
-        conf_plugin_path = config_map.get(ConfigType.PLUGIN_PATH)
-        conf_file_passthrough = config_map.get_str_list_opt(ConfigType.FILE_PASSTHROUGH)
-        BuiltinPluginLoader.load(config_map)
-        plugin_map = PluginHandler.import_plugins(conf_plugin_path, config_map)
-
-        mdd_files = DollarFileReader.read_mdd_files(conf_docs_path)
-
-        dollar_object_list = []
-
-        dollar_id_map = DollarObjectIdMap()
-
-        for mdd_file in mdd_files:
-            path = mdd_file.get_path()
-            content = mdd_file.get_content()
-
-            dollar_object = DollarObjectImpl(
-                    content,
-                    path,
-                    path[:-1],
-                    "/" + path[:-1].replace("\\", "/"))
-
-            dollar_context = DollarContext(path, 0, 0)
-
-            header_parser_result = HeaderParser.parse(content, dollar_context)
-            dollar_object.set_unparsed_header(header_parser_result.header_object)
-            dollar_object.set_header_end(header_parser_result.header_end)
+    def init(path: str, content: str, dollar_id_map: Optional[DollarObjectIdMap]) -> DollarObjectImpl:
+        dollar_object = DollarObjectImpl(
+                content,
+                path,
+                path[:-1],
+                "/" + path[:-1].replace("\\", "/"))
+
+        dollar_context = DollarContext(path, 0, 0)
+
+        header_parser_result = HeaderParser.parse(content, dollar_context)
+        dollar_object.set_unparsed_header(header_parser_result.header_object)
+        dollar_object.set_header_end(header_parser_result.header_end)
 
+        if dollar_id_map is not None:
             try:
                 dollar_id_map.add(dollar_object)
             except DollarException as e:
                 raise DollarExecutionException(
                         e.get_message(),
                         dollar_context) from e
-            dollar_object_list.append(dollar_object)
-
-        for dollar_object in dollar_object_list:
+        return dollar_object
 
-            dollar_context = DollarContext(dollar_object.get_path(), 0, 0)
-
-            dollar_object.set_header(
-                    HeaderTransformer.transform(
-                            dollar_object,
-                            dollar_object.get_unparsed_header(),
-                            dollar_context,
-                            dollar_id_map))
-            try:
-                primary_plugin = plugin_map.get_extension(dollar_object.get_type())
-            except DollarException as e:
+    @staticmethod
+    def transform_header_primary(
+            dollar_object: DollarObjectImpl,
+            dollar_id_map: DollarObjectIdMap,
+            plugin_map: PluginMap):
+        dollar_context = DollarContext(dollar_object.get_path(), 0, 0)
+
+        dollar_object.set_header(
+                HeaderTransformer.transform(
+                        dollar_object,
+                        dollar_object.get_unparsed_header(),
+                        dollar_context,
+                        dollar_id_map))
+        try:
+            primary_plugin = plugin_map.get_extension(dollar_object.get_type())
+        except DollarException as e:
+            raise DollarExecutionException(
+                    e.get_message(),
+                    dollar_context) from e
+        validate_plugin = primary_plugin
+        visited = [dollar_object.get_type()]
+        while True:
+            if validate_plugin.extends() in visited:
                 raise DollarExecutionException(
-                        e.get_message(),
-                        dollar_context) from e
-            validate_plugin = primary_plugin
-            visited = [dollar_object.get_type()]
-            while True:
-                if validate_plugin.extends() in visited:
-                    raise DollarExecutionException(
-                            "Extension plugin {} in Dollar Object {} was caught in a circular dependency loop"
-                            .format(primary_plugin.get_name(), dollar_object.get_id()),
-                            dollar_context)
-                validation = validate_plugin.validate_primary(dollar_object)
-                if validation is not None:
+                        "Extension plugin {} in Dollar Object {} was caught in a circular dependency loop"
+                        .format(primary_plugin.get_name(), dollar_object.get_id()),
+                        dollar_context)
+            validation = validate_plugin.validate_primary(dollar_object)
+            if validation is not None:
+                raise DollarExecutionException(
+                        "Validation on {} failed: {}"
+                        .format(dollar_object.get_id(), validation),
+                        dollar_context)
+            if validate_plugin.extends() is not None:
+                visited.append(validate_plugin.extends())
+                try:
+                    validate_plugin = plugin_map.get_extension(validate_plugin.extends())
+                except DollarException as e:
                     raise DollarExecutionException(
-                            "Validation on {} failed: {}"
-                            .format(dollar_object.get_id(), validation),
-                            dollar_context)
-                if validate_plugin.extends() is not None:
-                    visited.append(validate_plugin.extends())
-                    try:
-                        validate_plugin = plugin_map.get_extension(validate_plugin.extends())
-                    except DollarException as e:
-                        raise DollarExecutionException(
-                                e.get_message(),
-                                dollar_context) from e
-                else:
-                    break
-
-            primary_plugin.exec_primary(dollar_object)
-
-            for key in dollar_object.get_header().keys():
-                if plugin_map.has_extension_with_secondary_key(key):
-                    plugin_map.get_extension_from_secondary_key(key)\
-                            .exec_secondary(dollar_object)
-
-        for dollar_object in dollar_object_list:
-            dollar_context_start = DollarContext(
-                    dollar_object.get_path(),
-                    dollar_object.get_header_end() + 2,
-                    0)
-            dollar_object.set_raw_formats(
-                    RawDollarParser.parse(
-                            dollar_object.get_content_without_header(),
-                            dollar_context_start))
-
-        for dollar_object in dollar_object_list:
-            dollar_object.set_input_formats(
-                    RawToInputTransformer.transform_list(
-                            dollar_object,
-                            dollar_object.get_raw_formats(),
-                            dollar_id_map,
-                            plugin_map))
-
-        for dollar_object in dollar_object_list:
-            dollar_object.set_output(
-                    InputToStrTransformer.transform_list(dollar_object, dollar_object.get_input_formats(), plugin_map))
-
-        outputs = []
-        for dollar_object in dollar_object_list:
-            dollar_file = DollarFile(
-                    dollar_object.get_output_path(),
-                    dollar_object.get_output())
-            outputs.append(dollar_file)
-        DollarFileWriter.write_files(conf_target_path, outputs)
-
-        for file_ending in conf_file_passthrough:
-            FileCopier.copy_files(
-                    conf_docs_path,
-                    conf_target_path,
-                    file_ending)
+                            e.get_message(),
+                            dollar_context) from e
+            else:
+                break
+
+        primary_plugin.exec_primary(dollar_object)
+
+    @staticmethod
+    def transform_header_secondary(
+            dollar_object: DollarObjectImpl,
+            dollar_id_map: DollarObjectIdMap,
+            plugin_map: PluginMap):
+        for key in dollar_object.get_header().keys():
+            if plugin_map.has_extension_with_secondary_key(key):
+                plugin_map.get_extension_from_secondary_key(key)\
+                        .exec_secondary(dollar_object)  # TODO: Handle backrefs in dollar instead
```

### Comparing `dollardoc-0.3.0/src/dollar/confighandler.py` & `dollardoc-0.4.0/src/dollar/confighandler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import yaml
-from typing import List
+import os
 
 from dollar.configmap import ConfigMap
 from dollar.configtype import ConfigType
 
 
 class ConfigHandler:
     required_config = [
         ConfigType.DOCS_PATH,
     ]
 
     @classmethod
-    def load_config_default(cls) -> ConfigMap:
-        return cls.load_config_file("dollarconfig.yaml")
+    def load_config_default(cls, path: str = "./") -> ConfigMap:
+        return cls.load_config_file(os.path.join(path, "dollarconfig.yaml"))
 
     @classmethod
-    def load_config_file(cls, path) -> ConfigMap:
+    def load_config_file(cls, path: str) -> ConfigMap:
         with open(path, "r") as f:
             config = yaml.safe_load(f.read())
             config_map = ConfigMap(config)
             config_map.validate(cls.required_config)
             return config_map
```

### Comparing `dollardoc-0.3.0/src/dollar/configmap.py` & `dollardoc-0.4.0/src/dollar/configmap.py`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/src/dollar/dollarcontext.py` & `dollardoc-0.4.0/src/dollar/dollarcontext.py`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/src/dollar/dollarexception.py` & `dollardoc-0.4.0/src/dollar/dollarexception.py`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/src/dollar/dollarobject.py` & `dollardoc-0.4.0/src/dollar/dollarobject.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,9 +37,14 @@
 
     def get_output_path(self):
         return self.output_path
 
     def get_target_path(self):
         return self.target_path
 
+    def equals(self, dollar_object):
+        return self.path == dollar_object.path and \
+                self.output_path == dollar_object.output_path and \
+                self.target_path == dollar_object.target_path
+
     def __repr__(self):
         return "DollarObject(id: " + self.get_id() + ")"
```

### Comparing `dollardoc-0.3.0/src/dollar/dollarobjectimpl.py` & `dollardoc-0.4.0/src/dollar/file/dollarfile.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,73 +1,42 @@
-from dollar.dollarobject import DollarObject
+from typing import List
 
-
-class DollarObjectImpl(DollarObject):
-
-    def __init__(self, content, path, output_path, target_path):
-        super().__init__(path, output_path, target_path)
-
-        self.content = content.split("\n")
-        self.header_end = 0
-        self.header = None
-        self.unparsed_header = {}
-        self.raw_formats = []
-        self.input_formats = []
-        self.output = ""
-
-    def get_id(self):
-        if self.header is None:
-            return self.unparsed_header["id"]
-        return self.header["id"]
-
-    def get_type(self):
-        if self.header is None:
-            return self.unparsed_header["type"]
-        return self.header["type"]
-
-    def get_header(self):
-        return self.header
-
-    def set_header(self, header):
-        self.header = header
-
-    def get_header_end(self):
-        return self.header_end
-
-    def set_header_end(self, header_end):
-        self.header_end = header_end
-
-    def get_unparsed_header(self):
-        return self.unparsed_header
-
-    def set_unparsed_header(self, unparsed_header):
-        self.unparsed_header = unparsed_header
-
-    def get_content_without_header(self):
-        return "\n".join(self.content[self.header_end + 1:])
-
-    def get_output(self) -> str:
-        return self.output
-
-    def set_output(self, output: str):
-        self.output = output
+from dollar.dollarexception import DollarExecutionException
+from dollar.dollarcontext import DollarContext
+from dollar.helper.validationhelper import ValidationHelper
+
+
+class DollarFile:
+
+    def __init__(self, path, content, file_ending):
+        if not ValidationHelper.valid_str(path):
+            raise DollarExecutionException(
+                    "Path passed to DollarFile must be valid string",
+                    DollarContext(path, 0, 0))
+        if not ValidationHelper.valid_str(content):
+            content = ""
+        if not ValidationHelper.valid_str(file_ending):
+            raise DollarExecutionException(
+                    "File Ending passed to DollarFile must be valid string",
+                    DollarContext(path, 0, 0))
+        self.path = path
+        self.content = content
+        self.file_ending = file_ending.lower()
 
     def get_path(self):
         return self.path
 
-    def get_output_path(self):
-        return self.output_path
-
-    def get_target_path(self):
-        return self.target_path
+    def get_content(self):
+        return self.content
 
-    def get_raw_formats(self):
-        return self.raw_formats
+    def get_file_ending(self):
+        return self.file_ending
 
-    def set_raw_formats(self, raw_formats):
-        self.raw_formats = raw_formats
+    def is_file_ending(self, file_ending_compare: str):
+        return self.file_ending == file_ending_compare.lower()
 
-    def get_input_formats(self):
-        return self.input_formats
+    def is_file_ending_in(self, file_ending_compares: List[str]):
+        file_ending_compares = [file_ending.lower() for file_ending in file_ending_compares]
+        return self.file_ending in file_ending_compares
 
-    def set_input_formats(self, input_formats):
-        self.input_formats = input_formats
+    def is_file_ending_in__assume_lower_case(self, file_ending_compares: List[str]):
+        return self.file_ending in file_ending_compares
```

### Comparing `dollardoc-0.3.0/src/dollar/file/dollarfilereader.py` & `dollardoc-0.4.0/src/dollar/file/dollarfilereader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 import os
+from typing import List
 
 from dollar.dollarexception import DollarException
 from dollar.file.dollarfile import DollarFile
 
 
 class DollarFileReader:
 
     @classmethod
-    def read_mdd_files(cls, src):
-        return cls._read_mdd_files(src)
+    def read_files(cls, src: str) -> List[DollarFile]:
+        return cls._read_files(src)
 
     @classmethod
-    def _read_mdd_files(cls, open_dir, _open_dir_start=None):
+    def _read_files(cls, open_dir, _open_dir_start=None) -> List[DollarFile]:
         if _open_dir_start is None:
             _open_dir_start = open_dir
         result = []
         dir_list = os.listdir(open_dir)
         for item in dir_list:
             full_path = os.path.join(open_dir, item)
             if os.path.isdir(full_path):
-                result2 = cls._read_mdd_files(full_path, _open_dir_start)
+                result2 = cls._read_files(full_path, _open_dir_start)
                 result = result + result2
-            elif item.endswith(".mdd"):
+            else:
                 try:
                     f = open(full_path, "r")
                 except Exception as e:
                     raise DollarException("Failed to open file {}".format(full_path)) from e
                 full_path_split = os.path.normpath(full_path).split(os.path.sep)
                 open_dir_start_split = os.path.normpath(_open_dir_start).split(os.path.sep)
                 to = len(full_path_split)
                 if to > len(open_dir_start_split):
                     to = len(open_dir_start_split)
                 new_path = str(os.path.sep).join(full_path_split[to:])
                 try:
                     file_output = f.read()
                 except Exception as e:
                     raise DollarException("Failed to read file {}".format(full_path)) from e
-                result.append(DollarFile(new_path, file_output))
+                result.append(DollarFile(new_path, file_output, item.split(".")[-1]))
                 f.close()
-            else:
-                pass  # Allow other files to exist in src
         return result
```

### Comparing `dollardoc-0.3.0/src/dollar/file/dollarfilewriter.py` & `dollardoc-0.4.0/src/dollar/file/dollarfilewriter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import os
 import shutil
+from typing import List
 
 from dollar.dollarexception import DollarException
+from dollar.file.dollarfile import DollarFile
 
 
 class DollarFileWriter:
 
     @staticmethod
-    def write_files(target_path, outputs):
+    def clean_dir(target_path):
         if os.path.exists(target_path):
             shutil.rmtree(target_path)
+    @staticmethod
+    def write_files(target_path, outputs: List[DollarFile]):
         for output in outputs:
             save_path = os.path.join(target_path, output.get_path())
             save_folder = os.path.split(save_path)[0]
             if not os.path.exists(save_folder):
                 os.makedirs(save_folder)
             try:
                 with open(save_path, "w") as f:
```

### Comparing `dollardoc-0.3.0/src/dollar/file/filecopier.py` & `dollardoc-0.4.0/src/dollar/file/filecopier.py`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/src/dollar/format/header/headerparser.py` & `dollardoc-0.4.0/src/dollar/format/header/headerparser.py`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/src/dollar/format/input/inputformat.py` & `dollardoc-0.4.0/src/dollar/format/input/inputformat.py`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/src/dollar/format/output/__init__.py` & `dollardoc-0.4.0/src/dollar/format/output/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,10 +12,11 @@
 from .outputformat import OutputFormatUnorderedList
 from .outputformat import OutputFormatListItem
 from .outputformat import OutputFormatCodeBlock
 from .outputformat import OutputFormatQuoteBlock
 from .outputformat import OutputFormatDefinition
 from .outputformat import OutputFormatPluginBlock
 from .outputformat import OutputFormatDollarObject
+from .outputformatdollarobjectlinktype import OutputFormatDollarObjectLinkType
 from .outputformatter import OutputFormatterMarkdown
 from .outputformatterhandler import OutputFormatterHandler
 from .outputformattype import OutputFormatType
```

### Comparing `dollardoc-0.3.0/src/dollar/format/output/outputfactory.py` & `dollardoc-0.4.0/src/dollar/format/output/outputfactory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 from dollar.dollarobject import DollarObject
 from dollar.format.output.outputformat import OutputFormatText
 from dollar.format.output.outputformat import OutputFormatLink
 from dollar.format.output.outputformat import OutputFormatDollarObject
-from dollar.format.output.outputformatterhandler import OutputFormatterHandler
+from dollar.format.output.outputformatter import OutputFormatter
 
 
 class OutputFactory:
 
     @classmethod
-    def create_link(cls, this_dollar_object: DollarObject, text, href):
-        return OutputFormatterHandler.get_formatter().format_inline(this_dollar_object, [
+    def create_link(
+            cls,
+            output_formatter: OutputFormatter,
+            this_dollar_object: DollarObject,
+            text,
+            href):
+        return output_formatter.format_inline(this_dollar_object, [
             OutputFormatLink(href, [
                 OutputFormatText(text)
             ])
         ])
 
     @classmethod
-    def create_link_dollar_object(cls, this_dollar_object: DollarObject, to_dollar_object: DollarObject):
-        return OutputFormatterHandler.get_formatter().format_inline(this_dollar_object, [
+    def create_link_dollar_object(
+            cls,
+            output_formatter: OutputFormatter,
+            this_dollar_object: DollarObject,
+            to_dollar_object: DollarObject):
+        return output_formatter.format_inline(this_dollar_object, [
             OutputFormatDollarObject(to_dollar_object)
         ])
 
     @classmethod
     def create_list(cls, list_structure):
         pass
```

### Comparing `dollardoc-0.3.0/src/dollar/format/output/outputformat.py` & `dollardoc-0.4.0/src/dollar/format/output/outputformat.py`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/src/dollar/format/output/outputformatter.py` & `dollardoc-0.4.0/src/dollar/format/output/outputformatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,20 +16,32 @@
 from dollar.format.output.outputformat import OutputFormatUnorderedList
 from dollar.format.output.outputformat import OutputFormatListItem
 from dollar.format.output.outputformat import OutputFormatCodeBlock
 from dollar.format.output.outputformat import OutputFormatQuoteBlock
 from dollar.format.output.outputformat import OutputFormatDefinition
 from dollar.format.output.outputformat import OutputFormatPluginBlock
 from dollar.format.output.outputformat import OutputFormatDollarObject
+from dollar.format.output.outputformatdollarobjectlinktype import OutputFormatDollarObjectLinkType
 
 
-class OutputFormatterMarkdown:
+class OutputFormatter:
 
-    @classmethod
-    def format(cls, this_dollar_object: DollarObject, dollar_formats: List[OutputFormat], context=""):
+    def format(self, this_dollar_object: DollarObject, dollar_formats: List[OutputFormat], context="") -> str:
+        pass
+
+    def format_inline(self, this_dollar_object: DollarObject, dollar_formats: List[OutputFormat]) -> str:
+        pass
+
+
+class OutputFormatterMarkdown(OutputFormatter):
+
+    def __init__(self, output_format_dollar_object_link_type: OutputFormatDollarObjectLinkType):
+        self.link_type = output_format_dollar_object_link_type
+
+    def format(self, this_dollar_object: DollarObject, dollar_formats: List[OutputFormat], context="") -> str:
         result = []
         for dollar_format in dollar_formats:
             dollar_format.validate()
             dollar_format_type = dollar_format.get_format_type()
             if not dollar_format.is_block():
                 raise DollarExecutionException(
                         "{} is not allowed as a root level block".format(dollar_format.get_format_type()))
@@ -39,31 +51,31 @@
                 head = ""
                 for i in range(0, dollar_format.get_level()):
                     head = head + "#"
                 result.append(
                         context
                         + head
                         + " "
-                        + cls.format_inline(this_dollar_object, dollar_format.get_children()))
+                        + self.format_inline(this_dollar_object, dollar_format.get_children()))
 
             elif dollar_format_type == OutputFormatType.PARAGRAPH:
                 dollar_format = cast(OutputFormatParagraph, dollar_format)
-                result.append(context + cls.format_inline(this_dollar_object, dollar_format.get_children()))
+                result.append(context + self.format_inline(this_dollar_object, dollar_format.get_children()))
 
             elif dollar_format_type == OutputFormatType.ORDERED_LIST:
                 dollar_format = cast(OutputFormatOrderedList, dollar_format)
                 result.append(
                         context
-                        + cls.format_list(this_dollar_object, dollar_format.get_children(), True, context))
+                        + self.format_list(this_dollar_object, dollar_format.get_children(), True, context))
 
             elif dollar_format_type == OutputFormatType.UNORDERED_LIST:
                 dollar_format = cast(OutputFormatUnorderedList, dollar_format)
                 result.append(
                         context
-                        + cls.format_list(this_dollar_object, dollar_format.get_children(), False, context))
+                        + self.format_list(this_dollar_object, dollar_format.get_children(), False, context))
 
             elif dollar_format_type == OutputFormatType.CODE_BLOCK:
                 dollar_format = cast(OutputFormatCodeBlock, dollar_format)
                 join_str = "\n" + context
                 text = join_str.join(dollar_format.get_text().split("\n"))
                 result.append(
                         context
@@ -74,25 +86,25 @@
                         + text
                         + "\n"
                         + context
                         + "```")
 
             elif dollar_format_type == OutputFormatType.QUOTE_BLOCK:
                 dollar_format = cast(OutputFormatQuoteBlock, dollar_format)
-                result.append(cls.format(this_dollar_object, dollar_format.get_children(), context + "> "))
+                result.append(self.format(this_dollar_object, dollar_format.get_children(), context + "> "))
 
             elif dollar_format_type == OutputFormatType.DEFINITION:
                 dollar_format = cast(OutputFormatDefinition, dollar_format)
                 result.append(
                         context
-                        + cls.format_inline(this_dollar_object, dollar_format.get_defined_children())
+                        + self.format_inline(this_dollar_object, dollar_format.get_defined_children())
                         + "\n"
                         + context
                         + ": "
-                        + cls.format_inline(this_dollar_object, dollar_format.get_definition_children()))
+                        + self.format_inline(this_dollar_object, dollar_format.get_definition_children()))
 
             elif dollar_format_type == OutputFormatType.PLUGIN_BLOCK:
                 dollar_format = cast(OutputFormatPluginBlock, dollar_format)
                 join_str = "\n" + context
                 text = join_str.join(dollar_format.get_text().split("\n"))
                 result.append(
                         context
@@ -108,94 +120,97 @@
             else:
                 raise DollarExecutionException(
                         "{} is not allowed as a root level block".format(dollar_format.get_format_type()))
 
         join_str = "\n" + context + "\n"
         return join_str.join(result)
 
-    @classmethod
-    def format_inline(cls, this_dollar_object: DollarObject, dollar_formats: List[OutputFormat]):
+    def format_inline(self, this_dollar_object: DollarObject, dollar_formats: List[OutputFormat]) -> str:
         result = ""
         for dollar_format in dollar_formats:
             dollar_format.validate()
             dollar_format_type = dollar_format.get_format_type()
             if dollar_format.is_block():
                 raise DollarExecutionException(
                         "{} is not allowed as a nested inline item".format(dollar_format.get_format_type()))
 
             if dollar_format_type == OutputFormatType.TEXT:
                 dollar_format = cast(OutputFormatText, dollar_format)
                 result = result + dollar_format.get_text()
 
             elif dollar_format_type == OutputFormatType.BOLD:
                 dollar_format = cast(OutputFormatBold, dollar_format)
-                result = result + "**" + cls.format_inline(this_dollar_object, dollar_format.get_children()) + "**"
+                result = result + "**" + self.format_inline(this_dollar_object, dollar_format.get_children()) + "**"
 
             elif dollar_format_type == OutputFormatType.ITALIC:
                 dollar_format = cast(OutputFormatItalic, dollar_format)
-                result = result + "*" + cls.format_inline(this_dollar_object, dollar_format.get_children()) + "*"
+                result = result + "*" + self.format_inline(this_dollar_object, dollar_format.get_children()) + "*"
 
             elif dollar_format_type == OutputFormatType.CODE:
                 dollar_format = cast(OutputFormatCode, dollar_format)
                 result = result + "`" + dollar_format.get_text() + "`"
 
             elif dollar_format_type == OutputFormatType.LINK:
                 dollar_format = cast(OutputFormatLink, dollar_format)
                 result = result + "["
-                result = result + cls.format_inline(this_dollar_object, dollar_format.get_children())
+                result = result + self.format_inline(this_dollar_object, dollar_format.get_children())
                 result = result + "]("
                 result = result + dollar_format.get_href()
                 result = result + ")"
 
             elif dollar_format_type == OutputFormatType.DOLLAR_OBJECT:
                 dollar_format = cast(OutputFormatDollarObject, dollar_format)
                 dollar_object = dollar_format.get_dollar_object()
                 title = dollar_object.get_id()
                 if "title" in dollar_object.get_header():
                     title = dollar_object.get_header()["title"]
-                result = result + "[" + title + "](" + dollar_format.get_href(this_dollar_object) + ")"
+                result = result + "[" + title + "]("
+                if self.link_type == OutputFormatDollarObjectLinkType.TO_MARKDOWN_FILE:
+                    result = result + dollar_format.get_href(this_dollar_object)
+                elif self.link_type == OutputFormatDollarObjectLinkType.TO_DOLLAR_ID:
+                    result = result + dollar_format.get_dollar_object().get_id()
+                result = result + ")"
 
             else:
                 raise DollarExecutionException("Format {} is not supported".format(dollar_format_type))
 
         return result
 
-    @classmethod
-    def format_list(cls, this_dollar_object: DollarObject, dollar_formats: List[OutputFormat], ordered, context=""):
+    def format_list(self, this_dollar_object: DollarObject, dollar_formats: List[OutputFormat], ordered, context=""):
         count = 1
         result = ""
         for dollar_format in dollar_formats:
             dollar_format.validate()
             dollar_format_type = dollar_format.get_format_type()
             if dollar_format_type == OutputFormatType.LIST_ITEM:
                 dollar_format = cast(OutputFormatListItem, dollar_format)
                 if count > 1:
                     result = result + "\n"
                 if ordered:
                     result = result + context + str(count) + ". "
                 else:
                     result = result + context + "* "
                 count = count + 1
-                result = result + cls.format_inline(this_dollar_object, dollar_format.get_children())
+                result = result + self.format_inline(this_dollar_object, dollar_format.get_children())
 
             elif dollar_format_type == OutputFormatType.ORDERED_LIST:
                 dollar_format = cast(OutputFormatOrderedList, dollar_format)
                 if count == 1:
                     raise DollarExecutionException("List can not be the first item inside a List")
-                result = result + "\n" + cls.format_list(
+                result = result + "\n" + self.format_list(
                         this_dollar_object,
                         dollar_format.get_children(),
                         True,
                         context + "    ")
 
             elif dollar_format_type == OutputFormatType.UNORDERED_LIST:
                 dollar_format = cast(OutputFormatUnorderedList, dollar_format)
                 if count == 1:
                     raise DollarExecutionException("List can not be the first item inside a List")
-                result = result + "\n" + cls.format_list(
+                result = result + "\n" + self.format_list(
                         this_dollar_object,
                         dollar_format.get_children(),
                         False,
                         context + "    ")
 
             else:
                 raise DollarExecutionException("Format {} is not supported on List".format(dollar_format_type))
```

### Comparing `dollardoc-0.3.0/src/dollar/format/raw/rawdollarformat.py` & `dollardoc-0.4.0/src/dollar/format/raw/rawdollarformat.py`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/src/dollar/format/raw/rawdollarparser.py` & `dollardoc-0.4.0/src/dollar/format/raw/rawdollarparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             if last_char == "\\":
                 escape = True
                 if char == "\\":
                     text = text + "\\"
                     last_char = char
                     continue
             if char == "$" and not escape and not quotes:
-                if dollar_open == 3 and raw_content[i+1] != "$" and dollar_count != 2:
+                if dollar_open == 3 and (i + 1) < len(raw_content) and raw_content[i+1] != "$" and dollar_count != 2:
                     text = text + "$"
                 elif dollar_open not in (0, 3):
                     text = text + "$"
                     last_char = char
                     continue
                 dollar_count = dollar_count + 1
                 if dollar_open == 0 and text != "":
```

### Comparing `dollardoc-0.3.0/src/dollar/format/transformer/headertransformer.py` & `dollardoc-0.4.0/src/dollar/format/transformer/headertransformer.py`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/src/dollar/format/transformer/inputtostrtransformer.py` & `dollardoc-0.4.0/src/dollar/format/transformer/inputtostrtransformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,81 +10,97 @@
 from dollar.format.input.inputformat import InputFormatDollarObject
 from dollar.format.input.inputformat import InputFormatDollarObjectValue
 from dollar.format.input.inputformat import InputFormatFunction
 from dollar.format.input.inputformat import InputFormatBlock
 from dollar.format.input.inputformat import InputFormatUnion
 from dollar.format.input.inputformattype import InputFormatType
 from dollar.format.output.outputfactory import OutputFactory
-from dollar.format.output.outputformatterhandler import OutputFormatterHandler
+from dollar.format.output.outputformatter import OutputFormatter
 from dollar.plugin.pluginargvalidatior import PluginArgValidator
 from dollar.plugin.pluginmap import PluginMap
 
 
 class InputToStrTransformer:
 
     @classmethod
-    def transform(cls, this_dollar_object: DollarObject, input_format: InputFormat, plugin_map: PluginMap) -> str:
+    def transform(
+            cls,
+            output_formatter: OutputFormatter,
+            this_dollar_object: DollarObject,
+            input_format: InputFormat,
+            plugin_map: PluginMap) -> str:
         if input_format.get_format_type() == InputFormatType.TEXT:
             input_format = cast(InputFormatText, input_format)
             return input_format.get_text()
 
         elif input_format.get_format_type() == InputFormatType.DOLLAR_OBJECT:
             input_format = cast(InputFormatDollarObject, input_format)
-            return OutputFactory.create_link_dollar_object(this_dollar_object, input_format.get_dollar_object())
+            return OutputFactory.create_link_dollar_object(
+                    output_formatter,
+                    this_dollar_object,
+                    input_format.get_dollar_object())
 
         elif input_format.get_format_type() == InputFormatType.DOLLAR_OBJECT_VALUE:
             input_format = cast(InputFormatDollarObjectValue, input_format)
             if type(input_format.get_value()) == str:
                 if not ValidationHelper.valid_str(input_format.get_value()):
                     raise DollarExecutionException(
                             "When rendering, dollar header referenced value needs to be a non blank str",
                             input_format.get_dollar_context())
                 return input_format.get_value()
             elif isinstance(input_format.get_value(), DollarObject):
-                return OutputFactory.create_link_dollar_object(this_dollar_object, input_format.get_value())
+                return OutputFactory.create_link_dollar_object(
+                        output_formatter,
+                        this_dollar_object,
+                        input_format.get_value())
             else:
                 raise DollarExecutionException(
                         "When rendering, dollar header referenced value needs to be str or DollarObject",
                         input_format.get_dollar_context())
 
         elif input_format.get_format_type() == InputFormatType.FUNCTION:
             input_format = cast(InputFormatFunction, input_format)
             plugin = input_format.get_function_plugin()
             params = input_format.get_parameters()
             plugin.get_arg_info()
 
             try:
                 PluginArgValidator.validate(params, plugin.get_arg_info(), plugin_map)
                 plugin_output = plugin.exec_function(*params)
-                return OutputFormatterHandler.get_formatter().format(this_dollar_object, plugin_output)
+                return output_formatter.format(this_dollar_object, plugin_output)
             except DollarException as e:
                 raise DollarExecutionException(
                         e.get_message(),
                         input_format.get_dollar_context()) from e
 
         elif input_format.get_format_type() == InputFormatType.BLOCK:
             input_format = cast(InputFormatBlock, input_format)
             plugin = input_format.get_block_plugin()
             content = input_format.get_content()
             plugin_output = plugin.exec_block(content)
             try:
-                return OutputFormatterHandler.get_formatter().format(this_dollar_object, plugin_output)
+                return output_formatter.format(this_dollar_object, plugin_output)
             except DollarException as e:
                 raise DollarExecutionException(
                         e.get_message(),
                         input_format.get_dollar_context()) from e
 
         elif input_format.get_format_type() == InputFormatType.UNION:
             input_format = cast(InputFormatUnion, input_format)
-            return cls.transform_list(this_dollar_object, input_format.get_children())
+            return cls.transform_list(output_formatter, this_dollar_object, input_format.get_children(), plugin_map)
 
         else:
             raise DollarExecutionException(
                     "Format {} is not supported".format(input_format.get_format_type()),
                     input_format.get_dollar_context())
 
     @classmethod
-    def transform_list(cls, this_dollar_object: DollarObject, input_formats: List[InputFormat], plugin_map: PluginMap):
+    def transform_list(
+            cls,
+            output_formatter: OutputFormatter,
+            this_dollar_object: DollarObject,
+            input_formats: List[InputFormat],
+            plugin_map: PluginMap):
         result = []
         for input_format in input_formats:
-            result.append(cls.transform(this_dollar_object, input_format, plugin_map))
+            result.append(cls.transform(output_formatter, this_dollar_object, input_format, plugin_map))
         return "".join(result)
```

### Comparing `dollardoc-0.3.0/src/dollar/format/transformer/rawtoinputtransformer.py` & `dollardoc-0.4.0/src/dollar/format/transformer/rawtoinputtransformer.py`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/src/dollar/helper/dollarobjecthelper.py` & `dollardoc-0.4.0/src/dollar/helper/dollarobjecthelper.py`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/src/dollar/plugin/builtin/dollarbaseextensionplugin.py` & `dollardoc-0.4.0/src/dollar/plugin/builtin/dollarbaseextensionplugin.py`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/src/dollar/plugin/builtin/linkfunctionplugin.py` & `dollardoc-0.4.0/src/dollar/plugin/builtin/linkfunctionplugin.py`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/src/dollar/plugin/builtin/listbacklinksfunctionplugin.py` & `dollardoc-0.4.0/src/dollar/plugin/builtin/listbacklinksfunctionplugin.py`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/src/dollar/plugin/builtin/listfunctionplugin.py` & `dollardoc-0.4.0/src/dollar/plugin/builtin/listfunctionplugin.py`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/src/dollar/plugin/builtin/listreffunctionplugin.py` & `dollardoc-0.4.0/src/dollar/plugin/builtin/listreffunctionplugin.py`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/src/dollar/plugin/builtin/pageextensionplugin.py` & `dollardoc-0.4.0/src/dollar/plugin/builtin/pageextensionplugin.py`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/src/dollar/plugin/dollarplugin.py` & `dollardoc-0.4.0/src/dollar/plugin/dollarplugin.py`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/src/dollar/plugin/pluginarg.py` & `dollardoc-0.4.0/src/dollar/plugin/pluginarg.py`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/src/dollar/plugin/pluginargvalidatior.py` & `dollardoc-0.4.0/src/dollar/plugin/pluginargvalidatior.py`

 * *Files identical despite different names*

### Comparing `dollardoc-0.3.0/src/dollar/plugin/pluginhandler.py` & `dollardoc-0.4.0/src/dollar/plugin/pluginhandler.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 import os
 import importlib.util
 import inspect
 
+from dollar.plugin.builtinpluginloader import BuiltinPluginLoader
 from dollar.plugin.dollarplugin import DollarPlugin
 from dollar.plugin.pluginmap import PluginMap
 from dollar.configmap import ConfigMap
 
 
 class PluginHandler:
 
-    plugin_map = PluginMap()
-
     @classmethod
     def _import_plugin_path(cls, path, plugin_map: PluginMap, config_map: ConfigMap):
         spec = importlib.util.spec_from_file_location(path, path)
         module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(module)
+        skip = 0
         for key in module.__dict__:
             if inspect.isclass(module.__dict__[key]) and issubclass(module.__dict__[key], DollarPlugin):
-                plugin_map.add(module.__dict__[key](config_map))
+                instance = module.__dict__[key](config_map)
+                if instance.get_name() is not None:
+                    plugin_map.add(instance)
 
     @classmethod
     def import_plugins(cls, path: str, config_map: ConfigMap) -> PluginMap:
-        plugin_map = cls.plugin_map._copy()
+        plugin_map = PluginMap()
+        BuiltinPluginLoader.load(config_map, plugin_map)
         cls._import_plugins(os.path.join(os.path.curdir, path), plugin_map, config_map)
         return plugin_map
 
     @classmethod
     def _import_plugins(cls, abs_path, plugin_map: PluginMap, config_map: ConfigMap):
         dir_list = os.listdir(abs_path)
         for item in dir_list:
             new_path = os.path.join(abs_path, item)
             if os.path.isdir(new_path):
                 cls._import_plugins(new_path, plugin_map, config_map)
             elif item.endswith(".py"):
                 cls._import_plugin_path(new_path, plugin_map, config_map)
-
-    @classmethod
-    def register(cls, plugin: DollarPlugin):
-        cls.plugin_map.add(plugin)
```

### Comparing `dollardoc-0.3.0/src/dollar/plugin/pluginmap.py` & `dollardoc-0.4.0/src/dollar/plugin/pluginmap.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 
     def get_extension(self, plugin_name) -> DollarExtensionPlugin:
         if not self.has_extension(plugin_name):
             raise DollarException("Extension plugin with name {}, cannot be found".format(plugin_name))
         return self.extension_map[plugin_name]
 
     def has_extension(self, plugin_name):
+        if plugin_name is None:
+            return False
         return plugin_name in self.extension_map
 
     def get_extension_from_secondary_key(self, key) -> DollarExtensionPlugin:
         if key not in self.extension_secondary_map:
             raise DollarException("No extension plugin with handler for secondary key {}".format(key))
         return self.extension_secondary_map[key]
```

### Comparing `dollardoc-0.3.0/src/dollardoc.egg-info/PKG-INFO` & `dollardoc-0.4.0/src/dollardoc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dollardoc
-Version: 0.3.0
+Version: 0.4.0
 Summary: Object oriented markdown documentation
 Home-page: https://github.com/dollardoc/dollardoc
 Author: dollardoc
 Author-email: development@dollardoc.dev
 License: UNKNOWN
 Description: # DollarDoc
         
@@ -148,15 +148,15 @@
         $ python build.py
         ```
         
         Unless there is an exception, all your generated markdown files will show up in the `output/` folder.
         
         ## Dollar Syntax Specification Document
         
-        *Specification currently under development*
+        [dollar-syntax-specification-v0_1_0.pdf](https://github.com/dollardoc/dollar-syntax-specification/releases/download/v0.1.0/dollar-syntax-specification-v0_1_0.pdf)
         
         ## Outputs Supported
         
         This project only supports plain markdown files. Other alternatives has been considered, like docusaurus style markdown output, but nothing has been decided at this moment.
         
         ## Future of the Project
```

### Comparing `dollardoc-0.3.0/src/dollardoc.egg-info/SOURCES.txt` & `dollardoc-0.4.0/src/dollardoc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/dollar/dollarcontext.py
 src/dollar/dollarexception.py
 src/dollar/dollarobject.py
 src/dollar/dollarobjectidmap.py
 src/dollar/dollarobjectimpl.py
 src/dollar/builder/__init__.py
 src/dollar/builder/dollarbuilder.py
+src/dollar/builder/dollarlivebuilder.py
 src/dollar/cli/__init__.py
 src/dollar/cli/cli.py
 src/dollar/file/__init__.py
 src/dollar/file/dollarfile.py
 src/dollar/file/dollarfilereader.py
 src/dollar/file/dollarfilewriter.py
 src/dollar/file/filecopier.py
@@ -27,26 +28,28 @@
 src/dollar/format/header/headerparserresult.py
 src/dollar/format/input/__init__.py
 src/dollar/format/input/inputformat.py
 src/dollar/format/input/inputformattype.py
 src/dollar/format/output/__init__.py
 src/dollar/format/output/outputfactory.py
 src/dollar/format/output/outputformat.py
+src/dollar/format/output/outputformatdollarobjectlinktype.py
 src/dollar/format/output/outputformatter.py
 src/dollar/format/output/outputformatterhandler.py
 src/dollar/format/output/outputformattype.py
 src/dollar/format/raw/__init__.py
 src/dollar/format/raw/rawdollarformat.py
 src/dollar/format/raw/rawdollarformattype.py
 src/dollar/format/raw/rawdollarparser.py
 src/dollar/format/transformer/__init__.py
 src/dollar/format/transformer/headertransformer.py
 src/dollar/format/transformer/inputtostrtransformer.py
 src/dollar/format/transformer/rawtoinputtransformer.py
 src/dollar/helper/__init__.py
+src/dollar/helper/dollarobjectcreationhelper.py
 src/dollar/helper/dollarobjecthelper.py
 src/dollar/helper/validationhelper.py
 src/dollar/plugin/__init__.py
 src/dollar/plugin/builtinpluginloader.py
 src/dollar/plugin/dollarplugin.py
 src/dollar/plugin/pluginarg.py
 src/dollar/plugin/pluginargvalidatior.py
```

