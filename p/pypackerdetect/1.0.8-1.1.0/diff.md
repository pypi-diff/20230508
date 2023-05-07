# Comparing `tmp/pypackerdetect-1.0.8.tar.gz` & `tmp/pypackerdetect-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypackerdetect-1.0.8.tar", last modified: Sat Feb 25 22:00:59 2023, max compression
+gzip compressed data, was "pypackerdetect-1.1.0.tar", last modified: Sun May  7 23:19:37 2023, max compression
```

## Comparing `pypackerdetect-1.0.8.tar` & `pypackerdetect-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:00:59.235569 pypackerdetect-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:00:59.227569 pypackerdetect-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:00:59.231569 pypackerdetect-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-02-25 22:00:50.000000 pypackerdetect-1.0.8/.github/workflows/python-package.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-02-25 22:00:50.000000 pypackerdetect-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-25 22:00:50.000000 pypackerdetect-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    45307 2023-02-25 22:00:59.235569 pypackerdetect-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-02-25 22:00:50.000000 pypackerdetect-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:00:59.231569 pypackerdetect-1.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    26902 2023-02-25 22:00:50.000000 pypackerdetect-1.0.8/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-02-25 22:00:50.000000 pypackerdetect-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-25 22:00:50.000000 pypackerdetect-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-25 22:00:59.235569 pypackerdetect-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:00:59.231569 pypackerdetect-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:00:59.231569 pypackerdetect-1.0.8/src/pypackerdetect/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-25 22:00:50.000000 pypackerdetect-1.0.8/src/pypackerdetect/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-02-25 22:00:50.000000 pypackerdetect-1.0.8/src/pypackerdetect/__info__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-02-25 22:00:50.000000 pypackerdetect-1.0.8/src/pypackerdetect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-02-25 22:00:50.000000 pypackerdetect-1.0.8/src/pypackerdetect/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:00:59.235569 pypackerdetect-1.0.8/src/pypackerdetect/db/
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-02-25 22:00:50.000000 pypackerdetect-1.0.8/src/pypackerdetect/db/packers.json
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-02-25 22:00:50.000000 pypackerdetect-1.0.8/src/pypackerdetect/db/sections.json
--rw-r--r--   0 runner    (1001) docker     (123)  1188755 2023-02-25 22:00:50.000000 pypackerdetect-1.0.8/src/pypackerdetect/db/sigs_long.txt
--rw-r--r--   0 runner    (1001) docker     (123)   492372 2023-02-25 22:00:50.000000 pypackerdetect-1.0.8/src/pypackerdetect/db/sigs_short.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:00:59.231569 pypackerdetect-1.0.8/src/pypackerdetect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    45307 2023-02-25 22:00:59.000000 pypackerdetect-1.0.8/src/pypackerdetect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-02-25 22:00:59.000000 pypackerdetect-1.0.8/src/pypackerdetect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 22:00:59.000000 pypackerdetect-1.0.8/src/pypackerdetect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-25 22:00:59.000000 pypackerdetect-1.0.8/src/pypackerdetect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-25 22:00:59.000000 pypackerdetect-1.0.8/src/pypackerdetect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-25 22:00:59.000000 pypackerdetect-1.0.8/src/pypackerdetect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:19:37.722865 pypackerdetect-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:19:37.714865 pypackerdetect-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:19:37.714865 pypackerdetect-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-07 23:19:29.000000 pypackerdetect-1.1.0/.github/workflows/python-package.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-05-07 23:19:29.000000 pypackerdetect-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 23:19:29.000000 pypackerdetect-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    45307 2023-05-07 23:19:37.722865 pypackerdetect-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-07 23:19:29.000000 pypackerdetect-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:19:37.714865 pypackerdetect-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    26902 2023-05-07 23:19:29.000000 pypackerdetect-1.1.0/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-07 23:19:29.000000 pypackerdetect-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-07 23:19:29.000000 pypackerdetect-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 23:19:37.722865 pypackerdetect-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:19:37.714865 pypackerdetect-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:19:37.718865 pypackerdetect-1.1.0/src/pypackerdetect/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 23:19:29.000000 pypackerdetect-1.1.0/src/pypackerdetect/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-07 23:19:29.000000 pypackerdetect-1.1.0/src/pypackerdetect/__info__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-07 23:19:29.000000 pypackerdetect-1.1.0/src/pypackerdetect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-05-07 23:19:29.000000 pypackerdetect-1.1.0/src/pypackerdetect/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:19:37.718865 pypackerdetect-1.1.0/src/pypackerdetect/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-07 23:19:29.000000 pypackerdetect-1.1.0/src/pypackerdetect/db/packers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-07 23:19:29.000000 pypackerdetect-1.1.0/src/pypackerdetect/db/sections.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1188755 2023-05-07 23:19:29.000000 pypackerdetect-1.1.0/src/pypackerdetect/db/sigs_long.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   492372 2023-05-07 23:19:29.000000 pypackerdetect-1.1.0/src/pypackerdetect/db/sigs_short.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:19:37.718865 pypackerdetect-1.1.0/src/pypackerdetect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    45307 2023-05-07 23:19:37.000000 pypackerdetect-1.1.0/src/pypackerdetect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-07 23:19:37.000000 pypackerdetect-1.1.0/src/pypackerdetect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 23:19:37.000000 pypackerdetect-1.1.0/src/pypackerdetect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-07 23:19:37.000000 pypackerdetect-1.1.0/src/pypackerdetect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-07 23:19:37.000000 pypackerdetect-1.1.0/src/pypackerdetect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-07 23:19:37.000000 pypackerdetect-1.1.0/src/pypackerdetect.egg-info/top_level.txt
```

### Comparing `pypackerdetect-1.0.8/.github/workflows/python-package.yml` & `pypackerdetect-1.1.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pypackerdetect-1.0.8/.gitignore` & `pypackerdetect-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pypackerdetect-1.0.8/LICENSE` & `pypackerdetect-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypackerdetect-1.0.8/PKG-INFO` & `pypackerdetect-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypackerdetect
-Version: 1.0.8
+Version: 1.1.0
 Summary: Re-implementation and packaging of PyPackerDetect
 Author-email: Alexandre D'Hondt <alexandre.dhondt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pypackerdetect-1.0.8/README.md` & `pypackerdetect-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pypackerdetect-1.0.8/docs/logo.png` & `pypackerdetect-1.1.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `pypackerdetect-1.0.8/pyproject.toml` & `pypackerdetect-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pypackerdetect-1.0.8/src/pypackerdetect/__info__.py` & `pypackerdetect-1.1.0/src/pypackerdetect/__info__.py`

 * *Files identical despite different names*

### Comparing `pypackerdetect-1.0.8/src/pypackerdetect/__init__.py` & `pypackerdetect-1.1.0/src/pypackerdetect/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,133 +1,159 @@
-# -*- coding: UTF-8 -*-
-import json
-import os
-import pefile
-import peid
-
-
-__all__ = ["PyPackerDetect", "PACKERS", "SECTIONS"]
-
-
-with open(os.path.join(os.path.dirname(__file__), "db", "packers.json")) as f:
-    PACKERS = json.load(f)['packers']
-with open(os.path.join(os.path.dirname(__file__), "db", "sections.json")) as f:
-    SECTIONS = json.load(f)['sections']
-
-
-class PyPackerDetect:
-    def __init__(self, peid=True, peid_large_db=False, peid_ep_only=True, bad_ep_sections=True, low_imports=True,
-                 packer_sections=True, unknown_sections=True, import_threshold=10, unknown_sections_threshold=3,
-                 bad_sections_threshold=2, logger=None, **kwargs):
-        """ Configure the detector with various parameters. """
-        self.__config = {
-            'peid_large_db': peid_large_db, 'peid_ep_only': peid_ep_only, 'packer_sections': packer_sections,
-            'peid': peid, 'bad_ep_sec': bad_ep_sections, 'low_imports': low_imports, 'unknown_sec': unknown_sections,
-        }
-        self.__thresholds = {
-            'bad_sections':     bad_sections_threshold,
-            'imports':          import_threshold,
-            'unknown_sections': unknown_sections_threshold,
-        }
-        self.logger = logger
-    
-    def detect(self, pe):
-        """ Analyze the input PE file for suspicions and/or detections of packers. """
-        r, s = {'detections': [], 'suspicions': []}, .0
-        def __add(i, msg):
-            if self.logger:
-                self.logger.debug("%s:%s" % (['DETECTION', 'SUSPICION'][i], msg))
-            r[['detections', 'suspicions'][i]].append(msg)
-        if not isinstance(pe, pefile.PE):
-            path = pe
-            pe = pefile.PE(path)
-            pe.path = path
-        ep = pe.OPTIONAL_HEADER.AddressOfEntryPoint
-        # parse the input PE file
-        d = {'all': [], 'bad': [], 'ep': [], 'packer': [], 'unknown': []}
-        for s in pe.sections:
-            try:
-                n = s.Name.decode("ascii").strip().rstrip("\0")
-                d['all'].append(n)
-                if ep >= s.VirtualAddress and ep <= (s.VirtualAddress + s.Misc_VirtualSize):
-                    d['ep'].append(n)
-                if n not in SECTIONS['known']:
-                    d['unknown'].append(n)
-                p = PACKERS.get(n)
-                if p is not None:
-                    d['packer'].append(n)
-            except UnicodeDecodeError:
-                d['bad'].append(s.Name.decode('latin1').strip().rstrip("\0"))
-                __add(1, "Section name with invalid characters")
-        # bad entry point sections
-        __intersect = lambda l1, l2: len(set(l1).intersection(l2)) > 0
-        if self.__config['bad_ep_sec']:
-            ep_sec_list = "', '".join(d['ep'])
-            if ep == 0:
-                __add(1, "Null entry point")
-            l_ep = len(d['ep'])
-            if l_ep == 0:
-                __add(0, "Entry point 0x%x falls in overlapping sections: '%s'" % (ep, ep_sec_list))
-            else:
-                if l_ep > 1:
-                    __add(0, "Entry point 0x%x falls in overlapping sections: '%s'" % (ep, ep_sec_list))
-                if not __intersect(SECTIONS['acceptable'], d['ep']):
-                    bad_ep_sec = False
-                    if __intersect(SECTIONS['delphi-bss'], d['all']):
-                        # has bss, see if we have a delphi ep section
-                        bad_ep_sec = not __intersect(SECTIONS['delphi'], d['ep'])
-                    elif not __intersect(SECTIONS['acceptable'], d['all']):
-                        # normal entry section doesn't exist anywhere, so check for alternatives
-                        bad_ep_sec = not __intersect(SECTIONS['alternative'], d['ep'])
-                    else:
-                        # not regular ep section, not a delphi entry section, not an alternative entry section, and
-                        #  regular entry section name exists, so the only possibility left is a driver entry section
-                        bad_ep_sec = not __intersect(SECTIONS['driver'], d['ep'])
-                    if bad_ep_sec:
-                        __add(0, "Entry point 0x%x in irregular section(s): '%s'" % (ep, ep_sec_list))
-        # low import count
-        if self.__config['low_imports']:
-            c = 0
-            try:
-                for lib in pe.DIRECTORY_ENTRY_IMPORT:
-                    if lib.dll.decode("ascii").strip().rstrip("\0").lower() == "mscoree.dll":
-                        c = -1  # .NET assembly, counting imports is misleading as they will have a low number
-                        break
-                    c += len(lib.imports)
-            except AttributeError as e:
-                pass
-            if (0 <= c <= self.__thresholds['imports']):
-                __add(0, "Too few imports (total: %d)" % c)
-        # non standard sections
-        if self.__config['unknown_sec']:
-            u = len(d['unknown'])
-            un_sec_list = "', '".join(d['unknown'])
-            if u >= self.__thresholds['unknown_sections']:
-                __add(0, "Detected %d non-standard sections: '%s'" % (u, un_sec_list))
-            if len(d['bad']) >= self.__thresholds['bad_sections']:
-                __add(0, "Detected %d sections with invalid names" % len(d['bad']))
-        # packer sections
-        if self.__config['packer_sections']:
-            for n in d['packer']:
-                __add(0, "Section name '%s' matches known packer: [%s]" % (n, PACKERS[n]))
-        # apply PEiD
-        if self.__config['peid']:
-            db = os.path.join(os.path.dirname(__file__), "db", "sigs_long.txt") if self.__config['peid_large_db'] \
-                 else os.path.join(os.path.dirname(__file__), "db", "sigs_short.txt")
-            for m in peid.identify_packer(pe, db=db, ep_only=self.__config['peid_ep_only'], logger=self.logger):
-                if len(m[1]) > 0:
-                    __add(0, "Found PEID signature: %s" % ", ".join(m[1]))
-        return r
-    
-    @staticmethod
-    def report(pe, findings):
-        """ Report findings like the original project. """
-        print("Packer report for: %s" % (getattr(pe, "path", "unknown path") if isinstance(pe, pefile.PE) else pe))
-        print("\tDetections: %d" % len(findings['detections']))
-        print("\tSuspicions: %d" % len(findings['suspicions']))
-        if len(findings['detections']) > 0 or len(findings['suspicions']) > 0:
-            print("\tLog:")
-            for d in findings['detections']:
-                print("\t\t[DETECTION] %s" % d)
-            for s in findings['suspicions']:
-                print("\t\t[SUSPICION] %s" % s)
-
+# -*- coding: UTF-8 -*-
+import json
+import os
+import pefile
+import peid
+import re
+from functools import cached_property
+
+
+__all__ = ["PyPackerDetect", "PACKERS", "SECTIONS"]
+
+
+with open(os.path.join(os.path.dirname(__file__), "db", "packers.json")) as f:
+    PACKERS = json.load(f)['packers']
+with open(os.path.join(os.path.dirname(__file__), "db", "sections.json")) as f:
+    SECTIONS = json.load(f)['sections']
+
+
+# dirty fix for section names requiring to get their real names from the string table (as pefile does not seem to handle
+#  this in every case)
+class PE(pefile.PE):
+    @cached_property
+    def real_section_names(self):
+        from subprocess import check_output
+        try:
+            names, out = [], check_output(["objdump", "-h", self.path]).decode()
+        except FileNotFoundError:
+            return
+        for l in out.split("\n"):
+            m = re.match(r"\s+\d+\s(.*?)\s+", l)
+            if m:
+                names.append(m.group(1))
+        return names
+
+
+class PyPackerDetect:
+    def __init__(self, peid=True, peid_large_db=False, peid_ep_only=True, bad_ep_sections=True, low_imports=True,
+                 packer_sections=True, unknown_sections=True, import_threshold=10, unknown_sections_threshold=3,
+                 bad_sections_threshold=2, logger=None, **kwargs):
+        """ Configure the detector with various parameters. """
+        self.__config = {
+            'peid_large_db': peid_large_db, 'peid_ep_only': peid_ep_only, 'packer_sections': packer_sections,
+            'peid': peid, 'bad_ep_sec': bad_ep_sections, 'low_imports': low_imports, 'unknown_sec': unknown_sections,
+        }
+        self.__thresholds = {
+            'bad_sections':     bad_sections_threshold,
+            'imports':          import_threshold,
+            'unknown_sections': unknown_sections_threshold,
+        }
+        self.logger = logger
+    
+    def detect(self, pe):
+        """ Analyze the input PE file for suspicions and/or detections of packers. """
+        r, s = {'detections': [], 'suspicions': []}, .0
+        def __add(i, msg):
+            if self.logger:
+                self.logger.debug("%s:%s" % (['DETECTION', 'SUSPICION'][i], msg))
+            r[['detections', 'suspicions'][i]].append(msg)
+        if not isinstance(pe, pefile.PE):
+            path = pe
+            pe = PE(path)
+            pe.path = path
+        ep = pe.OPTIONAL_HEADER.AddressOfEntryPoint
+        # parse the input PE file
+        d = {'all': [], 'bad': [], 'ep': [], 'packer': [], 'unknown': []}
+        for i, s in enumerate(pe.sections):
+            try:
+                n = s.Name.decode("ascii").strip().rstrip("\0")
+                # special case: for some executables compiled with debug information, some sections may be named with
+                #                the format "/[N]" where N is the offset in the string table ; in this case, we compute
+                #                the real section names and map them to the shortened ones to compare the relevant names
+                #                with the database of known section names
+                if re.match(r"^\/\d+$", n) and pe.real_section_names:
+                    n = pe.real_section_names[i]
+                d['all'].append(n)
+                if ep >= s.VirtualAddress and ep <= (s.VirtualAddress + s.Misc_VirtualSize):
+                    d['ep'].append(n)
+                if n not in SECTIONS['known']:
+                    d['unknown'].append(n)
+                p = PACKERS.get(n)
+                # even if found in the packers database, ensure the related section name does not clash with a known one
+                if p is not None and n not in SECTIONS['known']:
+                    d['packer'].append(n)
+            except UnicodeDecodeError:
+                d['bad'].append(s.Name.decode('latin1').strip().rstrip("\0"))
+                __add(1, "Section name with invalid characters")
+        # bad entry point sections
+        __intersect = lambda l1, l2: len(set(l1).intersection(l2)) > 0
+        if self.__config['bad_ep_sec']:
+            ep_sec_list = "', '".join(d['ep'])
+            if ep == 0:
+                __add(1, "Null entry point")
+            l_ep = len(d['ep'])
+            if l_ep == 0:
+                __add(0, "Entry point 0x%x falls in overlapping sections: '%s'" % (ep, ep_sec_list))
+            else:
+                if l_ep > 1:
+                    __add(0, "Entry point 0x%x falls in overlapping sections: '%s'" % (ep, ep_sec_list))
+                if not __intersect(SECTIONS['acceptable'], d['ep']):
+                    bad_ep_sec = False
+                    if __intersect(SECTIONS['delphi-bss'], d['all']):
+                        # has bss, see if we have a delphi ep section
+                        bad_ep_sec = not __intersect(SECTIONS['delphi'], d['ep'])
+                    elif not __intersect(SECTIONS['acceptable'], d['all']):
+                        # normal entry section doesn't exist anywhere, so check for alternatives
+                        bad_ep_sec = not __intersect(SECTIONS['alternative'], d['ep'])
+                    else:
+                        # not regular ep section, not a delphi entry section, not an alternative entry section, and
+                        #  regular entry section name exists, so the only possibility left is a driver entry section
+                        bad_ep_sec = not __intersect(SECTIONS['driver'], d['ep'])
+                    if bad_ep_sec:
+                        __add(0, "Entry point 0x%x in irregular section(s): '%s'" % (ep, ep_sec_list))
+        # low import count
+        if self.__config['low_imports']:
+            c = 0
+            try:
+                for lib in pe.DIRECTORY_ENTRY_IMPORT:
+                    if lib.dll.decode("ascii").strip().rstrip("\0").lower() == "mscoree.dll":
+                        c = -1  # .NET assembly, counting imports is misleading as they will have a low number
+                        break
+                    c += len(lib.imports)
+            except AttributeError as e:
+                pass
+            if (0 <= c <= self.__thresholds['imports']):
+                __add(0, "Too few imports (total: %d)" % c)
+        # non standard sections
+        if self.__config['unknown_sec']:
+            u = len(d['unknown'])
+            un_sec_list = "', '".join(d['unknown'])
+            if u >= self.__thresholds['unknown_sections']:
+                __add(0, "Detected %d non-standard sections: '%s'" % (u, un_sec_list))
+            if len(d['bad']) >= self.__thresholds['bad_sections']:
+                __add(0, "Detected %d sections with invalid names" % len(d['bad']))
+        # packer sections
+        if self.__config['packer_sections']:
+            for n in d['packer']:
+                __add(0, "Section name '%s' matches known packer: [%s]" % (n, PACKERS[n]))
+        # apply PEiD
+        if self.__config['peid']:
+            db = os.path.join(os.path.dirname(__file__), "db", "sigs_long.txt") if self.__config['peid_large_db'] \
+                 else os.path.join(os.path.dirname(__file__), "db", "sigs_short.txt")
+            for m in peid.identify_packer(pe, db=db, ep_only=self.__config['peid_ep_only'], logger=self.logger):
+                if len(m[1]) > 0:
+                    __add(0, "Found PEID signature: %s" % ", ".join(m[1]))
+        return r
+    
+    @staticmethod
+    def report(pe, findings):
+        """ Report findings like the original project. """
+        print("Packer report for: %s" % (getattr(pe, "path", "unknown path") if isinstance(pe, pefile.PE) else pe))
+        print("\tDetections: %d" % len(findings['detections']))
+        print("\tSuspicions: %d" % len(findings['suspicions']))
+        if len(findings['detections']) > 0 or len(findings['suspicions']) > 0:
+            print("\tLog:")
+            for d in findings['detections']:
+                print("\t\t[DETECTION] %s" % d)
+            for s in findings['suspicions']:
+                print("\t\t[SUSPICION] %s" % s)
+
```

### Comparing `pypackerdetect-1.0.8/src/pypackerdetect/__main__.py` & `pypackerdetect-1.1.0/src/pypackerdetect/__main__.py`

 * *Files identical despite different names*

### Comparing `pypackerdetect-1.0.8/src/pypackerdetect/db/packers.json` & `pypackerdetect-1.1.0/src/pypackerdetect/db/packers.json`

 * *Files identical despite different names*

### Comparing `pypackerdetect-1.0.8/src/pypackerdetect/db/sections.json` & `pypackerdetect-1.1.0/src/pypackerdetect/db/sections.json`

 * *Files identical despite different names*

### Comparing `pypackerdetect-1.0.8/src/pypackerdetect/db/sigs_long.txt` & `pypackerdetect-1.1.0/src/pypackerdetect/db/sigs_long.txt`

 * *Files identical despite different names*

### Comparing `pypackerdetect-1.0.8/src/pypackerdetect/db/sigs_short.txt` & `pypackerdetect-1.1.0/src/pypackerdetect/db/sigs_short.txt`

 * *Files identical despite different names*

### Comparing `pypackerdetect-1.0.8/src/pypackerdetect.egg-info/PKG-INFO` & `pypackerdetect-1.1.0/src/pypackerdetect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypackerdetect
-Version: 1.0.8
+Version: 1.1.0
 Summary: Re-implementation and packaging of PyPackerDetect
 Author-email: Alexandre D'Hondt <alexandre.dhondt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pypackerdetect-1.0.8/src/pypackerdetect.egg-info/SOURCES.txt` & `pypackerdetect-1.1.0/src/pypackerdetect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

