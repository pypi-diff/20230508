# Comparing `tmp/smda-1.9.8.tar.gz` & `tmp/smda-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smda-1.9.8.tar", last modified: Tue Aug 30 11:53:01 2022, max compression
+gzip compressed data, was "smda-1.9.9.tar", last modified: Wed Aug 31 13:29:38 2022, max compression
```

## Comparing `smda-1.9.8.tar` & `smda-1.9.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-08-30 11:53:01.708990 smda-1.9.8/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1311 2020-04-29 08:21:45.000000 smda-1.9.8/LICENSE
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6720 2022-08-30 11:53:01.708990 smda-1.9.8/PKG-INFO
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     5332 2022-08-30 11:52:26.000000 smda-1.9.8/README.md
--rw-rw-r--   0 pnx       (1000) pnx       (1000)       38 2022-08-30 11:53:01.708990 smda-1.9.8/setup.cfg
--rwxrwxr-x   0 pnx       (1000) pnx       (1000)     1290 2022-08-30 11:52:14.000000 smda-1.9.8/setup.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-08-30 11:53:01.444995 smda-1.9.8/smda/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     4986 2021-08-20 08:00:19.000000 smda-1.9.8/smda/Disassembler.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10783 2022-01-27 10:16:44.000000 smda-1.9.8/smda/DisassemblyResult.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     4125 2020-09-03 13:50:44.000000 smda-1.9.8/smda/DisassemblyStatistics.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1367 2022-08-30 11:52:18.000000 smda-1.9.8/smda/SmdaConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)       24 2018-07-01 10:56:42.000000 smda-1.9.8/smda/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-08-30 11:53:01.564993 smda-1.9.8/smda/common/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      346 2018-08-01 08:20:46.000000 smda-1.9.8/smda/common/BasicBlock.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2543 2022-08-22 09:10:18.000000 smda-1.9.8/smda/common/BinaryInfo.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      856 2022-01-27 09:03:22.000000 smda-1.9.8/smda/common/CodeXref.py
--rw-r--r--   0 pnx       (1000) pnx       (1000)     6353 2020-10-31 18:30:40.000000 smda-1.9.8/smda/common/DominatorTree.py
--rw-r--r--   0 pnx       (1000) pnx       (1000)     1112 2020-10-26 20:05:00.000000 smda-1.9.8/smda/common/SmdaBasicBlock.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10019 2022-08-04 06:53:55.000000 smda-1.9.8/smda/common/SmdaFunction.py
--rw-r--r--   0 pnx       (1000) pnx       (1000)     2999 2020-10-27 21:33:20.000000 smda-1.9.8/smda/common/SmdaInstruction.py
--rw-r--r--   0 pnx       (1000) pnx       (1000)    11515 2022-07-22 21:06:41.000000 smda-1.9.8/smda/common/SmdaReport.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6056 2020-05-01 11:23:35.000000 smda-1.9.8/smda/common/TailcallAnalyzer.py
--rw-r--r--   0 pnx       (1000) pnx       (1000)     2843 2020-05-26 14:37:36.000000 smda-1.9.8/smda/common/Tarjan.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)       24 2018-07-01 10:56:42.000000 smda-1.9.8/smda/common/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-08-30 11:53:01.576993 smda-1.9.8/smda/common/labelprovider/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1321 2020-05-01 10:53:58.000000 smda-1.9.8/smda/common/labelprovider/AbstractLabelProvider.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3853 2022-08-23 08:09:13.000000 smda-1.9.8/smda/common/labelprovider/DelphiKbSymbolProvider.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2474 2021-08-19 04:49:28.000000 smda-1.9.8/smda/common/labelprovider/ElfApiResolver.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2255 2021-05-20 09:55:33.000000 smda-1.9.8/smda/common/labelprovider/ElfSymbolProvider.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     7283 2022-08-12 09:08:04.000000 smda-1.9.8/smda/common/labelprovider/GoLabelProvider.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1390 2018-09-18 19:15:38.000000 smda-1.9.8/smda/common/labelprovider/OrdinalHelper.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2745 2020-10-31 18:31:47.000000 smda-1.9.8/smda/common/labelprovider/PdbSymbolProvider.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3886 2021-08-19 04:49:28.000000 smda-1.9.8/smda/common/labelprovider/WinApiResolver.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2018-12-17 09:29:59.000000 smda-1.9.8/smda/common/labelprovider/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-08-30 11:53:01.620992 smda-1.9.8/smda/ida/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      815 2020-05-01 11:12:54.000000 smda-1.9.8/smda/ida/BackendInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     4323 2021-01-16 19:24:11.000000 smda-1.9.8/smda/ida/IdaExporter.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     9634 2022-08-03 08:01:49.000000 smda-1.9.8/smda/ida/IdaInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2019-08-19 15:44:21.000000 smda-1.9.8/smda/ida/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-08-30 11:53:01.636992 smda-1.9.8/smda/intel/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2430 2021-08-24 10:31:54.000000 smda-1.9.8/smda/intel/BitnessAnalyzer.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    11242 2022-08-29 14:02:04.000000 smda-1.9.8/smda/intel/FunctionAnalysisState.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     7348 2020-10-29 21:47:56.000000 smda-1.9.8/smda/intel/FunctionCandidate.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    29587 2022-08-29 10:56:57.000000 smda-1.9.8/smda/intel/FunctionCandidateManager.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     7656 2021-08-19 04:49:28.000000 smda-1.9.8/smda/intel/IndirectCallAnalyzer.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    27082 2022-08-30 11:52:01.000000 smda-1.9.8/smda/intel/IntelDisassembler.py
--rw-r--r--   0 pnx       (1000) pnx       (1000)    21131 2022-08-22 11:40:17.000000 smda-1.9.8/smda/intel/IntelInstructionEscaper.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10988 2021-01-20 08:52:50.000000 smda-1.9.8/smda/intel/JumpTableAnalyzer.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    11755 2022-08-22 09:58:52.000000 smda-1.9.8/smda/intel/LanguageAnalyzer.py
--rw-r--r--   0 pnx       (1000) pnx       (1000)    17733 2020-05-01 11:00:35.000000 smda-1.9.8/smda/intel/MnemonicTfIdf.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)       24 2018-07-01 10:56:42.000000 smda-1.9.8/smda/intel/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     7616 2021-08-24 10:31:54.000000 smda-1.9.8/smda/intel/definitions.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-08-30 11:53:01.708990 smda-1.9.8/smda/utility/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      579 2022-08-22 11:21:35.000000 smda-1.9.8/smda/utility/DelphiKbFileLoader.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     7451 2022-08-23 08:29:52.000000 smda-1.9.8/smda/utility/ElfFileLoader.py
--rw-r--r--   0 pnx       (1000) pnx       (1000)     1791 2022-08-22 11:21:57.000000 smda-1.9.8/smda/utility/FileLoader.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     7669 2022-08-12 09:14:49.000000 smda-1.9.8/smda/utility/MachoFileLoader.py
--rw-r--r--   0 pnx       (1000) pnx       (1000)      253 2021-01-16 17:57:55.000000 smda-1.9.8/smda/utility/MemoryFileLoader.py
--rw-r--r--   0 pnx       (1000) pnx       (1000)     6815 2021-05-20 09:55:02.000000 smda-1.9.8/smda/utility/PeFileLoader.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      852 2020-05-01 11:14:03.000000 smda-1.9.8/smda/utility/PriorityQueue.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)       24 2018-07-01 10:56:42.000000 smda-1.9.8/smda/utility/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-08-30 11:53:01.444995 smda-1.9.8/smda.egg-info/
--rw-r--r--   0 pnx       (1000) pnx       (1000)     6720 2022-08-30 11:53:01.000000 smda-1.9.8/smda.egg-info/PKG-INFO
--rw-r--r--   0 pnx       (1000) pnx       (1000)     1709 2022-08-30 11:53:01.000000 smda-1.9.8/smda.egg-info/SOURCES.txt
--rw-r--r--   0 pnx       (1000) pnx       (1000)        1 2022-08-30 11:53:01.000000 smda-1.9.8/smda.egg-info/dependency_links.txt
--rw-r--r--   0 pnx       (1000) pnx       (1000)       20 2022-08-30 11:53:01.000000 smda-1.9.8/smda.egg-info/requires.txt
--rw-r--r--   0 pnx       (1000) pnx       (1000)        5 2022-08-30 11:53:01.000000 smda-1.9.8/smda.egg-info/top_level.txt
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-08-31 13:29:38.072929 smda-1.9.9/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1311 2020-04-29 08:21:45.000000 smda-1.9.9/LICENSE
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6804 2022-08-31 13:29:38.072929 smda-1.9.9/PKG-INFO
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     5408 2022-08-31 13:28:11.000000 smda-1.9.9/README.md
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)       38 2022-08-31 13:29:38.072929 smda-1.9.9/setup.cfg
+-rwxrwxr-x   0 pnx       (1000) pnx       (1000)     1290 2022-08-31 13:27:26.000000 smda-1.9.9/setup.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-08-31 13:29:38.068929 smda-1.9.9/smda/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     4986 2021-08-20 08:00:19.000000 smda-1.9.9/smda/Disassembler.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    10783 2022-01-27 10:16:44.000000 smda-1.9.9/smda/DisassemblyResult.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     4125 2020-09-03 13:50:44.000000 smda-1.9.9/smda/DisassemblyStatistics.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1367 2022-08-31 13:27:31.000000 smda-1.9.9/smda/SmdaConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)       24 2018-07-01 10:56:42.000000 smda-1.9.9/smda/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-08-31 13:29:38.068929 smda-1.9.9/smda/common/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      346 2018-08-01 08:20:46.000000 smda-1.9.9/smda/common/BasicBlock.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2543 2022-08-22 09:10:18.000000 smda-1.9.9/smda/common/BinaryInfo.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      856 2022-01-27 09:03:22.000000 smda-1.9.9/smda/common/CodeXref.py
+-rw-r--r--   0 pnx       (1000) pnx       (1000)     6353 2020-10-31 18:30:40.000000 smda-1.9.9/smda/common/DominatorTree.py
+-rw-r--r--   0 pnx       (1000) pnx       (1000)     1112 2020-10-26 20:05:00.000000 smda-1.9.9/smda/common/SmdaBasicBlock.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    10019 2022-08-04 06:53:55.000000 smda-1.9.9/smda/common/SmdaFunction.py
+-rw-r--r--   0 pnx       (1000) pnx       (1000)     2999 2020-10-27 21:33:20.000000 smda-1.9.9/smda/common/SmdaInstruction.py
+-rw-r--r--   0 pnx       (1000) pnx       (1000)    11515 2022-07-22 21:06:41.000000 smda-1.9.9/smda/common/SmdaReport.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6056 2020-05-01 11:23:35.000000 smda-1.9.9/smda/common/TailcallAnalyzer.py
+-rw-r--r--   0 pnx       (1000) pnx       (1000)     2843 2020-05-26 14:37:36.000000 smda-1.9.9/smda/common/Tarjan.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)       24 2018-07-01 10:56:42.000000 smda-1.9.9/smda/common/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-08-31 13:29:38.072929 smda-1.9.9/smda/common/labelprovider/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1321 2020-05-01 10:53:58.000000 smda-1.9.9/smda/common/labelprovider/AbstractLabelProvider.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3853 2022-08-23 08:09:13.000000 smda-1.9.9/smda/common/labelprovider/DelphiKbSymbolProvider.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2474 2021-08-19 04:49:28.000000 smda-1.9.9/smda/common/labelprovider/ElfApiResolver.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2255 2021-05-20 09:55:33.000000 smda-1.9.9/smda/common/labelprovider/ElfSymbolProvider.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     7283 2022-08-12 09:08:04.000000 smda-1.9.9/smda/common/labelprovider/GoLabelProvider.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1390 2018-09-18 19:15:38.000000 smda-1.9.9/smda/common/labelprovider/OrdinalHelper.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2745 2020-10-31 18:31:47.000000 smda-1.9.9/smda/common/labelprovider/PdbSymbolProvider.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3886 2021-08-19 04:49:28.000000 smda-1.9.9/smda/common/labelprovider/WinApiResolver.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2018-12-17 09:29:59.000000 smda-1.9.9/smda/common/labelprovider/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-08-31 13:29:38.072929 smda-1.9.9/smda/ida/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      815 2020-05-01 11:12:54.000000 smda-1.9.9/smda/ida/BackendInterface.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     4323 2021-01-16 19:24:11.000000 smda-1.9.9/smda/ida/IdaExporter.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     9634 2022-08-03 08:01:49.000000 smda-1.9.9/smda/ida/IdaInterface.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2019-08-19 15:44:21.000000 smda-1.9.9/smda/ida/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-08-31 13:29:38.072929 smda-1.9.9/smda/intel/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2430 2021-08-24 10:31:54.000000 smda-1.9.9/smda/intel/BitnessAnalyzer.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    11730 2022-08-31 13:20:41.000000 smda-1.9.9/smda/intel/FunctionAnalysisState.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     7348 2020-10-29 21:47:56.000000 smda-1.9.9/smda/intel/FunctionCandidate.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    29587 2022-08-29 10:56:57.000000 smda-1.9.9/smda/intel/FunctionCandidateManager.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     7656 2021-08-19 04:49:28.000000 smda-1.9.9/smda/intel/IndirectCallAnalyzer.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    27087 2022-08-31 13:20:31.000000 smda-1.9.9/smda/intel/IntelDisassembler.py
+-rw-r--r--   0 pnx       (1000) pnx       (1000)    21131 2022-08-22 11:40:17.000000 smda-1.9.9/smda/intel/IntelInstructionEscaper.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    10988 2021-01-20 08:52:50.000000 smda-1.9.9/smda/intel/JumpTableAnalyzer.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    11755 2022-08-22 09:58:52.000000 smda-1.9.9/smda/intel/LanguageAnalyzer.py
+-rw-r--r--   0 pnx       (1000) pnx       (1000)    17733 2020-05-01 11:00:35.000000 smda-1.9.9/smda/intel/MnemonicTfIdf.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)       24 2018-07-01 10:56:42.000000 smda-1.9.9/smda/intel/__init__.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     7616 2021-08-24 10:31:54.000000 smda-1.9.9/smda/intel/definitions.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-08-31 13:29:38.072929 smda-1.9.9/smda/utility/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      579 2022-08-22 11:21:35.000000 smda-1.9.9/smda/utility/DelphiKbFileLoader.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     7451 2022-08-23 08:29:52.000000 smda-1.9.9/smda/utility/ElfFileLoader.py
+-rw-r--r--   0 pnx       (1000) pnx       (1000)     1791 2022-08-22 11:21:57.000000 smda-1.9.9/smda/utility/FileLoader.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     7669 2022-08-12 09:14:49.000000 smda-1.9.9/smda/utility/MachoFileLoader.py
+-rw-r--r--   0 pnx       (1000) pnx       (1000)      253 2021-01-16 17:57:55.000000 smda-1.9.9/smda/utility/MemoryFileLoader.py
+-rw-r--r--   0 pnx       (1000) pnx       (1000)     6815 2021-05-20 09:55:02.000000 smda-1.9.9/smda/utility/PeFileLoader.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      852 2020-05-01 11:14:03.000000 smda-1.9.9/smda/utility/PriorityQueue.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)       24 2018-07-01 10:56:42.000000 smda-1.9.9/smda/utility/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-08-31 13:29:38.068929 smda-1.9.9/smda.egg-info/
+-rw-r--r--   0 pnx       (1000) pnx       (1000)     6804 2022-08-31 13:29:37.000000 smda-1.9.9/smda.egg-info/PKG-INFO
+-rw-r--r--   0 pnx       (1000) pnx       (1000)     1709 2022-08-31 13:29:37.000000 smda-1.9.9/smda.egg-info/SOURCES.txt
+-rw-r--r--   0 pnx       (1000) pnx       (1000)        1 2022-08-31 13:29:37.000000 smda-1.9.9/smda.egg-info/dependency_links.txt
+-rw-r--r--   0 pnx       (1000) pnx       (1000)       20 2022-08-31 13:29:37.000000 smda-1.9.9/smda.egg-info/requires.txt
+-rw-r--r--   0 pnx       (1000) pnx       (1000)        5 2022-08-31 13:29:37.000000 smda-1.9.9/smda.egg-info/top_level.txt
```

### Comparing `smda-1.9.8/LICENSE` & `smda-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/PKG-INFO` & `smda-1.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smda
-Version: 1.9.8
+Version: 1.9.9
 Summary: A recursive disassmbler optimized for CFG recovery from memory dumps. Based on capstone.
 Home-page: https://github.com/danielplohmann/smda
 Author: Daniel Plohmann
 Author-email: daniel.plohmann@mailbox.org
 License: BSD 2-Clause
 Description: 
         # SMDA
@@ -61,14 +61,15 @@
         
         To take full advantage of SMDA's capabilities, make sure to (optionally) install:
          * lief 
          * pdbparse (currently as fork from https://github.com/VPaulV/pdbparse to support Python3)
         
         ## Version History
         
+         * 2022-08-31: v1.9.9 - Better handling of colliding code due to tailjumps.
          * 2022-08-30: v1.9.8 - Improved accuracy for references around tailcalls.
          * 2022-08-25: v1.9.6 - Fixed bug in delphi knowledge base handling and improved performance.
          * 2022-08-23: v1.9.4 - Fixed bug in section padding for ELF files.
          * 2022-08-22: v1.9.3 - Added parsing for Delphi knowledge base files (THX to @danielenders1!).
          * 2022-08-22: v1.9.2 - Improved structural parsing of Delphi binaries (THX to @danielenders1!).
          * 2022-08-12: v1.9.1 - Added support for parsing intel MachO files, including Go parsing.
          * 2022-08-01: v1.8.0 - Added support for parsing Go function information (THX to @danielenders1!).
```

### Comparing `smda-1.9.8/README.md` & `smda-1.9.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
 To take full advantage of SMDA's capabilities, make sure to (optionally) install:
  * lief 
  * pdbparse (currently as fork from https://github.com/VPaulV/pdbparse to support Python3)
 
 ## Version History
 
+ * 2022-08-31: v1.9.9 - Better handling of colliding code due to tailjumps.
  * 2022-08-30: v1.9.8 - Improved accuracy for references around tailcalls.
  * 2022-08-25: v1.9.6 - Fixed bug in delphi knowledge base handling and improved performance.
  * 2022-08-23: v1.9.4 - Fixed bug in section padding for ELF files.
  * 2022-08-22: v1.9.3 - Added parsing for Delphi knowledge base files (THX to @danielenders1!).
  * 2022-08-22: v1.9.2 - Improved structural parsing of Delphi binaries (THX to @danielenders1!).
  * 2022-08-12: v1.9.1 - Added support for parsing intel MachO files, including Go parsing.
  * 2022-08-01: v1.8.0 - Added support for parsing Go function information (THX to @danielenders1!).
```

### Comparing `smda-1.9.8/setup.py` & `smda-1.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     # py2 - newer LIEF is Python3 only
     requirements.append("lief==0.9.0")
 
 
 setup(
     name='smda',
     # note to self: always change this in config as well.
-    version='1.9.8',
+    version='1.9.9',
     description='A recursive disassmbler optimized for CFG recovery from memory dumps. Based on capstone.',
     long_description_content_type="text/markdown",
     long_description=long_description,
     author='Daniel Plohmann',
     author_email='daniel.plohmann@mailbox.org',
     url='https://github.com/danielplohmann/smda',
     license="BSD 2-Clause",
```

### Comparing `smda-1.9.8/smda/Disassembler.py` & `smda-1.9.9/smda/Disassembler.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/DisassemblyResult.py` & `smda-1.9.9/smda/DisassemblyResult.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/DisassemblyStatistics.py` & `smda-1.9.9/smda/DisassemblyStatistics.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/SmdaConfig.py` & `smda-1.9.9/smda/SmdaConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import logging
 
 
 class SmdaConfig(object):
 
     # note to self: always change this in setup.py as well!
-    VERSION = "1.9.8"
+    VERSION = "1.9.9"
     CONFIG_FILE_PATH = str(os.path.abspath(__file__))
     PROJECT_ROOT = str(os.path.abspath(os.sep.join([CONFIG_FILE_PATH, "..", ".."])))
 
     ### An (optional) WinAPI database as generated by ApiScout (https://github.com/danielplohmann/apiscout)
     API_COLLECTION_FILES = {}
     ### global logging-config setup
     # Only do basicConfig if no handlers have been configured
```

### Comparing `smda-1.9.8/smda/common/BinaryInfo.py` & `smda-1.9.9/smda/common/BinaryInfo.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/common/CodeXref.py` & `smda-1.9.9/smda/common/CodeXref.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/common/DominatorTree.py` & `smda-1.9.9/smda/common/DominatorTree.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/common/SmdaBasicBlock.py` & `smda-1.9.9/smda/common/SmdaBasicBlock.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/common/SmdaFunction.py` & `smda-1.9.9/smda/common/SmdaFunction.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/common/SmdaInstruction.py` & `smda-1.9.9/smda/common/SmdaInstruction.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/common/SmdaReport.py` & `smda-1.9.9/smda/common/SmdaReport.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/common/TailcallAnalyzer.py` & `smda-1.9.9/smda/common/TailcallAnalyzer.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/common/Tarjan.py` & `smda-1.9.9/smda/common/Tarjan.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/common/labelprovider/AbstractLabelProvider.py` & `smda-1.9.9/smda/common/labelprovider/AbstractLabelProvider.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/common/labelprovider/DelphiKbSymbolProvider.py` & `smda-1.9.9/smda/common/labelprovider/DelphiKbSymbolProvider.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/common/labelprovider/ElfApiResolver.py` & `smda-1.9.9/smda/common/labelprovider/ElfApiResolver.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/common/labelprovider/ElfSymbolProvider.py` & `smda-1.9.9/smda/common/labelprovider/ElfSymbolProvider.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/common/labelprovider/GoLabelProvider.py` & `smda-1.9.9/smda/common/labelprovider/GoLabelProvider.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/common/labelprovider/OrdinalHelper.py` & `smda-1.9.9/smda/common/labelprovider/OrdinalHelper.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/common/labelprovider/PdbSymbolProvider.py` & `smda-1.9.9/smda/common/labelprovider/PdbSymbolProvider.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/common/labelprovider/WinApiResolver.py` & `smda-1.9.9/smda/common/labelprovider/WinApiResolver.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/ida/BackendInterface.py` & `smda-1.9.9/smda/ida/BackendInterface.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/ida/IdaExporter.py` & `smda-1.9.9/smda/ida/IdaExporter.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/ida/IdaInterface.py` & `smda-1.9.9/smda/ida/IdaInterface.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/intel/BitnessAnalyzer.py` & `smda-1.9.9/smda/intel/BitnessAnalyzer.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/intel/FunctionAnalysisState.py` & `smda-1.9.9/smda/intel/FunctionAnalysisState.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         self.code_refs_to = {}
         self.suspicious_ins_count = 0
         self.is_jmp = False
         self.is_next_instruction_reachable = True
         self.is_block_ending_instruction = False
         self.is_sanely_ending = False
         self.has_collision = False
+        self.colliding_addresses = set()
         # set a flag that this tailcall has already been resolved so it does not have to be reanalyzed several times
         self.is_tailcall_function = False
         self.is_leaf_function = True
         self.is_recursive = False
         self.is_thunk_call = False
         self.label = ""
 
@@ -199,14 +200,19 @@
                 current = self.instructions[i]
                 block.append(current)
                 # if one code reference is to another address than the next
                 if current[0] in self.code_refs_from:
                     if not current[2] in CALL_INS and not i == len(self.instructions) - 1:
                         if any([r != self.instructions[i+1][0] for r in self.code_refs_from[current[0]]]):
                             break
+                    # if we can reach a colliding address from here, the block is broken and should end.
+                    reachable_collisions = self.code_refs_from[current[0]].intersection(self.colliding_addresses)
+                    is_next_addr = current[0] + current[1] in reachable_collisions
+                    if reachable_collisions and is_next_addr:
+                        break
                 if not i == len(self.instructions) - 1 and self.instructions[i+1][0] in self.code_refs_to:
                     if len(self.code_refs_to[self.instructions[i+1][0]]) > 1 or self.instructions[i+1][0] in potential_starts:
                         break
                 if current[2] in END_INS:
                     break
             if block:
                 blocks.append(block)
@@ -236,16 +242,17 @@
 
     def setBlockEndingInstruction(self, is_ending):
         self.is_block_ending_instruction = is_ending
 
     def setSanelyEnding(self, is_sanely_ending):
         self.is_sanely_ending = is_sanely_ending
 
-    def setCollision(self, is_colliding):
-        self.has_collision = is_colliding
+    def addCollision(self, colliding_address):
+        self.has_collision = True
+        self.colliding_addresses.add(colliding_address)
 
     def setRecursion(self, is_recursive):
         self.is_recursive = is_recursive
 
     def setThunkCall(self, is_thunk_call):
         self.is_thunk_call = is_thunk_call
```

### Comparing `smda-1.9.8/smda/intel/FunctionCandidate.py` & `smda-1.9.9/smda/intel/FunctionCandidate.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/intel/FunctionCandidateManager.py` & `smda-1.9.9/smda/intel/FunctionCandidateManager.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/intel/IndirectCallAnalyzer.py` & `smda-1.9.9/smda/intel/IndirectCallAnalyzer.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/intel/IntelDisassembler.py` & `smda-1.9.9/smda/intel/IntelDisassembler.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,15 +374,15 @@
                     previous_op_str = i_op_str
                     if not i_address in self.disassembly.code_map and not i_address in self.disassembly.data_map and not state.isProcessed(i_address):
                         LOGGER.debug("  analyzeFunction() booked instruction @0x%08x: %s for processed state", i_address, i_mnemonic + " " + i_op_str)
                         state.addInstruction(i_address, i_size, i_mnemonic, i_op_str, i_bytes)
                     elif i_address in self.disassembly.code_map:
                         LOGGER.debug("  analyzeFunction() was already present?! instruction @0x%08x: %s (function: 0x%08x)", i_address, i_mnemonic + " " + i_op_str, self.disassembly.ins2fn[i_address])
                         state.setBlockEndingInstruction(True)
-                        state.setCollision(True)
+                        state.addCollision(i_address)
                     else:
                         LOGGER.debug("  analyzeFunction() was already present in local function.")
                         state.setBlockEndingInstruction(True)
                     if state.isBlockEndingInstruction():
                         state.endBlock()
                         break
                 else:
```

### Comparing `smda-1.9.8/smda/intel/IntelInstructionEscaper.py` & `smda-1.9.9/smda/intel/IntelInstructionEscaper.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/intel/JumpTableAnalyzer.py` & `smda-1.9.9/smda/intel/JumpTableAnalyzer.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/intel/LanguageAnalyzer.py` & `smda-1.9.9/smda/intel/LanguageAnalyzer.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/intel/MnemonicTfIdf.py` & `smda-1.9.9/smda/intel/MnemonicTfIdf.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/intel/definitions.py` & `smda-1.9.9/smda/intel/definitions.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/utility/DelphiKbFileLoader.py` & `smda-1.9.9/smda/utility/DelphiKbFileLoader.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/utility/ElfFileLoader.py` & `smda-1.9.9/smda/utility/ElfFileLoader.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/utility/FileLoader.py` & `smda-1.9.9/smda/utility/FileLoader.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/utility/MachoFileLoader.py` & `smda-1.9.9/smda/utility/MachoFileLoader.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/utility/PeFileLoader.py` & `smda-1.9.9/smda/utility/PeFileLoader.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda/utility/PriorityQueue.py` & `smda-1.9.9/smda/utility/PriorityQueue.py`

 * *Files identical despite different names*

### Comparing `smda-1.9.8/smda.egg-info/PKG-INFO` & `smda-1.9.9/smda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smda
-Version: 1.9.8
+Version: 1.9.9
 Summary: A recursive disassmbler optimized for CFG recovery from memory dumps. Based on capstone.
 Home-page: https://github.com/danielplohmann/smda
 Author: Daniel Plohmann
 Author-email: daniel.plohmann@mailbox.org
 License: BSD 2-Clause
 Description: 
         # SMDA
@@ -61,14 +61,15 @@
         
         To take full advantage of SMDA's capabilities, make sure to (optionally) install:
          * lief 
          * pdbparse (currently as fork from https://github.com/VPaulV/pdbparse to support Python3)
         
         ## Version History
         
+         * 2022-08-31: v1.9.9 - Better handling of colliding code due to tailjumps.
          * 2022-08-30: v1.9.8 - Improved accuracy for references around tailcalls.
          * 2022-08-25: v1.9.6 - Fixed bug in delphi knowledge base handling and improved performance.
          * 2022-08-23: v1.9.4 - Fixed bug in section padding for ELF files.
          * 2022-08-22: v1.9.3 - Added parsing for Delphi knowledge base files (THX to @danielenders1!).
          * 2022-08-22: v1.9.2 - Improved structural parsing of Delphi binaries (THX to @danielenders1!).
          * 2022-08-12: v1.9.1 - Added support for parsing intel MachO files, including Go parsing.
          * 2022-08-01: v1.8.0 - Added support for parsing Go function information (THX to @danielenders1!).
```

### Comparing `smda-1.9.8/smda.egg-info/SOURCES.txt` & `smda-1.9.9/smda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

