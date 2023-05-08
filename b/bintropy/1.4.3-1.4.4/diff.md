# Comparing `tmp/bintropy-1.4.3.tar.gz` & `tmp/bintropy-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bintropy-1.4.3.tar", last modified: Mon Apr 17 20:33:42 2023, max compression
+gzip compressed data, was "bintropy-1.4.4.tar", last modified: Mon May  8 20:15:49 2023, max compression
```

## Comparing `bintropy-1.4.3.tar` & `bintropy-1.4.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:33:42.403380 bintropy-1.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:33:42.403380 bintropy-1.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:33:42.403380 bintropy-1.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-17 20:33:34.000000 bintropy-1.4.3/.github/workflows/python-package.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-04-17 20:33:34.000000 bintropy-1.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 20:33:34.000000 bintropy-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-17 20:33:42.403380 bintropy-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-17 20:33:34.000000 bintropy-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:33:42.403380 bintropy-1.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    65270 2023-04-17 20:33:34.000000 bintropy-1.4.3/docs/example-not-packed.png
--rw-r--r--   0 runner    (1001) docker     (123)    56052 2023-04-17 20:33:34.000000 bintropy-1.4.3/docs/example-packed.png
--rw-r--r--   0 runner    (1001) docker     (123)    32366 2023-04-17 20:33:34.000000 bintropy-1.4.3/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-17 20:33:34.000000 bintropy-1.4.3/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-04-17 20:33:34.000000 bintropy-1.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 20:33:42.403380 bintropy-1.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:33:42.403380 bintropy-1.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:33:42.403380 bintropy-1.4.3/src/bintropy/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 20:33:34.000000 bintropy-1.4.3/src/bintropy/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-17 20:33:34.000000 bintropy-1.4.3/src/bintropy/__info__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23759 2023-04-17 20:33:34.000000 bintropy-1.4.3/src/bintropy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-17 20:33:34.000000 bintropy-1.4.3/src/bintropy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:33:42.403380 bintropy-1.4.3/src/bintropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-17 20:33:42.000000 bintropy-1.4.3/src/bintropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-17 20:33:42.000000 bintropy-1.4.3/src/bintropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 20:33:42.000000 bintropy-1.4.3/src/bintropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 20:33:42.000000 bintropy-1.4.3/src/bintropy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 20:33:42.000000 bintropy-1.4.3/src/bintropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 20:33:42.000000 bintropy-1.4.3/src/bintropy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:15:49.877858 bintropy-1.4.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:15:49.873858 bintropy-1.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:15:49.877858 bintropy-1.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-08 20:15:41.000000 bintropy-1.4.4/.github/workflows/python-package.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-05-08 20:15:41.000000 bintropy-1.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 20:15:41.000000 bintropy-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-05-08 20:15:49.877858 bintropy-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-08 20:15:42.000000 bintropy-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:15:49.877858 bintropy-1.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    65270 2023-05-08 20:15:41.000000 bintropy-1.4.4/docs/example-not-packed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56052 2023-05-08 20:15:41.000000 bintropy-1.4.4/docs/example-packed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32366 2023-05-08 20:15:41.000000 bintropy-1.4.4/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-08 20:15:41.000000 bintropy-1.4.4/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-05-08 20:15:41.000000 bintropy-1.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:15:49.877858 bintropy-1.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:15:49.877858 bintropy-1.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:15:49.877858 bintropy-1.4.4/src/bintropy/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 20:15:41.000000 bintropy-1.4.4/src/bintropy/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-08 20:15:41.000000 bintropy-1.4.4/src/bintropy/__info__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25137 2023-05-08 20:15:41.000000 bintropy-1.4.4/src/bintropy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-08 20:15:41.000000 bintropy-1.4.4/src/bintropy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:15:49.877858 bintropy-1.4.4/src/bintropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-05-08 20:15:49.000000 bintropy-1.4.4/src/bintropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-08 20:15:49.000000 bintropy-1.4.4/src/bintropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:15:49.000000 bintropy-1.4.4/src/bintropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 20:15:49.000000 bintropy-1.4.4/src/bintropy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:15:49.000000 bintropy-1.4.4/src/bintropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 20:15:49.000000 bintropy-1.4.4/src/bintropy.egg-info/top_level.txt
```

### Comparing `bintropy-1.4.3/.github/workflows/python-package.yml` & `bintropy-1.4.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.3/.gitignore` & `bintropy-1.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.3/LICENSE` & `bintropy-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.3/PKG-INFO` & `bintropy-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bintropy
-Version: 1.4.3
+Version: 1.4.4
 Summary: Analysis tool for estimating the likelihood that a binary contains compressed or encrypted bytes
 Author-email: Alexandre D'Hondt <alexandre.dhondt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bintropy-1.4.3/README.md` & `bintropy-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.3/docs/example-not-packed.png` & `bintropy-1.4.4/docs/example-not-packed.png`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.3/docs/example-packed.png` & `bintropy-1.4.4/docs/example-packed.png`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.3/docs/logo.png` & `bintropy-1.4.4/docs/logo.png`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.3/pyproject.toml` & `bintropy-1.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.3/src/bintropy/__info__.py` & `bintropy-1.4.4/src/bintropy/__info__.py`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.3/src/bintropy/__init__.py` & `bintropy-1.4.4/src/bintropy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -*- coding: UTF-8 -*-
 import lief
 import math
 import os
+import re
 import statistics
+from functools import lru_cache
 
 
 __all__ = ["bintropy", "characteristics", "entropy", "is_packed", "plot", "THRESHOLDS"]
 
 
 __btype = lambda b: str(type(b)).split(".")[2]
 __log = lambda l, m, lvl="debug": getattr(l, lvl)(m) if l else None
@@ -93,14 +95,30 @@
     i, units = 0, ["B", "KB", "MB", "GB", "TB", "PB", "EB", "ZB", "YB"]
     while size > 1024 and i < len(units):
         i += 1
         size /= 1024.0
     return "%.*f%s" % (precision, size, units[i])
 
 
+# dirty fix for section names requiring to get their real names from the string table (as lief does not seem to handle
+#  this in every case)
+@lru_cache
+def _real_section_names(path):
+    from subprocess import check_output
+    try:
+        names, out = [], check_output(["objdump", "-h", path]).decode()
+    except FileNotFoundError:
+        return
+    for l in out.split("\n"):
+        m = re.match(r"\s+\d+\s(.*?)\s+", l)
+        if m:
+            names.append(m.group(1))
+    return names
+
+
 def bintropy(executable, mode=0, blocksize=256, ignore_half_block_zeros=True, decide=True,
              threshold_average_entropy=None, threshold_highest_entropy=None, logger=None, **kwargs):
     """ Simple implementation of Bintropy as of https://ieeexplore.ieee.org/document/4140989.
     
     :param executable:                path to the executable to be analyzed
     :param full:                      process the executable as a whole or per section only (cfr modes of operation)
     :param blocksize:                 process per block of N bytes (0 means considering the executable as a whole)
@@ -108,25 +126,26 @@
     :param decide:                    decide if packed or not, otherwise simply return the entropy values
     :param threshold_average_entropy: threshold on average entropy for deciding if packed
     :param threshold_highest_entropy: threshold on highest entropy for deciding if packed
     :param logger:                    logger instance for debug purpose
     :return:                          if decide is True  => bool (whether the input executable is packed or not)
                                                    False => (average_entropy, highest_block_entropy)
     """
+    path = str(executable)
     # try to parse the binary first
-    binary = lief.parse(str(executable))
+    binary = lief.parse(path)
     if binary is None:
         raise OSError("Unknown format")
     # now select the right thresholds
     thresholds = THRESHOLDS.get(binary.format, THRESHOLDS['default'])
     _t1, _t2 = threshold_average_entropy, threshold_highest_entropy
     _t1, _t2 = [_t1, thresholds[0]][_t1 is None], [_t2, thresholds[1]][_t2 is None]
     # FIRST MODE: compute the entropy of the whole executable
     if mode == 0:
-        with open(str(executable), 'rb') as f:
+        with open(path, 'rb') as f:
             exe = f.read()
         __log(logger, "Entropy (Shannon): {}".format(entropy(exe)))
         e = entropy(exe, blocksize, ignore_half_block_zeros)
         if logger:
             msg = "Entropy (average): {}".format(e[1] or "-")
             if e[0] != [None]:
                 iw = len(str(len(e[0])))
@@ -145,16 +164,21 @@
         def _handle(n, d):
             r = entropy(d, blocksize, ignore_half_block_zeros)
             e[n] = r if isinstance(r, (list, tuple)) else ([r], r)
             w[n] = len(d)
         e, w = {}, {}
         if mode == 1:  # per section
             if len(binary.sections) > 0:
-                for section in binary.sections:
+                for i, section in enumerate(binary.sections):
                     n, d = section.name, section.content
+                    # special case: for some executables compiled with debug information, some sections may be named
+                    #                with the format "/[N]" where N is the offset in the string table ; in this case, we
+                    #                compute the real section names
+                    if re.match(r"^\/\d+$", n) and _real_section_names(path):
+                        n = _real_section_names(path)[i]
                     _handle(n, d)
             else:  # in some cases, packed executables can have no section ; e.g. UPX(/bin/ls)
                 __log(logger, "This file has no section", "error")
                 __log(logger, "please try another mode of operation", "warning")
                 return
         elif mode == 2:  # per segment
             for i, segment in enumerate(binary.segments):
@@ -189,19 +213,19 @@
         - executable type
         - entry point (set according to the 'x' samples)
     
     :param executable:  path to executable whose characteristics are to be computed
     :param n_samples:   number of samples of entropy required
     :param window_size: window size for computing the entropy
     """
-    data = {'name': os.path.basename(executable), 'entropy': [], 'sections': []}
+    data, path = {'name': os.path.basename(executable), 'entropy': [], 'sections': []}, str(executable)
     # compute window-based entropy
-    with open(str(executable), "rb") as f:
+    with open(path, "rb") as f:
         data['entropy*'] = entropy(f.read())
-    with open(str(executable), "rb") as f:
+    with open(path, "rb") as f:
         size = data['size'] = os.fstat(f.fileno()).st_size
         step = abs(size // n_samples)
         chunksize = data['chunksize'] = size / n_samples
         if isinstance(window_size, type(lambda: 0)):
             window_size = window_size(step)
         # ensure the window interval is at least 256 (that is 2^8 ; with a 'security' factor of 2)) because otherwise if
         #  using a too small executable, it may get undersampled and have lower entropy values than actual
@@ -214,30 +238,34 @@
             window += f.read(new_pos - cur_pos if i > 0 else winter)
             window = window[max(0, len(window)-window_size) if cur_pos + winter < size else step:]
             # compute entropy
             data['entropy'].append(entropy(window)/8.)
     # compute other characteristics using LIEF (catch warnings from stderr)
     tmp_fd, null_fd = os.dup(2), os.open(os.devnull, os.O_RDWR)
     os.dup2(null_fd, 2)
-    binary = lief.parse(str(executable))
+    binary = lief.parse(path)
     os.dup2(tmp_fd, 2)  # restore stderr
     os.close(null_fd)
     if binary is None:
         raise TypeError("Not an executable")
     data['type'] = __btype(binary)
     # entry point (EP)
     ep, ep_section = _get_ep_and_section(binary)
     # convert to 3-tuple (EP offset on plot, EP file offset, section name containing EP)
     data['entrypoint'] = None if ep is None else (int(ep // data['chunksize']), ep, __secname(ep_section))
     # sections
     __d = lambda s, e, n: (int(s), int(e), n, statistics.mean(data['entropy'][int(s):int(e)+1]))
     data['sections'] = [__d(0, int(max(MIN_ZONE_WIDTH, binary.sections[0].offset // chunksize)), "Headers")] \
                        if len(binary.sections) > 0 else []
-    for section in binary.sections:
+    for i, section in enumerate(binary.sections):
         name = __secname(section.name)
+        # special case: for some executables compiled with debug information, sections may be of the form "/[N]" (where
+        #                N is the offset in the string table ; in this case, we compute the real section names)
+        if re.match(r"^\/\d+$", name) and _real_section_names(path):
+            name = _real_section_names(path)[i]
         start = max(data['sections'][-1][1] if len(data['sections']) > 0 else 0, int(section.offset // chunksize))
         max_end = min(max(start + MIN_ZONE_WIDTH, int((section.offset + section.size) // chunksize)),
                       len(data['entropy']) - 1)
         data['sections'].append(__d(int(min(start, max_end - MIN_ZONE_WIDTH)), int(max_end), name))
     # adjust the entry point (be sure that its position on the plot is within the EP section)
     if ep:
         ep_pos, _, ep_sec_name = data['entrypoint']
```

### Comparing `bintropy-1.4.3/src/bintropy/__main__.py` & `bintropy-1.4.4/src/bintropy/__main__.py`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.3/src/bintropy.egg-info/PKG-INFO` & `bintropy-1.4.4/src/bintropy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bintropy
-Version: 1.4.3
+Version: 1.4.4
 Summary: Analysis tool for estimating the likelihood that a binary contains compressed or encrypted bytes
 Author-email: Alexandre D'Hondt <alexandre.dhondt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

