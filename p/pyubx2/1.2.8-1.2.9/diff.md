# Comparing `tmp/pyubx2-1.2.8.tar.gz` & `tmp/pyubx2-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyubx2-1.2.8.tar", last modified: Thu May  5 06:17:20 2022, max compression
+gzip compressed data, was "pyubx2-1.2.9.tar", last modified: Fri May  6 18:29:55 2022, max compression
```

## Comparing `pyubx2-1.2.8.tar` & `pyubx2-1.2.9.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-05-05 06:17:20.752275 pyubx2-1.2.8/
--rw-r--r--   0 stevensmith   (501) staff       (20)     1613 2021-03-20 08:52:42.000000 pyubx2-1.2.8/LICENSE
--rw-r--r--   0 stevensmith   (501) staff       (20)       64 2021-03-20 08:52:42.000000 pyubx2-1.2.8/MANIFEST.in
--rw-r--r--   0 stevensmith   (501) staff       (20)    24997 2022-05-05 06:17:20.751852 pyubx2-1.2.8/PKG-INFO
--rw-r--r--   0 stevensmith   (501) staff       (20)    23896 2022-04-24 17:37:30.000000 pyubx2-1.2.8/README.md
-drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-05-05 06:17:20.748187 pyubx2-1.2.8/pyubx2/
--rw-r--r--   0 stevensmith   (501) staff       (20)      677 2022-05-05 05:22:56.000000 pyubx2-1.2.8/pyubx2/__init__.py
--rw-r--r--   0 stevensmith   (501) staff       (20)      161 2022-05-05 06:11:36.000000 pyubx2-1.2.8/pyubx2/_version.py
--rw-r--r--   0 stevensmith   (501) staff       (20)      801 2022-01-18 11:12:50.000000 pyubx2-1.2.8/pyubx2/exceptions.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    11163 2022-04-24 17:37:30.000000 pyubx2-1.2.8/pyubx2/ubxhelpers.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    37613 2022-04-24 17:37:30.000000 pyubx2-1.2.8/pyubx2/ubxmessage.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    14197 2022-05-05 05:22:56.000000 pyubx2-1.2.8/pyubx2/ubxreader.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    62224 2022-01-07 08:36:43.000000 pyubx2-1.2.8/pyubx2/ubxtypes_configdb.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    17540 2022-05-05 06:10:04.000000 pyubx2-1.2.8/pyubx2/ubxtypes_core.py
--rw-r--r--   0 stevensmith   (501) staff       (20)   102234 2022-05-05 06:10:55.000000 pyubx2-1.2.8/pyubx2/ubxtypes_get.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     5151 2022-05-05 06:10:04.000000 pyubx2-1.2.8/pyubx2/ubxtypes_poll.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    25629 2022-04-24 17:37:30.000000 pyubx2-1.2.8/pyubx2/ubxtypes_set.py
-drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-05-05 06:17:20.750167 pyubx2-1.2.8/pyubx2.egg-info/
--rw-r--r--   0 stevensmith   (501) staff       (20)    24997 2022-05-05 06:17:20.000000 pyubx2-1.2.8/pyubx2.egg-info/PKG-INFO
--rw-r--r--   0 stevensmith   (501) staff       (20)      532 2022-05-05 06:17:20.000000 pyubx2-1.2.8/pyubx2.egg-info/SOURCES.txt
--rw-r--r--   0 stevensmith   (501) staff       (20)        1 2022-05-05 06:17:20.000000 pyubx2-1.2.8/pyubx2.egg-info/dependency_links.txt
--rw-r--r--   0 stevensmith   (501) staff       (20)       54 2022-05-05 06:17:20.000000 pyubx2-1.2.8/pyubx2.egg-info/entry_points.txt
--rw-r--r--   0 stevensmith   (501) staff       (20)       46 2022-05-05 06:17:20.000000 pyubx2-1.2.8/pyubx2.egg-info/requires.txt
--rw-r--r--   0 stevensmith   (501) staff       (20)       17 2022-05-05 06:17:20.000000 pyubx2-1.2.8/pyubx2.egg-info/top_level.txt
-drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-05-05 06:17:20.751233 pyubx2-1.2.8/pyubx2cli/
--rw-r--r--   0 stevensmith   (501) staff       (20)      357 2022-01-18 11:12:50.000000 pyubx2-1.2.8/pyubx2cli/__init__.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    12383 2022-04-24 17:37:30.000000 pyubx2-1.2.8/pyubx2cli/gnssdump.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     2472 2022-04-24 17:37:30.000000 pyubx2-1.2.8/pyubx2cli/helpstrings.py
--rw-r--r--   0 stevensmith   (501) staff       (20)       38 2022-05-05 06:17:20.752368 pyubx2-1.2.8/setup.cfg
--rw-r--r--   0 stevensmith   (501) staff       (20)     2144 2022-05-01 07:18:40.000000 pyubx2-1.2.8/setup.py
+drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-05-06 18:29:55.030051 pyubx2-1.2.9/
+-rw-r--r--   0 stevensmith   (501) staff       (20)     1613 2021-03-20 08:52:42.000000 pyubx2-1.2.9/LICENSE
+-rw-r--r--   0 stevensmith   (501) staff       (20)       64 2021-03-20 08:52:42.000000 pyubx2-1.2.9/MANIFEST.in
+-rw-r--r--   0 stevensmith   (501) staff       (20)    26844 2022-05-06 18:29:55.029704 pyubx2-1.2.9/PKG-INFO
+-rw-r--r--   0 stevensmith   (501) staff       (20)    25772 2022-05-06 18:24:52.000000 pyubx2-1.2.9/README.md
+drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-05-06 18:29:55.026092 pyubx2-1.2.9/pyubx2/
+-rw-r--r--   0 stevensmith   (501) staff       (20)      724 2022-05-06 18:19:21.000000 pyubx2-1.2.9/pyubx2/__init__.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)      161 2022-05-06 18:23:48.000000 pyubx2-1.2.9/pyubx2/_version.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)      801 2022-01-18 11:12:50.000000 pyubx2-1.2.9/pyubx2/exceptions.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     2477 2022-05-06 18:19:21.000000 pyubx2-1.2.9/pyubx2/socket_stream.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)    11163 2022-04-24 17:37:30.000000 pyubx2-1.2.9/pyubx2/ubxhelpers.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)    37613 2022-04-24 17:37:30.000000 pyubx2-1.2.9/pyubx2/ubxmessage.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)    14464 2022-05-06 18:19:21.000000 pyubx2-1.2.9/pyubx2/ubxreader.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)    62224 2022-01-07 08:36:43.000000 pyubx2-1.2.9/pyubx2/ubxtypes_configdb.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)    17540 2022-05-06 18:17:43.000000 pyubx2-1.2.9/pyubx2/ubxtypes_core.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)   102234 2022-05-06 18:17:43.000000 pyubx2-1.2.9/pyubx2/ubxtypes_get.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     5151 2022-05-06 18:17:43.000000 pyubx2-1.2.9/pyubx2/ubxtypes_poll.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)    25629 2022-04-24 17:37:30.000000 pyubx2-1.2.9/pyubx2/ubxtypes_set.py
+drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-05-06 18:29:55.028360 pyubx2-1.2.9/pyubx2.egg-info/
+-rw-r--r--   0 stevensmith   (501) staff       (20)    26844 2022-05-06 18:29:54.000000 pyubx2-1.2.9/pyubx2.egg-info/PKG-INFO
+-rw-r--r--   0 stevensmith   (501) staff       (20)      556 2022-05-06 18:29:54.000000 pyubx2-1.2.9/pyubx2.egg-info/SOURCES.txt
+-rw-r--r--   0 stevensmith   (501) staff       (20)        1 2022-05-06 18:29:54.000000 pyubx2-1.2.9/pyubx2.egg-info/dependency_links.txt
+-rw-r--r--   0 stevensmith   (501) staff       (20)       54 2022-05-06 18:29:54.000000 pyubx2-1.2.9/pyubx2.egg-info/entry_points.txt
+-rw-r--r--   0 stevensmith   (501) staff       (20)       46 2022-05-06 18:29:54.000000 pyubx2-1.2.9/pyubx2.egg-info/requires.txt
+-rw-r--r--   0 stevensmith   (501) staff       (20)       17 2022-05-06 18:29:54.000000 pyubx2-1.2.9/pyubx2.egg-info/top_level.txt
+drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-05-06 18:29:55.029212 pyubx2-1.2.9/pyubx2cli/
+-rw-r--r--   0 stevensmith   (501) staff       (20)      357 2022-01-18 11:12:50.000000 pyubx2-1.2.9/pyubx2cli/__init__.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)    12383 2022-04-24 17:37:30.000000 pyubx2-1.2.9/pyubx2cli/gnssdump.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     2472 2022-04-24 17:37:30.000000 pyubx2-1.2.9/pyubx2cli/helpstrings.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)       38 2022-05-06 18:29:55.030157 pyubx2-1.2.9/setup.cfg
+-rw-r--r--   0 stevensmith   (501) staff       (20)     2144 2022-05-01 07:18:40.000000 pyubx2-1.2.9/setup.py
```

### Comparing `pyubx2-1.2.8/LICENSE` & `pyubx2-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyubx2-1.2.8/PKG-INFO` & `pyubx2-1.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyubx2
-Version: 1.2.8
+Version: 1.2.9
 Summary: UBX Protocol Parser
 Home-page: https://github.com/semuconsulting/pyubx2
 Author: semuadmin
 Author-email: semuadmin@semuconsulting.com
 License: BSD 3-Clause 'Modified' License
 Project-URL: Bug Tracker, https://github.com/semuconsulting/pyubx2
 Project-URL: Documentation, https://github.com/semuconsulting/pyubx2
@@ -46,14 +46,15 @@
 [Parsing](#parsing) |
 [Generating](#generating) |
 [Serializing](#serializing) |
 [Configuration Interface](#configinterface) |
 [Examples](#examples) |
 [Extensibility](#extensibility) |
 [Command Line Utility](#cli) |
+[Troubleshooting](#troubleshoot) |
 [Graphical Client](#gui) |
 [Author & License](#author)
 
 `pyubx2` is an original Python 3 parser for the UBX &copy; protocol. UBX is a proprietary binary protocol implemented on u-blox &trade; GNSS/GPS receiver modules.
 
 The `pyubx2` homepage is located at [https://github.com/semuconsulting/pyubx2](https://github.com/semuconsulting/pyubx2).
 
@@ -81,17 +82,17 @@
 
 Sphinx API Documentation in HTML format is available at [https://www.semuconsulting.com/pyubx2](https://www.semuconsulting.com/pyubx2).
 
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyubx2/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pyubx2/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyubx2/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided.
 
-### New in v1.2.7
+### New in v1.2.9
 
-1. `pyubx2` can now parse RTCM3 messages as well as UBX and NMEA.
+1. Ability to read from socket as well as serial or file datastream.
 
 ---
 ## <a name="installation">Installation</a>
 
 `pyubx2` is compatible with Python >=3.7 and has no third-party library dependencies.
 
 In the following, `python` & `pip` refer to the Python 3 executables. You may need to type 
@@ -138,15 +139,15 @@
 
 ```
 class pyubx2.ubxreader.UBXReader(stream, *args, **kwargs)
 ```
 
 You can create a `UBXReader` object by calling the constructor with an active stream object. 
 The stream object can be any data stream which supports a `read(n) -> bytes` method (e.g. File or Serial, with 
-or without a buffer wrapper).
+or without a buffer wrapper). `pyubx2` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams (see example below).
 
 Individual input UBX, NMEA or RTCM3 messages can then be read using the `UBXReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `UBXMessage`, `NMEAMessage` or `RTCMMessage` object, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `UBXReader` also implements an iterator.
 
 The constructor accepts the following optional keyword arguments:
 
 * `protfilter`: 1 = NMEA, 2 = UBX, 4 = RTCM3 (can be OR'd. default is 3 - NMEA & UBX)
 * `quitonerror`: 0 = ignore errors, 1 = log errors and continue (default), 2 = (re)raise errors and terminate
@@ -169,14 +170,25 @@
 >>> from pyubx2 import UBXReader
 >>> stream = open('ubxdata.bin', 'rb')
 >>> ubr = UBXReader(stream, protfilter=2)
 >>> for (raw_data, parsed_data) in ubr: print(parsed_data)
 ...
 ```
 
+Example - Socket input (using enhanced iterator). This will output UBX, NMEA and RTCM3 data:
+```python
+>>> import socket
+>>> from pyubx2 import UBXReader
+>>> stream = socket.socket(socket.AF_INET, socket.SOCK_STREAM):
+>>> stream.connect(("localhost", 50007))
+>>> ubr = UBXReader(stream, protfilter=7)
+>>> for (raw_data, parsed_data) in ubr.iterate(): print(parsed_data)
+...
+```
+
 ---
 ## <a name="parsing">Parsing</a>
 
 You can parse individual UBX messages using the static `UBXReader.parse(data)` function, which takes a bytes array containing a binary UBX message and returns a `UBXMessage` object.
 
 **NB:** Once instantiated, a `UBXMessage` object is immutable.
 
@@ -397,14 +409,15 @@
 
 1. `ubxoptions.py` illustrates the various options available for parsing and constructing UBX messages.
 1. `ubxpoller.py` illustrates how to implement a simple threaded configuration polling utility for UBX messages. 
 1. `ubxsetrates.py` illustrates how to use legacy configuration messages (CFG-MSG) to set navigation message rates.
 1. `ubxconfigdb.py` illustrates how to invoke the Generation 9 configuration database interface via CFG-VALSET, CF-VALDEL and CFG-VALGET messages.
 1. `ubxfactoryreset.py` illustrates how to send a factory reset (CFG-CFG) command.
 1. `ubxfile.py` illustrates how to implement a binary file reader for UBX messages using `UBXReader` iterator functionality. 
+1. `ubxsocket.py` illustrates how to implement a TCP Socket reader for UBX messages using `UBXReader` iterator functionality. Can be used in conjunction with the `tcpserver_threaded.py` socket server test harness.
 1. `gpxtracker.py` illustrates a simple tool to convert a binary UBX data dump to a `*.gpx` track file.
 1. `ubxserver.py` in the \examples\webserver folder illustrates a simple HTTP web server wrapper around `pyubx2.UBXreader`; it presents data from selected UBX messages as a web page http://localhost:8080 or a RESTful API http://localhost:8080/gps.
 1. `benchmark.py` provides a simple performance benchmarking tool for the `pyubx2` parser.
 
 ---
 ## <a name="extensibility">Extensibility</a>
 
@@ -482,14 +495,30 @@
 The `gnssdump` utility implements a new `GNSSStreamer` class which may be used directly within Python application code via:
 
 ```python
 >>> from pyubx2cli import GNSSStreamer
 ```
 
 ---
+## <a name="troubleshoot">Troubleshooting</a>
+
+#### `Unknown Protocol` errors.
+These are usually due to corruption of the serial data stream, either because the serial port configuration is incorrect (baud rate, parity, etc.) or because another process is attempting to use the same data stream. 
+- Check that your UBX receiver UART1 or UART2 ports are configured for the desired baud rate - remember the factory default is 38400 (*not* 9600).
+- Check that no other process is attempting to use the same serial port, including daemon processes like gpsd.
+#### `Serial Permission` errors. 
+These are usually caused by inadequate user privileges or contention with another process. 
+- On Linux platforms, check that the user is a member of the `tty` and/or `dialout` groups.
+- Check that no other process is attempting to use the same serial port, including daemon processes like gpsd.
+#### `UnicodeDecode` errors.
+- If reading UBX data from a log file, check that the file.open() procedure is using the `rb` (read binary) setting e.g.
+`stream = open('ubxdatalog.log', 'rb')`.
+
+
+---
 ## <a name="gui">Graphical Client</a>
 
 A python/tkinter graphical GPS client which supports both NMEA and UBX protocols (via pynmeagps and pyubx2 
 respectively) is available at: 
 
 [https://github.com/semuconsulting/PyGPSClient](https://github.com/semuconsulting/PyGPSClient)
```

### Comparing `pyubx2-1.2.8/README.md` & `pyubx2-1.2.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 [Parsing](#parsing) |
 [Generating](#generating) |
 [Serializing](#serializing) |
 [Configuration Interface](#configinterface) |
 [Examples](#examples) |
 [Extensibility](#extensibility) |
 [Command Line Utility](#cli) |
+[Troubleshooting](#troubleshoot) |
 [Graphical Client](#gui) |
 [Author & License](#author)
 
 `pyubx2` is an original Python 3 parser for the UBX &copy; protocol. UBX is a proprietary binary protocol implemented on u-blox &trade; GNSS/GPS receiver modules.
 
 The `pyubx2` homepage is located at [https://github.com/semuconsulting/pyubx2](https://github.com/semuconsulting/pyubx2).
 
@@ -43,17 +44,17 @@
 
 Sphinx API Documentation in HTML format is available at [https://www.semuconsulting.com/pyubx2](https://www.semuconsulting.com/pyubx2).
 
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyubx2/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pyubx2/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyubx2/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided.
 
-### New in v1.2.7
+### New in v1.2.9
 
-1. `pyubx2` can now parse RTCM3 messages as well as UBX and NMEA.
+1. Ability to read from socket as well as serial or file datastream.
 
 ---
 ## <a name="installation">Installation</a>
 
 `pyubx2` is compatible with Python >=3.7 and has no third-party library dependencies.
 
 In the following, `python` & `pip` refer to the Python 3 executables. You may need to type 
@@ -100,15 +101,15 @@
 
 ```
 class pyubx2.ubxreader.UBXReader(stream, *args, **kwargs)
 ```
 
 You can create a `UBXReader` object by calling the constructor with an active stream object. 
 The stream object can be any data stream which supports a `read(n) -> bytes` method (e.g. File or Serial, with 
-or without a buffer wrapper).
+or without a buffer wrapper). `pyubx2` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams (see example below).
 
 Individual input UBX, NMEA or RTCM3 messages can then be read using the `UBXReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `UBXMessage`, `NMEAMessage` or `RTCMMessage` object, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `UBXReader` also implements an iterator.
 
 The constructor accepts the following optional keyword arguments:
 
 * `protfilter`: 1 = NMEA, 2 = UBX, 4 = RTCM3 (can be OR'd. default is 3 - NMEA & UBX)
 * `quitonerror`: 0 = ignore errors, 1 = log errors and continue (default), 2 = (re)raise errors and terminate
@@ -131,14 +132,25 @@
 >>> from pyubx2 import UBXReader
 >>> stream = open('ubxdata.bin', 'rb')
 >>> ubr = UBXReader(stream, protfilter=2)
 >>> for (raw_data, parsed_data) in ubr: print(parsed_data)
 ...
 ```
 
+Example - Socket input (using enhanced iterator). This will output UBX, NMEA and RTCM3 data:
+```python
+>>> import socket
+>>> from pyubx2 import UBXReader
+>>> stream = socket.socket(socket.AF_INET, socket.SOCK_STREAM):
+>>> stream.connect(("localhost", 50007))
+>>> ubr = UBXReader(stream, protfilter=7)
+>>> for (raw_data, parsed_data) in ubr.iterate(): print(parsed_data)
+...
+```
+
 ---
 ## <a name="parsing">Parsing</a>
 
 You can parse individual UBX messages using the static `UBXReader.parse(data)` function, which takes a bytes array containing a binary UBX message and returns a `UBXMessage` object.
 
 **NB:** Once instantiated, a `UBXMessage` object is immutable.
 
@@ -359,14 +371,15 @@
 
 1. `ubxoptions.py` illustrates the various options available for parsing and constructing UBX messages.
 1. `ubxpoller.py` illustrates how to implement a simple threaded configuration polling utility for UBX messages. 
 1. `ubxsetrates.py` illustrates how to use legacy configuration messages (CFG-MSG) to set navigation message rates.
 1. `ubxconfigdb.py` illustrates how to invoke the Generation 9 configuration database interface via CFG-VALSET, CF-VALDEL and CFG-VALGET messages.
 1. `ubxfactoryreset.py` illustrates how to send a factory reset (CFG-CFG) command.
 1. `ubxfile.py` illustrates how to implement a binary file reader for UBX messages using `UBXReader` iterator functionality. 
+1. `ubxsocket.py` illustrates how to implement a TCP Socket reader for UBX messages using `UBXReader` iterator functionality. Can be used in conjunction with the `tcpserver_threaded.py` socket server test harness.
 1. `gpxtracker.py` illustrates a simple tool to convert a binary UBX data dump to a `*.gpx` track file.
 1. `ubxserver.py` in the \examples\webserver folder illustrates a simple HTTP web server wrapper around `pyubx2.UBXreader`; it presents data from selected UBX messages as a web page http://localhost:8080 or a RESTful API http://localhost:8080/gps.
 1. `benchmark.py` provides a simple performance benchmarking tool for the `pyubx2` parser.
 
 ---
 ## <a name="extensibility">Extensibility</a>
 
@@ -444,14 +457,30 @@
 The `gnssdump` utility implements a new `GNSSStreamer` class which may be used directly within Python application code via:
 
 ```python
 >>> from pyubx2cli import GNSSStreamer
 ```
 
 ---
+## <a name="troubleshoot">Troubleshooting</a>
+
+#### `Unknown Protocol` errors.
+These are usually due to corruption of the serial data stream, either because the serial port configuration is incorrect (baud rate, parity, etc.) or because another process is attempting to use the same data stream. 
+- Check that your UBX receiver UART1 or UART2 ports are configured for the desired baud rate - remember the factory default is 38400 (*not* 9600).
+- Check that no other process is attempting to use the same serial port, including daemon processes like gpsd.
+#### `Serial Permission` errors. 
+These are usually caused by inadequate user privileges or contention with another process. 
+- On Linux platforms, check that the user is a member of the `tty` and/or `dialout` groups.
+- Check that no other process is attempting to use the same serial port, including daemon processes like gpsd.
+#### `UnicodeDecode` errors.
+- If reading UBX data from a log file, check that the file.open() procedure is using the `rb` (read binary) setting e.g.
+`stream = open('ubxdatalog.log', 'rb')`.
+
+
+---
 ## <a name="gui">Graphical Client</a>
 
 A python/tkinter graphical GPS client which supports both NMEA and UBX protocols (via pynmeagps and pyubx2 
 respectively) is available at: 
 
 [https://github.com/semuconsulting/PyGPSClient](https://github.com/semuconsulting/PyGPSClient)
```

### Comparing `pyubx2-1.2.8/pyubx2/__init__.py` & `pyubx2-1.2.9/pyubx2/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     UBXTypeError,
     UBXStreamError,
     ParameterError,
     GNSSStreamError,
 )
 from pyubx2.ubxmessage import UBXMessage
 from pyubx2.ubxreader import UBXReader
+from pyubx2.socket_stream import SocketStream
 from pyubx2.ubxtypes_core import *
 from pyubx2.ubxtypes_get import *
 from pyubx2.ubxtypes_poll import *
 from pyubx2.ubxtypes_set import *
 from pyubx2.ubxhelpers import *
 from pyubx2.ubxtypes_configdb import *
```

### Comparing `pyubx2-1.2.8/pyubx2/exceptions.py` & `pyubx2-1.2.9/pyubx2/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyubx2-1.2.8/pyubx2/ubxhelpers.py` & `pyubx2-1.2.9/pyubx2/ubxhelpers.py`

 * *Files identical despite different names*

### Comparing `pyubx2-1.2.8/pyubx2/ubxmessage.py` & `pyubx2-1.2.9/pyubx2/ubxmessage.py`

 * *Files identical despite different names*

### Comparing `pyubx2-1.2.8/pyubx2/ubxreader.py` & `pyubx2-1.2.9/pyubx2/ubxreader.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,23 @@
 Created on 2 Oct 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
 
+from socket import socket
 from pyrtcm import RTCMReader
-from pyrtcm.rtcmhelpers import calc_crc24q
+
+# from pyrtcm.rtcmhelpers import calc_crc24q
 import pyrtcm.exceptions as rte
 from pynmeagps import NMEAReader
 import pynmeagps.exceptions as nme
-from pyubx2 import UBXMessage
+from pyubx2.socket_stream import SocketStream
+from pyubx2.ubxmessage import UBXMessage
 from pyubx2.ubxhelpers import calc_checksum, val2bytes, bytes2val
 import pyubx2.ubxtypes_core as ubt
 import pyubx2.exceptions as ube
 
 
 class UBXReader:
     """
@@ -39,19 +42,24 @@
         :param datastream stream: input data stream
         :param int quitonerror: (kwarg) 0 = ignore errors,  1 = log errors and continue, 2 = (re)raise errors (1)
         :param int protfilter: (kwarg) protocol filter 1 = NMEA, 2 = UBX, 4 = RTCM3 (3)
         :param int validate: (kwarg) 0 = ignore invalid checksum, 1 = validate checksum (1)
         :param int msgmode: (kwarg) 0=GET, 1=SET, 2=POLL (0)
         :param bool parsebitfield: (kwarg) 1 = parse bitfields, 0 = leave as bytes (1)
         :param bool scaling: (kwarg) 1 = apply scale factors, 0 = do not apply (1)
+        :param int bufsize: (kwarg) socket recv buffer size (1024)
         :raises: UBXStreamError (if mode is invalid)
 
         """
 
-        self._stream = datastream
+        bufsize = int(kwargs.get("bufsize", 4096))
+        if isinstance(datastream, socket):
+            self._stream = SocketStream(datastream, bufsize=bufsize)
+        else:
+            self._stream = datastream
         self._protfilter = int(
             kwargs.get("protfilter", ubt.NMEA_PROTOCOL | ubt.UBX_PROTOCOL)
         )
         self._quitonerror = int(kwargs.get("quitonerror", ubt.ERR_LOG))
         self._validate = int(kwargs.get("validate", ubt.VALCKSUM))
         self._parsebf = int(kwargs.get("parsebitfield", True))
         self._scaling = int(kwargs.get("scaling", True))
@@ -135,18 +143,17 @@
                         parsing = False
                     else:
                         continue
                 # unrecognised protocol header
                 else:
                     if self._quitonerror == ubt.ERR_RAISE:
                         raise ube.UBXStreamError(f"Unknown protocol {bytehdr}.")
-                    elif self._quitonerror == ubt.ERR_LOG:
+                    if self._quitonerror == ubt.ERR_LOG:
                         return (bytehdr, f"<UNKNOWN PROTOCOL(header={bytehdr})>")
-                    else:  # ignore unknown protocol and continue
-                        continue
+                    continue
 
         except EOFError:
             return (None, None)
 
         return (raw_data, parsed_data)
 
     def _parse_ubx(self, hdr: bytes) -> tuple:
@@ -282,15 +289,15 @@
                 rte.RTCMStreamError,
                 rte.RTCMTypeError,
             ) as err:
                 # raise, log or ignore any error depending
                 # on the quitonerror setting
                 if quitonerror == ubt.ERR_RAISE:
                     raise err
-                elif quitonerror == ubt.ERR_LOG:
+                if quitonerror == ubt.ERR_LOG:
                     # pass to error handler if there is one
                     if errorhandler is None:
                         print(err)
                     else:
                         errorhandler(err)
                 # continue
```

### Comparing `pyubx2-1.2.8/pyubx2/ubxtypes_configdb.py` & `pyubx2-1.2.9/pyubx2/ubxtypes_configdb.py`

 * *Files identical despite different names*

### Comparing `pyubx2-1.2.8/pyubx2/ubxtypes_core.py` & `pyubx2-1.2.9/pyubx2/ubxtypes_core.py`

 * *Files identical despite different names*

### Comparing `pyubx2-1.2.8/pyubx2/ubxtypes_get.py` & `pyubx2-1.2.9/pyubx2/ubxtypes_get.py`

 * *Files 0% similar despite different names*

```diff
@@ -3037,15 +3037,15 @@
         "magDec": [I2, SCAL2],
         "magAcc": [U2, SCAL2],
     },
     "NAV2-SAT": {
         "iTOW": U4,
         "version": U1,
         "numSvs": U1,
-        "reserved0": I1,
+        "reserved0": U2,
         "group": (
             "numSvs",
             {  # repeating group * numSvs
                 "gnssId": U1,
                 "svId": U1,
                 "cno": U1,
                 "elev": I1,
```

### Comparing `pyubx2-1.2.8/pyubx2/ubxtypes_poll.py` & `pyubx2-1.2.9/pyubx2/ubxtypes_poll.py`

 * *Files identical despite different names*

### Comparing `pyubx2-1.2.8/pyubx2/ubxtypes_set.py` & `pyubx2-1.2.9/pyubx2/ubxtypes_set.py`

 * *Files identical despite different names*

### Comparing `pyubx2-1.2.8/pyubx2.egg-info/PKG-INFO` & `pyubx2-1.2.9/pyubx2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyubx2
-Version: 1.2.8
+Version: 1.2.9
 Summary: UBX Protocol Parser
 Home-page: https://github.com/semuconsulting/pyubx2
 Author: semuadmin
 Author-email: semuadmin@semuconsulting.com
 License: BSD 3-Clause 'Modified' License
 Project-URL: Bug Tracker, https://github.com/semuconsulting/pyubx2
 Project-URL: Documentation, https://github.com/semuconsulting/pyubx2
@@ -46,14 +46,15 @@
 [Parsing](#parsing) |
 [Generating](#generating) |
 [Serializing](#serializing) |
 [Configuration Interface](#configinterface) |
 [Examples](#examples) |
 [Extensibility](#extensibility) |
 [Command Line Utility](#cli) |
+[Troubleshooting](#troubleshoot) |
 [Graphical Client](#gui) |
 [Author & License](#author)
 
 `pyubx2` is an original Python 3 parser for the UBX &copy; protocol. UBX is a proprietary binary protocol implemented on u-blox &trade; GNSS/GPS receiver modules.
 
 The `pyubx2` homepage is located at [https://github.com/semuconsulting/pyubx2](https://github.com/semuconsulting/pyubx2).
 
@@ -81,17 +82,17 @@
 
 Sphinx API Documentation in HTML format is available at [https://www.semuconsulting.com/pyubx2](https://www.semuconsulting.com/pyubx2).
 
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyubx2/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pyubx2/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyubx2/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided.
 
-### New in v1.2.7
+### New in v1.2.9
 
-1. `pyubx2` can now parse RTCM3 messages as well as UBX and NMEA.
+1. Ability to read from socket as well as serial or file datastream.
 
 ---
 ## <a name="installation">Installation</a>
 
 `pyubx2` is compatible with Python >=3.7 and has no third-party library dependencies.
 
 In the following, `python` & `pip` refer to the Python 3 executables. You may need to type 
@@ -138,15 +139,15 @@
 
 ```
 class pyubx2.ubxreader.UBXReader(stream, *args, **kwargs)
 ```
 
 You can create a `UBXReader` object by calling the constructor with an active stream object. 
 The stream object can be any data stream which supports a `read(n) -> bytes` method (e.g. File or Serial, with 
-or without a buffer wrapper).
+or without a buffer wrapper). `pyubx2` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams (see example below).
 
 Individual input UBX, NMEA or RTCM3 messages can then be read using the `UBXReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `UBXMessage`, `NMEAMessage` or `RTCMMessage` object, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `UBXReader` also implements an iterator.
 
 The constructor accepts the following optional keyword arguments:
 
 * `protfilter`: 1 = NMEA, 2 = UBX, 4 = RTCM3 (can be OR'd. default is 3 - NMEA & UBX)
 * `quitonerror`: 0 = ignore errors, 1 = log errors and continue (default), 2 = (re)raise errors and terminate
@@ -169,14 +170,25 @@
 >>> from pyubx2 import UBXReader
 >>> stream = open('ubxdata.bin', 'rb')
 >>> ubr = UBXReader(stream, protfilter=2)
 >>> for (raw_data, parsed_data) in ubr: print(parsed_data)
 ...
 ```
 
+Example - Socket input (using enhanced iterator). This will output UBX, NMEA and RTCM3 data:
+```python
+>>> import socket
+>>> from pyubx2 import UBXReader
+>>> stream = socket.socket(socket.AF_INET, socket.SOCK_STREAM):
+>>> stream.connect(("localhost", 50007))
+>>> ubr = UBXReader(stream, protfilter=7)
+>>> for (raw_data, parsed_data) in ubr.iterate(): print(parsed_data)
+...
+```
+
 ---
 ## <a name="parsing">Parsing</a>
 
 You can parse individual UBX messages using the static `UBXReader.parse(data)` function, which takes a bytes array containing a binary UBX message and returns a `UBXMessage` object.
 
 **NB:** Once instantiated, a `UBXMessage` object is immutable.
 
@@ -397,14 +409,15 @@
 
 1. `ubxoptions.py` illustrates the various options available for parsing and constructing UBX messages.
 1. `ubxpoller.py` illustrates how to implement a simple threaded configuration polling utility for UBX messages. 
 1. `ubxsetrates.py` illustrates how to use legacy configuration messages (CFG-MSG) to set navigation message rates.
 1. `ubxconfigdb.py` illustrates how to invoke the Generation 9 configuration database interface via CFG-VALSET, CF-VALDEL and CFG-VALGET messages.
 1. `ubxfactoryreset.py` illustrates how to send a factory reset (CFG-CFG) command.
 1. `ubxfile.py` illustrates how to implement a binary file reader for UBX messages using `UBXReader` iterator functionality. 
+1. `ubxsocket.py` illustrates how to implement a TCP Socket reader for UBX messages using `UBXReader` iterator functionality. Can be used in conjunction with the `tcpserver_threaded.py` socket server test harness.
 1. `gpxtracker.py` illustrates a simple tool to convert a binary UBX data dump to a `*.gpx` track file.
 1. `ubxserver.py` in the \examples\webserver folder illustrates a simple HTTP web server wrapper around `pyubx2.UBXreader`; it presents data from selected UBX messages as a web page http://localhost:8080 or a RESTful API http://localhost:8080/gps.
 1. `benchmark.py` provides a simple performance benchmarking tool for the `pyubx2` parser.
 
 ---
 ## <a name="extensibility">Extensibility</a>
 
@@ -482,14 +495,30 @@
 The `gnssdump` utility implements a new `GNSSStreamer` class which may be used directly within Python application code via:
 
 ```python
 >>> from pyubx2cli import GNSSStreamer
 ```
 
 ---
+## <a name="troubleshoot">Troubleshooting</a>
+
+#### `Unknown Protocol` errors.
+These are usually due to corruption of the serial data stream, either because the serial port configuration is incorrect (baud rate, parity, etc.) or because another process is attempting to use the same data stream. 
+- Check that your UBX receiver UART1 or UART2 ports are configured for the desired baud rate - remember the factory default is 38400 (*not* 9600).
+- Check that no other process is attempting to use the same serial port, including daemon processes like gpsd.
+#### `Serial Permission` errors. 
+These are usually caused by inadequate user privileges or contention with another process. 
+- On Linux platforms, check that the user is a member of the `tty` and/or `dialout` groups.
+- Check that no other process is attempting to use the same serial port, including daemon processes like gpsd.
+#### `UnicodeDecode` errors.
+- If reading UBX data from a log file, check that the file.open() procedure is using the `rb` (read binary) setting e.g.
+`stream = open('ubxdatalog.log', 'rb')`.
+
+
+---
 ## <a name="gui">Graphical Client</a>
 
 A python/tkinter graphical GPS client which supports both NMEA and UBX protocols (via pynmeagps and pyubx2 
 respectively) is available at: 
 
 [https://github.com/semuconsulting/PyGPSClient](https://github.com/semuconsulting/PyGPSClient)
```

### Comparing `pyubx2-1.2.8/pyubx2.egg-info/SOURCES.txt` & `pyubx2-1.2.9/pyubx2.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 pyubx2/__init__.py
 pyubx2/_version.py
 pyubx2/exceptions.py
+pyubx2/socket_stream.py
 pyubx2/ubxhelpers.py
 pyubx2/ubxmessage.py
 pyubx2/ubxreader.py
 pyubx2/ubxtypes_configdb.py
 pyubx2/ubxtypes_core.py
 pyubx2/ubxtypes_get.py
 pyubx2/ubxtypes_poll.py
```

### Comparing `pyubx2-1.2.8/pyubx2cli/gnssdump.py` & `pyubx2-1.2.9/pyubx2cli/gnssdump.py`

 * *Files identical despite different names*

### Comparing `pyubx2-1.2.8/pyubx2cli/helpstrings.py` & `pyubx2-1.2.9/pyubx2cli/helpstrings.py`

 * *Files identical despite different names*

### Comparing `pyubx2-1.2.8/setup.py` & `pyubx2-1.2.9/setup.py`

 * *Files identical despite different names*

