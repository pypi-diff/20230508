# Comparing `tmp/rawpipe-0.9.7.tar.gz` & `tmp/rawpipe-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rawpipe-0.9.7.tar", last modified: Tue Apr 27 10:55:13 2021, max compression
+gzip compressed data, was "dist/rawpipe-0.9.9.tar", last modified: Mon Jun  7 12:33:52 2021, max compression
```

## Comparing `rawpipe-0.9.7.tar` & `rawpipe-0.9.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2021-04-27 10:55:13.000000 rawpipe-0.9.7/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      266 2021-04-27 10:55:13.000000 rawpipe-0.9.7/PKG-INFO
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1396 2021-02-10 09:05:38.000000 rawpipe-0.9.7/README.md
-drwxr-xr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2021-04-27 10:55:13.000000 rawpipe-0.9.7/rawpipe/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1617 2021-04-27 10:54:21.000000 rawpipe-0.9.7/rawpipe/__init__.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    20002 2021-04-27 10:55:04.000000 rawpipe-0.9.7/rawpipe/rawpipe.py
-drwxr-xr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2021-04-27 10:55:13.000000 rawpipe-0.9.7/rawpipe.egg-info/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      266 2021-04-27 10:55:13.000000 rawpipe-0.9.7/rawpipe.egg-info/PKG-INFO
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      283 2021-04-27 10:55:13.000000 rawpipe-0.9.7/rawpipe.egg-info/SOURCES.txt
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)        1 2021-04-27 10:55:13.000000 rawpipe-0.9.7/rawpipe.egg-info/dependency_links.txt
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       64 2021-04-27 10:55:13.000000 rawpipe-0.9.7/rawpipe.egg-info/requires.txt
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       13 2021-04-27 10:55:13.000000 rawpipe-0.9.7/rawpipe.egg-info/top_level.txt
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)        1 2021-04-27 10:55:13.000000 rawpipe-0.9.7/rawpipe.egg-info/zip-safe
--rw-rw-rw-   0 toaarnio  (1000) toaarnio  (1000)      107 2021-04-27 10:55:13.000000 rawpipe-0.9.7/setup.cfg
--rw-rw-rw-   0 toaarnio  (1000) toaarnio  (1000)      628 2020-03-05 13:36:58.000000 rawpipe-0.9.7/setup.py
-drwxr-xr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2021-04-27 10:55:13.000000 rawpipe-0.9.7/test/
--rw-rw-rw-   0 toaarnio  (1000) toaarnio  (1000)        0 2020-03-05 13:36:58.000000 rawpipe-0.9.7/test/__init__.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1645 2021-04-27 10:46:46.000000 rawpipe-0.9.7/test/regression.py
+drwxr-xr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2021-06-07 12:33:52.000000 rawpipe-0.9.9/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      266 2021-06-07 12:33:52.000000 rawpipe-0.9.9/PKG-INFO
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1396 2021-02-10 09:05:38.000000 rawpipe-0.9.9/README.md
+drwxr-xr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2021-06-07 12:33:52.000000 rawpipe-0.9.9/rawpipe/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1613 2021-06-07 12:29:15.000000 rawpipe-0.9.9/rawpipe/__init__.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    20812 2021-06-07 12:33:30.000000 rawpipe-0.9.9/rawpipe/rawpipe.py
+drwxr-xr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2021-06-07 12:33:52.000000 rawpipe-0.9.9/rawpipe.egg-info/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      266 2021-06-07 12:33:51.000000 rawpipe-0.9.9/rawpipe.egg-info/PKG-INFO
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      283 2021-06-07 12:33:51.000000 rawpipe-0.9.9/rawpipe.egg-info/SOURCES.txt
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)        1 2021-06-07 12:33:51.000000 rawpipe-0.9.9/rawpipe.egg-info/dependency_links.txt
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       64 2021-06-07 12:33:51.000000 rawpipe-0.9.9/rawpipe.egg-info/requires.txt
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       13 2021-06-07 12:33:51.000000 rawpipe-0.9.9/rawpipe.egg-info/top_level.txt
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)        1 2021-06-07 12:33:51.000000 rawpipe-0.9.9/rawpipe.egg-info/zip-safe
+-rw-rw-rw-   0 toaarnio  (1000) toaarnio  (1000)      107 2021-06-07 12:33:52.000000 rawpipe-0.9.9/setup.cfg
+-rw-rw-rw-   0 toaarnio  (1000) toaarnio  (1000)      628 2020-03-05 13:36:58.000000 rawpipe-0.9.9/setup.py
+drwxr-xr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2021-06-07 12:33:52.000000 rawpipe-0.9.9/test/
+-rw-rw-rw-   0 toaarnio  (1000) toaarnio  (1000)        0 2020-03-05 13:36:58.000000 rawpipe-0.9.9/test/__init__.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     2347 2021-04-29 08:30:22.000000 rawpipe-0.9.9/test/regression.py
```

### Comparing `rawpipe-0.9.7/README.md` & `rawpipe-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `rawpipe-0.9.7/rawpipe/__init__.py` & `rawpipe-0.9.9/rawpipe/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   rgb = rawpipe.resize(rgb, 400, 300)
   rgb = rawpipe.wb(rgb, [1.5, 2.0])
   rgb = rawpipe.ccm(rgb, my_3x3_color_matrix)
   rgb = rawpipe.tonemap(rgb, "Reinhard")
   rgb = rawpipe.chroma_denoise(rgb)
   rgb = pipe.saturate(rgb, lambda x: x ** 0.75)
   rgb = rawpipe.gamma(rgb, "sRGB")
-  rgb = rawpipe.quantize(rgb, 255)
+  rgb = rawpipe.quantize8(rgb)
 
 Example:
   raw = rawpipe.verbose.linearize(raw)
   raw = rawpipe.silent.demosaic(raw, "RGGB")
 """
 
 from .rawpipe import Algorithms
@@ -34,9 +34,9 @@
 quiet = silent  # pylint: disable=invalid-name
 
 _methods = [f for f in dir(Algorithms) if callable(getattr(Algorithms, f)) and not f.startswith("_")]
 
 for m in _methods:
     globals()[m] = getattr(silent, m)
 
-__version__ = "0.9.7"
+__version__ = "0.9.9"
 __all__ = _methods
```

### Comparing `rawpipe-0.9.7/rawpipe/rawpipe.py` & `rawpipe-0.9.9/rawpipe/rawpipe.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         resize() for arbitrary resizing with proper interpolation in RGB domain.
         """
         if iterations >= 1:
             t0 = time.time()
             orgh, orgw = frame.shape[:2]
             if frame.ndim == 3:  # RGB mode
                 mode = "RGB"
-                frame = frame[::2*iterations, ::2*iterations]
+                frame = frame[::2**iterations, ::2**iterations]
             if frame.ndim == 2:  # Bayer mode
                 mode = "Bayer"
                 for _ in range(iterations):
                     ch1, ch2, ch3, ch4 = self.bayer_split(frame)
                     ch1 = ch1[::2, ::2]
                     ch2 = ch2[::2, ::2]
                     ch3 = ch3[::2, ::2]
@@ -152,15 +152,16 @@
             whitelevel = np.percentile(frame, percentile)
             self._vprint(f"{_elapsed(t0)} - estimating white level: {percentile:5.2f}th percentile = {whitelevel:.2f}")
         assert whitelevel > blacklevel, f"{whitelevel} is not greater than {blacklevel}"
         frame = np.clip(frame, blacklevel, whitelevel)
         t0 = time.time()
         frame -= blacklevel
         frame /= whitelevel - blacklevel
-        self._vprint(f"{_elapsed(t0)} - linearizing from {minmax} to [{blacklevel:.2f}, {whitelevel:.2f}] to [0, 1]")
+        ranges = f"{minmax} => [{blacklevel:.2f}, {whitelevel:.2f}] => {self._minmax(frame)}"
+        self._vprint(f"{_elapsed(t0)} - linearizing: range = {ranges}")
         return frame
 
     def demosaic(self,
                  frame: np.ndarray,
                  bayer_pattern: str,
                  downsample: bool = False) -> np.ndarray:
         """
@@ -332,17 +333,18 @@
               lut: np.ndarray = None) -> np.ndarray:
         """
         Apply rec709 or sRGB gamma or a custom tone curve on the given frame.
         Input colors are clipped to [0, 1] to avoid any arithmetic exceptions.
         In "LUT" mode, the frame is quantized to match the number of entries N
         in the look-up table; for example, if N=64, the output frame will have
         6-bit colors (and severe banding). This algorithm is format-agnostic.
-        If mode is None, the frame is returned untouched.
+        If mode evaluates to False, the frame is returned untouched.
         """
-        if mode is not None:
+        assert mode in ["sRGB", "rec709", "LUT"] or not mode, f"Unrecognized mode '{repr(mode)}'"
+        if mode in ["sRGB", "rec709", "LUT"]:
             t0 = time.time()
             realmode = mode
             input_range = self._minmax(frame)
             frame = np.clip(frame, 0, 1)  # can't handle values outside of [0, 1]
             if realmode in ["sRGB", "rec709"]:
                 bpp = 14
                 maxval = 2 ** bpp - 1
@@ -362,15 +364,15 @@
                     lut = lut * maxval
             if mode == "LUT":
                 assert lut is not None
                 maxval = len(lut) - 1
                 frame = self._quantize(frame, maxval)  # [0, 1] ==> [0, maxval]
                 frame = lut[frame]                     # [0, maxval] ==> [0, maxval]
                 frame = frame / maxval                 # [0, maxval] ==> [0, 1]
-            self._vprint(f"{_elapsed(t0)} - applying gamma curve [{realmode}]: input range = {input_range}")
+            self._vprint(f"{_elapsed(t0)} - applying gamma curve [{realmode}]: range = {input_range} => {self._minmax(frame)}")
         return frame
 
     def quantize(self,
                  frame: np.ndarray,
                  maxval: int = 65535,
                  dtype: np.dtype = np.uint16) -> np.ndarray:
         """
@@ -378,15 +380,31 @@
         it to the given dtype with proper rounding. This algorithm is format-
         agnostic.
         """
         t0 = time.time()
         input_range = self._minmax(frame)
         frame = np.clip(frame * maxval + 0.5, 0, maxval)
         frame = frame.astype(dtype)
-        self._vprint(f"{_elapsed(t0)} - quantizing from [0, 1] to {np.dtype(dtype).name} [0, {maxval}]; input range = {input_range}")
+        self._vprint(f"{_elapsed(t0)} - quantizing from [0, 1] to {np.dtype(dtype).name} [0, {maxval}]: input range = {input_range}")
+        return frame
+
+    def quantize8(self, frame: np.ndarray) -> np.ndarray:
+        """
+        Clip the given frame to [0, 1], rescale it to [0, 255], and convert it
+        to np.uint8. This algorithm is format-agnostic.
+        """
+        frame = self.quantize(frame, maxval=255, dtype=np.uint8)
+        return frame
+
+    def quantize16(self, frame: np.ndarray) -> np.ndarray:
+        """
+        Clip the given frame to [0, 1], rescale it to [0, 65535], and convert it
+        to np.uint16. This algorithm is format-agnostic.
+        """
+        frame = self.quantize(frame, maxval=65535, dtype=np.uint16)
         return frame
 
     def _quantize(self, frame: np.ndarray, maxval: int = 65535, dtype: np.dtype = np.uint16) -> np.ndarray:
         """
         Forced silent version of quantize().
         """
         verbose = self.verbose
```

### Comparing `rawpipe-0.9.7/setup.py` & `rawpipe-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `rawpipe-0.9.7/test/regression.py` & `rawpipe-0.9.9/test/regression.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,11 +34,24 @@
         raw = alg.wb(raw, wb)
         raw = alg.ccm(raw, ccm)
         raw = alg.saturate(raw, lambda x: x ** 0.5)
         raw = rawpipe.verbose.gamma(raw, gamma_mode)
         raw = rawpipe.verbose.quantize(raw, maxval, expected.dtype)
         self.assertEqual(np.count_nonzero(expected - raw), 0)
 
+    def test_errors(self):
+        raw = np.fromfile(os.path.join(thisdir, "input.raw"), dtype=np.uint16)
+        res = rawpipe.verbose.gamma(raw, None)  # should be no-op
+        res = rawpipe.verbose.gamma(res, "")  # should be no-op
+        res = rawpipe.verbose.gamma(res, False)  # should be no-op
+        self.assertTrue(np.all(raw == res))
+        with self.assertRaises(AssertionError):
+            raw = rawpipe.gamma(raw, "srgb")  # expecting "sRGB"
+        with self.assertRaises(AssertionError):
+            raw = rawpipe.gamma(raw, True)  # does not evaluate to False
+        with self.assertRaises(AssertionError):
+            raw = rawpipe.demosaic(raw, "RGGB")  # raw is not in [0, 1]
+
 
 if __name__ == "__main__":
     np.set_printoptions(formatter={'float': lambda x: f"{x:6.4f}"}, linewidth=180)
     unittest.main()
```

