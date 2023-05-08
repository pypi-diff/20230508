# Comparing `tmp/pyutplugins-0.8.60.tar.gz` & `tmp/pyutplugins-0.8.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutplugins-0.8.60.tar", last modified: Fri May  5 01:33:48 2023, max compression
+gzip compressed data, was "pyutplugins-0.8.70.tar", last modified: Mon May  8 19:04:56 2023, max compression
```

## Comparing `pyutplugins-0.8.60.tar` & `pyutplugins-0.8.70.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.783559 pyutplugins-0.8.60/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2311 2023-05-05 01:33:48.783406 pyutplugins-0.8.60/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1956 2023-04-14 20:22:33.000000 pyutplugins-0.8.60/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.768492 pyutplugins-0.8.60/pyutplugins/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6400 2023-01-04 04:59:38.000000 pyutplugins-0.8.60/pyutplugins/ExternalTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3210 2023-01-20 18:33:44.000000 pyutplugins-0.8.60/pyutplugins/IPluginAdapter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8054 2023-03-31 00:30:02.000000 pyutplugins-0.8.60/pyutplugins/PluginManager.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.769621 pyutplugins-0.8.60/pyutplugins/common/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1130 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/common/ElementTreeData.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2353 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/common/LinkMakerMixin.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      469 2023-01-19 02:57:18.000000 pyutplugins-0.8.60/pyutplugins/common/PluginTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/common/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/common/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.769919 pyutplugins-0.8.60/pyutplugins/common/ui/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2224 2023-01-20 15:07:17.000000 pyutplugins-0.8.60/pyutplugins/common/ui/BaseEditDialog.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/common/ui/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.770163 pyutplugins-0.8.60/pyutplugins/common/ui/preferences/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5175 2023-05-03 19:43:51.000000 pyutplugins-0.8.60/pyutplugins/common/ui/preferences/PluginPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-01 02:55:47.000000 pyutplugins-0.8.60/pyutplugins/common/ui/preferences/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/common/ui/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.770756 pyutplugins-0.8.60/pyutplugins/exceptions/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       66 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/exceptions/AbstractMethodNotImplementedException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       60 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/exceptions/InvalidPluginExtensionException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/exceptions/InvalidPluginNameException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/exceptions/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/exceptions/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.771988 pyutplugins-0.8.60/pyutplugins/ioplugins/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1924 2023-01-20 18:45:21.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/IOAscii.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2893 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/IODTD.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2849 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/IOGML.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4134 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/IOJava.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3245 2023-01-30 01:49:48.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/IOMermaid.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3864 2023-02-03 02:52:30.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/IOPdf.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7942 2023-05-05 01:14:03.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/IOPython.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4078 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/IOWxImage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8266 2023-01-30 01:49:48.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/IOXml.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.772533 pyutplugins-0.8.60/pyutplugins/ioplugins/dtd/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      326 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/dtd/DTDAttribute.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      430 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/dtd/DTDElementTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10397 2023-01-20 18:33:44.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/dtd/DTDParser.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/dtd/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/dtd/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.772995 pyutplugins-0.8.60/pyutplugins/ioplugins/gml/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8647 2023-02-01 01:59:25.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/gml/GMLExporter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/gml/UnsupportedOperation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/gml/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/gml/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.773468 pyutplugins-0.8.60/pyutplugins/ioplugins/java/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    27944 2023-01-20 18:45:21.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/java/JavaReader.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11156 2023-02-01 01:52:43.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/java/JavaWriter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/java/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/java/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.773929 pyutplugins-0.8.60/pyutplugins/ioplugins/mermaid/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      994 2023-02-01 20:38:32.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/mermaid/MermaidDirection.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12464 2023-04-17 23:17:22.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/mermaid/MermaidWriter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-30 01:49:48.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/mermaid/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/mermaid/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.774492 pyutplugins-0.8.60/pyutplugins/ioplugins/pdf/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      132 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/pdf/ImageFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      554 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/pdf/ImageOptions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9553 2023-01-20 18:33:44.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/pdf/OglToPyUmlDefinition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/pdf/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/pdf/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.775671 pyutplugins-0.8.60/pyutplugins/ioplugins/python/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6135 2023-05-05 01:14:03.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/DlgSelectMultiplePackages.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3579 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/Python3LexerBase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      192 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/Python3ParserBase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/PythonParseException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12836 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/PyutPythonVisitor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12487 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/PyutToPython.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    18319 2023-05-05 01:14:03.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/ReverseEngineerPython2.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.776577 pyutplugins-0.8.60/pyutplugins/ioplugins/python/pyantlrparser/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    47673 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/pyantlrparser/Python3Lexer.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)   399206 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/pyantlrparser/Python3Parser.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    37475 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserListener.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    22412 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserVisitor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/pyantlrparser/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      804 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/transformGrammar.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.777006 pyutplugins-0.8.60/pyutplugins/ioplugins/wximage/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4853 2023-05-05 01:14:03.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      929 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/wximage/WxImageFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/wximage/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/wximage/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.777521 pyutplugins-0.8.60/pyutplugins/plugininterfaces/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11797 2023-05-03 19:43:51.000000 pyutplugins-0.8.60/pyutplugins/plugininterfaces/BasePluginInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5202 2023-01-20 21:59:06.000000 pyutplugins-0.8.60/pyutplugins/plugininterfaces/IOPluginInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1226 2023-01-20 15:37:30.000000 pyutplugins-0.8.60/pyutplugins/plugininterfaces/ToolPluginInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/plugininterfaces/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/plugininterfaces/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.778739 pyutplugins-0.8.60/pyutplugins/plugintypes/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2131 2023-02-03 02:56:53.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/BaseFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      112 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/BaseRequestResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      225 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/ExportDirectoryResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      205 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/ImportDirectoryResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      532 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/InputFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      330 2023-01-20 18:45:21.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/MultipleFileRequestResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      533 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/OutputFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1766 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/PluginDataTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      202 2023-01-20 18:45:21.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/SingleFileRequestResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.779050 pyutplugins-0.8.60/pyutplugins/preferences/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7651 2023-03-31 00:30:24.000000 pyutplugins-0.8.60/pyutplugins/preferences/PluginPreferences.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-18 02:02:54.000000 pyutplugins-0.8.60/pyutplugins/preferences/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyutplugins-0.8.60/pyutplugins/preferences/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.780276 pyutplugins-0.8.60/pyutplugins/toolplugins/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1730 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/ToolArrangeLinks.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3592 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/ToolAscii.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4402 2023-01-20 18:45:21.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3159 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/ToolSugiyama.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1989 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/ToolTransforms.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.781273 pyutplugins-0.8.60/pyutplugins/toolplugins/orthogonal/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1996 2023-05-03 19:43:51.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      737 2023-01-19 03:33:52.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5230 2023-01-20 18:33:44.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/orthogonal/OrthogonalAdapterException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/orthogonal/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/orthogonal/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.783219 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3545 2023-02-22 02:39:48.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/ALayoutLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1025 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/ALayoutNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3262 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    28462 2023-02-01 01:51:21.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/Sugiyama.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      263 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/SugiyamaConstants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2108 2023-01-20 15:25:55.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3228 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14778 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1387 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.769069 pyutplugins-0.8.60/pyutplugins.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2311 2023-05-05 01:33:48.000000 pyutplugins-0.8.60/pyutplugins.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5161 2023-05-05 01:33:48.000000 pyutplugins-0.8.60/pyutplugins.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-05-05 01:33:48.000000 pyutplugins-0.8.60/pyutplugins.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      203 2023-05-05 01:33:48.000000 pyutplugins-0.8.60/pyutplugins.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-05-05 01:33:48.000000 pyutplugins-0.8.60/pyutplugins.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-05-05 01:33:48.783600 pyutplugins-0.8.60/setup.cfg
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3207 2023-05-03 19:43:51.000000 pyutplugins-0.8.60/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.325317 pyutplugins-0.8.70/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2311 2023-05-08 19:04:56.325175 pyutplugins-0.8.70/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1956 2023-04-14 20:22:33.000000 pyutplugins-0.8.70/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.302172 pyutplugins-0.8.70/pyutplugins/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6400 2023-01-04 04:59:38.000000 pyutplugins-0.8.70/pyutplugins/ExternalTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3210 2023-01-20 18:33:44.000000 pyutplugins-0.8.70/pyutplugins/IPluginAdapter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8054 2023-03-31 00:30:02.000000 pyutplugins-0.8.70/pyutplugins/PluginManager.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.303904 pyutplugins-0.8.70/pyutplugins/common/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1130 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/common/ElementTreeData.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2353 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/common/LinkMakerMixin.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      469 2023-01-19 02:57:18.000000 pyutplugins-0.8.70/pyutplugins/common/PluginTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/common/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/common/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.304499 pyutplugins-0.8.70/pyutplugins/common/ui/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2224 2023-01-20 15:07:17.000000 pyutplugins-0.8.70/pyutplugins/common/ui/BaseEditDialog.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/common/ui/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.304876 pyutplugins-0.8.70/pyutplugins/common/ui/preferences/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5175 2023-05-03 19:43:51.000000 pyutplugins-0.8.70/pyutplugins/common/ui/preferences/PluginPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-01 02:55:47.000000 pyutplugins-0.8.70/pyutplugins/common/ui/preferences/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/common/ui/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.305799 pyutplugins-0.8.70/pyutplugins/exceptions/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       66 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/exceptions/AbstractMethodNotImplementedException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       60 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/exceptions/InvalidPluginExtensionException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/exceptions/InvalidPluginNameException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/exceptions/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/exceptions/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.308385 pyutplugins-0.8.70/pyutplugins/ioplugins/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1924 2023-01-20 18:45:21.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/IOAscii.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2893 2023-01-20 18:45:20.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/IODTD.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2849 2023-01-20 18:45:20.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/IOGML.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4134 2023-01-20 18:45:20.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/IOJava.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3245 2023-01-30 01:49:48.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/IOMermaid.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3864 2023-02-03 02:52:30.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/IOPdf.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7942 2023-05-05 01:14:03.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/IOPython.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4078 2023-01-20 18:45:20.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/IOWxImage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8266 2023-01-30 01:49:48.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/IOXml.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.309150 pyutplugins-0.8.70/pyutplugins/ioplugins/dtd/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      326 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/dtd/DTDAttribute.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      430 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/dtd/DTDElementTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10397 2023-01-20 18:33:44.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/dtd/DTDParser.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/dtd/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/dtd/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.309809 pyutplugins-0.8.70/pyutplugins/ioplugins/gml/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8647 2023-02-01 01:59:25.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/gml/GMLExporter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/gml/UnsupportedOperation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/gml/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/gml/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.310736 pyutplugins-0.8.70/pyutplugins/ioplugins/java/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    27944 2023-01-20 18:45:21.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/java/JavaReader.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11156 2023-02-01 01:52:43.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/java/JavaWriter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/java/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/java/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.311480 pyutplugins-0.8.70/pyutplugins/ioplugins/mermaid/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      994 2023-02-01 20:38:32.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/mermaid/MermaidDirection.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12464 2023-04-17 23:17:22.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/mermaid/MermaidWriter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-30 01:49:48.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/mermaid/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/mermaid/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.312294 pyutplugins-0.8.70/pyutplugins/ioplugins/pdf/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      132 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/pdf/ImageFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      554 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/pdf/ImageOptions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9553 2023-01-20 18:33:44.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/pdf/OglToPyUmlDefinition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/pdf/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/pdf/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.314039 pyutplugins-0.8.70/pyutplugins/ioplugins/python/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6135 2023-05-05 01:14:03.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/python/DlgSelectMultiplePackages.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3579 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/python/Python3LexerBase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      192 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/python/Python3ParserBase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/python/PythonParseException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12836 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/python/PyutPythonVisitor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12487 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/python/PyutToPython.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    18319 2023-05-05 01:14:03.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/python/ReverseEngineerPython2.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/python/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/python/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.315807 pyutplugins-0.8.70/pyutplugins/ioplugins/python/pyantlrparser/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    47673 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/python/pyantlrparser/Python3Lexer.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)   399206 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/python/pyantlrparser/Python3Parser.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    37475 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserListener.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    22412 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserVisitor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/python/pyantlrparser/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      804 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/python/transformGrammar.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.316347 pyutplugins-0.8.70/pyutplugins/ioplugins/wximage/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4853 2023-05-05 01:14:03.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      929 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/wximage/WxImageFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/wximage/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/ioplugins/wximage/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.317345 pyutplugins-0.8.70/pyutplugins/plugininterfaces/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11797 2023-05-03 19:43:51.000000 pyutplugins-0.8.70/pyutplugins/plugininterfaces/BasePluginInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5202 2023-01-20 21:59:06.000000 pyutplugins-0.8.70/pyutplugins/plugininterfaces/IOPluginInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1226 2023-01-20 15:37:30.000000 pyutplugins-0.8.70/pyutplugins/plugininterfaces/ToolPluginInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/plugininterfaces/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/plugininterfaces/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.319616 pyutplugins-0.8.70/pyutplugins/plugintypes/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2131 2023-02-03 02:56:53.000000 pyutplugins-0.8.70/pyutplugins/plugintypes/BaseFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      112 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/plugintypes/BaseRequestResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      225 2023-01-20 18:45:20.000000 pyutplugins-0.8.70/pyutplugins/plugintypes/ExportDirectoryResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      205 2023-01-20 18:45:20.000000 pyutplugins-0.8.70/pyutplugins/plugintypes/ImportDirectoryResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      532 2023-01-20 18:45:20.000000 pyutplugins-0.8.70/pyutplugins/plugintypes/InputFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      330 2023-01-20 18:45:21.000000 pyutplugins-0.8.70/pyutplugins/plugintypes/MultipleFileRequestResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      533 2023-01-20 18:45:20.000000 pyutplugins-0.8.70/pyutplugins/plugintypes/OutputFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1766 2023-01-20 18:45:20.000000 pyutplugins-0.8.70/pyutplugins/plugintypes/PluginDataTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      202 2023-01-20 18:45:21.000000 pyutplugins-0.8.70/pyutplugins/plugintypes/SingleFileRequestResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/plugintypes/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/plugintypes/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.320073 pyutplugins-0.8.70/pyutplugins/preferences/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7651 2023-03-31 00:30:24.000000 pyutplugins-0.8.70/pyutplugins/preferences/PluginPreferences.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-18 02:02:54.000000 pyutplugins-0.8.70/pyutplugins/preferences/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyutplugins-0.8.70/pyutplugins/preferences/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.321384 pyutplugins-0.8.70/pyutplugins/toolplugins/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1730 2023-01-20 18:45:20.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/ToolArrangeLinks.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3592 2023-01-20 18:45:20.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/ToolAscii.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4402 2023-01-20 18:45:21.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3159 2023-01-20 18:45:20.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/ToolSugiyama.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1989 2023-01-20 18:45:20.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/ToolTransforms.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.322628 pyutplugins-0.8.70/pyutplugins/toolplugins/orthogonal/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1996 2023-05-03 19:43:51.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      737 2023-01-19 03:33:52.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5230 2023-01-20 18:33:44.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/orthogonal/OrthogonalAdapterException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/orthogonal/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/orthogonal/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.324999 pyutplugins-0.8.70/pyutplugins/toolplugins/sugiyama/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3545 2023-02-22 02:39:48.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/sugiyama/ALayoutLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1025 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/sugiyama/ALayoutNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3262 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    28462 2023-02-01 01:51:21.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/sugiyama/Sugiyama.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      263 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/sugiyama/SugiyamaConstants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2108 2023-01-20 15:25:55.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3228 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14778 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1387 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/sugiyama/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.70/pyutplugins/toolplugins/sugiyama/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-08 19:04:56.302814 pyutplugins-0.8.70/pyutplugins.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2311 2023-05-08 19:04:56.000000 pyutplugins-0.8.70/pyutplugins.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5161 2023-05-08 19:04:56.000000 pyutplugins-0.8.70/pyutplugins.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-05-08 19:04:56.000000 pyutplugins-0.8.70/pyutplugins.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      203 2023-05-08 19:04:56.000000 pyutplugins-0.8.70/pyutplugins.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-05-08 19:04:56.000000 pyutplugins-0.8.70/pyutplugins.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-05-08 19:04:56.325355 pyutplugins-0.8.70/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3207 2023-05-08 18:54:05.000000 pyutplugins-0.8.70/setup.py
```

### Comparing `pyutplugins-0.8.60/LICENSE` & `pyutplugins-0.8.70/LICENSE`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/PKG-INFO` & `pyutplugins-0.8.70/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutplugins
-Version: 0.8.60
+Version: 0.8.70
 Summary: Pyut Plugins
 Home-page: https://github.com/hasii2011/pyutplugins
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyutplugins Version: 0.8.60 Summary: Pyut Plugins
+Metadata-Version: 2.1 Name: pyutplugins Version: 0.8.70 Summary: Pyut Plugins
 Home-page: https://github.com/hasii2011/pyutplugins Author: Humberto A. Sanchez
 II Author-email: humberto.a.sanchez.ii@gmail.com Maintainer: Humberto A.
 Sanchez II Maintainer-email: humberto.a.sanchez.ii@gmail.com Description-
 Content-Type: text/markdown License-File: LICENSE [./developer/agpl-license-
 web-badge-version-2-256x48.png] [![Maintenance](https://img.shields.io/badge/
 Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/
 commit-activity) [![CircleCI](https://dl.circleci.com/status-badge/img/gh/
```

### Comparing `pyutplugins-0.8.60/README.md` & `pyutplugins-0.8.70/README.md`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ExternalTypes.py` & `pyutplugins-0.8.70/pyutplugins/ExternalTypes.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/IPluginAdapter.py` & `pyutplugins-0.8.70/pyutplugins/IPluginAdapter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/PluginManager.py` & `pyutplugins-0.8.70/pyutplugins/PluginManager.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/common/ElementTreeData.py` & `pyutplugins-0.8.70/pyutplugins/common/ElementTreeData.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/common/LinkMakerMixin.py` & `pyutplugins-0.8.70/pyutplugins/common/LinkMakerMixin.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/common/ui/BaseEditDialog.py` & `pyutplugins-0.8.70/pyutplugins/common/ui/BaseEditDialog.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/common/ui/preferences/PluginPreferencesPage.py` & `pyutplugins-0.8.70/pyutplugins/common/ui/preferences/PluginPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/IOAscii.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/IOAscii.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/IODTD.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/IODTD.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/IOGML.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/IOGML.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/IOJava.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/IOJava.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/IOMermaid.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/IOMermaid.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/IOPdf.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/IOPdf.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/IOPython.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/IOPython.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/IOWxImage.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/IOWxImage.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/IOXml.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/IOXml.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/dtd/DTDParser.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/dtd/DTDParser.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/gml/GMLExporter.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/gml/GMLExporter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/java/JavaReader.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/java/JavaReader.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/java/JavaWriter.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/java/JavaWriter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/mermaid/MermaidDirection.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/mermaid/MermaidDirection.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/mermaid/MermaidWriter.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/mermaid/MermaidWriter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/pdf/ImageOptions.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/pdf/ImageOptions.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/pdf/OglToPyUmlDefinition.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/pdf/OglToPyUmlDefinition.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/python/DlgSelectMultiplePackages.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/python/DlgSelectMultiplePackages.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/python/Python3LexerBase.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/python/Python3LexerBase.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/python/PyutPythonVisitor.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/python/PyutPythonVisitor.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/python/PyutToPython.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/python/PyutToPython.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/python/ReverseEngineerPython2.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/python/ReverseEngineerPython2.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/python/pyantlrparser/Python3Lexer.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/python/pyantlrparser/Python3Lexer.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/python/pyantlrparser/Python3Parser.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/python/pyantlrparser/Python3Parser.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserListener.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserListener.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserVisitor.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserVisitor.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/python/transformGrammar.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/python/transformGrammar.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/ioplugins/wximage/WxImageFormat.py` & `pyutplugins-0.8.70/pyutplugins/ioplugins/wximage/WxImageFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/plugininterfaces/BasePluginInterface.py` & `pyutplugins-0.8.70/pyutplugins/plugininterfaces/BasePluginInterface.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/plugininterfaces/IOPluginInterface.py` & `pyutplugins-0.8.70/pyutplugins/plugininterfaces/IOPluginInterface.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/plugininterfaces/ToolPluginInterface.py` & `pyutplugins-0.8.70/pyutplugins/plugininterfaces/ToolPluginInterface.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/plugintypes/BaseFormat.py` & `pyutplugins-0.8.70/pyutplugins/plugintypes/BaseFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/plugintypes/InputFormat.py` & `pyutplugins-0.8.70/pyutplugins/plugintypes/InputFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/plugintypes/OutputFormat.py` & `pyutplugins-0.8.70/pyutplugins/plugintypes/OutputFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/plugintypes/PluginDataTypes.py` & `pyutplugins-0.8.70/pyutplugins/plugintypes/PluginDataTypes.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/preferences/PluginPreferences.py` & `pyutplugins-0.8.70/pyutplugins/preferences/PluginPreferences.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/toolplugins/ToolArrangeLinks.py` & `pyutplugins-0.8.70/pyutplugins/toolplugins/ToolArrangeLinks.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/toolplugins/ToolAscii.py` & `pyutplugins-0.8.70/pyutplugins/toolplugins/ToolAscii.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py` & `pyutplugins-0.8.70/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/toolplugins/ToolSugiyama.py` & `pyutplugins-0.8.70/pyutplugins/toolplugins/ToolSugiyama.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/toolplugins/ToolTransforms.py` & `pyutplugins-0.8.70/pyutplugins/toolplugins/ToolTransforms.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py` & `pyutplugins-0.8.70/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py` & `pyutplugins-0.8.70/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py` & `pyutplugins-0.8.70/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/ALayoutLink.py` & `pyutplugins-0.8.70/pyutplugins/toolplugins/sugiyama/ALayoutLink.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/ALayoutNode.py` & `pyutplugins-0.8.70/pyutplugins/toolplugins/sugiyama/ALayoutNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py` & `pyutplugins-0.8.70/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/Sugiyama.py` & `pyutplugins-0.8.70/pyutplugins/toolplugins/sugiyama/Sugiyama.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py` & `pyutplugins-0.8.70/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py` & `pyutplugins-0.8.70/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py` & `pyutplugins-0.8.70/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py` & `pyutplugins-0.8.70/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/pyutplugins.egg-info/PKG-INFO` & `pyutplugins-0.8.70/pyutplugins.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutplugins
-Version: 0.8.60
+Version: 0.8.70
 Summary: Pyut Plugins
 Home-page: https://github.com/hasii2011/pyutplugins
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyutplugins Version: 0.8.60 Summary: Pyut Plugins
+Metadata-Version: 2.1 Name: pyutplugins Version: 0.8.70 Summary: Pyut Plugins
 Home-page: https://github.com/hasii2011/pyutplugins Author: Humberto A. Sanchez
 II Author-email: humberto.a.sanchez.ii@gmail.com Maintainer: Humberto A.
 Sanchez II Maintainer-email: humberto.a.sanchez.ii@gmail.com Description-
 Content-Type: text/markdown License-File: LICENSE [./developer/agpl-license-
 web-badge-version-2-256x48.png] [![Maintenance](https://img.shields.io/badge/
 Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/
 commit-activity) [![CircleCI](https://dl.circleci.com/status-badge/img/gh/
```

### Comparing `pyutplugins-0.8.60/pyutplugins.egg-info/SOURCES.txt` & `pyutplugins-0.8.70/pyutplugins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.60/setup.py` & `pyutplugins-0.8.70/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 LICENSE = (HERE / 'LICENSE').read_text()
 
 setup(
     name="pyutplugins",
-    version="0.8.60",
+    version="0.8.70",
     author='Humberto A. Sanchez II',
     author_email='humberto.a.sanchez.ii@gmail.com',
     maintainer='Humberto A. Sanchez II',
     maintainer_email='humberto.a.sanchez.ii@gmail.com',
     description='Pyut Plugins',
     long_description=README,
     long_description_content_type="text/markdown",
@@ -59,11 +59,11 @@
                       'networkx==3.0',
                       'orthogonal==1.1.8',
                       'wxPython~=4.2.0',
                       'hasiihelper~=0.2.0',
                       'hasiicommon~=0.2.2',
                       'pyutmodel==1.4.3',
                       'ogl==0.70.26',
-                      'untanglepyut==0.6.56',
-                      'oglio==0.7.2',
+                      'untanglepyut==0.6.58',
+                      'oglio==0.7.3',
                       ]
 )
```

