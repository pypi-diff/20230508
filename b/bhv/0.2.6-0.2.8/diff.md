# Comparing `tmp/bhv-0.2.6.tar.gz` & `tmp/bhv-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.2.6.tar", last modified: Tue May  2 19:26:51 2023, max compression
+gzip compressed data, was "bhv-0.2.8.tar", last modified: Mon May  8 19:42:57 2023, max compression
```

## Comparing `bhv-0.2.6.tar` & `bhv-0.2.8.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-02 19:26:51.645224 bhv-0.2.6/
--rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.2.6/LICENSE
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1027 2023-05-02 19:26:51.645224 bhv-0.2.6/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3202 2023-04-29 09:52:26.000000 bhv-0.2.6/README.md
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-02 19:26:51.645224 bhv-0.2.6/bhv/
--rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.2.6/bhv/__init__.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11962 2023-04-28 20:37:06.000000 bhv-0.2.6/bhv/abstract.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1635 2023-04-11 14:49:00.000000 bhv-0.2.6/bhv/embedding.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11207 2023-05-02 19:20:22.000000 bhv-0.2.6/bhv/np.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-04-24 21:41:56.000000 bhv-0.2.6/bhv/poibin.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.2.6/bhv/positions.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     8226 2023-05-02 19:26:10.000000 bhv-0.2.6/bhv/pytorch.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2356 2023-04-28 22:56:24.000000 bhv-0.2.6/bhv/shared.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1152 2023-04-24 02:20:49.000000 bhv-0.2.6/bhv/slice.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    21307 2023-05-02 16:47:02.000000 bhv-0.2.6/bhv/symbolic.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3325 2023-04-28 20:51:52.000000 bhv-0.2.6/bhv/vanilla.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)      782 2023-04-28 16:55:18.000000 bhv-0.2.6/bhv/visualization.py
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-02 19:26:51.645224 bhv-0.2.6/bhv.egg-info/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1027 2023-05-02 19:26:51.000000 bhv-0.2.6/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)      344 2023-05-02 19:26:51.000000 bhv-0.2.6/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-05-02 19:26:51.000000 bhv-0.2.6/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       73 2023-05-02 19:26:51.000000 bhv-0.2.6/bhv.egg-info/requires.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-05-02 19:26:51.000000 bhv-0.2.6/bhv.egg-info/top_level.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-05-02 19:26:51.645224 bhv-0.2.6/setup.cfg
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1331 2023-05-02 19:26:36.000000 bhv-0.2.6/setup.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-08 19:42:57.625020 bhv-0.2.8/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.2.8/LICENSE
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1027 2023-05-08 19:42:57.625020 bhv-0.2.8/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3202 2023-04-29 09:52:26.000000 bhv-0.2.8/README.md
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-08 19:42:57.625020 bhv-0.2.8/bhv/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.2.8/bhv/__init__.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    12173 2023-05-08 14:41:53.000000 bhv-0.2.8/bhv/abstract.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2119 2023-05-05 13:49:14.000000 bhv-0.2.8/bhv/embedding.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11275 2023-05-08 19:42:15.000000 bhv-0.2.8/bhv/np.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-04-24 21:41:56.000000 bhv-0.2.8/bhv/poibin.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.2.8/bhv/positions.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     8226 2023-05-02 19:26:10.000000 bhv-0.2.8/bhv/pytorch.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2769 2023-05-03 12:10:28.000000 bhv-0.2.8/bhv/shared.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1152 2023-04-24 02:20:49.000000 bhv-0.2.8/bhv/slice.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    24158 2023-05-05 11:23:02.000000 bhv-0.2.8/bhv/symbolic.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        7 2023-05-05 10:13:11.000000 bhv-0.2.8/bhv/test.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3359 2023-05-08 19:17:04.000000 bhv-0.2.8/bhv/vanilla.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      782 2023-04-28 16:55:18.000000 bhv-0.2.8/bhv/visualization.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-08 19:42:57.625020 bhv-0.2.8/bhv.egg-info/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1027 2023-05-08 19:42:57.000000 bhv-0.2.8/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      356 2023-05-08 19:42:57.000000 bhv-0.2.8/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-05-08 19:42:57.000000 bhv-0.2.8/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       73 2023-05-08 19:42:57.000000 bhv-0.2.8/bhv.egg-info/requires.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-05-08 19:42:57.000000 bhv-0.2.8/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-05-08 19:42:57.625020 bhv-0.2.8/setup.cfg
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1331 2023-05-08 19:33:57.000000 bhv-0.2.8/setup.py
```

### Comparing `bhv-0.2.6/LICENSE` & `bhv-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bhv-0.2.6/PKG-INFO` & `bhv-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.2.6
+Version: 0.2.8
 Summary: Boolean Hypervectors
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bhv-0.2.6/README.md` & `bhv-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `bhv-0.2.6/bhv/abstract.py` & `bhv-0.2.8/bhv/abstract.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,14 +56,20 @@
 
     def flip_half(self) -> Self:
         return self ^ self.rand()
 
     def flip_pow(self, pow_flip=1) -> Self:
         return self ^ self.rand2(pow_flip)
 
+    def flip_pow_on(self, flip_on_frac) -> Self:
+        return self | self.flip_pow(flip_on_frac + 1)
+
+    def flip_pow_off(self, flip_off_frac) -> Self:
+        return self & self.flip_pow(flip_off_frac + 1)
+
     def flip_frac(self, frac_flip=0.5) -> Self:
         return self ^ self.random(frac_flip)
 
     def flip_frac_on(self, flip_on_frac) -> Self:
         return self | self.flip_frac(2*flip_on_frac)
 
     def flip_frac_off(self, flip_off_frac) -> Self:
```

### Comparing `bhv-0.2.6/bhv/np.py` & `bhv-0.2.8/bhv/np.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .abstract import *
 import numpy as np
+from sys import byteorder
 
 
 class NumPyBoolPermutation(MemoizedPermutation):
     _permutations: 'dict[int | tuple[int, ...], Self]' = {}
     rng = np.random.default_rng()
 
     def __init__(self, array: np.ndarray):
@@ -165,15 +166,15 @@
     def __or__(self, other: 'NumPyPacked8BHV') -> 'NumPyPacked8BHV':
         return NumPyPacked8BHV(np.bitwise_or(self.data, other.data))
 
     def __invert__(self) -> 'NumPyPacked8BHV':
         return NumPyPacked8BHV(np.bitwise_not(self.data))
 
     def active(self) -> int:
-        return sum(x.bit_count() for x in self.data)
+        return int.from_bytes(self.data.tobytes(), byteorder).bit_count()
 
     def unpack(self) -> 'NumPyBoolBHV':
         return NumPyBoolBHV(np.unpackbits(self.data))
 
     def repack64(self) -> 'NumPyPacked64BHV':
         return NumPyPacked64BHV(self.data.view(dtype=np.uint64))
 
@@ -268,15 +269,15 @@
     def __or__(self, other: 'NumPyPacked64BHV') -> 'NumPyPacked64BHV':
         return NumPyPacked64BHV(np.bitwise_or(self.data, other.data))
 
     def __invert__(self) -> 'NumPyPacked64BHV':
         return NumPyPacked64BHV(np.bitwise_not(self.data))
 
     def active(self) -> int:
-        return sum(x.bit_count() for x in self.data)
+        return int.from_bytes(self.data.tobytes(), byteorder).bit_count()
 
     def unpack(self) -> 'NumPyBoolBHV':
         return NumPyBoolBHV(np.unpackbits(self.data.view(np.uint8)))
 
     def repack8(self) -> 'NumPyPacked8BHV':
         return NumPyPacked8BHV(self.data.view(dtype=np.uint8))
```

### Comparing `bhv-0.2.6/bhv/poibin.py` & `bhv-0.2.8/bhv/poibin.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.6/bhv/positions.py` & `bhv-0.2.8/bhv/positions.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.6/bhv/pytorch.py` & `bhv-0.2.8/bhv/pytorch.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.6/bhv/shared.py` & `bhv-0.2.8/bhv/shared.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,75 @@
 try:
     from typing import Self
 except ImportError:
     Self = 'AbstractBHV'
 
 DIMENSION = 8192
 
+from functools import partial
 from dataclasses import fields, is_dataclass
 from base64 import _urlsafe_encode_translation
 import hashlib
 import binascii
 import sys
 
 sys.setrecursionlimit(75_000)
 
 
-def stable_hash(d) -> bytes:
+def stable_hash(d, try_cache=False) -> bytes:
     """
     Python's `hash` is not stable. That's a problem if you want to use it for persistence and inter-run consistency.
     This one is hand rolled, so don't fully trust it. In fact, if you see anything suspicious, please let me know.
     :param d: Something you want to hash
     :return: The 16-byte md5 hash of the bytes of all (nested) items.
     """
+    if try_cache and hasattr(d, "__stable_hash"):
+        return d.__stable_hash
+
+    stable_hash_try_cache = partial(stable_hash, try_cache=try_cache)
+
     t = bytes(type(d).__name__, 'utf-8')
     t += bytes([2])
     if isinstance(d, str):
         t += bytes(d, 'utf-8')
     elif isinstance(d, float):
         t += bytes(d.hex(), 'ascii')
     elif isinstance(d, list) or isinstance(d, tuple):
-        t += b''.join(map(stable_hash, d))
+        t += b''.join(map(stable_hash_try_cache, d))
     elif isinstance(d, set) or isinstance(d, frozenset):
-        t += b''.join(sorted(map(stable_hash, d)))
+        t += b''.join(sorted(map(stable_hash_try_cache, d)))
     elif isinstance(d, dict):
         for k, v in d.items():
-            t += stable_hash(k)
+            t += stable_hash_try_cache(k)
             t += bytes([1])
-            t += stable_hash(v)
+            t += stable_hash_try_cache(v)
     elif is_dataclass(d):
         for f in fields(d):
             t += bytes(f.name, 'utf-8')
             t += bytes([1])
-            t += stable_hash(getattr(d, f.name))
-    else: t += bytes(d)
-    return hashlib.md5(t, usedforsecurity=False).digest()
+            t += stable_hash_try_cache(getattr(d, f.name))
+    else:
+        t += bytes(d)
+    res = hashlib.md5(t, usedforsecurity=False).digest()
+    if try_cache:
+        try:
+            d.__stable_hash = res
+        except AttributeError:
+            pass
+    return res
 
 
-def stable_hashcode(d, version=0) -> str:
+def stable_hashcode(d, version=0, try_cache=False) -> str:
     """
     A thin wrapper around `stable_hash` which returns a string and incorporates a version.
     :param d: Something you want to hash
     :param version: Increase this number if you want to unconditionally break all hashcodes
     :return: The 24 character base64 (with - and _) string hash
     """
-    h = stable_hash(d)
+    h = stable_hash(d, try_cache)
     padded = h.rjust(18, version.to_bytes(1, "little"))
     base64 = binascii.b2a_base64(padded, newline=False)
     url_safe = base64.translate(_urlsafe_encode_translation)
     return url_safe.decode()
 
 
 def nbs(i, w):
```

### Comparing `bhv-0.2.6/bhv/slice.py` & `bhv-0.2.8/bhv/slice.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.6/bhv/symbolic.py` & `bhv-0.2.8/bhv/symbolic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from dataclasses import dataclass, field, fields
 from .abstract import *
 from .shared import stable_hashcode, bitconfigs
 from .slice import Slice
-from .poibin import PoiBin
 
 
 class Symbolic:
     def nodename(self, **kwargs):
         return f"{type(self).__name__.upper()}"
 
     def nodeid(self, structural=False, **kwargs):
-        return f"{type(self).__name__}{stable_hashcode(self).replace('-', '') if structural else str(id(self))}"
+        return f"{type(self).__name__}{stable_hashcode(self, try_cache=True).replace('-', '') if structural else str(id(self))}"
 
     def children(self, **kwargs):
         return [(getattr(self, f.name), f.name) for f in fields(self) if type(f.type) is type and issubclass(f.type, Symbolic)]
 
+    def reconstruct(self, *cs):
+        assert not self.children()
+        return self
+
     def draw_node(self, **kwargs):
         print(f"{self.nodeid(**kwargs)} [label=\"{self.nodename(**kwargs)}\"];")
 
     def draw_edges(self, **kwargs):
         for c, label in self.children(**kwargs):
             print(f"{c.nodeid(**kwargs)} -> {self.nodeid(**kwargs)} [label=\"{label}\"];")
 
@@ -65,22 +68,43 @@
         if id(self) in calculated:
             return calculated[id(self)]
         else:
             result = self.instantiate(**kwargs)
             calculated[id(self)] = result
             return result
 
+    def optimal_sharing(self, form=None, **kwargs):
+        if form is None: form = {}
+        kwargs |= dict(form=form)
+
+        sh = stable_hashcode(self, try_cache=True)
+        if sh in form:
+            return form[sh]
+        else:
+            r = self.reconstruct(*(c.optimal_sharing(**kwargs) for c, _ in self.children()))
+            shr = stable_hashcode(r, try_cache=True)
+            if shr in form:
+                raise RuntimeError("Includes check failed")
+            form[shr] = r
+            return r
+
     def internal_size(self):
         return 1
 
-    def size(self):
-        t = self.internal_size()
-        for c, _ in self.children():
-            t += c.size()
-        return t
+    def size(self, counted=None, recount=False, **kwargs):
+        if counted is None: counted = {}
+        kwargs |= dict(counted=counted)
+        if id(self) in counted:
+            return counted[id(self)] if recount else 0
+        else:
+            t = self.internal_size()
+            for c, _ in self.children():
+                t += c.size(**kwargs)
+            counted[id(self)] = t
+            return t
 
     def simplify(self, **kwargs):
         x = self
         while True:
             x_ = x.reduce(**kwargs)
             if x == x_:
                 return x
@@ -107,14 +131,17 @@
 
     def show(self, **kwargs):
         return self.name + " {\n" + '\n'.join("  " + x.show(**kwargs) + ";" for x in self.xs) + "\n}"
 
     def children(self, **kwargs):
         return [(x, str(i)) for i, x in enumerate(self.xs)]
 
+    def reconstruct(self, *cs):
+        return List(self.name, cs)
+
     def graphviz(self, structural=False, done=None, **kwargs):
         noden = self.nodeid(structural, **kwargs)
         if done is None:
             done = set()
         if noden in done:
             return
         done.add(noden)
@@ -192,23 +219,29 @@
             randomperms[self.id] = r
             return r
 @dataclass
 class PermCompose(SymbolicPermutation):
     l: SymbolicPermutation
     r: SymbolicPermutation
 
+    def reconstruct(self, l, r):
+        return PermCompose(l, r)
+
     def show(self, **kwargs):
         return f"({self.l.show(**kwargs)} * {self.r.show(**kwargs)})"
 
     def instantiate(self, **kwargs):
         return self.l.execute(**kwargs) * self.r.execute(**kwargs)
 @dataclass
 class PermInvert(SymbolicPermutation):
     p: SymbolicPermutation
 
+    def reconstruct(self, p):
+        return PermInvert(p)
+
     def show(self, **kwargs):
         return f"(~{self.p.show(**kwargs)})"
 
     def instantiate(self, **kwargs):
         return ~self.p.execute(**kwargs)
 
 
@@ -280,14 +313,17 @@
 
 
 @dataclass
 class PermApply(SymbolicBHV):
     p: SymbolicPermutation
     v: SymbolicBHV
 
+    def reconstruct(self, p, v):
+        return PermApply(p, v)
+
     def show(self, **kwargs):
         return f"{self.p.show(**kwargs)}({self.v.show(**kwargs)})"
 
     def instantiate(self, **kwargs):
         return self.p.execute(**kwargs)(self.v.execute(**kwargs))
 
     def expected_active_fraction(self, **kwargs):
@@ -353,15 +389,15 @@
         rand = kwargs.get("rand")
         if self.id in rand:
             return rand[self.id]
         else:
             r = kwargs.get("bhv").rand()
             rand[self.id] = r
             return r
-    
+
     def expected_active_fraction(self, **kwargs):
         return .5
 @dataclass
 class Rand2(SymbolicBHV):
     power: int
 
     def show(self, **kwargs):
@@ -389,117 +425,144 @@
         random = kwargs.get("random")
         if self.id in random:
             return random[self.id]
         else:
             r = kwargs.get("bhv").random(self.frac)
             random[self.id] = r
             return r
-        
+
     def expected_active_fraction(self, **kwargs):
         return self.frac
 @dataclass
 class Majority(SymbolicBHV):
     vs: list[SymbolicBHV]
 
     def children(self, **kwargs):
         return list(zip(self.vs, map(str, range(len(self.vs)))))
 
+    def reconstruct(self, *cs):
+        return Majority(cs)
+
     def show(self, **kwargs):
         return kwargs.get("impl", "") + f"majority({[v.show(**kwargs) for v in self.vs]})"
 
     def instantiate(self, **kwargs):
         return kwargs.get("bhv").majority([v.execute(**kwargs) for v in self.vs])
 
     def expected_active_fraction(self, **kwargs):
+        from .poibin import PoiBin
         return 1. - PoiBin([v.expected_active_fraction(**kwargs) for v in self.vs]).cdf(len(self.vs)//2)
 @dataclass
 class Permute(SymbolicBHV):
     id: 'int | tuple[int, ...]'
     v: SymbolicBHV
 
+    def reconstruct(self, v):
+        return Permute(self.id, v)
+
     def show(self, **kwargs):
         return f"{self.v.show(**kwargs)}.permute({self.id})"
 
     def instantiate(self, **kwargs):
         return self.v.execute(**kwargs).permute(self.id)
 
     def expected_active_fraction(self, **kwargs):
         return self.v.expected_active_fraction(**kwargs)
 @dataclass
 class SwapHalves(SymbolicBHV):
     v: SymbolicBHV
 
+    def reconstruct(self, v):
+        return SwapHalves(v)
+
     def show(self, **kwargs):
         return f"{self.v.show(**kwargs)}.swap_halves()"
 
     def instantiate(self, **kwargs):
         return self.v.execute(**kwargs).swap_halves()
 
     def expected_active_fraction(self, **kwargs):
         return self.v.expected_active_fraction(**kwargs)
 @dataclass
 class ReHash(SymbolicBHV):
     v: SymbolicBHV
 
+    def reconstruct(self, v):
+        return ReHash(v)
+
     def show(self, **kwargs):
         return f"{self.v.show(**kwargs)}.rehash()"
 
     def instantiate(self, **kwargs):
         return self.v.execute(**kwargs).rehash()
 
     def expected_active_fraction(self, **kwargs):
         return .5
 @dataclass
 class Eq:
     l: SymbolicBHV
     r: SymbolicBHV
 
+    def reconstruct(self, l, r):
+        return Eq(l, r)
+
     def show(self, **kwargs):
         return f"({self.l.show(**kwargs)} == {self.r.show(**kwargs)})"
 
     def instantiate(self, **kwargs):
         return self.l.execute(**kwargs) == self.r.execute(**kwargs)
 @dataclass
 class Xor(SymbolicBHV):
     l: SymbolicBHV
     r: SymbolicBHV
 
+    def reconstruct(self, l, r):
+        return Xor(l, r)
+
     def show(self, **kwargs):
         return f"({self.l.show(**kwargs)} ^ {self.r.show(**kwargs)})"
 
     def instantiate(self, **kwargs):
         return self.l.execute(**kwargs) ^ self.r.execute(**kwargs)
 
     def reduce(self, **kwargs):
         if self.l == self.ONE:
             return ~self.r.simplify(**kwargs)
         elif self.r == self.ONE:
             return ~self.l.simplify(**kwargs)
-        if self.l == self.ZERO:
+        elif self.l == self.ZERO:
             return self.r.simplify(**kwargs)
         elif self.r == self.ZERO:
             return self.l.simplify(**kwargs)
         elif self.l == self.r:
             return self.ZERO
         elif self.l == ~self.r or ~self.l == self.r:
             return self.ONE
         elif isinstance(self.l, Invert) and isinstance(self.r, Invert):
             return ~Xor(self.l.v.simplify(**kwargs), self.r.v.simplify(**kwargs))
+        elif isinstance(self.l, And) and isinstance(self.r, And):
+            if self.l.l == self.r.l: return And(self.l.l, Xor(self.l.r, self.r.r)).simplify(**kwargs)
+            elif self.l.l == self.r.r: return And(self.l.l, Xor(self.l.r, self.r.l)).simplify(**kwargs)
+            elif self.l.r == self.r.l: return And(self.l.r, Xor(self.l.l, self.r.r)).simplify(**kwargs)
+            elif self.l.r == self.r.r: return And(self.l.r, Xor(self.l.l, self.r.l)).simplify(**kwargs)
         else:
             return Xor(self.l.simplify(**kwargs), self.r.simplify(**kwargs))
 
     def expected_active_fraction(self, **kwargs):
         afl = self.l.expected_active_fraction(**kwargs)
         afr = self.r.expected_active_fraction(**kwargs)
         return afl*(1. - afr) + (1. - afl)*afr
 @dataclass
 class And(SymbolicBHV):
     l: SymbolicBHV
     r: SymbolicBHV
 
+    def reconstruct(self, l, r):
+        return And(l, r)
+
     def show(self, **kwargs):
         return f"({self.l.show(**kwargs)} & {self.r.show(**kwargs)})"
 
     def instantiate(self, **kwargs):
         return self.l.execute(**kwargs) & self.r.execute(**kwargs)
 
     def reduce(self, **kwargs):
@@ -519,14 +582,17 @@
         afr = self.r.expected_active_fraction(**kwargs)
         return afl*afr
 @dataclass
 class Or(SymbolicBHV):
     l: SymbolicBHV
     r: SymbolicBHV
 
+    def reconstruct(self, l, r):
+        return Or(l, r)
+
     def show(self, **kwargs):
         return f"({self.l.show(**kwargs)} | {self.r.show(**kwargs)})"
 
     def instantiate(self, **kwargs):
         return self.l.execute(**kwargs) | self.r.execute(**kwargs)
 
     def reduce(self, **kwargs):
@@ -545,14 +611,17 @@
         afl = self.l.expected_active_fraction(**kwargs)
         afr = self.r.expected_active_fraction(**kwargs)
         return 1. - ((1. - afl)*(1. - afr))
 @dataclass
 class Invert(SymbolicBHV):
     v: SymbolicBHV
 
+    def reconstruct(self, v):
+        return Invert(v)
+
     def show(self, **kwargs):
         return f"(~{self.v.show(**kwargs)})"
 
     def instantiate(self, **kwargs):
         return ~self.v.execute(**kwargs)
 
     def reduce(self, **kwargs):
@@ -568,97 +637,122 @@
     def expected_active_fraction(self, **kwargs):
         return 1. - self.v.expected_active_fraction(**kwargs)
 @dataclass
 class Select(SymbolicBHV):
     cond: SymbolicBHV
     when1: SymbolicBHV
     when0: SymbolicBHV
+
+    def reconstruct(self, c, w1, w0):
+        return Select(c, w1, w0)
+
     def nodename(self, compact_select=True, **kwargs):
         return f"ON {self.cond.nodename()}" if compact_select else super().nodename(**kwargs)
-    def children(self, compact_select=True, **kwargs):
+
+    def children(self, compact_select=False, **kwargs):
         return [(self.when1, "1"), (self.when0, "0")] if compact_select else super().children(**kwargs)
 
     def show(self, **kwargs):
         return f"{self.cond.show(**kwargs)}.select({self.when1.show(**kwargs)}, {self.when0.show(**kwargs)})"
 
     def instantiate(self, **kwargs):
         return self.cond.execute(**kwargs).select(self.when1.execute(**kwargs), self.when0.execute(**kwargs))
 
     def internal_size(self):
         return 3
 
     def reduce(self, **kwargs):
+        expand_select_xor = kwargs.get("expand_select_xor", False)
+        expand_select_and_or = kwargs.get("expand_select_and_or", False)
+
         if self.when1 == self.ONE and self.when0 == self.ZERO:
             return self.cond.simplify(**kwargs)
         elif self.when1 == self.ZERO and self.when0 == self.ONE:
-            return ~self.cond.simplify(**kwargs)
+            return (~self.cond).simplify(**kwargs)
         elif self.when0 == self.when1:
             return self.when0.simplify(**kwargs)
         elif self.when1 == self.ONE:
             return self.cond.simplify(**kwargs) | self.when0.simplify(**kwargs)
         elif self.when1 == self.ZERO:
-            return ~self.cond.simplify(**kwargs) & self.when0.simplify(**kwargs)
+            return (~self.cond).simplify(**kwargs) & self.when0.simplify(**kwargs)
         elif self.when0 == self.ONE:
-            return ~self.cond.simplify(**kwargs) | self.when1.simplify(**kwargs)
+            return (~self.cond).simplify(**kwargs) | self.when1.simplify(**kwargs)
         elif self.when0 == self.ZERO:
             return self.cond.simplify(**kwargs) & self.when1.simplify(**kwargs)
         else:
             when1_ = self.when1.simplify(**kwargs)
             when0_ = self.when0.simplify(**kwargs)
+            cond_ = self.cond.simplify(**kwargs)
 
             if when1_ == ~when0_:
-                return self.cond ^ when0_
+                return cond_ ^ when0_
             elif when0_ == ~when1_:
-                return self.cond ^ when0_
+                return cond_ ^ when0_
             elif isinstance(when0_, Invert) and isinstance(when1_, Invert):
-                return ~Select(self.cond.simplify(**kwargs), when1_.v, when0_.v)
+                return ~Select(cond_, when1_.v, when0_.v)
             else:
-                # return when0_ ^ (self.cond.simplify(**kwargs) & (when0_ ^ when1_))
-                return Select(self.cond.simplify(**kwargs), when1_, when0_)
+                if expand_select_xor:
+                    return when0_ ^ (cond_ & (when0_ ^ when1_))
+                elif expand_select_and_or:
+                    return (cond_ & when1_) | ((~cond_).simplify(**kwargs) & when0_)
+                else:
+                    return Select(cond_, when1_, when0_)
 
     def expected_active_fraction(self, **kwargs):
         afc = self.cond.expected_active_fraction(**kwargs)
         af1 = self.when1.expected_active_fraction(**kwargs)
         af0 = self.when0.expected_active_fraction(**kwargs)
         return afc*af1 + (1. - afc)*af0
 @dataclass
 class ActiveFraction(Symbolic):
     v: SymbolicBHV
 
+    def reconstruct(self, v):
+        return ActiveFraction(v)
+
     def show(self, **kwargs):
         return f"{self.v.show(**kwargs)}.active_fraction()"
 
     def instantiate(self, **kwargs):
         return self.v.execute(**kwargs).active_fraction()
 @dataclass
 class BiasRel(Symbolic):
     rel: SymbolicBHV
     l: SymbolicBHV
     r: SymbolicBHV
 
+    def reconstruct(self, rel, l, r):
+        return BiasRel(rel, l, r)
+
     def show(self, **kwargs):
         return f"{self.l.show(**kwargs)}.bias_rel({self.r.show(**kwargs)}, {self.rel.show(**kwargs)})"
 
     def instantiate(self, **kwargs):
         return self.l.execute(**kwargs).bias_rel(self.r.execute(**kwargs), self.rel.execute(**kwargs))
 @dataclass
 class Related(Symbolic):
     l: SymbolicBHV
     r: SymbolicBHV
     stdvs: float
 
+    def reconstruct(self, l, r):
+        return Related(l, r, self.stdvs)
+
     def show(self, **kwargs):
         return f"{self.l.show(**kwargs)}.related({self.r.show(**kwargs)}, {self.stdvs})"
 
     def instantiate(self, **kwargs):
         return self.l.execute(**kwargs).related(self.r.execute(**kwargs), self.stdvs)
 @dataclass
 class Unrelated(Symbolic):
     l: SymbolicBHV
     r: SymbolicBHV
     stdvs: float
 
+    def reconstruct(self, l, r):
+        return Unrelated(l, r, self.stdvs)
+
     def show(self, **kwargs):
         return f"{self.l.show(**kwargs)}.unrelated({self.r.show(**kwargs)}, {self.stdvs})"
 
     def instantiate(self, **kwargs):
         return self.l.execute(**kwargs).unrelated(self.r.execute(**kwargs), self.stdvs)
```

### Comparing `bhv-0.2.6/bhv/vanilla.py` & `bhv-0.2.8/bhv/vanilla.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .abstract import *
 import random
+from sys import byteorder
 
 
 class VanillaPermutation(MemoizedPermutation):
     _permutations: 'dict[int | tuple[int, ...], Self]' = {}
 
     def __init__(self, indices):
         self.data = indices
@@ -73,18 +74,18 @@
     def __invert__(self) -> 'VanillaBHV':
         return self.from_int(~self.to_int())
 
     def active(self) -> int:
         return self.to_int().bit_count()
 
     def to_int(self) -> int:
-        return int.from_bytes(self.data, "big", signed=True)
+        return int.from_bytes(self.data, byteorder, signed=True)
 
     @classmethod
     def from_int(cls, i: int):
-        return VanillaBHV(i.to_bytes(DIMENSION//8, "big", signed=True))
+        return VanillaBHV(i.to_bytes(DIMENSION//8, byteorder, signed=True))
 
 
 VanillaBHV.ZERO = VanillaBHV(bytes([0 for _ in range(DIMENSION//8)]))
 VanillaBHV.ONE = VanillaBHV(bytes([0xff for _ in range(DIMENSION//8)]))
 VanillaBHV._FEISTAL_SUBKEYS = VanillaBHV.nrand2(VanillaBHV._FEISTAL_ROUNDS, 4)
 VanillaBHV.HALF = VanillaBHV(bytes([0 for _ in range(DIMENSION//16)] + [0xff for _ in range(DIMENSION//16)]))
```

### Comparing `bhv-0.2.6/bhv/visualization.py` & `bhv-0.2.8/bhv/visualization.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.6/bhv.egg-info/PKG-INFO` & `bhv-0.2.8/bhv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.2.6
+Version: 0.2.8
 Summary: Boolean Hypervectors
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bhv-0.2.6/setup.py` & `bhv-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.6'
+VERSION = '0.2.8'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 setup(
     name="bhv",
     version=VERSION,
     author="Adam Vandervorst",
```

