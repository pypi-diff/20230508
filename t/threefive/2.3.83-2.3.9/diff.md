# Comparing `tmp/threefive-2.3.83.tar.gz` & `tmp/threefive-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threefive-2.3.83.tar", last modified: Mon May  8 17:48:40 2023, max compression
+gzip compressed data, was "threefive-2.3.9.tar", last modified: Sat Nov 27 23:24:29 2021, max compression
```

## Comparing `threefive-2.3.83.tar` & `threefive-2.3.9.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-08 17:48:40.322925 threefive-2.3.83/
--rw-r--r--   0 a         (1000) a         (1000)     1074 2023-03-31 20:38:41.000000 threefive-2.3.83/LICENSE
--rw-r--r--   0 a         (1000) a         (1000)    12937 2023-05-08 17:48:40.322925 threefive-2.3.83/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)    12366 2023-05-08 17:39:17.000000 threefive-2.3.83/README.md
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-08 17:48:40.314925 threefive-2.3.83/bin/
--rwxr-xr-x   0 a         (1000) a         (1000)      667 2023-03-31 20:38:41.000000 threefive-2.3.83/bin/threefive
--rw-r--r--   0 a         (1000) a         (1000)       38 2023-05-08 17:48:40.322925 threefive-2.3.83/setup.cfg
--rw-r--r--   0 a         (1000) a         (1000)     1026 2023-03-31 20:38:41.000000 threefive-2.3.83/setup.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-08 17:48:40.318925 threefive-2.3.83/threefive/
--rw-r--r--   0 a         (1000) a         (1000)      628 2023-03-31 20:38:41.000000 threefive-2.3.83/threefive/__init__.py
--rw-r--r--   0 a         (1000) a         (1000)     2873 2023-03-31 20:38:41.000000 threefive-2.3.83/threefive/base.py
--rw-r--r--   0 a         (1000) a         (1000)     4790 2023-05-08 17:39:17.000000 threefive-2.3.83/threefive/bitn.py
--rw-r--r--   0 a         (1000) a         (1000)     4211 2023-04-15 23:26:40.000000 threefive-2.3.83/threefive/cmd.py
--rw-r--r--   0 a         (1000) a         (1000)    11730 2023-05-08 17:39:17.000000 threefive-2.3.83/threefive/commands.py
--rw-r--r--   0 a         (1000) a         (1000)     4091 2023-04-17 21:47:35.000000 threefive-2.3.83/threefive/commands2.py
--rw-r--r--   0 a         (1000) a         (1000)      846 2023-03-31 20:38:41.000000 threefive-2.3.83/threefive/crc.py
--rw-r--r--   0 a         (1000) a         (1000)    10706 2023-04-30 20:57:21.000000 threefive-2.3.83/threefive/cue.py
--rw-r--r--   0 a         (1000) a         (1000)     1837 2023-03-31 20:38:41.000000 threefive-2.3.83/threefive/decode.py
--rw-r--r--   0 a         (1000) a         (1000)    13805 2023-05-08 17:39:17.000000 threefive-2.3.83/threefive/descriptors.py
--rw-r--r--   0 a         (1000) a         (1000)     2719 2023-03-31 20:38:41.000000 threefive-2.3.83/threefive/encode.py
--rw-r--r--   0 a         (1000) a         (1000)     1038 2023-03-31 20:38:41.000000 threefive-2.3.83/threefive/packetdata.py
--rw-r--r--   0 a         (1000) a         (1000)     5709 2023-03-31 20:38:41.000000 threefive-2.3.83/threefive/section.py
--rw-r--r--   0 a         (1000) a         (1000)     2972 2023-03-31 20:38:41.000000 threefive-2.3.83/threefive/segment.py
--rw-r--r--   0 a         (1000) a         (1000)     1970 2023-03-31 20:38:41.000000 threefive-2.3.83/threefive/segmentation.py
--rw-r--r--   0 a         (1000) a         (1000)     1660 2023-03-31 20:38:41.000000 threefive-2.3.83/threefive/smoketest.py
--rw-r--r--   0 a         (1000) a         (1000)    17492 2023-03-31 20:38:41.000000 threefive-2.3.83/threefive/stream.py
--rw-r--r--   0 a         (1000) a         (1000)      199 2023-03-31 20:38:41.000000 threefive-2.3.83/threefive/stuff.py
--rw-r--r--   0 a         (1000) a         (1000)     6505 2023-03-31 20:38:41.000000 threefive-2.3.83/threefive/upids.py
--rw-r--r--   0 a         (1000) a         (1000)       43 2023-05-08 17:39:17.000000 threefive-2.3.83/threefive/version.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-08 17:48:40.322925 threefive-2.3.83/threefive.egg-info/
--rw-r--r--   0 a         (1000) a         (1000)    12937 2023-05-08 17:48:40.000000 threefive-2.3.83/threefive.egg-info/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)      617 2023-05-08 17:48:40.000000 threefive-2.3.83/threefive.egg-info/SOURCES.txt
--rw-r--r--   0 a         (1000) a         (1000)        1 2023-05-08 17:48:40.000000 threefive-2.3.83/threefive.egg-info/dependency_links.txt
--rw-r--r--   0 a         (1000) a         (1000)       24 2023-05-08 17:48:40.000000 threefive-2.3.83/threefive.egg-info/requires.txt
--rw-r--r--   0 a         (1000) a         (1000)       10 2023-05-08 17:48:40.000000 threefive-2.3.83/threefive.egg-info/top_level.txt
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2021-11-27 23:24:29.638433 threefive-2.3.9/
+-rw-r--r--   0 a         (1000) a         (1000)    19018 2021-11-27 23:24:29.638433 threefive-2.3.9/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)    14493 2021-11-27 18:18:35.000000 threefive-2.3.9/README.md
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2021-11-27 23:24:29.634432 threefive-2.3.9/exp-js/
+-rw-r--r--   0 a         (1000) a         (1000)      558 2021-10-02 16:42:08.000000 threefive-2.3.9/exp-js/__init__.py
+-rw-r--r--   0 a         (1000) a         (1000)     1957 2021-11-09 22:25:03.000000 threefive-2.3.9/exp-js/base.py
+-rw-r--r--   0 a         (1000) a         (1000)     4581 2021-09-27 02:46:37.000000 threefive-2.3.9/exp-js/bitn.py
+-rw-r--r--   0 a         (1000) a         (1000)    10529 2021-10-09 10:22:11.000000 threefive-2.3.9/exp-js/commands.py
+-rw-r--r--   0 a         (1000) a         (1000)     5676 2021-11-22 23:44:03.000000 threefive-2.3.9/exp-js/cue.py
+-rw-r--r--   0 a         (1000) a         (1000)    12952 2021-10-09 06:32:28.000000 threefive-2.3.9/exp-js/descriptors.py
+-rw-r--r--   0 a         (1000) a         (1000)      257 2021-10-03 09:12:58.000000 threefive-2.3.9/exp-js/reader.py
+-rw-r--r--   0 a         (1000) a         (1000)     5690 2021-09-25 05:27:38.000000 threefive-2.3.9/exp-js/section.py
+-rw-r--r--   0 a         (1000) a         (1000)     1586 2021-08-24 15:22:16.000000 threefive-2.3.9/exp-js/segmentation.py
+-rw-r--r--   0 a         (1000) a         (1000)     5363 2021-10-09 02:44:37.000000 threefive-2.3.9/exp-js/upid.py
+-rw-r--r--   0 a         (1000) a         (1000)      590 2021-11-08 13:04:50.000000 threefive-2.3.9/exp-js/version.py
+-rw-r--r--   0 a         (1000) a         (1000)       38 2021-11-27 23:24:29.638433 threefive-2.3.9/setup.cfg
+-rw-r--r--   0 a         (1000) a         (1000)     1056 2021-10-01 15:20:13.000000 threefive-2.3.9/setup.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2021-11-27 23:24:29.634432 threefive-2.3.9/threefive/
+-rw-r--r--   0 a         (1000) a         (1000)      558 2021-10-02 16:42:08.000000 threefive-2.3.9/threefive/__init__.py
+-rw-r--r--   0 a         (1000) a         (1000)     1967 2021-10-08 21:03:11.000000 threefive-2.3.9/threefive/base.py
+-rw-r--r--   0 a         (1000) a         (1000)     4581 2021-09-27 02:46:37.000000 threefive-2.3.9/threefive/bitn.py
+-rw-r--r--   0 a         (1000) a         (1000)    10854 2021-11-17 03:47:48.000000 threefive-2.3.9/threefive/commands.py
+-rw-r--r--   0 a         (1000) a         (1000)    10021 2021-11-27 18:18:33.000000 threefive-2.3.9/threefive/cue.py
+-rw-r--r--   0 a         (1000) a         (1000)     3187 2021-11-27 23:22:53.000000 threefive-2.3.9/threefive/decode.py
+-rw-r--r--   0 a         (1000) a         (1000)    12952 2021-10-09 06:32:28.000000 threefive-2.3.9/threefive/descriptors.py
+-rw-r--r--   0 a         (1000) a         (1000)      932 2021-10-04 01:49:55.000000 threefive-2.3.9/threefive/packetdata.py
+-rw-r--r--   0 a         (1000) a         (1000)      257 2021-10-03 09:12:58.000000 threefive-2.3.9/threefive/reader.py
+-rw-r--r--   0 a         (1000) a         (1000)     5690 2021-11-24 16:23:39.000000 threefive-2.3.9/threefive/section.py
+-rw-r--r--   0 a         (1000) a         (1000)     2805 2021-11-24 16:16:42.000000 threefive-2.3.9/threefive/segment.py
+-rw-r--r--   0 a         (1000) a         (1000)     1586 2021-08-24 15:22:16.000000 threefive-2.3.9/threefive/segmentation.py
+-rw-r--r--   0 a         (1000) a         (1000)     1631 2021-10-08 19:09:37.000000 threefive-2.3.9/threefive/smoketest.py
+-rw-r--r--   0 a         (1000) a         (1000)    15791 2021-11-27 23:22:43.000000 threefive-2.3.9/threefive/stream.py
+-rw-r--r--   0 a         (1000) a         (1000)     5363 2021-10-09 02:44:37.000000 threefive-2.3.9/threefive/upid.py
+-rw-r--r--   0 a         (1000) a         (1000)      590 2021-11-27 23:22:32.000000 threefive-2.3.9/threefive/version.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2021-11-27 23:24:29.638433 threefive-2.3.9/threefive.egg-info/
+-rw-r--r--   0 a         (1000) a         (1000)    19018 2021-11-27 23:24:29.000000 threefive-2.3.9/threefive.egg-info/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)      713 2021-11-27 23:24:29.000000 threefive-2.3.9/threefive.egg-info/SOURCES.txt
+-rw-r--r--   0 a         (1000) a         (1000)        1 2021-11-27 23:24:29.000000 threefive-2.3.9/threefive.egg-info/dependency_links.txt
+-rw-r--r--   0 a         (1000) a         (1000)       13 2021-11-27 23:24:29.000000 threefive-2.3.9/threefive.egg-info/requires.txt
+-rw-r--r--   0 a         (1000) a         (1000)       17 2021-11-27 23:24:29.000000 threefive-2.3.9/threefive.egg-info/top_level.txt
```

### Comparing `threefive-2.3.83/setup.py` & `threefive-2.3.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 #!/usr/bin/env python3
 
 import setuptools
+import threefive
 
-with open("README.md", "r", encoding="utf-8") as fh:
+with open("README.md", "r") as fh:
     readme = fh.read()
 
-with open("threefive/version.py","r", encoding="utf-8") as latest:
-    version = latest.read().split("'")[1]
-
 setuptools.setup(
     name="threefive",
-    version=version,
-    author="Adrian and a Cast of Thousands.",
-    author_email="spam@iodisco.com",
-    description="Pythonic SCTE35",
+    version=threefive.version(),
+    author="Adrian Thiele, Vlad Doster, James Fining, Richard Van Dijk",
+    author_email="spam@so.slo.me",
+    description="Pythonic SCTE-35.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/futzu/threefive",
     install_requires=[
-        'new_reader >= 0.1.7',
+        "crcmod",
         "pyaes",
     ],
-
-    scripts=['bin/threefive'],
     packages=setuptools.find_packages(),
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: Implementation :: PyPy",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
     ],
     python_requires=">=3.6",
 )
```

### Comparing `threefive-2.3.83/threefive/__init__.py` & `threefive-2.3.9/exp-js/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 threefive.__init__.py
 """
 
-from .stuff import print2
 from .cue import Cue
 from .decode import decode
+from .reader import reader
 from .section import SpliceInfoSection
 from .segment import Segment
 from .smoketest import smoke
 from .stream import Stream
-from .version import version
+from .version import version, version_number
 
 from .commands import (
     TimeSignal,
     SpliceInsert,
     SpliceNull,
     SpliceSchedule,
     PrivateCommand,
@@ -23,13 +23,7 @@
 from .descriptors import (
     AudioDescriptor,
     AvailDescriptor,
     DtmfDescriptor,
     SegmentationDescriptor,
     TimeDescriptor,
 )
-
-from .encode import (
-    mk_splice_null,
-    mk_splice_insert,
-    mk_time_signal,
-)
```

### Comparing `threefive-2.3.83/threefive/base.py` & `threefive-2.3.9/exp-js/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,67 +1,35 @@
 """
 threefive.base contains
 the class SCTE35Base.
 """
-import json
 from .bitn import NBin
 
 
 class SCTE35Base:
     """
     SCTE35Base is a base class for
     SpliceCommand and SpliceDescriptor classes
     """
 
-    ROLLOVER = 8589934591
-
     def __repr__(self):
         return str(self.__dict__)
 
     @staticmethod
-    def as_90k(int_time):
-        """
-        ticks to 90k timestamps
-        """
-        return round((int_time / 90000.0), 6)
-
-    @staticmethod
-    def as_ticks(float_time):
-        """
-        90k timestamps to ticks
-        """
-        return int(round(float_time * 90000))
-
-    @staticmethod
-    def as_hms(secs_of_time):
-        """
-        as_hms converts timestamp to
-        00:00:00.000 format
-        """
-        hours, seconds = divmod(secs_of_time, 3600)
-        mins, seconds = divmod(seconds, 60)
-        seconds = round(seconds, 3)
-        output = f"{int(hours):02}:{int(mins):02}:{seconds:02}"
-        if len(output.split(".")[1]) < 2:
-            output += "0"
-        return output
+    def _chk_nbin(nbin):
+        if not nbin:
+            nbin = NBin()
+        return nbin
 
     def get(self):
         """
         Returns instance as a dict
         """
         return self.kv_clean()
 
-    def get_json(self):
-        """
-        get_json returns the instance
-        data as json.
-        """
-        return json.dumps(self.get(), indent=4)
-
     def kv_clean(self):
         """
         kv_clean removes items from a dict if the value is None
         """
 
         def b2l(val):
             if isinstance(val, (SCTE35Base)):
@@ -72,27 +40,21 @@
                 val = {k: b2l(v) for k, v in val.items()}
             if isinstance(val, (bytes, bytearray)):
                 val = list(val)
             return val
 
         return {k: b2l(v) for k, v in vars(self).items() if v is not None}
 
-    @staticmethod
-    def _chk_nbin(nbin):
-        if not nbin:
-            nbin = NBin()
-        return nbin
-
     def load(self, stuff):
         """
         load is used to load
         data from a dict or json string
         """
-        if isinstance(stuff, str):
-            stuff = json.loads(stuff)
+        #if isinstance(stuff, str):
+           # stuff = json.loads(stuff)
         if isinstance(stuff, dict):
             self.__dict__.update(stuff)
 
     def _chk_var(self, var_type, nbin_method, var_name, bit_count):
         """
         _chk_var is used to check var values and types before encoding
         """
```

### Comparing `threefive-2.3.83/threefive/bitn.py` & `threefive-2.3.9/exp-js/bitn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 The bitn.BitBin and bitn.NBin classes
 """
 
 
-from .stuff import print2
+import sys
 
 
 class BitBin:
     """
     bitn.Bitbin takes a byte string and
     converts it to a integer, a very large integer
     if needed. A 1500 bit integer is no problem.
@@ -31,39 +31,33 @@
         """
         Starting at self.idx of self.bits,
         slice off num_bits of bits.
         """
         if self.idx >= num_bits:
             self.idx -= num_bits
             return (self.bits >> (self.idx)) & ~(~0 << num_bits)
-        # return self.negative_shift(num_bits)
+        return self.negative_shift(num_bits)
 
     def as_hex(self, num_bits):
         """
         Returns the hex value
         of num_bits of bits
         """
         return hex(self.as_int(num_bits))
 
-    def as_charset(self, num_bits, charset="ascii"):
+    def as_ascii(self, num_bits):
         """
         Returns num_bits of bits
-        as bytes decoded as charset
-        default charset is ascii.
+        as bytes decoded to as_ascii
         """
-        # print(charset)
         stuff = self.as_int(num_bits)
         wide = num_bits >> 3
-        if charset is None:
-            return int.to_bytes(stuff, wide, byteorder="big")
-        return int.to_bytes(stuff, wide, byteorder="big").decode(
-            charset, errors="replace"
-        )
+        return int.to_bytes(stuff, wide, byteorder="big").decode()
 
-    def as_bytes(self, num_bits):
+    def as_raw(self, num_bits):
         """
         Returns num_bits of bits
         as bytes
         """
         stuff = self.as_int(num_bits)
         wide = num_bits >> 3
         return int.to_bytes(stuff, wide, byteorder="big")
@@ -82,19 +76,21 @@
         self.idx -= num_bits
 
     def negative_shift(self, num_bits):
         """
         negative_shift is called instead of
         throwing a negative shift count error.
         """
-        print2(
-            f"{num_bits} bits requested, but only {self.idx} bits left."
+        print(
+            f"{num_bits} bits requested, but only {self.idx} bits left.",
+            file=sys.stderr,
         )
-        print2(
-            f"\n bytes remaining: {self.as_bytes(self.idx)} "
+        print(
+            f"\n bytes remaining: {self.as_raw(self.idx)} ",
+            file=sys.stderr,
         )
 
 
 class NBin:
     """
     bitn.NBin is
     the reverse BitBin.
@@ -120,17 +116,15 @@
 
     def add_bites(self, plus_bites):
         """
         add_bites appends plus_bites
         to self.bites
         """
         self.bites += plus_bites
-
-    #  if self.idx % 8 == 0:
-    #     self.nbits2bites()
+        self.nbits2bites()
 
     def add_int(self, int_bits, bit_len):
         """
         left shift nbits and append new_bits
         """
         self.idx += bit_len
         self.nbits = (self.nbits << bit_len) | int_bits
```

### Comparing `threefive-2.3.83/threefive/commands.py` & `threefive-2.3.9/threefive/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class SpliceCommand(SCTE35Base):
     """
     Base class, not used directly.
     """
 
     def __init__(self, bites=None):
-        self.command_length = 0
+        self.command_length = None
         self.command_type = None
         self.name = None
         self.bites = bites
 
     def decode(self):
         """
         default decode method
@@ -99,15 +99,14 @@
 
     def __init__(self, bites=None):
         super().__init__(bites)
         self.command_type = 6
         self.name = "Time Signal"
         self.time_specified_flag = None
         self.pts_time = None
-        self.pts_time_ticks = None
 
     def decode(self):
         """
         TimeSignal.decode method
         """
         bitbin = BitBin(self.bites)
         start = bitbin.idx
@@ -128,31 +127,23 @@
         parse_pts is called by either a
         TimeSignal or SpliceInsert instance
         to decode pts.
         """
         self.time_specified_flag = bitbin.as_flag(1)
         if self.time_specified_flag:
             bitbin.forward(6)
-            self.pts_time_ticks = bitbin.as_int(33)
-            self.pts_time = self.as_90k(self.pts_time_ticks)
+            self.pts_time = bitbin.as_90k(33)
         else:
             bitbin.forward(7)
 
     def _encode_splice_time(self, nbin):
         self._chk_var(bool, nbin.add_flag, "time_specified_flag", 1)
         if self.time_specified_flag:
             nbin.reserve(6)
-            if not self.pts_time and not self.pts_time_ticks:
-                err_mesg = ' self.time_specified_flag is set. Please set self.pts_time ( float )  or self.pts_time_ticks ( int  )'
-                raise ValueError(err_mesg)
-            if not self.pts_time_ticks:
-                self.pts_time_ticks = self.as_ticks(self.pts_time)
-            if not self.pts_time:
-                self.pts_time = self.as_90k(self.pts_time_ticks)
-            self._chk_var(int, nbin.add_int, "pts_time_ticks", 33)
+            self._chk_var(float, nbin.add_90k, "pts_time", 33)
         else:
             nbin.reserve(7)
 
 
 class SpliceInsert(TimeSignal):
     """
     Table 9 - splice_insert()
@@ -160,163 +151,157 @@
 
     def __init__(self, bites=None):
         super().__init__(bites)
         self.command_type = 5
         self.name = "Splice Insert"
         self.break_auto_return = None
         self.break_duration = None
-        self.break_duration_ticks = None
         self.splice_event_id = None
         self.splice_event_cancel_indicator = None
         self.out_of_network_indicator = None
         self.program_splice_flag = None
         self.duration_flag = None
         self.splice_immediate_flag = None
         self.component_count = None
         self.components = None
         self.unique_program_id = None
         self.avail_num = None
         self.avail_expected = None
 
-    def decode(self):
-        """
-        SpliceInsert.decode
-        """
-        bitbin = BitBin(self.bites)
-        start = bitbin.idx
-        self._decode_event(bitbin)
-        if not self.splice_event_cancel_indicator:
-            self._decode_flags(bitbin)
-            if self.program_splice_flag:
-                if not self.splice_immediate_flag:
-                    self._splice_time(bitbin)
-            else:
-                self._decode_components(bitbin)
-                if not self.splice_immediate_flag:
-                    self._splice_time(bitbin)
-            self._decode_break(bitbin)
-            self._decode_unique_avail(bitbin)
-        self._set_len(start, bitbin.idx)
-
     def _decode_break(self, bitbin):
         """
         SpliceInsert._decode_break(bitbin) is called
         if SpliceInsert.duration_flag is set
         """
         if self.duration_flag:
             self.break_auto_return = bitbin.as_flag(1)
             bitbin.forward(6)
-            self.break_duration_ticks = bitbin.as_int(33)
-            self.break_duration = self.as_90k(self.break_duration_ticks)
+            self.break_duration = bitbin.as_90k(33)
 
-    def _decode_components(self, bitbin):
+    def _encode_break(self, nbin):
         """
-        SpliceInsert._decode_components loops
-        over SpliceInsert.components,
-        and is called from SpliceInsert.decode()
+        SpliceInsert._encode_break(nbin) is called
+        if SpliceInsert.duration_flag is set
         """
-        self.component_count = bitbin.as_int(8)
-        self.components = []
-        for i in range(0, self.component_count):
-            self.components[i] = bitbin.as_int(8)
+        if self.duration_flag:
+            self._chk_var(bool, nbin.add_flag, "break_auto_return", 1)
+            nbin.forward(6)
+            self._chk_var(float, nbin.add_90k, "break_duration", 33)
 
     def _decode_event(self, bitbin):
         """
         SpliceInsert._decode_event parses
         self.splice_event_id and self.splice_event_cancel_indicator
         and is called from SpliceInsert.decode()
         """
         self.splice_event_id = bitbin.as_int(32)
         self.splice_event_cancel_indicator = bitbin.as_flag(1)
         bitbin.forward(7)
 
-    def _decode_flags(self, bitbin):
-        """
-        SpliceInsert._decode_flags parses four bit flags
-        """
-        self.out_of_network_indicator = bitbin.as_flag(1)
-        self.program_splice_flag = bitbin.as_flag(1)
-        self.duration_flag = bitbin.as_flag(1)
-        self.splice_immediate_flag = bitbin.as_flag(1)
-        bitbin.forward(4)
-
-    def _decode_unique_avail(self, bitbin):
-        self.unique_program_id = bitbin.as_int(16)
-        self.avail_num = bitbin.as_int(8)
-        self.avail_expected = bitbin.as_int(8)
-
-    def encode(self, nbin=None):
-        """
-        SpliceInsert.encode
-        """
-        nbin = self._chk_nbin(nbin)
-        self._encode_event(nbin)
-        if not self.splice_event_cancel_indicator:
-            self._encode_flags(nbin)
-            if self.program_splice_flag:
-                if not self.splice_immediate_flag:
-                    self._encode_splice_time(nbin)
-            else:
-                self._encode_components(nbin)
-                if not self.splice_immediate_flag:
-                    self._encode_splice_time(nbin)
-            self._encode_break(nbin)
-            self._encode_unique_avail(nbin)
-        return nbin.bites
-
     def _encode_event(self, nbin):
         """
         SpliceInsert._encode_event encodes
         self.splice_event_id and self.splice_event_cancel_indicator
         and is called from SpliceInsert.encode()
         """
         self._chk_var(int, nbin.add_int, "splice_event_id", 32)
         self._chk_var(bool, nbin.add_flag, "splice_event_cancel_indicator", 1)
         nbin.forward(7)
 
-    def _encode_break(self, nbin):
+    def _decode_flags(self, bitbin):
         """
-        SpliceInsert._encode_break(nbin) is called
-        if SpliceInsert.duration_flag is set
+        SpliceInsert._decode_flags parses four bit flags
         """
-        if self.duration_flag:
-            self._chk_var(bool, nbin.add_flag, "break_auto_return", 1)
-            nbin.forward(6)
-            if not self.break_duration_ticks:
-                self.break_duration_ticks = 0
-            if self.break_duration:
-                self.break_duration_ticks = self.as_ticks(self.break_duration)
-            self._chk_var(int, nbin.add_int, "break_duration_ticks", 33)
+        self.out_of_network_indicator = bitbin.as_flag(1)
+        self.program_splice_flag = bitbin.as_flag(1)
+        self.duration_flag = bitbin.as_flag(1)
+        self.splice_immediate_flag = bitbin.as_flag(1)
+        bitbin.forward(4)
 
     def _encode_flags(self, nbin):
         """
         SpliceInsert._encode_flags converts four flags
         to bits
         """
         self._chk_var(bool, nbin.add_flag, "out_of_network_indicator", 1)
         self._chk_var(bool, nbin.add_flag, "program_splice_flag", 1)
         self._chk_var(bool, nbin.add_flag, "duration_flag", 1)
         self._chk_var(bool, nbin.add_flag, "splice_immediate_flag", 1)
         nbin.forward(4)
 
+    def _decode_components(self, bitbin):
+        """
+        SpliceInsert._decode_components loops
+        over SpliceInsert.components,
+        and is called from SpliceInsert.decode()
+        """
+        self.component_count = bitbin.as_int(8)
+        self.components = []
+        for i in range(0, self.component_count):
+            self.components[i] = bitbin.as_int(8)
+
     def _encode_components(self, nbin):
         """
         SpliceInsert._encode_components loops
         over SpliceInsert.components,
         and is called from SpliceInsert.encode()
         """
         nbin.add_int(self.component_count, 8)
         for i in range(0, self.component_count):
             nbin.add_int(self.components[i], 8)
 
+    def _decode_unique_avail(self, bitbin):
+        self.unique_program_id = bitbin.as_int(16)
+        self.avail_num = bitbin.as_int(8)
+        self.avail_expected = bitbin.as_int(8)
+
     def _encode_unique_avail(self, nbin):
         self._chk_var(int, nbin.add_int, "unique_program_id", 16)
         self._chk_var(int, nbin.add_int, "avail_num", 8)
         self._chk_var(int, nbin.add_int, "avail_expected", 8)
 
+    def decode(self):
+        """
+        SpliceInsert.decode
+        """
+        bitbin = BitBin(self.bites)
+        start = bitbin.idx
+        self._decode_event(bitbin)
+        if not self.splice_event_cancel_indicator:
+            self._decode_flags(bitbin)
+            if self.program_splice_flag:
+                if not self.splice_immediate_flag:
+                    self._splice_time(bitbin)
+            else:
+                self._decode_components(bitbin)
+                if not self.splice_immediate_flag:
+                    self._splice_time(bitbin)
+            self._decode_break(bitbin)
+            self._decode_unique_avail(bitbin)
+        self._set_len(start, bitbin.idx)
+
+    def encode(self, nbin=None):
+        """
+        SpliceInsert.encode
+        """
+        nbin = self._chk_nbin(nbin)
+        self._encode_event(nbin)
+        if not self.splice_event_cancel_indicator:
+            self._encode_flags(nbin)
+            if self.program_splice_flag:
+                if not self.splice_immediate_flag:
+                    self._encode_splice_time(nbin)
+            else:
+                self._encode_components(nbin)
+                if not self.splice_immediate_flag:
+                    self._encode_splice_time(nbin)
+            self._encode_break(nbin)
+            self._encode_unique_avail(nbin)
+        return nbin.bites
+
 
 class SpliceSchedule(SpliceCommand):
     """
     Table 8 - splice_schedule()
     """
 
     class SpliceEvent(SpliceInsert):
```

### Comparing `threefive-2.3.83/threefive/cue.py` & `threefive-2.3.9/threefive/cue.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 threefive.Cue Class
 """
 from base64 import b64decode, b64encode
 import json
-from .stuff import print2
+from sys import stderr
+import crcmod.predefined
 from .bitn import NBin
 from .base import SCTE35Base
 from .section import SpliceInfoSection
-from .commands import command_map, SpliceCommand
+from .commands import command_map
 from .descriptors import splice_descriptor, descriptor_map
-from .crc import crc32
 
 
 class Cue(SCTE35Base):
     """
     The threefive.Splice class handles parsing
     SCTE 35 message strings.
     Example usage:
@@ -43,53 +43,168 @@
     """
 
     def __init__(self, data=None, packet_data=None):
         """
         data may be packet bites or encoded string
         packet_data is a instance passed from a Stream instance
         """
-        self.bites = None
         if data:
             self.bites = self._mk_bits(data)
         self.info_section = SpliceInfoSection()
         self.command = None
         self.descriptors = []
         self.packet_data = packet_data
 
-    def __repr__(self):
-        return str(self.__dict__)
-
-    # decode
-
     def decode(self):
         """
         Cue.decode() parses for SCTE35 data
         """
-        bites = self.bites
         self.descriptors = []
-        while bites:
-            bites = self.mk_info_section(bites)
-            bites = self._set_splice_command(bites)
-            bites = self._mk_descriptors(bites)
-            crc = hex(int.from_bytes(bites[0:4], byteorder="big"))
-            self.info_section.crc = crc
-            return True
+        # self.bites after_info section decoding
+        after_info = self.mk_info_section(self.bites)
+        # self.bites = self.bites[0 : self.info_section.section_length + 3]
+        if after_info:
+            after_cmd = self._set_splice_command(after_info)
+            if after_cmd:
+                after_dscrptrs = self._mk_descriptors(after_cmd)
+                if after_dscrptrs:
+                    crc = hex(int.from_bytes(after_dscrptrs[0:4], byteorder="big"))
+                    self.info_section.crc = crc
+                    return True
         return False
 
-    def _descriptor_loop(self, loop_bites):
+    def encode(self):
+        """
+        Cue.encode() converts SCTE35 data
+        to a base64 encoded string.
+        """
+        dscptr_bites = self._unloop_descriptors()
+        dll = len(dscptr_bites)
+        self.info_section.descriptor_loop_length = dll
+        if not self.command:
+            raise Exception("A splice command is required")
+        cmd_bites = self.command.encode()
+        cmdl = self.command.command_length = len(cmd_bites)
+        self.info_section.splice_command_length = cmdl
+        self.info_section.splice_command_type = self.command.command_type
+        # 11 bytes for info section + command + 2 descriptor loop length
+        # + descriptor loop + 4 for crc
+        self.info_section.section_length = 11 + cmdl + 2 + dll + 4
+        self.bites = self.info_section.encode()
+        self.bites += cmd_bites
+        self.bites += int.to_bytes(
+            self.info_section.descriptor_loop_length, 2, byteorder="big"
+        )
+        self.bites += dscptr_bites
+        self._encode_crc()
+        return b64encode(self.bites).decode()
+
+    def encode_as_hex(self):
+        """
+        encode_as_hex returns self.bites as
+        a hex string
+        """
+        self.encode()
+        return hex(int.from_bytes(self.bites, byteorder="big"))
+
+    def _encode_crc(self):
+        crc32_func = crcmod.predefined.mkCrcFun("crc-32-mpeg")
+        crc_int = crc32_func(self.bites)
+        self.info_section.crc = hex(crc_int)
+        self.bites += int.to_bytes(crc_int, 4, byteorder="big")
+
+    def load_info_section(self, isec):
+        """
+        load_info_section loads data for Cue.info_section
+        isec should be a dict.
+        if 'splice_command_type' is included,
+        an empty command instance will be created for Cue.command
+        """
+        self.info_section.load(isec)
+        if "splice_command_type" in isec:
+            cmd_type = isec["splice_command_type"]
+            command_map[cmd_type]()
+
+    def load_command(self, cmd):
+        """
+        load_command loads data for Cue.command
+        cmd should be a dict.
+        if 'command_type' is included,
+        the command instance will be created.
+        """
+        if "command_type" in cmd:
+            self.command = command_map[cmd["command_type"]]()
+        if self.command:
+            self.command.load(cmd)
+
+    def load_descriptors(self, dlist):
+        """
+        Load_descriptors loads descriptor data.
+        dlist is a list of dicts
+        if 'tag' is included in each dict,
+        a descriptor instance will be created.
+        """
+        if not isinstance(dlist, list):
+            raise Exception("descriptors should be a list")
+        for dstuff in dlist:
+            if "tag" in dstuff:
+                dscptr = descriptor_map[dstuff["tag"]]()
+                dscptr.load(dstuff)
+                self.descriptors.append(dscptr)
+
+    def load(self, stuff):
         """
-        Cue._descriptor_loop parses all splice descriptors
+        Cue.load loads SCTE35 data for encoding.
+        stuff is a dict or json
+        with any or all of these keys
+        stuff = {
+            'info_section': {dict} ,
+            'command': {dict},
+            'descriptors': [list of {dicts}],
+            }
         """
-        tag_n_len = 2
-        while loop_bites:
-            spliced = splice_descriptor(loop_bites)
+        if isinstance(stuff, str):
+            stuff = json.loads(stuff)
+        if "info_section" in stuff:
+            self.load_info_section(stuff["info_section"])
+        if "command" in stuff:
+            self.load_command(stuff["command"])
+        if "descriptors" in stuff:
+            self.load_descriptors(stuff["descriptors"])
+
+    def _unloop_descriptors(self):
+        """
+        _unloop_descriptors
+        for each descriptor in self.descriptors
+        encode descriptor tag, descriptor length,
+        and the descriptor into all_bites.bites
+        """
+        all_bites = NBin()
+        dbite_chunks = [dsptr.encode() for dsptr in self.descriptors]
+        for chunk, dsptr in zip(dbite_chunks, self.descriptors):
+            dsptr.descriptor_length = len(chunk)
+            all_bites.add_int(dsptr.tag, 8)
+            all_bites.add_int(dsptr.descriptor_length, 8)
+            all_bites.add_bites(chunk)
+        return all_bites.bites
+
+    def _descriptorloop(self, bites, dll):
+        """
+        Cue._descriptorloop parses all splice descriptors
+        """
+        tag_n_len_bites = 2  # 1 byte for descriptor tag,
+        # 1 byte for descriptor length
+        while dll:
+            spliced = splice_descriptor(bites)
             if not spliced:
                 return
-            sd_size = tag_n_len + spliced.descriptor_length
-            loop_bites = loop_bites[sd_size:]
+            sdl = spliced.descriptor_length
+            sd_size = tag_n_len_bites + sdl
+            dll -= sd_size
+            bites = bites[sd_size:]
             del spliced.bites
             self.descriptors.append(spliced)
 
     def get(self):
         """
         Cue.get returns the SCTE-35 Cue
         data as a dict of dicts.
@@ -122,20 +237,18 @@
     @staticmethod
     def _mk_bits(data):
         """
         cue._mk_bits Converts
         Hex and Base64 strings into bytes.
         """
         if isinstance(data, bytes):
-            return data[data.index(b"\xfc") :]
-        # handles int and unquoted hex
-        if isinstance(data, int):
-            length = data.bit_length() >> 3
-            bites = int.to_bytes(data, length, byteorder="big")
-            return bites
+            if data[0] == 0x0:
+                data = data[1:]
+            if data[0] == 0xFC:
+                return data
         try:
             # Handles hex byte strings
             i = int(data, 16)
             i_len = i.bit_length() >> 3
             bites = int.to_bytes(i, i_len, byteorder="big")
             return bites
         except (LookupError, TypeError, ValueError):
@@ -148,20 +261,23 @@
         except (LookupError, TypeError, ValueError):
             return data
 
     def _mk_descriptors(self, bites):
         """
         Cue._mk_descriptors parses
         Cue.info_section.descriptor_loop_length,
-        then call Cue._descriptor_loop
+        then call Cue._descriptorloop
         """
-        dll = (bites[0] << 8) | bites[1]
+        try:
+            dll = (bites[0] << 8) | bites[1]
+        except (LookupError, TypeError, ValueError):
+            return False
         self.info_section.descriptor_loop_length = dll
         bites = bites[2:]
-        self._descriptor_loop(bites[:dll])
+        self._descriptorloop(bites, dll)
         return bites[dll:]
 
     def mk_info_section(self, bites):
         """
         Cue.mk_info_section parses the
         Splice Info Section
         of a SCTE35 cue.
@@ -177,166 +293,23 @@
         the command section of a SCTE35 cue.
         """
         sct = self.info_section.splice_command_type
         if sct not in command_map:
             return False
         self.command = command_map[sct](bites)
         self.command.decode()
-        #self.command=SpliceCommand(bites)
-        #self.command.decode(sct)
-        #print(bites[self.command.command_length :])
         del self.command.bites
-        self.info_section.splice_command_length = self.command.command_length
         bites = bites[self.command.command_length :]
         return bites
 
     def show(self):
         """
         Cue.show prints the Cue as JSON
         """
-        print2(self.get_json())
+        print(self.get_json())
 
     def to_stderr(self):
         """
         Cue.to_stderr prints the Cue
         as JSON to sys.stderr
         """
-        # print(self.get_json(), file=stderr)
-        self.show()
-
-    # encode related
-
-    def encode(self):
-        """
-        Cue.encode() converts SCTE35 data
-        to a base64 encoded string.
-        """
-        dscptr_bites = self._unloop_descriptors()
-        dll = len(dscptr_bites)
-        self.info_section.descriptor_loop_length = dll
-        if not self.command:
-            err_mesg = "\033[7mA splice command is required\033[27m"
-            raise ValueError(err_mesg)
-        cmd_bites = self.command.encode()
-        cmdl = self.command.command_length = len(cmd_bites)
-        self.info_section.splice_command_length = cmdl
-        self.info_section.splice_command_type = self.command.command_type
-        # 11 bytes for info section + command + 2 descriptor loop length
-        # + descriptor loop + 4 for crc
-        self.info_section.section_length = 11 + cmdl + 2 + dll + 4
-        self.bites = self.info_section.encode()
-        self.bites += cmd_bites
-        self.bites += int.to_bytes(
-            self.info_section.descriptor_loop_length, 2, byteorder="big"
-        )
-        self.bites += dscptr_bites
-        self._encode_crc()
-        return b64encode(self.bites).decode()
-
-    def encode_as_int(self):
-        """
-        encode_as_int returns self.bites as an int.
-        """
-        self.encode()
-        return int.from_bytes(self.bites, byteorder="big")
-
-    def encode_as_hex(self):
-        """
-        encode_as_hex returns self.bites as
-        a hex string
-        """
-        return hex(self.encode_as_int())
-
-    def _encode_crc(self):
-        """
-        _encode_crc encode crc32
-        """
-        crc_int = crc32(self.bites)
-        self.info_section.crc = hex(crc_int)
-        self.bites += int.to_bytes(crc_int, 4, byteorder="big")
-
-    def _unloop_descriptors(self):
-        """
-        _unloop_descriptors
-        for each descriptor in self.descriptors
-        encode descriptor tag, descriptor length,
-        and the descriptor into all_bites.bites
-        """
-        all_bites = NBin()
-        dbite_chunks = [dsptr.encode() for dsptr in self.descriptors]
-        for chunk, dsptr in zip(dbite_chunks, self.descriptors):
-            dsptr.descriptor_length = len(chunk)
-            all_bites.add_int(dsptr.tag, 8)
-            all_bites.add_int(dsptr.descriptor_length, 8)
-            all_bites.add_bites(chunk)
-        return all_bites.bites
-
-    def load(self, stuff):
-        """
-        Cue.load loads SCTE35 data for encoding.
-        stuff is a dict or json
-        with any or all of these keys
-        stuff = {
-            'info_section': {dict} ,
-            'command': {dict},
-            'descriptors': [list of {dicts}],
-            }
-        """
-        if isinstance(stuff, str):
-            stuff = json.loads(stuff)
-        if "info_section" in stuff:
-            self.load_info_section(stuff["info_section"])
-        if "command" in stuff:
-            self.load_command(stuff["command"])
-        if "descriptors" in stuff:
-            self.load_descriptors(stuff["descriptors"])
-
-    def load_info_section(self, isec):
-        """
-        load_info_section loads data for Cue.info_section
-        isec should be a dict.
-        if 'splice_command_type' is included,
-        an empty command instance will be created for Cue.command
-        """
-        self.info_section.load(isec)
-        if "splice_command_type" in isec:
-            cmd_type = isec["splice_command_type"]
-            command_map[cmd_type]()
-
-    def load_command(self, cmd):
-        """
-        load_command loads data for Cue.command
-        cmd should be a dict.
-        if 'command_type' is included,
-        the command instance will be created.
-        """
-        if not isinstance(cmd, dict):
-            try:
-                cmd = cmd.get()
-            except:
-                print2(f" cmd is a {type(cmd)} should be a dict,")
-                return
-        if "command_type" in cmd:
-            self.command = command_map[cmd["command_type"]]()
-        if self.command:
-            self.command.load(cmd)
-
-    def load_descriptors(self, dlist):
-        """
-        Load_descriptors loads descriptor data.
-        dlist is a list of dicts
-        if 'tag' is included in each dict,
-        a descriptor instance will be created.
-        """
-        if not isinstance(dlist, list):
-            raise Exception("descriptors should be a list")
-        for dstuff in dlist:
-            if not isinstance(dstuff, dict):
-                try:
-                    dstuff = dstuff.get()
-                except:
-                    print(f" dstuff is a {type(dstuff)} should be a dict,")
-                    return
-            if "tag" in dstuff:
-                dscptr = descriptor_map[dstuff["tag"]]()
-                dscptr.load(dstuff)
-                self.descriptors.append(dscptr)
+        print(self.get_json(), file=stderr)
```

### Comparing `threefive-2.3.83/threefive/descriptors.py` & `threefive-2.3.9/exp-js/descriptors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 SCTE35 Splice Descriptors
 """
 from .bitn import BitBin
 from .base import SCTE35Base
 from .segmentation import table20, table22
-from .upids import UpidDecoder, upid_encoder
+from .upid import upid_decoder, upid_encoder
 
 
 def k_by_v(adict, avalue):
     """
     dict key lookup by value
     """
     for kay, vee in adict.items():
@@ -24,15 +24,15 @@
     It should not be used directly
     """
 
     def __init__(self, bites=None):
         self.tag = None
         self.descriptor_length = 0
         self.name = None
-        self.identifier = "CUEI"
+        self.identifier = None
         self.bites = bites
         self.parse_tag_and_len()
         self.parse_id()
         self.provider_avail_id = None
         self.components = None
 
     def parse_tag_and_len(self):
@@ -136,23 +136,19 @@
 
 
 class AvailDescriptor(SpliceDescriptor):
     """
     Table 17 -  avail_descriptor()
     """
 
-    def __init__(self, bites=None):
-        super().__init__(bites)
-        self.name = "Avail Descriptor"
-        self.tag = 0
-
     def decode(self):
         """
         decode SCTE35 Avail Descriptor
         """
+        self.name = "Avail Descriptor"
         bitbin = BitBin(self.bites)
         self.provider_avail_id = bitbin.as_int(32)
 
     def encode(self, nbin=None):
         """
         encode SCTE35 Avail Descriptor
         """
@@ -162,25 +158,25 @@
 
 
 class DtmfDescriptor(SpliceDescriptor):
     """
     Table 18 -  DTMF_descriptor()
     """
 
-    def __init__(self, bites=None):
+    def __init__(self, bites):
         super().__init__(bites)
-        self.name = "DTMF Descriptor"
         self.preroll = None
-        self.dtmf_count = 0
+        self.dtmf_count = None
         self.dtmf_chars = None
 
     def decode(self):
         """
         decode SCTE35 Dtmf Descriptor
         """
+        self.name = "DTMF Descriptor"
         self.preroll = self.bites[0]
         self.dtmf_count = self.bites[1] >> 5
         self.bites = self.bites[2:]
         self.dtmf_chars = list(self.bites[: self.dtmf_count].decode())
 
     def encode(self, nbin=None):
         """
@@ -198,48 +194,47 @@
 
 
 class TimeDescriptor(SpliceDescriptor):
     """
     Table 25 - time_descriptor()
     """
 
-    def __init__(self, bites=None):
+    def __init__(self, bites):
         super().__init__(bites)
-        self.tag = 3
-        self.name = "Time Descriptor"
-        self.tai_seconds = 0
-        self.tai_ns = 0
-        self.utc_offset = 0
+        self.tai_seconds = None
+        self.tai_ns = None
+        self.utc_offset = None
 
     def decode(self):
         """
         decode SCTE35 Time Descriptor
         """
+        self.name = "Time Descriptor"
         bitbin = BitBin(self.bites)
         self.tai_seconds = bitbin.as_int(48)
         self.tai_ns = bitbin.as_int(32)
         self.utc_offset = bitbin.as_int(16)
 
     def encode(self, nbin=None):
         """
-        encode SCTE35 Time Descriptor
+        encode SCTE35 Avail Descriptor
         """
         nbin = super().encode(nbin)
         self._chk_var(int, nbin.add_int, "tai_seconds", 48)
         self._chk_var(int, nbin.add_int, "tai_ns", 32)
         self._chk_var(int, nbin.add_int, "utc_offset", 16)
         return nbin.bites
 
 
 class SegmentationDescriptor(SpliceDescriptor):
     """
     Table 19 - segmentation_descriptor()
     """
 
-    def __init__(self, bites=None):
+    def __init__(self, bites):
         super().__init__(bites)
         self.tag = 2
         self.name = "Segmentation Descriptor"
         self.segmentation_event_id = None
         self.segmentation_event_cancel_indicator = None
         self.component_count = None
         self.components = []
@@ -247,15 +242,14 @@
         self.segmentation_duration_flag = None
         self.delivery_not_restricted_flag = None
         self.web_delivery_allowed_flag = None
         self.no_regional_blackout_flag = None
         self.archive_allowed_flag = None
         self.device_restrictions = None
         self.segmentation_duration = None
-        self.segmentation_duration_ticks = None
         self.segmentation_message = None
         self.segmentation_upid_type = None
         self.segmentation_upid_type_name = None
         self.segmentation_upid_length = None
         self.segmentation_upid = None
         self.segmentation_type_id = None
         self.segment_num = None
@@ -273,64 +267,14 @@
         bitbin.forward(7)  # 1 byte
         if not self.segmentation_event_cancel_indicator:
             self._decode_flags(bitbin)  # 1 byte
             if not self.program_segmentation_flag:
                 self._decode_components(bitbin)
             self._decode_segmentation(bitbin)
 
-    def _decode_flags(self, bitbin):  # 1 byte for set flags
-        self.program_segmentation_flag = bitbin.as_flag(1)
-        self.segmentation_duration_flag = bitbin.as_flag(1)
-        self.delivery_not_restricted_flag = bitbin.as_flag(1)
-        if not self.delivery_not_restricted_flag:
-            self.web_delivery_allowed_flag = bitbin.as_flag(1)
-            self.no_regional_blackout_flag = bitbin.as_flag(1)
-            self.archive_allowed_flag = bitbin.as_flag(1)
-            self.device_restrictions = table20[bitbin.as_int(2)]
-        else:
-            bitbin.forward(5)
-
-    def _decode_components(self, bitbin):
-        self.component_count = c_c = bitbin.as_int(8)  # 1 byte
-        while c_c:  # 6 bytes each
-            c_c -= 1
-            comp = {}
-            comp["component_tag"] = bitbin.as_int(8)
-            bitbin.forward(7)
-            comp["pts_offset"] = bitbin.as_90k(33)
-            self.components.append(comp)
-
-    def _decode_segmentation(self, bitbin):
-        if self.segmentation_duration_flag:
-            self.segmentation_duration_ticks = bitbin.as_int(40)  # 5 bytes
-            self.segmentation_duration = self.as_90k(self.segmentation_duration_ticks)
-        self.segmentation_upid_type = bitbin.as_int(8)  # 1 byte
-        self.segmentation_upid_length = bitbin.as_int(8)  # 1 byte
-        self.segmentation_upid_type_name, self.segmentation_upid = UpidDecoder(
-            bitbin, self.segmentation_upid_type, self.segmentation_upid_length
-        ).decode()
-        self.segmentation_type_id = bitbin.as_int(8)  # 1 byte
-        if self.segmentation_type_id in table22:
-            self.segmentation_message = table22[self.segmentation_type_id]
-            self._decode_segments(bitbin)
-
-    def _decode_segments(self, bitbin):
-        self.segment_num = bitbin.as_int(8)  # 1 byte
-        self.segments_expected = bitbin.as_int(8)  # 1 byte
-        if self.segmentation_type_id in [0x34, 0x36, 0x38, 0x3A]:
-            # if sub_segment_num and sub_segments_expected
-            # are not available set both of them to zero
-            # This has been an issue at CBS and CNN just recently.
-            self.sub_segment_num = self.sub_segments_expected = 0
-            try:
-                self.sub_segment_num = bitbin.as_int(8)  # 1 byte
-                self.sub_segments_expected = bitbin.as_int(8)  # 1 byte
-            except:
-                pass
-
     def encode(self, nbin=None):
         """
         encode a segmentation descriptor
         """
         nbin = super().encode(nbin)
         self._chk_var(str, nbin.add_hex, "segmentation_event_id", 32)  # 4 bytes
         self._chk_var(bool, nbin.add_flag, "segmentation_event_cancel_indicator", 1)
@@ -338,59 +282,93 @@
         if not self.segmentation_event_cancel_indicator:
             self._encode_flags(nbin)  # 1 byte
             if not self.program_segmentation_flag:
                 self._encode_components(nbin)
             self._encode_segmentation(nbin)
         return nbin.bites
 
+    def _decode_components(self, bitbin):
+        self.component_count = c_c = bitbin.as_int(8)  # 1 byte
+        while c_c:  # 6 bytes each
+            c_c -= 1
+            comp = {}
+            comp["component_tag"] = bitbin.as_int(8)
+            bitbin.forward(7)
+            comp["pts_offset"] = bitbin.as_90k(33)
+            self.components.append(comp)
+
     def _encode_components(self, nbin):
         nbin.add_int(self.component_count, 8)  # 1 byte
         c_c = 0
         while c_c < self.component_count:  # 6 bytes each
             comp = self.components[c_c]
             nbin.add_int(comp["component_tag"], 8)
             nbin.forward(7)
             nbin.add_90k(comp["pts_offset"], 33)
             c_c += 1
 
+    def _decode_flags(self, bitbin):  # 1 byte for set flags
+        self.program_segmentation_flag = bitbin.as_flag(1)
+        self.segmentation_duration_flag = bitbin.as_flag(1)
+        self.delivery_not_restricted_flag = bitbin.as_flag(1)
+        if not self.delivery_not_restricted_flag:
+            self.web_delivery_allowed_flag = bitbin.as_flag(1)
+            self.no_regional_blackout_flag = bitbin.as_flag(1)
+            self.archive_allowed_flag = bitbin.as_flag(1)
+            self.device_restrictions = table20[bitbin.as_int(2)]
+        else:
+            bitbin.forward(5)
+
     def _encode_flags(self, nbin):  # 1 byte for set flags
         self._chk_var(bool, nbin.add_flag, "program_segmentation_flag", 1)
         self._chk_var(bool, nbin.add_flag, "segmentation_duration_flag", 1)
         self._chk_var(bool, nbin.add_flag, "delivery_not_restricted_flag", 1)
         if not self.delivery_not_restricted_flag:
             self._chk_var(bool, nbin.add_flag, "web_delivery_allowed_flag", 1)
             self._chk_var(bool, nbin.add_flag, "no_regional_blackout_flag", 1)
             self._chk_var(bool, nbin.add_flag, "archive_allowed_flag", 1)
             a_key = k_by_v(table20, self.device_restrictions)
             nbin.add_int(a_key, 2)
         else:
             nbin.reserve(5)
 
+    def _decode_segmentation(self, bitbin):
+        if self.segmentation_duration_flag:
+            self.segmentation_duration = bitbin.as_90k(40)  # 5 bytes
+        self.segmentation_upid_type = bitbin.as_int(8)  # 1 byte
+        self.segmentation_upid_length = bitbin.as_int(8)  # 1 byte
+        self.segmentation_upid_type_name, self.segmentation_upid = upid_decoder(
+            bitbin, self.segmentation_upid_type, self.segmentation_upid_length
+        )
+        self.segmentation_type_id = bitbin.as_int(8)  # 1 byte
+        if self.segmentation_type_id in table22.keys():
+            self.segmentation_message = table22[self.segmentation_type_id]
+            self._decode_segments(bitbin)
+
     def _encode_segmentation(self, nbin):
         if self.segmentation_duration_flag:
-            if not self.segmentation_duration_ticks:
-                self.segmentation_duration_ticks = 0
-            if self.segmentation_duration:
-                self.segmentation_duration_ticks = self.as_ticks(
-                    self.segmentation_duration
-                    )
-            self._chk_var(
-                int, nbin.add_int, "segmentation_duration_ticks", 40
-            )  # 5 bytes
+            self._chk_var(float, nbin.add_90k, "segmentation_duration", 40)  # 5 bytes
         self._chk_var(int, nbin.add_int, "segmentation_upid_type", 8)  # 1 byte
         self._chk_var(int, nbin.add_int, "segmentation_upid_length", 8)  # 1 byte
         upid_encoder(
             nbin,
             self.segmentation_upid_type,
             self.segmentation_upid_length,
             self.segmentation_upid,
         )
         self._chk_var(int, nbin.add_int, "segmentation_type_id", 8)  # 1 byte
         self._encode_segments(nbin)
 
+    def _decode_segments(self, bitbin):
+        self.segment_num = bitbin.as_int(8)  # 1 byte
+        self.segments_expected = bitbin.as_int(8)  # 1 byte
+        if self.segmentation_type_id in [0x34, 0x36, 0x38, 0x3A]:
+            self.sub_segment_num = bitbin.as_int(8)  # 1 byte
+            self.sub_segments_expected = bitbin.as_int(8)  # 1 byte
+
     def _encode_segments(self, nbin):
         self._chk_var(int, nbin.add_int, "segment_num", 8)  # 1 byte
         self._chk_var(int, nbin.add_int, "segments_expected", 8)  # 1 byte
         if self.segmentation_type_id in [0x34, 0x36, 0x38, 0x3A]:
             self._chk_var(int, nbin.add_int, "sub_segment_num", 8)  # 1 byte
             self._chk_var(int, nbin.add_int, "sub_segments_expected", 8)  # 1 byte
 
@@ -407,13 +385,14 @@
 
 def splice_descriptor(bites):
     """
     splice_descriptor reads the
     descriptor tag and decodes and
     returns an instance self._descriptor_map[tag]
     """
+    # splice_descriptor_tag 8 uimsbf
     tag = bites[0]
     if tag not in descriptor_map:
         return False
     spliced = descriptor_map[tag](bites)
     spliced.decode()
     return spliced
```

### Comparing `threefive-2.3.83/threefive/packetdata.py` & `threefive-2.3.9/threefive/packetdata.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,37 +11,33 @@
     to hold packet pid, program, pcr and pts
     for SCTE-35 packets.
     """
 
     def __init__(self, pid, prgm):
         self.pid = hex(pid)
         self.program = prgm
-        self.pcr_ticks = None
         self.pcr = None
-        self.pts_ticks = None
         self.pts = None
 
     @staticmethod
     def _mk_timestamp(seconds):
         if seconds:
             return round((seconds / 90000.0), 6)
         return seconds
 
+    def _chk_table(self, table):
+        seconds = None
+        if self.program in table:
+            seconds = self._mk_timestamp(table[self.program])
+        return seconds
+
     def mk_pcr(self, table):
         """
         calculates and formats pcr
         """
-        try:
-            self.pcr_ticks = table[self.program]
-            self.pcr = self._mk_timestamp(self.pcr_ticks)
-        except:
-            pass
+        self.pcr = self._chk_table(table)
 
     def mk_pts(self, table):
         """
         mk_pts calculates and formats pts
         """
-        try:
-            self.pts_ticks = table[self.program]
-            self.pts = self._mk_timestamp(self.pts_ticks)
-        except:
-            pass
+        self.pts = self._chk_table(table)
```

### Comparing `threefive-2.3.83/threefive/section.py` & `threefive-2.3.9/exp-js/section.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         # sap_type used to be marked reserved.
         self.sap_type = None
         self.sap_details = None
         self.section_length = None
         self.protocol_version = None
         self.encrypted_packet = None
         self.encryption_algorithm = None
-        self.pts_adjustment_ticks = None
         self.pts_adjustment = None
         self.cw_index = None
         self.tier = None
         self.splice_command_length = None
         self.splice_command_type = None
         self.descriptor_loop_length = 0
         self.crc = None
@@ -47,23 +46,26 @@
         bitbin = BitBin(bites)
         self.table_id = bitbin.as_hex(8)
         if self.table_id != "0xfc":
             raise ValueError(
                 ("splice_info_section.table_id should be 0xfc Not: ", self.table_id)
             )
         self.section_syntax_indicator = bitbin.as_flag(1)
+        if self.section_syntax_indicator != 0:
+            raise ValueError("section_syntax_indicator should be 0")
         self.private = bitbin.as_flag(1)
         self.sap_type = bitbin.as_hex(2)
         self.sap_details = sap_map[self.sap_type]
         self.section_length = bitbin.as_int(12)
         self.protocol_version = bitbin.as_int(8)
+        if self.protocol_version != 0:
+            raise ValueError("splice_info_section.protocol_version should be 0")
         self.encrypted_packet = bitbin.as_flag(1)
         self.encryption_algorithm = bitbin.as_int(6)
-        self.pts_adjustment_ticks = bitbin.as_int(33)
-        self.pts_adjustment = self.as_90k(self.pts_adjustment_ticks)
+        self.pts_adjustment = bitbin.as_90k(33)
         self.cw_index = bitbin.as_hex(8)
         self.tier = bitbin.as_hex(12)
         self.splice_command_length = bitbin.as_int(12)
         self.splice_command_type = bitbin.as_int(8)
 
     def _encode_table_id(self, nbin):
         """
@@ -86,15 +88,15 @@
         self.private = False
         nbin.add_flag(self.private, 1)
 
     def _encode_sap(self, nbin):
         """
         the 3 reserved bits now map SAP
         """
-        if self.sap_type not in sap_map:
+        if self.sap_type not in sap_map.keys():
             self.sap_type = "0x3"
         self.sap_details = sap_map[self.sap_type]
         nbin.add_hex(self.sap_type, 2)
 
     def _encode_section_length(self, nbin):
         """
         encode SpliceInfoSection.section_length
@@ -121,21 +123,19 @@
         nbin.add_flag(self.encrypted_packet)
         if not self.encryption_algorithm:
             self.encryption_algorithm = 0
         nbin.add_int(self.encryption_algorithm, 6)
 
     def _encode_pts_adjustment(self, nbin):
         """
-        encode SpliceInfoSection.pts_adjustment_ticks
+        encode SpliceInfoSection.pts_adjustment
         """
-        if not self.pts_adjustment_ticks:
-            self.pts_adjustment_ticks = 0
-        if self.pts_adjustment:
-            self.pts_adjustment_ticks = self.as_ticks(self.pts_adjustment)
-        self._chk_var(int, nbin.add_int, "pts_adjustment_ticks", 33)
+        if not self.pts_adjustment:
+            self.pts_adjustment = 0.0
+        nbin.add_90k(self.pts_adjustment, 33)
 
     def _encode_cw_index(self, nbin):
         """
         encode SpliceInfoSection.cw_index
         """
         if not self.cw_index:
             self.cw_index = "0x0"
```

### Comparing `threefive-2.3.83/threefive/segment.py` & `threefive-2.3.9/threefive/segment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 """
 The threefive.Segment class
 """
 import os
-from new_reader import reader
-from .stream import Stream
 
-AES = True
-try:
-    import pyaes
-except:
-    AES = False
+import pyaes
+
+from .reader import reader
+from .stream import Stream
 
 
 class Segment(Stream):
     """
     The Segment class is a Sub Class of threefive.Stream
     made for small, fixed size MPEGTS files,like HLS segments.
 
@@ -52,22 +49,21 @@
 
     def __init__(self, seg_uri, key_uri=None, iv=None):
         self.seg_uri = seg_uri
         self.key_uri = key_uri
         self.key = None
         self.iv = None
         self.cues = []
-        self.pts_start = None
+        self.start = None
         self.tmp = None
-        if AES:
-            if iv:
-                self.iv = int.to_bytes(int(iv), 16, byteorder="big")
-            if self.key_uri:
-                self._aes_get_key()
-                self._aes_decrypt()
+        if iv:
+            self.iv = int.to_bytes(int(iv), 16, byteorder="big")
+        if self.key_uri:
+            self._aes_get_key()
+            self._aes_decrypt()
         super().__init__(self.seg_uri)
 
     def __repr__(self):
         return str(self.__dict__)
 
     def _mk_tmp(self):
         self.tmp = "tf-"
@@ -76,39 +72,35 @@
     def _aes_get_key(self):
         with reader(self.key_uri) as quay:
             self.key = quay.read()
 
     def _aes_decrypt(self):
         mode = pyaes.AESModeOfOperationCBC(self.key, iv=self.iv)
         self._mk_tmp()
-        with open(
-                self.tmp,
-                "wb",
-                encoding="utf-8") as outfile, reader(self.seg_uri) as infile:
-            pyaes.decrypt_stream(mode, infile, outfile)
-        self.seg_uri = self.tmp
+        with open(self.tmp, "wb") as outfile:
+            with reader(self.seg_uri) as infile:
+                pyaes.decrypt_stream(mode, infile, outfile)
+            self.seg_uri = self.tmp
 
     def add_cue(self, cue):
         """
-        add_cue is called  by a segment instance
+        add_cue is passed to a Stream instance
         to collect SCTE35 cues.
         """
         self.cues.append(cue)
 
     def show_cue(self, cue):
         """
         show_cue prints SCTE35 Cue data
         and calls add_cue to append the cue to
         the Segment,cues list.
         """
         cue.show()
         self.add_cue(cue)
 
-    def decode(self, func=None):
+    def decode(self):
         """
         decode a mpegts segment.
         """
         super().decode(func=self.show_cue)
-        # self.pts_start
-
         if self.tmp:
             os.unlink(self.tmp)
```

### Comparing `threefive-2.3.83/threefive/segmentation.py` & `threefive-2.3.9/exp-js/segmentation.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,22 +42,12 @@
     0x35: "Provider Placement Opportunity End",
     0x36: "Distributor Placement Opportunity Start",
     0x37: "Distributor Placement Opportunity End",
     0x38: "Provider Overlay Placement Opportunity Start",
     0x39: "Provider Overlay Placement Opportunity End",
     0x3A: "Distributor Overlay Placement Opportunity Start",
     0x3B: "Distributor Overlay Placement Opportunity End",
-    0x3C: "Provider Promo Start",
-    0x3D: "Provider Promo End",
-    0x3E: "Distributor Promo Start",
-    0x3F: "Distributor Promo End",
     0x40: "Unscheduled Event Start",
     0x41: "Unscheduled Event End",
-    0x42: "Alternate Content Opportunity Start",
-    0x43: "Alternate Content Opportunity End",
-    0x44: "Provider Ad Block Start",
-    0x45: "Provider Ad Block End",
-    0x46: "Distributor Ad Block Start",
-    0x47: "Distributor Ad Block End",
     0x50: "Network Start",
     0x51: "Network End",
 }
```

### Comparing `threefive-2.3.83/threefive/smoketest.py` & `threefive-2.3.9/threefive/smoketest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 smoke_test.py
 """
 
 from .decode import decode
-from .stuff import print2
 
 # The format for tests is a dict of { "test_name" : value to pass to threefive.decode}
 ten_tests = {
     "Base64": "/DAvAAAAAAAA///wBQb+dGKQoAAZAhdDVUVJSAAAjn+fCAgAAAAALKChijUCAKnMZ1g=",
     "Bytes": b"\xfc0\x11\x00\x00\x00\x00\x00\x00\x00\xff\xff\xff\x00\x00\x00O%3\x96",
     "Hex String": "0XFC301100000000000000FFFFFF0000004F253396",
     "Hex Literal": 0xFC301100000000000000FFFFFF0000004F253396,
@@ -20,15 +19,15 @@
     " Bad String": "your momma",
 }
 
 
 def _decode_test(test_name, test_data):
     passed = "✔"
     failed = "✘"
-    print2(f"testing {test_name}\n Data: {test_data}\n")
+    print(f"testing {test_name}\n Data: {test_data}\n")
     if decode(test_data):
         return passed
     return failed
 
 
 def smoke(tests=None):
     """
@@ -46,14 +45,14 @@
     import threefive
     threefive.smoke_test(my_tests)
 
     """
     if not tests:
         tests = ten_tests
     results = {k: _decode_test(k, v) for k, v in tests.items()}
-    print2("Smoke Test\n")
+    print("Smoke Test\n")
     for kay, vee in results.items():
-        print2(f"{kay}  {vee}")
+        print(f"{kay}  {vee}")
 
 
 if __name__ == "__main__":
     smoke()
```

### Comparing `threefive-2.3.83/threefive/stream.py` & `threefive-2.3.9/threefive/stream.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,15 @@
 """
 Mpeg-TS Stream parsing class Stream
 """
 import sys
 from functools import partial
-from new_reader import reader
-from .stuff import print2
 from .cue import Cue
 from .packetdata import PacketData
-
-
-streamtype_map = {
-    "0x02": "MP2 Video",
-    "0x03": "MP2 Audio",
-    "0x04": "MP2 Audio",
-    "0x06": "PES Packets/Private Data",
-    "0x0f": "AAC Audio",
-    "0x1b": "AVC Video",
-    "0x81": "AC3 Audio ",
-    "0x86": "SCTE35 Data",
-    "0xc0": "Unknown",
-}
+from .reader import reader
 
 
 def no_op(cue):
     """
     no_op is just a dummy func to pass to Stream.decode()
     to suppress output.
     """
@@ -36,108 +22,60 @@
     when a SCTE-35 packet is found.
     """
     cue.show()
 
 
 def show_cue_stderr(cue):
     """
-    print2 cue data to sys.stderr
+    print cue data to sys.stderr
     for Stream.decode_proxy
     """
     cue.to_stderr()
 
 
 class ProgramInfo:
     """
     ProgramInfo is a class to
     hold Program information
     for use with Stream.show()
     """
 
-    def __init__(self, pid=None, pcr_pid=None):
-        self.pid = pid
-        self.pcr_pid = pcr_pid
+    def __init__(self):
+        self.pid = None
+        self.pcr_pid = None
         self.provider = b""
         self.service = b""
         self.streams = {}  # pid to stream_type mapping
 
     def show(self):
         """
-        show print2 the Program Infomation
+        show print the Program Infomation
         in a familiar format.
         """
         serv = self.service.decode(errors="ignore")
         prov = self.provider.decode(errors="ignore")
-        print2(f"    Service:\t{ serv}\n    Provider:\t{prov}")
-        print2(f"    Pid:\t{self.pid}")
-        print2(f"    Pcr Pid:\t{self.pcr_pid}")
-        print2("    Streams:")
-        # sorted_dict = {k:my_dict[k] for k in sorted(my_dict)})
-        keys = sorted(self.streams)
-        for k in keys:
-            vee = self.streams[k]
-            if vee in streamtype_map:
-                vee = f"{vee} {streamtype_map[vee]}"
-            else:
-                vee = f"{vee} Unknown"
-            print2(f"\t\tPid: {k}[{hex(k)}]\tType: {vee}")
-        print2()
-
-
-class Pids:
-    """
-    Pids holds sets of pids for pat,pcr,pmt, and scte35
-    """
-
-    SDT_PID = 0x11
-    PAT_PID = 0x00
-
-    def __init__(self):
-        self.pcr = set()
-        self.pmt = set()
-        self.scte35 = set()
-        self.tables = set()
-        self.tables.add(self.PAT_PID)
-        self.tables.add(self.SDT_PID)
-
-
-class Maps:
-    """
-    Maps holds mappings
-    pids mapped to continuity_counters,
-    programs, partial tables and last payload.
-
-    programs mapped to pcr and pts
-
-    """
-
-    def __init__(self):
-        self.pid_cc = {}
-        self.pid_prgm = {}
-        self.prgm_pcr = {}
-        self.prgm_pts = {}
-        self.prgm = {}
-        self.partial = {}
-        self.last = {}
+        print(f"    Service: { serv}\n    Provider: {prov}\n")
+        print(f"    Pcr Pid: {self.pcr_pid}[{hex(self.pcr_pid)}]")
+        print("    Streams:")
+        for k, vee in self.streams.items():
+            print(f"\t    Pid: {k}[{hex(k)}]    Type: {vee}")
+        print()
 
 
 class Stream:
     """
     Stream class for parsing MPEG-TS data.
     """
 
-    _PACKET_SIZE = 188
-    _SYNC_BYTE = 0x47
-    # tids
-    _PMT_TID = b"\x02"
-    _SCTE35_TID = b"\xFC0"
-    _SDT_TID = b"\x42"
-    # pts
-    ROLLOVER = 8589934591  # 95443.717678
-    NO_PTS_PIDS = [188, 190, 191, 240, 241, 242, 248]
+    _PACKET_SIZE = 188  # Mpegts packet size in bytes
+    _SYNC_BYTE = 0x47  # Mpegts sync byte
+    _SDT_PID = 0x0011  # Stream Descriptor Table Pid
+    _PAT_PID = 0x00  # Program Association Pid
+    _PMT_TID = b"\x02"  # PMT Table Id as bytes
+    _SCTE35_TID = b"\xFC0"  # SCTE35 Table Id as bytes
 
     def __init__(self, tsdata, show_null=True):
         """
         tsdata is an file or http/https url
         set show_null=False to exclude Splice Nulls
 
         Use like...
@@ -151,459 +89,413 @@
             self._tsdata = reader(tsdata)
         else:
             self._tsdata = tsdata
         self.show_null = show_null
         self.start = {}
         self.info = None
         self.the_program = None
-        self.pids = Pids()
-        self.maps = Maps()
+        self._pids = {"pcr": set(), "tables": set(), "scte35": set()}
+        self._pids["tables"].add(self._PAT_PID)
+        self._pids["tables"].add(self._SDT_PID)
+        self._pid_prgm = {}
+        self._prgm_pcr = {}
+        self._prgm_pts = {}
+        self._prgm = {}
+        self._partial = {}
+        self._last = {}
 
     def __repr__(self):
         return str(self.__dict__)
 
     def _find_start(self):
-        """
-        _find_start locates the first SYNC_BYTE
-        parses 1 packet and returns a iterator
-        of packets
-        """
         while self._tsdata:
             one = self._tsdata.read(1)
             if not one:
-                print2("\nNo Stream Found. \n")
-                return []
+                return False
             if one[0] == self._SYNC_BYTE:
                 tail = self._tsdata.read(self._PACKET_SIZE - 1)
                 if tail:
                     self._parse(one + tail)
-                    return self.iter_pkts()
-
-    def pid2prgm(self, pid):
-        """
-        pid2prgm takes a pid,
-        returns the program
-        """
-        prgm = 1
-        if pid in self.maps.pid_prgm:
-            prgm = self.maps.pid_prgm[pid]
-        return prgm
-
-    def pid2pts(self, pid):
-        """
-        pid2pts takes a pid
-        returns the current pts
-        """
-        prgm = self.pid2prgm(pid)
-        if prgm not in self.maps.prgm_pts:
-            return False
-        return self.as_90k(self.maps.prgm_pts[prgm])
-
-    def pid2pcr(self, pid):
-        """
-        pid2pcr takes a pid
-        returns the current pcr
-        """
-        prgm = self.pid2prgm(pid)
-        if prgm not in self.maps.prgm_pcr:
-            return False
-        return self.as_90k(self.maps.prgm_pcr[prgm])
-
-    def iter_pkts(self, num_pkts=1):
-        """
-        iter_pkts iterates a mpegts stream into packets
-        """
-        return iter(partial(self._tsdata.read, self._PACKET_SIZE * num_pkts), b"")
+                    return True
+        return False
 
     def decode(self, func=show_cue):
         """
         Stream.decode reads self.tsdata to find SCTE35 packets.
         func can be set to a custom function that accepts
         a threefive.Cue instance as it's only argument.
         """
-        for pkt in self._find_start():
-            cue = self._parse(pkt)
-            if cue:
-                if not func:
-                    return cue
-                func(cue)
-        return False
+        if self._find_start():
+            for pkt in iter(partial(self._tsdata.read, self._PACKET_SIZE), b""):
+                cue = self._parse(pkt)
+                if cue:
+                    if not func:
+                        return cue
+                    func(cue)
+        self._tsdata.close()
+        return True
 
     def _mk_pkts(self, chunk):
         return [
             self._parse(chunk[i : i + self._PACKET_SIZE])
             for i in range(0, len(chunk), self._PACKET_SIZE)
         ]
 
     def decode_fu(self, func=show_cue):
         """
         Stream.decode_fu decodes
-        num_pkts packets at a time.
-        Super Fast with pypy3.
+        1880 packets at a time.
         """
-        num_pkts = 1000
-        for chunk in self.iter_pkts(num_pkts):
-            _ = [func(cue) for cue in self._mk_pkts(chunk) if cue]
-            del _
+        pkts = 1880
+        if self._find_start():
+            for chunk in iter(
+                partial(self._tsdata.read, (self._PACKET_SIZE * pkts)), b""
+            ):
+                for cue in self._mk_pkts(chunk):
+                    if cue:
+                        func(cue)
         self._tsdata.close()
-        return False
 
     def decode_next(self):
         """
         Stream.decode_next returns the next
         SCTE35 cue as a threefive.Cue instance.
         """
-        return self.decode(func=None)
+        cue = self.decode(func=False)
+        if cue:
+            return cue
+        return None
 
     def decode_program(self, the_program, func=show_cue):
         """
         Stream.decode_program limits SCTE35 parsing
         to a specific MPEGTS program.
         """
         self.the_program = the_program
         return self.decode(func)
 
-    def proxy(self, func=show_cue_stderr):
+    def decode_proxy(self, func=show_cue_stderr):
         """
         Stream.decode_proxy writes all ts packets are written to stdout
         for piping into another program like mplayer.
-        SCTE-35 cues are print2ed to stderr.
+        SCTE-35 cues are printed to stderr.
+        """
+        if self._find_start():
+            for pkt in iter(partial(self._tsdata.read, self._PACKET_SIZE), b""):
+                cue = self._parse(pkt)
+                if cue:
+                    func(cue)
+                sys.stdout.buffer.write(pkt)
+        self._tsdata.close()
+
+    def strip_scte35(self, func=show_cue_stderr):
         """
-        for pkt in self._find_start():
-            cue = self._parse(pkt)
-            if cue:
-                func(cue)
-            sys.stdout.buffer.write(pkt)
+        Stream.strip_scte35 works just likle Stream.decode_proxy,
+        MPEGTS packets, ( Except the SCTE-35 packets) ,
+        are written to stdout after being parsed.
+        SCTE-35 cues are printed to stderr.
+        """
+        if self._find_start():
+            for pkt in iter(partial(self._tsdata.read, self._PACKET_SIZE), b""):
+                cue = self._parse(pkt)
+                if cue:
+                    func(cue)
+                else:
+                    sys.stdout.buffer.write(pkt)
+        self._tsdata.close()
 
     def show(self):
         """
         displays streams that will be
         parsed for SCTE-35.
         """
         self.info = True
-        for pkt in self._find_start():
-            self._parse_info(pkt)
-        sopro = sorted(self.maps.prgm.items())
+        self.decode(func=False)
+        sopro = sorted(self._prgm.items())
         for k, vee in sopro:
             if len(vee.streams.items()) > 0:
-                print2(f"Program: {k}")
+                print(f"Program: {k}")
                 vee.show()
-        return True
 
     def decode_start_time(self):
         """
         displays streams that will be
         parsed for SCTE-35.
         """
         self.decode(func=no_op)
         if len(self.start.values()) > 0:
             return self.start.popitem()[1]
-        return False
+        return None
 
     def _mk_packet_data(self, pid):
-        prgm = self.maps.pid_prgm[pid]
+        prgm = self._pid_prgm[pid]
         pdata = PacketData(pid, prgm)
-        pdata.mk_pcr(self.maps.prgm_pcr)
-        pdata.mk_pts(self.maps.prgm_pts)
+        pdata.mk_pcr(self._prgm_pcr)
+        pdata.mk_pts(self._prgm_pts)
         return pdata
 
     @staticmethod
-    def as_90k(ticks):
-        """
-        as_90k returns ticks as 90k clock time
-        """
-        return round((ticks / 90000.0), 6)
-
-    @staticmethod
-    def _pusi_flag(pkt):
-        return pkt[1] & 0x40
-
-    @staticmethod
-    def _afc_flag(pkt3):
-        return pkt3 & 0x20
-
-    @staticmethod
-    def _pcr_flag(pkt):
-        return pkt[5] & 0x10
-
-    @staticmethod
-    def _spi_flag(pkt):
-        return pkt[5] & 0x20
-
-    @staticmethod
-    def _pts_flag(pay):
-        # uses pay not pkt
-        return pay[7] & 0x80
-
-    @staticmethod
-    def _has_pts(pkt_one, pkt_eleven):
-        if pkt_one & 0x40:
-            return pkt_eleven & 0x80
-        return False
+    def _parse_payload(pkt):
+        head_size = 4
+        afc = pkt[3] & 0x20
+        if afc:
+            afl = pkt[4]
+            head_size += afl + 1  # +1 for afl byte
+        return pkt[head_size:]
 
     @staticmethod
     def _parse_length(byte1, byte2):
         """
         parse a 12 bit length value
         """
-        return (byte1 & 0xF) << 8 | byte2
+        return (byte1 << 8 | byte2) & 0x0FFF
 
     @staticmethod
     def _parse_pid(byte1, byte2):
         """
         parse a 13 bit pid value
         """
-        pid = (byte1 & 0x1F) << 8 | byte2
-        return pid
+        return (byte1 << 8 | byte2) & 0x01FFF
 
     @staticmethod
     def _parse_program(byte1, byte2):
         """
         parse a 16 bit program number value
         """
         return (byte1 << 8) | byte2
 
     @staticmethod
-    def _split_by_idx(pay, marker):
-        try:
-            return pay[pay.index(marker) :]
-        except ValueError:
-            return False
-
-    def _parse_cc(self, pkt, pid):
-        last_cc = None
-        c_c = pkt[3] & 0xF
-        if pid in self.maps.pid_cc:
-            last_cc = self.maps.pid_cc[pid]
-            good = (last_cc, ((last_cc + 1) % 16))
-            if c_c not in good:
-                # print2 prints to stderr, get it?  print 2>
-                # That's mine too. I shoiuld know better.
-                print2(f"BAD --> pid: {hex(pid)} last cc: {last_cc} cc: {c_c}" )
-        self.maps.pid_cc[pid] = c_c
+    def _parse_pusi(byte1):
+        """
+        used to determine if pts data is available.
+        """
+        return byte1 & 0x40
 
     def _parse_pts(self, pkt, pid):
         """
         parse pts and store by program key
         in the dict Stream._pid_pts
         """
-        # if len(payload) > 13:
-        if self._has_pts(pkt[1], pkt[11]):
-            payload = self._parse_payload(pkt)
-            pts = (payload[9] & 14) << 29
-            pts |= payload[10] << 22
-            pts |= (payload[11] >> 1) << 15
-            pts |= payload[12] << 7
-            pts |= payload[13] >> 1
-            prgm = self.pid2prgm(pid)
-            self.maps.prgm_pts[prgm] = pts
-            if prgm not in self.start:
-                self.start[prgm] = pts
+        if pid in self._pid_prgm:
+            if pkt[11] & 0x80:
+                pts = ((pkt[13] >> 1) & 7) << 30
+                pts |= pkt[14] << 22
+                pts |= (pkt[15] >> 1) << 15
+                pts |= pkt[16] << 7
+                pts |= pkt[17] >> 1
+                prgm = self._pid_prgm[pid]
+                self._prgm_pts[prgm] = pts
+
+    def _parse_pcr(self, pkt, pid):
+        """
+        parse pcr and store by program key
+        in the dict Stream._pid_pcr
+        """
+        if pkt[3] & 0x20:
+            if pkt[5] & 0x10:
+                pcr = pkt[6] << 25
+                pcr |= pkt[7] << 17
+                pcr |= pkt[8] << 9
+                pcr |= pkt[9] << 1
+                pcr |= pkt[10] >> 7
+                prgm = 1
+                if pid in self._pid_prgm:
+                    prgm = self._pid_prgm[pid]
+                self._prgm_pcr[prgm] = pcr
+                if prgm not in self.start:
+                    self.start[prgm] = pcr
 
-    def _parse_payload(self, pkt):
-        """
-        _parse_payload returns the packet payload
-        """
-        head_size = 4
-        if self._afc_flag(pkt[3]):
-            afl = pkt[4]
-            head_size += afl + 1  # +1 for afl byte
-        return pkt[head_size:]
+    @staticmethod
+    def _split_by_idx(payload, marker):
+        try:
+            return payload[payload.index(marker) :]
+        except (LookupError, TypeError, ValueError):
+            return False
 
     def _parse_tables(self, pkt, pid):
         """
         _parse_tables parse for
         PAT, PMT,  and SDT tables
         based on pid of the pkt
         """
-        pay = self._parse_payload(pkt)
-        if self._same_as_last(pay, pid):
-            return False
-        if pid in self.pids.pmt:
-            return self._parse_pmt(pay, pid)
-        if pid == self.pids.PAT_PID:
-            return self._parse_pat(pay)
-        if pid == self.pids.SDT_PID and self.info:
-            return self._parse_sdt(pay)
-        return False
-
-    def _parse_info(self, pkt):
-        """
-        _parse_info parses the packet for tables
-        and returns the pid
-        """
-        pid = self._parse_pid(pkt[1], pkt[2])
-        if pid in self.pids.tables:
-            self._parse_tables(pkt, pid)
-        return pid
+        payload = self._parse_payload(pkt)
+        if not self._chk_last(payload, pid):
+            if pid == self._PAT_PID:
+                self._program_association_table(payload)
+            elif pid == self._SDT_PID:
+                if self.info:
+                    self._stream_descriptor_table(payload)
+            else:
+                self._program_map_table(payload, pid)
 
     def _parse(self, pkt):
-        cue = False
-        pid = self._parse_info(pkt)
-        # self._parse_cc(pkt, pid)
-        self._parse_pts(pkt, pid)
-        if pid in self.pids.scte35:
-            cue = self._parse_scte35(pkt, pid)
-        return cue
-
-    def _chk_partial(self, pay, pid, sep):
-        if pid in self.maps.partial:
-            pay = self.maps.partial.pop(pid) + pay
-        return self._split_by_idx(pay, sep)
-
-    def _same_as_last(self, pay, pid):
-        if pid in self.maps.last:
-            return pay == self.maps.last[pid]
-        self.maps.last[pid] = pay
+        pid = self._parse_pid(pkt[1], pkt[2])
+        if pid in self._pids["pcr"]:
+            self._parse_pcr(pkt, pid)
+        if pid in self._pids["tables"]:
+            return self._parse_tables(pkt, pid)
+        if pid in self._pids["scte35"]:
+            return self._parse_scte35(pkt, pid)
+        if self._parse_pusi(pkt[1]):
+            self._parse_pts(pkt, pid)
+        return None
+
+    def _chk_partial(self, payload, pid, sep):
+        if pid in self._partial:
+            payload = self._partial.pop(pid) + payload
+        return self._split_by_idx(payload, sep)
+
+    def _chk_last(self, payload, pid):
+        if pid in self._last:
+            return payload == self._last[pid]
+        self._last[pid] = payload
         return False
 
-    def _section_incomplete(self, pay, pid, seclen):
+    def _section_done(self, payload, pid, seclen):
         # + 3 for the bytes before section starts
-        if (seclen + 3) > len(pay):
-            self.maps.partial[pid] = pay
-            return True
-        return False
+        if (seclen + 3) > len(payload):
+            self._partial[pid] = payload
+            return False
+        return True
 
-    def _parse_cue(self, pay, pid):
+    def _parse_cue(self, payload, pid):
         packet_data = None
         packet_data = self._mk_packet_data(pid)
-        cue = Cue(pay, packet_data)
+        cue = Cue(payload, packet_data)
         if cue.decode():
             return cue
-        return False
+        return None
 
     def _parse_scte35(self, pkt, pid):
         """
         parse a scte35 cue from one or more packets
         """
-        pay = self._parse_payload(pkt)
-        if not pay:
+        payload = self._chk_partial(self._parse_payload(pkt), pid, self._SCTE35_TID)
+        if not payload:
+            self._pids["scte35"].remove(pid)
             return False
-        pay = self._chk_partial(pay, pid, self._SCTE35_TID)
-        if not pay:
-            self.pids.scte35.remove(pid)
+        if payload[13] == self.show_null:
             return False
-        if pay[13] == self.show_null:
+        seclen = self._parse_length(payload[1], payload[2])
+        if not self._section_done(payload, pid, seclen):
             return False
-        seclen = self._parse_length(pay[1], pay[2])
-        if self._section_incomplete(pay, pid, seclen):
-            return False
-        pay = pay[: seclen + 3]
-        cue = self._parse_cue(pay, pid)
+        payload = payload[: seclen + 3]
+        cue = self._parse_cue(payload, pid)
         return cue
 
-    def _parse_sdt(self, pay):
+    def _stream_descriptor_table(self, payload):
         """
-        _parse_sdt parses the SDT for program metadata
+        _stream_descriptor_table parses the SDT for program metadata
         """
-        pay = self._chk_partial(pay, self.pids.SDT_PID, self._SDT_TID)
-        if not pay:
-            return False
-        seclen = self._parse_length(pay[1], pay[2])
-        if self._section_incomplete(pay, self.pids.SDT_PID, seclen):
+        payload = self._chk_partial(payload, self._SDT_PID, b"")
+        seclen = self._parse_length(payload[2], payload[3])
+        if not self._section_done(payload, self._SDT_PID, seclen):
             return False
-        idx = 11
+        idx = 12
         while idx < seclen + 3:
-            service_id = self._parse_program(pay[idx], pay[idx + 1])
+            service_id = self._parse_program(payload[idx], payload[idx + 1])
             idx += 3
-            dloop_len = self._parse_length(pay[idx], pay[idx + 1])
+            dloop_len = self._parse_length(payload[idx], payload[idx + 1])
             idx += 2
             i = 0
             while i < dloop_len:
-                if pay[idx] == 0x48:
+                if payload[idx] == 0x48:
                     i += 3
-                    spnl = pay[idx + i]
+                    spnl = payload[idx + i]
                     i += 1
-                    service_provider_name = pay[idx + i : idx + i + spnl]
+                    service_provider_name = payload[idx + i : idx + i + spnl]
                     i += spnl
-                    snl = pay[idx + i]
+                    snl = payload[idx + i]
                     i += 1
-                    service_name = pay[idx + i : idx + i + snl]
+                    service_name = payload[idx + i : idx + i + snl]
                     i += snl
-                    if service_id not in self.maps.prgm:
-                        self.maps.prgm[service_id] = ProgramInfo()
-                    pinfo = self.maps.prgm[service_id]
+                    if service_id not in self._prgm:
+                        self._prgm[service_id] = ProgramInfo()
+                    pinfo = self._prgm[service_id]
                     pinfo.provider = service_provider_name
                     pinfo.service = service_name
                 i = dloop_len
                 idx += i
 
-    def _parse_pat(self, pay):
+    def _program_association_table(self, payload):
         """
         parse program association table
         for program to pmt_pid mappings.
         """
-        pay = self._chk_partial(pay, self.pids.PAT_PID, b"")
-        seclen = self._parse_length(pay[2], pay[3])
-        if self._section_incomplete(pay, self.pids.PAT_PID, seclen):
+        payload = self._chk_partial(payload, self._PAT_PID, b"")
+        seclen = self._parse_length(payload[2], payload[3])
+        if not self._section_done(payload, self._PAT_PID, seclen):
             return False
-        seclen -= 5  # pay bytes 4,5,6,7,8
+        seclen -= 5  # payload bytes 4,5,6,7,8
         idx = 9
         chunk_size = 4
         while seclen > 4:  #  4 bytes for crc
-            program_number = self._parse_program(pay[idx], pay[idx + 1])
+            program_number = self._parse_program(payload[idx], payload[idx + 1])
             if program_number > 0:
-                pmt_pid = self._parse_pid(pay[idx + 2], pay[idx + 3])
-                self.pids.pmt.add(pmt_pid)
-                self.pids.tables.add(pmt_pid)
+                pmt_pid = self._parse_pid(payload[idx + 2], payload[idx + 3])
+                self._pids["tables"].add(pmt_pid)
             seclen -= chunk_size
             idx += chunk_size
 
-    def _parse_pmt(self, pay, pid):
+    def _program_map_table(self, payload, pid):
         """
         parse program maps for streams
         """
-        pay = self._chk_partial(pay, pid, self._PMT_TID)
-        if not pay:
+        payload = self._chk_partial(payload, pid, self._PMT_TID)
+        if not payload:
             return False
-        seclen = self._parse_length(pay[1], pay[2])
-        if self._section_incomplete(pay, pid, seclen):
+        seclen = self._parse_length(payload[1], payload[2])
+        if not self._section_done(payload, pid, seclen):
             return False
-        program_number = self._parse_program(pay[3], pay[4])
+        program_number = self._parse_program(payload[3], payload[4])
         if self.the_program and (program_number != self.the_program):
             return False
-        pcr_pid = self._parse_pid(pay[8], pay[9])
-        if program_number not in self.maps.prgm:
-            self.maps.prgm[program_number] = ProgramInfo()
-        pinfo = self.maps.prgm[program_number]
+        pcr_pid = self._parse_pid(payload[8], payload[9])
+        if program_number not in self._prgm:
+            self._prgm[program_number] = ProgramInfo()
+        pinfo = self._prgm[program_number]
         pinfo.pid = pid
         pinfo.pcr_pid = pcr_pid
-        self.pids.pcr.add(pcr_pid)
-        self.maps.pid_prgm[pcr_pid] = program_number
-        proginfolen = self._parse_length(pay[10], pay[11])
-        idx = 12 + proginfolen
-        si_len = seclen - (9 + proginfolen)
-        self._parse_program_streams(si_len, pay, idx, program_number)
+        self._prgm[program_number] = pinfo
+        self._pids["pcr"].add(pcr_pid)
+        self._pid_prgm[pcr_pid] = program_number
+        proginfolen = self._parse_length(payload[10], payload[11])
+        idx = 12
+        idx += proginfolen
+        si_len = seclen - 9
+        si_len -= proginfolen
+        self._parse_program_streams(si_len, payload, idx, program_number)
         return True
 
-    def _parse_program_streams(self, si_len, pay, idx, program_number):
+    def _parse_program_streams(self, si_len, payload, idx, program_number):
         """
         parse the elementary streams
         from a program
         """
         # 5 bytes for stream_type info
         chunk_size = 5
         end_idx = (idx + si_len) - chunk_size
         while idx < end_idx:
-            stream_type, pid, ei_len = self._parse_stream_type(pay, idx)
-            pinfo = self.maps.prgm[program_number]
+            stream_type, pid, ei_len = self._parse_stream_type(payload, idx)
+            pinfo = self._prgm[program_number]
             pinfo.streams[pid] = stream_type
-            idx += chunk_size + ei_len
-            self.maps.pid_prgm[pid] = program_number
+            idx += chunk_size
+            idx += ei_len
+            self._pid_prgm[pid] = program_number
+            self._chk_pid_stream_type(pid, stream_type)
 
-    def _parse_stream_type(self, pay, idx):
+    def _parse_stream_type(self, payload, idx):
         """
         extract stream pid and type
         """
-        stream_type = hex(pay[idx])
-        el_pid = self._parse_pid(pay[idx + 1], pay[idx + 2])
-        ei_len = self._parse_length(pay[idx + 3], pay[idx + 4])
-        self._set_scte35_pids(el_pid, stream_type)
+        stream_type = hex(payload[idx])
+        el_pid = self._parse_pid(payload[idx + 1], payload[idx + 2])
+        ei_len = self._parse_length(payload[idx + 3], payload[idx + 4])
         return stream_type, el_pid, ei_len
 
-    def _set_scte35_pids(self, pid, stream_type):
+    def _chk_pid_stream_type(self, pid, stream_type):
         """
         if stream_type is 0x06 or 0x86
         add it to self._scte35_pids.
         """
         if stream_type in ["0x6", "0x86"]:
-            self.pids.scte35.add(pid)
+            self._pids["scte35"].add(pid)
```

