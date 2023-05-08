# Comparing `tmp/pygnssutils-1.0.7.tar.gz` & `tmp/pygnssutils-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygnssutils-1.0.7.tar", last modified: Tue Apr 25 08:37:22 2023, max compression
+gzip compressed data, was "pygnssutils-1.0.8.tar", last modified: Mon May  8 08:43:22 2023, max compression
```

## Comparing `pygnssutils-1.0.7.tar` & `pygnssutils-1.0.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-25 08:37:22.495053 pygnssutils-1.0.7/
--rw-r--r--   0 steve      (501) staff       (20)     1613 2022-05-26 12:22:57.000000 pygnssutils-1.0.7/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)       64 2022-05-26 12:22:57.000000 pygnssutils-1.0.7/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)    24113 2023-04-25 08:37:22.494872 pygnssutils-1.0.7/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)    21117 2023-03-23 11:19:25.000000 pygnssutils-1.0.7/README.md
--rw-r--r--   0 steve      (501) staff       (20)     2934 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-04-25 08:37:22.495106 pygnssutils-1.0.7/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-25 08:37:22.490402 pygnssutils-1.0.7/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-25 08:37:22.493075 pygnssutils-1.0.7/src/pygnssutils/
--rw-r--r--   0 steve      (501) staff       (20)      704 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      161 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/_version.py
--rw-r--r--   0 steve      (501) staff       (20)      297 2023-03-23 22:14:27.000000 pygnssutils-1.0.7/src/pygnssutils/exceptions.py
--rw-r--r--   0 steve      (501) staff       (20)     1712 2023-03-23 22:14:27.000000 pygnssutils-1.0.7/src/pygnssutils/globals.py
--rw-r--r--   0 steve      (501) staff       (20)    25351 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/gnssdump.py
--rw-r--r--   0 steve      (501) staff       (20)    17471 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/gnssmqttclient.py
--rw-r--r--   0 steve      (501) staff       (20)    24022 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/gnssntripclient.py
--rw-r--r--   0 steve      (501) staff       (20)    13831 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/gnssserver.py
--rw-r--r--   0 steve      (501) staff       (20)     4030 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/helpers.py
--rw-r--r--   0 steve      (501) staff       (20)    12997 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/socket_server.py
--rw-r--r--   0 steve      (501) staff       (20)     8924 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/ubxload.py
--rw-r--r--   0 steve      (501) staff       (20)    10943 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/ubxsave.py
--rw-r--r--   0 steve      (501) staff       (20)     7008 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/ubxsetrate.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-25 08:37:22.493904 pygnssutils-1.0.7/src/pygnssutils.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    24113 2023-04-25 08:37:22.000000 pygnssutils-1.0.7/src/pygnssutils.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      755 2023-04-25 08:37:22.000000 pygnssutils-1.0.7/src/pygnssutils.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-04-25 08:37:22.000000 pygnssutils-1.0.7/src/pygnssutils.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)      307 2023-04-25 08:37:22.000000 pygnssutils-1.0.7/src/pygnssutils.egg-info/entry_points.txt
--rw-r--r--   0 steve      (501) staff       (20)      232 2023-04-25 08:37:22.000000 pygnssutils-1.0.7/src/pygnssutils.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)       12 2023-04-25 08:37:22.000000 pygnssutils-1.0.7/src/pygnssutils.egg-info/top_level.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-25 08:37:22.494570 pygnssutils-1.0.7/tests/
--rw-r--r--   0 steve      (501) staff       (20)     9075 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/tests/test_gnssdump.py
--rw-r--r--   0 steve      (501) staff       (20)    27167 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/tests/test_sourcetable.py
--rw-r--r--   0 steve      (501) staff       (20)     4003 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/tests/test_static.py
--rw-r--r--   0 steve      (501) staff       (20)     3492 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/tests/test_stream.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-08 08:43:22.555854 pygnssutils-1.0.8/
+-rw-r--r--   0 steve      (501) staff       (20)     1613 2022-05-26 12:22:57.000000 pygnssutils-1.0.8/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)       64 2022-05-26 12:22:57.000000 pygnssutils-1.0.8/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)    24113 2023-05-08 08:43:22.555703 pygnssutils-1.0.8/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)    21117 2023-03-23 11:19:25.000000 pygnssutils-1.0.8/README.md
+-rw-r--r--   0 steve      (501) staff       (20)     2957 2023-05-08 08:36:54.000000 pygnssutils-1.0.8/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-05-08 08:43:22.555898 pygnssutils-1.0.8/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-08 08:43:22.551882 pygnssutils-1.0.8/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-08 08:43:22.554160 pygnssutils-1.0.8/src/pygnssutils/
+-rw-r--r--   0 steve      (501) staff       (20)      704 2023-04-25 08:36:15.000000 pygnssutils-1.0.8/src/pygnssutils/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      161 2023-05-08 08:36:54.000000 pygnssutils-1.0.8/src/pygnssutils/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)      297 2023-03-23 22:14:27.000000 pygnssutils-1.0.8/src/pygnssutils/exceptions.py
+-rw-r--r--   0 steve      (501) staff       (20)     1743 2023-05-08 08:36:54.000000 pygnssutils-1.0.8/src/pygnssutils/globals.py
+-rw-r--r--   0 steve      (501) staff       (20)    26375 2023-05-08 08:36:54.000000 pygnssutils-1.0.8/src/pygnssutils/gnssdump.py
+-rw-r--r--   0 steve      (501) staff       (20)    17785 2023-05-08 08:36:54.000000 pygnssutils-1.0.8/src/pygnssutils/gnssmqttclient.py
+-rw-r--r--   0 steve      (501) staff       (20)    25271 2023-05-08 08:36:54.000000 pygnssutils-1.0.8/src/pygnssutils/gnssntripclient.py
+-rw-r--r--   0 steve      (501) staff       (20)    14710 2023-05-08 08:36:54.000000 pygnssutils-1.0.8/src/pygnssutils/gnssserver.py
+-rw-r--r--   0 steve      (501) staff       (20)     5440 2023-05-08 08:36:54.000000 pygnssutils-1.0.8/src/pygnssutils/helpers.py
+-rw-r--r--   0 steve      (501) staff       (20)    13171 2023-05-08 08:36:54.000000 pygnssutils-1.0.8/src/pygnssutils/socket_server.py
+-rw-r--r--   0 steve      (501) staff       (20)     8924 2023-04-25 08:36:15.000000 pygnssutils-1.0.8/src/pygnssutils/ubxload.py
+-rw-r--r--   0 steve      (501) staff       (20)    10943 2023-04-25 08:36:15.000000 pygnssutils-1.0.8/src/pygnssutils/ubxsave.py
+-rw-r--r--   0 steve      (501) staff       (20)     7008 2023-04-25 08:36:15.000000 pygnssutils-1.0.8/src/pygnssutils/ubxsetrate.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-08 08:43:22.554983 pygnssutils-1.0.8/src/pygnssutils.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    24113 2023-05-08 08:43:22.000000 pygnssutils-1.0.8/src/pygnssutils.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      755 2023-05-08 08:43:22.000000 pygnssutils-1.0.8/src/pygnssutils.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-05-08 08:43:22.000000 pygnssutils-1.0.8/src/pygnssutils.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)      307 2023-05-08 08:43:22.000000 pygnssutils-1.0.8/src/pygnssutils.egg-info/entry_points.txt
+-rw-r--r--   0 steve      (501) staff       (20)      181 2023-05-08 08:43:22.000000 pygnssutils-1.0.8/src/pygnssutils.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       12 2023-05-08 08:43:22.000000 pygnssutils-1.0.8/src/pygnssutils.egg-info/top_level.txt
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-08 08:43:22.555515 pygnssutils-1.0.8/tests/
+-rw-r--r--   0 steve      (501) staff       (20)     9075 2023-04-25 08:36:15.000000 pygnssutils-1.0.8/tests/test_gnssdump.py
+-rw-r--r--   0 steve      (501) staff       (20)    27167 2023-04-25 08:36:15.000000 pygnssutils-1.0.8/tests/test_sourcetable.py
+-rw-r--r--   0 steve      (501) staff       (20)     5508 2023-05-08 08:36:54.000000 pygnssutils-1.0.8/tests/test_static.py
+-rw-r--r--   0 steve      (501) staff       (20)     3492 2023-04-25 08:36:15.000000 pygnssutils-1.0.8/tests/test_stream.py
```

### Comparing `pygnssutils-1.0.7/LICENSE` & `pygnssutils-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.7/PKG-INFO` & `pygnssutils-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygnssutils
-Version: 1.0.7
+Version: 1.0.8
 Summary: GNSS Command Line Utilities
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2020, SEMU Consulting
         All rights reserved.
```

### Comparing `pygnssutils-1.0.7/README.md` & `pygnssutils-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.7/pyproject.toml` & `pygnssutils-1.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = [
     {name = "semuadmin", email = "semuadmin@semuconsulting.com"},
 ]
 maintainers = [
   {name = "semuadmin", email = "semuadmin@semuconsulting.com"}
 ]
 description = "GNSS Command Line Utilities"
-version = "1.0.7"
+version = "1.0.8"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Operating System :: OS Independent",
     "Development Status :: 5 - Production/Stable",
     "Environment :: MacOS X",
@@ -37,15 +37,15 @@
     "Topic :: Scientific/Engineering :: GIS",
     ]
 
 dependencies = [
     "paho-mqtt>=1.6.1",
     "pyserial>=3.5",
     "pyspartn>=0.1.6",
-    "pyubx2>=1.2.24",
+    "pyubx2>=1.2.25",
 ]
 
 [project.scripts]
 gnssdump = "pygnssutils.gnssdump:main"
 gnssserver = "pygnssutils.gnssserver:main"
 gnssntripclient = "pygnssutils.gnssntripclient:main"
 gnssmqttclient = "pygnssutils.gnssmqttclient:main"
@@ -57,38 +57,46 @@
 homepage = "https://github.com/semuconsulting/pygnssutils"
 documentation = "https://www.semuconsulting.com/pygnssutils/"
 repository = "https://github.com/semuconsulting/pygnssutils"
 changelog = "https://github.com/semuconsulting/pygnssutils/blob/master/RELEASE_NOTES.md"
 
 [project.optional-dependencies]
 deploy = [
-    "build >= 0.10",
-    "pip >= 23.0",
+    "build",
+    "pip",
     "setuptools >= 66.0",
-    "wheel >= 0.40"
+    "wheel"
 ] 
 test = [
-    "bandit >= 1.7",
-    "black >= 23.1",
-    "pylint >= 2.17",
-    "pytest >= 7.2",
-    "pytest-cov >= 4.0",
-    "Sphinx >= 5.3",
-    "sphinx-rtd-theme >= 1.2.0"
+    "bandit",
+    "black",
+    "isort",
+    "pylint",
+    "pytest",
+    "pytest-cov",
+    "Sphinx",
+    "sphinx-rtd-theme"
 ]
 
+[tool.black]
+target-version = ['py37']
+
+[tool.isort]
+py_version = 37
+profile = "black"
+
 [tool.bandit]
 exclude_dirs = ["docs", "examples", "tests"]
 skips = ["B104","B307"] # bind 0.0.0.0; use of eval
 
 [tool.pylint]
 jobs = 0
 reports = "y"
+recursive = "y"
 py-version = "3.7"
-#exit-zero = "y"
 fail-under = "9.8"
 fail-on = "E,F"
 clear-cache-post-run = "y"
 disable = """
     raw-checker-failed,
     bad-inline-option,
     locally-disabled,
```

### Comparing `pygnssutils-1.0.7/src/pygnssutils/__init__.py` & `pygnssutils-1.0.8/src/pygnssutils/__init__.py`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.7/src/pygnssutils/globals.py` & `pygnssutils-1.0.8/src/pygnssutils/globals.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 MINMMEA_ID = [b"\xF0\x00", b"\xF0\x02", b"\xF0\x03", b"\xF0\x04", b"\xF0\x05"]
 ALLUBX_CLS = [b"\x01"]
 MINUBX_ID = [b"\x01\x07", b"\x01\x35"]
 
 TOPIC_RXM = "/pp/ubx/0236/ip"
 TOPIC_MGA = "/pp/ubx/mga"
 TOPIC_IP = "/pp/ip/{}"
+NTRIP_EVENT = "<<ntrip_read>>"
 SPARTN_EVENT = "<<spartn_read>>"
 SPARTN_PPSERVER = "pp.services.u-blox.com"
 OUTPORT_SPARTN = 8883
 PMP_DATARATES = {
     "B600": 600,
     "B1200": 1200,
     "B2400": 2400,
```

### Comparing `pygnssutils-1.0.7/src/pygnssutils/gnssdump.py` & `pygnssutils-1.0.8/src/pygnssutils/gnssdump.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import os
 from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser
 from collections import defaultdict
 from datetime import datetime
 from io import BufferedWriter, TextIOWrapper
 from queue import Queue
-from socket import socket
+from socket import AF_INET6, SOCK_STREAM, socket
 from time import time
 
 import pynmeagps.exceptions as nme
 import pyrtcm.exceptions as rte
 import pyubx2.exceptions as ube
 from pynmeagps import NMEAMessage
 from pyrtcm import RTCMMessage
@@ -52,15 +52,15 @@
     FORMAT_PARSED,
     FORMAT_PARSEDSTRING,
     LOGLIMIT,
     VERBOSITY_DEBUG,
     VERBOSITY_HIGH,
     VERBOSITY_MEDIUM,
 )
-from pygnssutils.helpers import format_json
+from pygnssutils.helpers import format_conn, format_json, ipprot2int
 
 
 class GNSSStreamer:
     """
     GNSS Streamer Class.
 
     Streams and parses UBX, NMEA or RTCM3 GNSS messages from any data stream (e.g. Serial, Socket or File)
@@ -85,15 +85,16 @@
 
         gnssdump port=COM3 msgfilter=NAV-PVT ubxhandler="lambda msg: print(f'lat: {msg.lat}, lon: {msg.lon}')"
 
         :param object app: application from which this class is invoked (None)
         :param object stream: (kwarg) stream object (must implement read(n) -> bytes method)
         :param str port: (kwarg) serial port name
         :param str filename: (kwarg) input file FQN
-        :param str socket: (kwarg) input socket host:port
+        :param str socket: (kwarg) input socket "host:port" - IPv6 addresses must be in format "[host]:port"
+        :param str ipprot: (kwarg) IP protocol IPv4 / IPv6
         :param int baudrate: (kwarg) serial baud rate (9600)
         :param int timeout: (kwarg) serial timeout in seconds (3)
         :param int validate: (kwarg) 1 = validate checksums, 0 = do not validate (1)
         :param int msgmode: (kwarg) 0 = GET, 1 = SET, 2 = POLL (0)
         :param int parsebitfield: (kwarg) 1 = parse UBX 'X' attributes as bitfields, 0 = leave as bytes (1)
         :param int format: (kwarg) output format 1 = parsed, 2 = raw, 4 = hex, 8 = tabulated hex, 16 = parsed as string, 32 = JSON (1) (can be OR'd)
         :param int quitonerror: (kwarg) 0 = ignore errors,  1 = log errors and continue, 2 = (re)raise errors (1)
@@ -114,22 +115,33 @@
 
         self._reader = None
         self.ctx_mgr = False
         self._datastream = kwargs.get("datastream", None)
         self._port = kwargs.get("port", None)
         self._socket = kwargs.get("socket", None)
         self._outfile = kwargs.get("outfile", None)
+        self._ipprot = ipprot2int(kwargs.get("ipprot", "IPv4"))
+
         if self._socket is not None:
-            sock = self._socket.split(":")
-            if len(sock) != 2:
-                raise ParameterError(
-                    "socket keyword must be in the format host:port.\nType gnssdump -h for help."
-                )
-            self._socket_host = sock[0]
-            self._socket_port = int(sock[1])
+            if self._ipprot == AF_INET6:  # IPv6 host ip must be enclosed in []
+                sock = self._socket.replace("[", "").split("]")
+                if len(sock) != 2:
+                    raise ParameterError(
+                        "IPv6 socket keyword must be in the format [host]:port"
+                    )
+                self._socket_host = sock[0]
+                self._socket_port = int(sock[1].replace(":", ""))
+            else:  # AF_INET
+                sock = self._socket.split(":")
+                if len(sock) != 2:
+                    raise ParameterError(
+                        "IPv4 socket keyword must be in the format host:port"
+                    )
+                self._socket_host = sock[0]
+                self._socket_port = int(sock[1])
         self._filename = kwargs.get("filename", None)
         if (
             self._datastream is None
             and self._port is None
             and self._socket is None
             and self._filename is None
         ):
@@ -257,16 +269,18 @@
                 self._start_reader()
         elif self._port is not None:  # serial
             with Serial(
                 self._port, self._baudrate, timeout=self._timeout
             ) as self._stream:
                 self._start_reader()
         elif self._socket is not None:  # socket
-            with socket() as self._stream:
-                self._stream.connect((self._socket_host, self._socket_port))
+            with socket(self._ipprot, SOCK_STREAM) as self._stream:
+                self._stream.connect(
+                    format_conn(self._ipprot, self._socket_host, self._socket_port)
+                )
                 self._start_reader()
         elif self._filename is not None:  # binary file
             with open(self._filename, "rb") as self._stream:
                 self._start_reader()
 
         return 1
 
@@ -612,15 +626,27 @@
         description="One of either -P port, -S socket or -F filename must be specified",
         epilog=EPILOG,
         formatter_class=ArgumentDefaultsHelpFormatter,
     )
     arp.add_argument("-V", "--version", action="version", version="%(prog)s " + VERSION)
     arp.add_argument("-P", "--port", required=False, help="Serial port")
     arp.add_argument("-F", "--filename", required=False, help="Input file path/name")
-    arp.add_argument("-S", "--socket", required=False, help="Input socket host:port")
+    arp.add_argument(
+        "-S",
+        "--socket",
+        required=False,
+        help="Input socket host:port; enclose IPv6 host in []",
+    )
+    arp.add_argument(
+        "--ipprot",
+        required=False,
+        help="IP protocol (for Socket connections)",
+        choices=["IPv4", "IPv6"],
+        default="IPv4",
+    )
     arp.add_argument(
         "--baudrate",
         required=False,
         help="Serial baud rate",
         type=int,
         choices=[4800, 9600, 19200, 38400, 57600, 115200, 230400, 460800],
         default=9600,
```

### Comparing `pygnssutils-1.0.7/src/pygnssutils/gnssmqttclient.py` & `pygnssutils-1.0.8/src/pygnssutils/gnssmqttclient.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 gnssmqttclient.py
 
 Command line utility, installed with PyPi library pygnssutils,
 which acts as an SPARTN MQTT client, retrieving correction data
 from an IP (MQTT) source and (optionally) sending the data to a
 designated writeable output medium (serial, file, socket, queue).
 
-Includes provision to be invoked from within PyGPSClient tkinter
-application (or any tkinter app which implements comparable
-GUI update methods).
+Calling app, if defined, can implement the following methods:
+- set_event() - create <<spartn_read>> event
+- dialog() - return reference to MQTT client configuration dialog
 
 Thingstream > Location Services > PointPerfect Thing > Credentials
 Default location for key files is user's HOME directory
 
 Created on 20 Feb 2023
 
 :author: semuadmin
@@ -53,14 +53,15 @@
     TOPIC_MGA,
     TOPIC_RXM,
     VERBOSITY_LOW,
     VERBOSITY_MEDIUM,
 )
 
 TIMEOUT = 8
+DLGTSPARTN = "SPARTN Configuration"
 
 
 class GNSSMQTTClient:
     """
     SPARTN MQTT client class.
     """
 
@@ -219,23 +220,23 @@
         if settings["topic_ip"]:
             topics.append((TOPIC_IP.format(settings["region"]), 0))
         if settings["topic_mga"]:
             topics.append((TOPIC_MGA, 0))
         if settings["topic_key"]:
             topics.append((TOPIC_RXM, 0))
         userdata = {
-            "gnss": settings["output"],
+            "output": settings["output"],
             "topics": topics,
             "app": app,
-            "readevent": SPARTN_EVENT,
         }
 
         try:
             client = mqtt.Client(client_id=settings["clientid"], userdata=userdata)
             client.on_connect = self.on_connect
+            client.on_disconnect = self.on_disconnect
             client.on_message = self.on_message
             client.tls_set(certfile=settings["tlscrt"], keyfile=settings["tlskey"])
             i = 1
             while not stopevent.is_set():
                 try:
                     client.connect(settings["server"], port=settings["port"])
                     break
@@ -251,20 +252,16 @@
 
             client.loop_start()
             while not stopevent.is_set():
                 # run the client loop in the same thread, as callback access gnss
                 # client.loop(timeout=0.1)
                 sleep(0.1)
         except (FileNotFoundError, TimeoutError) as err:
-            stopevent.set()
             self._do_log(f"ERROR! {err}", VERBOSITY_MEDIUM)
-            if app is not None:
-                if hasattr(app, "dlg_spartnconfig"):
-                    if hasattr(app.dlg_spartnconfig, "disconnect_ip"):
-                        app.dlg_spartnconfig.disconnect_ip(f"ERROR! {err}")
+            GNSSMQTTClient.on_error(userdata, err)
             self.stop()
             self.errevent.set()
 
         finally:
             client.loop_stop()
 
     @staticmethod
@@ -277,97 +274,119 @@
         :param list flags: optional flags
         :param int rcd: return status code
         """
 
         if rcd == 0:
             client.subscribe(userdata["topics"])
         else:
-            print(f"PyPGSClient MQTT Client - Connection failed, rc: {rcd}!")
+            GNSSMQTTClient.on_error(userdata, rcd)
+
+    @staticmethod
+    def on_connect_fail(client, userdata, rcd):  # pylint: disable=unused-argument
+        """
+        The callback for when the client fails to connect to the server.
+
+        :param object client: client
+        :param list userdata:  list of user defined data items
+        :param int rcd: return status code
+        """
+
+        GNSSMQTTClient.on_error(userdata, rcd)
+
+    @staticmethod
+    def on_disconnect(client, userdata, rcd):  # pylint: disable=unused-argument
+        """
+        The callback for when the client disconnects from the server.
+
+        :param object client: client
+        :param list userdata:  list of user defined data items
+        :param int rcd: return status code
+        """
+
+        GNSSMQTTClient.on_error(userdata, rcd)
 
     @staticmethod
     def on_message(client, userdata, msg):  # pylint: disable=unused-argument
         """
         The callback for when a PUBLISH message is received from the server.
         Some MQTT topics may contain more than one UBX or SPARTN message in
         a single payload.
 
+        :param object client: MQTT client
         :param list userdata: list of user defined data items
         :param object msg: SPARTN or UBX message topic content
         """
 
-        def do_write(output: object, raw: bytes, parsed: object):
+        def do_write(userdata: dict, raw: bytes, parsed: object):
             """
             Send SPARTN data to designated output medium.
 
             If output is Queue, will send both raw and parsed data.
 
-            :param object output: writeable output medium for SPARTN data
+            :param dict userdata: user defined data dict
             :param bytes raw: raw data
             :param object parsed: parsed message
             """
 
+            output = userdata["output"]
+            app = userdata["app"]
+
             if output is None:
                 print(parsed)
             else:
                 if isinstance(output, (Serial, BufferedWriter)):
                     output.write(raw)
                 elif isinstance(output, TextIOWrapper):
                     output.write(str(parsed))
                 elif isinstance(output, Queue):
                     output.put((raw, parsed))
                 elif isinstance(output, socket.socket):
                     output.sendall(raw)
 
-        def do_notify(app: object):
-            """
-            Notify any calling app of SPARTN read event.
-
-            :param object app: calling application
-            """
-
-            if hasattr(app, "appmaster"):
-                if hasattr(app.appmaster, "event_generate"):
-                    app.appmaster.event_generate("<<spartn_read>>")
+            if app is not None:
+                if hasattr(app, "set_event"):
+                    app.set_event(SPARTN_EVENT)
 
         if msg.topic in (TOPIC_MGA, TOPIC_RXM):  # multiple UBX MGA or RXM messages
             ubr = UBXReader(BytesIO(msg.payload), msgmode=SET)
             try:
                 for raw, parsed in ubr:
-                    # userdata["gnss"].put((raw, parsed))
-                    do_write(userdata["gnss"], raw, parsed)
-                    do_notify(userdata["app"])
+                    do_write(userdata, raw, parsed)
             except UBXParseError:
                 parsed = f"MQTT UBXParseError {msg.topic} {msg.payload}"
-                # userdata["gnss"].put((msg.payload, parsed))
-                do_write(userdata["gnss"], msg.payload, parsed)
-                do_notify(userdata["app"])
+                do_write(userdata, msg.payload, parsed)
         else:  # SPARTN protocol message
             spr = SPARTNReader(BytesIO(msg.payload))
             try:
                 for raw, parsed in spr:
-                    # userdata["gnss"].put((raw, parsed))
-                    do_write(userdata["gnss"], raw, parsed)
-                    do_notify(userdata["app"])
+                    do_write(userdata, raw, parsed)
             except (SPARTNMessageError, SPARTNParseError, SPARTNStreamError):
                 parsed = f"MQTT SPARTNParseError {msg.topic} {msg.payload}"
-                # userdata["gnss"].put((msg.payload, parsed))
-                do_write(userdata["gnss"], msg.payload, parsed)
-                do_notify(userdata["app"])
+                do_write(userdata, msg.payload, parsed)
 
-    def _app_update_status(self, status: bool, msg: tuple = None):
+    @staticmethod
+    def on_error(userdata: dict, err: object):
         """
-        THREADED
-        Update SPARTN connection status in calling application.
+        Report return code back to any calling application.
 
-        :param bool status: SPARTN server connection status
-        :param tuple msg: optional (message, color)
+        :param dict userdata: user defined data dict
+        :param object rcd: return code (int or str)
         """
 
-        if hasattr(self.__app, "update_spartn_status"):
-            self.__app.update_spartn_status(status, msg)
+        if isinstance(err, int):
+            err = mqtt.error_string(err)
+        app = userdata["app"]
+        if app is None:
+            print(err)
+        else:
+            if hasattr(app, "dialog"):
+                dlg = app.dialog(DLGTSPARTN)
+                if dlg is not None:
+                    if hasattr(dlg, "disconnect_ip"):
+                        dlg.disconnect_ip(f"{err} ")
 
     def _do_log(
         self,
         message: object,
         loglevel: int = VERBOSITY_MEDIUM,
         timestamp: bool = True,
     ):
```

### Comparing `pygnssutils-1.0.7/src/pygnssutils/gnssntripclient.py` & `pygnssutils-1.0.8/src/pygnssutils/gnssntripclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 correction data from an NTRIP server and (optionally)
 sending the correction data to a designated writeable output
 medium (serial, file, socket, queue).
 
 Can also transmit client position back to NTRIP server at specified
 intervals via formatted NMEA GGA sentences.
 
-Includes provision to be invoked from within PyGPSClient tkinter
-application (or any tkinter app which implements comparable
-GUI update methods).
+Calling app, if defined, can implement the following methods:
+- set_event() - create <<ntrip_read>> event
+- dialog() - return reference to NTRIP config client dialog
+- get_coordinates() - return coordinates from receiver
 
 Created on 03 Jun 2022
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2022
 :license: BSD 3-Clause
 """
@@ -42,23 +43,25 @@
 from pygnssutils.globals import (
     DEFAULT_BUFSIZE,
     EPILOG,
     HTTPERR,
     LOGLIMIT,
     MAXPORT,
     NOGGA,
+    NTRIP_EVENT,
     OUTPORT_NTRIP,
     VERBOSITY_LOW,
     VERBOSITY_MEDIUM,
 )
-from pygnssutils.helpers import find_mp_distance
+from pygnssutils.helpers import find_mp_distance, format_conn, ipprot2int
 
 TIMEOUT = 10
 GGALIVE = 0
 GGAFIXED = 1
+DLGTNTRIP = "NTRIP Configuration"
 
 
 class GNSSNTRIPClient:
     """
     NTRIP client class.
     """
 
@@ -74,16 +77,19 @@
 
         self.__app = app  # Reference to calling application class (if applicable)
         self._validargs = True
         self._loglines = 0
         self._ntripqueue = Queue()
         # persist settings to allow any calling app to retrieve them
         self._settings = {
+            "ipprot": socket.AF_INET,
             "server": "",
-            "port": "2101",
+            "port": 2101,
+            "flowinfo": 0,
+            "scopeid": 0,
             "mountpoint": "",
             "distance": "",
             "version": "2.0",
             "user": "anon",
             "password": "password",
             "ggainterval": "None",
             "ggamode": GGALIVE,
@@ -151,39 +157,46 @@
         If calling application implements a "get_coordinates" method to
         obtain live coordinates (i.e. from GNSS receiver), the method will
         use these instead of fixed reference coordinates.
 
         User login credentials can be obtained from environment variables
         NTRIP_USER and NTRIP_PASSWORD, or passed as kwargs.
 
-        :param str server: NTRIP server URL ("")
-        :param int port: NTRIP port (2101)
-        :param str mountpoint: NTRIP mountpoint ("", leave blank to get sourcetable)
-        :param str version: NTRIP protocol version ("2.0")
-        :param str user: login user ("anon" or env variable NTRIP_USER)
-        :param str password: login password ("password" or env variable NTRIP_PASSWORD)
-        :param int ggainterval: GGA sentence transmission interval (-1 = None)
-        :param int ggamode: GGA pos source; 0 = live from receiver, 1 = fixed reference (0)
-        :param str reflat: reference latitude (0.0)
-        :param str reflon: reference longitude (0.0)
-        :param str refalt: reference altitude (0.0)
-        :param str refsep: reference separation (0.0)
-        :param object output: writeable output medium (serial, file, socket, queue) (None)
+        :param str ipprot: (kwarg) IP protocol IPv4/IPv6 ("IPv4")
+        :param str server: (kwarg) NTRIP server URL ("")
+        :param int port: (kwarg) NTRIP port (2101)
+        :param int flowinfo: (kwarg) flowinfo for IPv6 (0)
+        :param int scopeid: (kwarg) scopeid for IPv6 (0)
+        :param str mountpoint: (kwarg) NTRIP mountpoint ("", leave blank to get sourcetable)
+        :param str version: (kwarg) NTRIP protocol version ("2.0")
+        :param str user: (kwarg) login user ("anon" or env variable NTRIP_USER)
+        :param str password: (kwarg) login password ("password" or env variable NTRIP_PASSWORD)
+        :param int ggainterval: (kwarg) GGA sentence transmission interval (-1 = None)
+        :param int ggamode: (kwarg) GGA pos source; 0 = live from receiver, 1 = fixed reference (0)
+        :param str reflat: (kwarg) reference latitude (0.0)
+        :param str reflon: (kwarg) reference longitude (0.0)
+        :param str refalt: (kwarg) reference altitude (0.0)
+        :param str refsep: (kwarg) reference separation (0.0)
+        :param object output: (kwarg) writeable output medium (serial, file, socket, queue) (None)
         :returns: boolean flag 0 = terminated, 1 = Ok to stream RTCM3 data from server
         :rtype: bool
         """
         # pylint: disable=unused-variable
 
         try:
             user = os.getenv("NTRIP_USER", "anon")
             password = os.getenv("NTRIP_PASSWORD", "password")
             self._last_gga = datetime.fromordinal(1)
 
+            ipprot = kwargs.get("ipprot", "IPv4")
+            self.settings["ipprot"] = ipprot2int(ipprot)
             self._settings["server"] = server = kwargs.get("server", "")
             self._settings["port"] = port = int(kwargs.get("port", OUTPORT_NTRIP))
+            self._settings["flowinfo"] = int(kwargs.get("flowinfo", 0))
+            self._settings["scopeid"] = int(kwargs.get("scopeid", 0))
             self._settings["mountpoint"] = mountpoint = kwargs.get("mountpoint", "")
             self._settings["version"] = kwargs.get("version", "2.0")
             self._settings["user"] = kwargs.get("user", user)
             self._settings["password"] = kwargs.get("password", password)
             self._settings["ggainterval"] = int(kwargs.get("ggainterval", NOGGA))
             self._settings["ggamode"] = int(kwargs.get("ggamode", GGALIVE))
             self._settings["reflat"] = kwargs.get("reflat", 0.0)
@@ -220,25 +233,28 @@
         """
         Close NTRIP server connection.
         """
 
         self._stop_read_thread()
         self._connected = False
 
-    def _app_update_status(self, status: bool, msg: tuple = None):
+    def _app_update_status(self, status: bool, msgt: tuple = None):
         """
         THREADED
         Update NTRIP connection status in calling application.
 
         :param bool status: NTRIP server connection status
-        :param tuple msg: optional (message, color)
+        :param tuple msgt: optional (message, color)
         """
 
-        if hasattr(self.__app, "update_ntrip_status"):
-            self.__app.update_ntrip_status(status, msg)
+        if hasattr(self.__app, "dialog"):
+            dlg = self.__app.dialog(DLGTNTRIP)
+            if dlg is not None:
+                if hasattr(dlg, "set_controls"):
+                    dlg.set_controls(status, msgt)
 
     def _app_get_coordinates(self) -> tuple:
         """
         THREADED
         Get live coordinates from receiver, or use fixed
         reference position, depending on ggamode setting.
 
@@ -257,25 +273,14 @@
 
         lat, lon, alt, sep = [
             0.0 if c == "" else float(c) for c in (lat, lon, alt, sep)
         ]
 
         return lat, lon, alt, sep
 
-    def _app_notify(self):
-        """
-        THREADED
-        If calling app is tkinter, generate event
-        to notify app that data is available
-        """
-
-        if hasattr(self.__app, "appmaster"):
-            if hasattr(self.__app.appmaster, "event_generate"):
-                self.__app.appmaster.event_generate("<<ntrip_read>>")
-
     def _formatGET(self, settings: dict) -> str:
         """
         THREADED
         Format HTTP GET Request.
 
         :param dict settings: settings dictionary
         :return: formatted HTTP GET request
@@ -420,20 +425,22 @@
         :param Event stopevent: stop event
         :param object output: output stream for RTCM3 data
         """
 
         try:
             server = settings["server"]
             port = int(settings["port"])
+            flowinfo = int(settings["flowinfo"])
+            scopeid = int(settings["scopeid"])
             mountpoint = settings["mountpoint"]
             ggainterval = int(settings["ggainterval"])
-
-            with socket.socket() as self._socket:
+            conn = format_conn(settings["ipprot"], server, port, flowinfo, scopeid)
+            with socket.socket(settings["ipprot"], socket.SOCK_STREAM) as self._socket:
                 self._socket.settimeout(TIMEOUT)
-                self._socket.connect((server, port))
+                self._socket.connect(conn)
                 self._socket.sendall(self._formatGET(settings))
                 # send GGA sentence with request
                 if mountpoint != "":
                     self._send_GGA(ggainterval, output)
                 while not stopevent.is_set():
                     rc = self._do_header(self._socket, stopevent)
                     if rc == "0":  # streaming RTMC3 data from mountpoint
@@ -475,29 +482,29 @@
 
         while data and not stopevent.is_set():
             try:
                 data = sock.recv(DEFAULT_BUFSIZE)
                 header_lines = data.decode(encoding="utf-8").split("\r\n")
                 for line in header_lines:
                     # if sourcetable request, populate list
-                    if line.find("STR;") >= 0:  # sourcetable entry
+                    if True in [line.find(cd) > 0 for cd in HTTPERR]:  # HTTP 40x
+                        self._do_log(line, VERBOSITY_MEDIUM, False)
+                        return line
+                    elif line.find("STR;") >= 0:  # sourcetable entry
                         strbits = line.split(";")
                         if strbits[0] == "STR":
                             strbits.pop(0)
                             stable.append(strbits)
                     elif line.find("ENDSOURCETABLE") >= 0:  # end of sourcetable
                         self._settings["sourcetable"] = stable
                         self._get_closest_mountpoint()
                         self._do_log("Complete sourcetable follows...\n")
                         for lines in self._settings["sourcetable"]:
                             self._do_log(lines, VERBOSITY_MEDIUM, False)
                         return "1"
-                    elif True in [line.find(cd) > 0 for cd in HTTPERR]:  # HTTP 40x
-                        self._do_log(line, VERBOSITY_MEDIUM, False)
-                        return line
 
             except UnicodeDecodeError:
                 data = False
 
         return "0"
 
     def _do_data(
@@ -559,15 +566,17 @@
             elif isinstance(output, TextIOWrapper):
                 output.write(str(parsed))
             elif isinstance(output, Queue):
                 output.put((raw, parsed))
             elif isinstance(output, socket.socket):
                 output.sendall(raw)
 
-        self._app_notify()  # notify any calling app that data is available
+        # self._app_notify()  # notify any calling app that data is available
+        if self.__app is not None:
+            self.__app.set_event(NTRIP_EVENT)
 
     def _do_log(
         self,
         message: object,
         loglevel: int = VERBOSITY_MEDIUM,
         timestamp: bool = True,
     ):
@@ -618,20 +627,34 @@
 
     ap = ArgumentParser(
         epilog=EPILOG,
         formatter_class=ArgumentDefaultsHelpFormatter,
     )
     ap.add_argument("-V", "--version", action="version", version="%(prog)s " + VERSION)
     ap.add_argument(
+        "-I",
+        "--ipprot",
+        required=False,
+        help="IP protocol",
+        choices=["IPv4", "IPv6"],
+        default="IPv4",
+    )
+    ap.add_argument(
         "-S", "--server", required=True, help="NTRIP server (caster) URL", default=""
     )
     ap.add_argument(
         "-P", "--port", required=False, help="NTRIP port", type=int, default=2101
     )
     ap.add_argument(
+        "--flowinfo", required=False, help="Flow info for IPv6", type=int, default=0
+    )
+    ap.add_argument(
+        "--scopeid", required=False, help="Scope ID for IPv6", type=int, default=0
+    )
+    ap.add_argument(
         "-M",
         "--mountpoint",
         required=False,
         help="NTRIP mountpoint (leave blank to get sourcetable)",
         default="",
     )
     ap.add_argument(
```

### Comparing `pygnssutils-1.0.7/src/pygnssutils/gnssserver.py` & `pygnssutils-1.0.8/src/pygnssutils/gnssserver.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     LOGLIMIT,
     OUTPORT,
     OUTPORT_NTRIP,
     VERBOSITY_LOW,
     VERBOSITY_MEDIUM,
 )
 from pygnssutils.gnssdump import GNSSStreamer
+from pygnssutils.helpers import format_conn, ipprot2int
 from pygnssutils.socket_server import ClientHandler, SocketServer
 
 
 class GNSSSocketServer:
     """
     GNSS Socket Server Class.
     """
@@ -53,14 +54,15 @@
         gnssserver inport=COM3 hostip=192.168.0.20 outport=50010 ntripmode=0
 
         :param object app: application from which this class is invoked (None)
         :param str inport: (kwarg) input serial port name (None)
         :param str socket: (kwarg) input socket host:port
         :param int baudrate: (kwarg) serial baud rate (9600)
         :param int timeout: (kwarg) serial timeout in seconds (3)
+        :param str ipprot: (kwarg) IP protocol IPv4/IPv6 ("IPv4")
         :param int hostip: (kwarg) host ip address (0.0.0.0)
         :param str outport: (kwarg) TCP port (50010, or 2101 in NTRIP mode)
         :param int maxclients: (kwarg) maximum number of connected clients (5)
         :param int ntripmode: (kwarg) 0 = socket server, 1 - NTRIP server (0)
         :param int validate: (kwarg) 1 = validate checksums, 0 = do not validate (1)
         :param int parsebitfield: (kwarg) 1 = parse UBX 'X' attributes as bitfields, 0 = leave as bytes (1)
         :param int format: (kwarg) output format 1 = parsed, 2 = raw, 4 = hex, 8 = tabulated hex, 16 = parsed as string (1), 32 = JSON (can be OR'd)
@@ -74,16 +76,21 @@
         """
 
         try:
             self._kwargs = kwargs
             # overrideable command line arguments..
             # 0 = TCP Socket Server mode, 1 = NTRIP Server mode
             self._kwargs["ntripmode"] = int(kwargs.get("ntripmode", 0))
-            # 0.0.0.0 binds to all host IP addresses
-            self._kwargs["hostip"] = kwargs.get("hostip", "0.0.0.0")
+            ipprot = kwargs.get("ipprot", "IPv4")
+            self._kwargs["ipprot"] = ipprot
+            self._kwargs["flowinfo"] = int(kwargs.get("flowinfo", 0))
+            self._kwargs["scopeid"] = int(kwargs.get("scopeid", 0))
+            # 0.0.0.0 (or :: on IPv6) binds to all host IP addresses
+            host = "::" if ipprot == "IPv6" else "0.0.0.0"
+            self._kwargs["hostip"] = kwargs.get("hostip", host)
             # amend default as required
             self._kwargs["port"] = kwargs.get("inport", None)
             self._kwargs["outport"] = int(
                 kwargs.get(
                     "outport", OUTPORT_NTRIP if self._kwargs["ntripmode"] else OUTPORT
                 )
             )
@@ -217,21 +224,25 @@
         """
         THREADED
 
         Output (socket server) thread.
         """
 
         try:
+            conn = format_conn(
+                ipprot2int(kwargs["ipprot"]), kwargs["hostip"], kwargs["outport"]
+            )
             with SocketServer(
                 app,
                 kwargs["ntripmode"],
                 kwargs["maxclients"],
                 kwargs["outputhandler"],
-                (kwargs["hostip"], kwargs["outport"]),
+                conn,
                 ClientHandler,
+                ipprot=kwargs["ipprot"],
             ) as self._socket_server:
                 self._socket_server.serve_forever()
         except OSError as err:
             self._do_log(f"Error starting socket server {err}", VERBOSITY_MEDIUM)
 
     def notify_client(self, address: tuple, status: int):
         """
@@ -308,15 +319,26 @@
         "--outport",
         required=False,
         help="Output TCP port",
         type=int,
         default=50010,
     )
     arp.add_argument(
-        "-H", "--hostip", required=False, help="Host IP Address", default="0.0.0.0"
+        "--ipprot",
+        required=False,
+        help="IP protocol",
+        choices=["IPv4", "IPv6"],
+        default="IPv4",
+    )
+    arp.add_argument(
+        "-H",
+        "--hostip",
+        required=False,
+        help="Host IP Address Binding (0.0.0.0/:: = all)",
+        default="0.0.0.0",
     )
     arp.add_argument(
         "-N",
         "--ntripmode",
         required=False,
         help="NTRIP Mode 0 = socket server, 1 = NTRIP caster",
         type=int,
@@ -441,14 +463,16 @@
         required=False,
         help="Fully qualified path to logfile folder",
         default=".",
     )
 
     args = arp.parse_args()
     kwargs = vars(args)
+    if kwargs["hostip"] == "0.0.0.0" and kwargs["ipprot"] == "IPv6":
+        kwargs["hostip"] = "::"
 
     try:
         with GNSSSocketServer(**kwargs) as server:
             goodtogo = server.run()
 
             while goodtogo:  # run until user presses CTRL-C
                 sleep(args.waittime)
```

### Comparing `pygnssutils-1.0.7/src/pygnssutils/helpers.py` & `pygnssutils-1.0.8/src/pygnssutils/helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
 # pylint: disable=invalid-name
 
 from math import cos, radians, sin
+from socket import AF_INET, AF_INET6
 
 from pynmeagps import haversine
 from pyubx2 import itow2utc
 
 
 def get_mp_distance(lat: float, lon: float, mp: list) -> float:
     """
@@ -132,7 +133,61 @@
             else:
                 stg += f'"{att}": "{str(val)}"'
             if i < len(message.__dict__) - 1:
                 stg += ", "
     stg += f"{end}{end}"
 
     return stg
+
+
+def format_conn(
+    family: int, server: str, port: int, flowinfo: int = 0, scopeid: int = 0
+) -> tuple:
+    """
+    Return formatted socket connection string.
+
+    :param int family: IP family (AF_INET, AF_INET6)
+    :param str server: server
+    :param int port: port
+    :param int flowinfo: flow info (0)
+    :param int scopeid: scope ID (0)
+    :return: connection tuple
+    :rtype: tuple
+    """
+
+    if family == AF_INET6:
+        return (server, port, flowinfo, scopeid)
+    if family == AF_INET:
+        return (server, port)
+    raise ValueError(f"Invalid family value {family}")
+
+
+def ipprot2int(family: str) -> int:
+    """
+    Convert IP family string to integer.
+
+    :param str family: family string ("IPv4", "IPv6")
+    :return: value as int AF_INET, AF_INET6
+    :rtype: int
+    """
+
+    if family == "IPv4":
+        return AF_INET
+    if family == "IPv6":
+        return AF_INET6
+    raise ValueError(f"Invalid family value {family}")
+
+
+def ipprot2str(family: int) -> str:
+    """
+    Convert IP family integer to string.
+
+    :param str family: family int (AF_INET, AF_INET6)
+    :return: value as str ("IPv4", "IPv6")
+    :rtype: int
+    """
+
+    if family == AF_INET:
+        return "IPv4"
+    if family == AF_INET6:
+        return "IPv6"
+    raise ValueError(f"Invalid family value {family}")
```

### Comparing `pygnssutils-1.0.7/src/pygnssutils/socket_server.py` & `pygnssutils-1.0.8/src/pygnssutils/socket_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from os import getenv
 from queue import Queue
 from socketserver import StreamRequestHandler, ThreadingTCPServer
 from threading import Event, Thread
 
 from pygnssutils._version import __version__ as VERSION
 from pygnssutils.globals import CONNECTED, DISCONNECTED
+from pygnssutils.helpers import ipprot2int
 
 # from pygpsclient import version as PYGPSVERSION
 
 RTCM = b"rtcm"
 BUFSIZE = 1024
 PYGPSMP = "pygnssutils"
 
@@ -55,14 +56,15 @@
     def __init__(
         self, app, ntripmode: int, maxclients: int, msgqueue: Queue, *args, **kwargs
     ):
         """
         Overridden constructor.
 
         :param Frame app: reference to main application class (if any)
+        :param str ipprot: IP protocol family (IPv4, IPv6)
         :param int ntripmode: 0 = open socket server, 1 = NTRIP server
         :param int maxclients: max no of clients allowed
         :param Queue msgqueue: queue containing raw GNSS messages
         """
 
         self.__app = app  # Reference to main application class
 
@@ -74,15 +76,15 @@
         self._stopmqread = Event()
         # set up pool of client queues
         self.clientqueues = []
         for _ in range(self._maxclients):
             self.clientqueues.append({"client": None, "queue": Queue()})
         self._start_read_thread()
         self.daemon_threads = True  # stops deadlock on abrupt termination
-
+        self.address_family = ipprot2int(kwargs.pop("ipprot", "IPv4"))
         super().__init__(*args, **kwargs)
 
     def server_close(self):
         """
         Overridden server close routine.
         """
```

### Comparing `pygnssutils-1.0.7/src/pygnssutils/ubxload.py` & `pygnssutils-1.0.8/src/pygnssutils/ubxload.py`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.7/src/pygnssutils/ubxsave.py` & `pygnssutils-1.0.8/src/pygnssutils/ubxsave.py`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.7/src/pygnssutils/ubxsetrate.py` & `pygnssutils-1.0.8/src/pygnssutils/ubxsetrate.py`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.7/src/pygnssutils.egg-info/PKG-INFO` & `pygnssutils-1.0.8/src/pygnssutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygnssutils
-Version: 1.0.7
+Version: 1.0.8
 Summary: GNSS Command Line Utilities
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2020, SEMU Consulting
         All rights reserved.
```

### Comparing `pygnssutils-1.0.7/src/pygnssutils.egg-info/SOURCES.txt` & `pygnssutils-1.0.8/src/pygnssutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.7/tests/test_gnssdump.py` & `pygnssutils-1.0.8/tests/test_gnssdump.py`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.7/tests/test_sourcetable.py` & `pygnssutils-1.0.8/tests/test_sourcetable.py`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.7/tests/test_static.py` & `pygnssutils-1.0.8/tests/test_static.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,18 +6,26 @@
 *** NB: must be saved in UTF-8 format ***
 
 @author: semuadmin
 """
 # pylint: disable=line-too-long, invalid-name, missing-docstring, no-member
 
 import unittest
-
+from socket import AF_INET, AF_INET6
 from pyubx2 import UBXReader, itow2utc
 
-from pygnssutils.helpers import cel2cart, find_mp_distance, format_json, get_mp_distance
+from pygnssutils.helpers import (
+    cel2cart,
+    find_mp_distance,
+    format_conn,
+    ipprot2int,
+    ipprot2str,
+    format_json,
+    get_mp_distance,
+)
 from tests.test_sourcetable import TESTSRT
 
 
 class StaticTest(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
         # dirname = os.path.dirname(__file__)
@@ -116,11 +124,39 @@
     def testgetmpdist3(self):  # invalid coords
         mp = TESTSRT[12]
         lat = ""
         lon = ""
         res = get_mp_distance(lat, lon, mp)
         self.assertEqual(res, None)
 
+    def testformatconn(self):  # test format connection string
+        res = format_conn(AF_INET, "192.168.0.23", 50010)
+        self.assertEqual(res, ("192.168.0.23", 50010))
+        res = format_conn(AF_INET6, "fe80::5f:89a3:300f:2dfa%en0", 50010)
+        self.assertEqual(res, ("fe80::5f:89a3:300f:2dfa%en0", 50010, 0, 0))
+        res = format_conn(AF_INET6, "fe80::5f:89a3:300f:2dfa%en0", 50010, 3456, 12)
+        self.assertEqual(res, ("fe80::5f:89a3:300f:2dfa%en0", 50010, 3456, 12))
+
+    def testformatconnerr(self):  # test format connection string
+        with self.assertRaisesRegex(ValueError, "Invalid family value 99"):
+            format_conn(99, "192.168.0.23", 50010)
+
+    def testipprot2int(self):  # test IP family to int
+        self.assertEqual(AF_INET, ipprot2int("IPv4"))
+        self.assertEqual(AF_INET6, ipprot2int("IPv6"))
+
+    def testipprot2interr(self):  # test IP family to int invalid
+        with self.assertRaisesRegex(ValueError, "Invalid family value IPv99"):
+            ipprot2int("IPv99")
+
+    def testipprot2str(self):  # test IP family to str
+        self.assertEqual("IPv4", ipprot2str(AF_INET))
+        self.assertEqual("IPv6", ipprot2str(AF_INET6))
+
+    def testipprot2strerr(self):  # test IP family to str invalid
+        with self.assertRaisesRegex(ValueError, "Invalid family value 99"):
+            ipprot2str(99)
+
 
 if __name__ == "__main__":
     # import sys;sys.argv = ['', 'Test.testName']
     unittest.main()
```

### Comparing `pygnssutils-1.0.7/tests/test_stream.py` & `pygnssutils-1.0.8/tests/test_stream.py`

 * *Files identical despite different names*

