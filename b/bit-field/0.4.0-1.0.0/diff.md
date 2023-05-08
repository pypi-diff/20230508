# Comparing `tmp/bit_field-0.4.0.tar.gz` & `tmp/bit_field-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bit_field-0.4.0.tar", last modified: Thu Mar 24 22:28:52 2022, max compression
+gzip compressed data, was "bit_field-1.0.0.tar", last modified: Mon May  8 19:55:51 2023, max compression
```

## Comparing `bit_field-0.4.0.tar` & `bit_field-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 22:28:52.578300 bit_field-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-03-24 22:28:39.000000 bit_field-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-03-24 22:28:39.000000 bit_field-0.4.0/LICENSE-ORIGINAL
--rw-r--r--   0 runner    (1001) docker     (121)     2240 2022-03-24 22:28:52.578300 bit_field-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-03-24 22:28:39.000000 bit_field-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 22:28:52.574300 bit_field-0.4.0/bit_field/
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-03-24 22:28:39.000000 bit_field-0.4.0/bit_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-03-24 22:28:39.000000 bit_field-0.4.0/bit_field/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2293 2022-03-24 22:28:39.000000 bit_field-0.4.0/bit_field/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-03-24 22:28:39.000000 bit_field-0.4.0/bit_field/jsonml_stringify.py
--rw-r--r--   0 runner    (1001) docker     (121)    10871 2022-03-24 22:28:39.000000 bit_field-0.4.0/bit_field/render.py
--rw-r--r--   0 runner    (1001) docker     (121)     2072 2022-03-24 22:28:39.000000 bit_field-0.4.0/bit_field/tspan.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 22:28:52.578300 bit_field-0.4.0/bit_field.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2240 2022-03-24 22:28:52.000000 bit_field-0.4.0/bit_field.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-03-24 22:28:52.000000 bit_field-0.4.0/bit_field.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-24 22:28:52.000000 bit_field-0.4.0/bit_field.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-03-24 22:28:52.000000 bit_field-0.4.0/bit_field.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-24 22:28:52.000000 bit_field-0.4.0/bit_field.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-03-24 22:28:52.000000 bit_field-0.4.0/bit_field.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-03-24 22:28:39.000000 bit_field-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-03-24 22:28:52.578300 bit_field-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:51.107464 bit_field-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-08 19:55:35.000000 bit_field-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-08 19:55:35.000000 bit_field-1.0.0/LICENSE-ORIGINAL
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-08 19:55:51.107464 bit_field-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-08 19:55:35.000000 bit_field-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:51.107464 bit_field-1.0.0/bit_field/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-08 19:55:35.000000 bit_field-1.0.0/bit_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 19:55:35.000000 bit_field-1.0.0/bit_field/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-08 19:55:35.000000 bit_field-1.0.0/bit_field/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-08 19:55:35.000000 bit_field-1.0.0/bit_field/jsonml_stringify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-05-08 19:55:35.000000 bit_field-1.0.0/bit_field/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-08 19:55:35.000000 bit_field-1.0.0/bit_field/tspan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:51.107464 bit_field-1.0.0/bit_field.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-08 19:55:51.000000 bit_field-1.0.0/bit_field.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-08 19:55:51.000000 bit_field-1.0.0/bit_field.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:55:51.000000 bit_field-1.0.0/bit_field.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-08 19:55:51.000000 bit_field-1.0.0/bit_field.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 19:55:51.000000 bit_field-1.0.0/bit_field.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 19:55:51.000000 bit_field-1.0.0/bit_field.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-08 19:55:35.000000 bit_field-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-08 19:55:51.111464 bit_field-1.0.0/setup.cfg
```

### Comparing `bit_field-0.4.0/LICENSE` & `bit_field-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bit_field-0.4.0/LICENSE-ORIGINAL` & `bit_field-1.0.0/LICENSE-ORIGINAL`

 * *Files identical despite different names*

### Comparing `bit_field-0.4.0/PKG-INFO` & `bit_field-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: bit_field
-Version: 0.4.0
+Version: 1.0.0
 Summary: A bitfield diagram renderer
 Home-page: https://github.com/Arth-ur/bitfield
 Author: Arthur Gay
 License: MIT
 Keywords: bitfield,bytefield,diagram,renderer,svg
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: JSON5
 License-File: LICENSE
 License-File: LICENSE-ORIGINAL
 
 A Python3 port of the javascript [bit-field library](https://github.com/drom/bitfield/) by [Aliaksei Chapyzhenka](https://github.com/drom).
 
+This package is also available as an extension for Sphinx: [sphinxcontrib-bitfield](https://github.com/Arth-ur/sphinxcontrib-bitfield).
+
 ## Install
 
 ```sh
 pip install bit_field
 ```
 
 To install this package with JSON5 support:
@@ -58,16 +59,19 @@
 --vspace     : vertical space - default 80
 --hspace     : horizontal space - default 640
 --lanes      : rectangle lanes - default 2
 --bits       : overall bitwidth - default 32
 --fontfamily : - default sans-serif
 --fontweight : - default normal
 --fontsize   : - default 14
+--strokewidth: - default 1
 --hflip      : horizontal flip
---vflip      : horizontal flip
+--vflip      : vertical flip
+--trim       : horizontal space available for a single character
+--uneven:    : uneven lanes
 
 --beautify   : use xml beautifier
 
 --json5      : force json5 input format (need json5 python module)
 --no-json5   : never use json5 input format
 ```
 
@@ -85,9 +89,7 @@
 ```
 ### alpha.svg
 
 ![Heat Sink](https://raw.githubusercontent.com/Arth-ur/bitfield/master/bit_field/test/alpha.svg?sanitize=true)
 
 ### Licensing
 This work is based on original work by [Aliaksei Chapyzhenka](https://github.com/drom) under the MIT license (see LICENSE-ORIGINAL).
-
-
```

### Comparing `bit_field-0.4.0/README.md` & `bit_field-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 A Python3 port of the javascript [bit-field library](https://github.com/drom/bitfield/) by [Aliaksei Chapyzhenka](https://github.com/drom).
 
+This package is also available as an extension for Sphinx: [sphinxcontrib-bitfield](https://github.com/Arth-ur/sphinxcontrib-bitfield).
+
 ## Install
 
 ```sh
 pip install bit_field
 ```
 
 To install this package with JSON5 support:
@@ -41,16 +43,19 @@
 --vspace     : vertical space - default 80
 --hspace     : horizontal space - default 640
 --lanes      : rectangle lanes - default 2
 --bits       : overall bitwidth - default 32
 --fontfamily : - default sans-serif
 --fontweight : - default normal
 --fontsize   : - default 14
+--strokewidth: - default 1
 --hflip      : horizontal flip
---vflip      : horizontal flip
+--vflip      : vertical flip
+--trim       : horizontal space available for a single character
+--uneven:    : uneven lanes
 
 --beautify   : use xml beautifier
 
 --json5      : force json5 input format (need json5 python module)
 --no-json5   : never use json5 input format
 ```
```

### Comparing `bit_field-0.4.0/bit_field/cli.py` & `bit_field-1.0.0/bit_field/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 from .render import render
 from .jsonml_stringify import jsonml_stringify
 import argparse
 
+
 def beautify(res):
     import xml.dom.minidom
     xml = xml.dom.minidom.parseString(res)
     res = xml.toprettyxml()
     return res
 
+
 def bit_field_cli():
     parser = argparse.ArgumentParser('bitfield')
 
     parser.add_argument(
         'input', help='input JSON filename - must be specified always')
     parser.add_argument(
         '--input', help='(compatibility option)', action='store_true')
     parser.add_argument('--vspace', help='vertical space', default=80, type=int)
     parser.add_argument('--hspace', help='horizontal space', default=800, type=int)
     parser.add_argument('--lanes', help='rectangle lanes', default=1, type=int)
-    parser.add_argument('--bits', help='overall bitwidth', default=32, type=int)
+    parser.add_argument('--bits', help='overall bitwidth', default=None, type=int)
     parser.add_argument('--fontfamily', default='sans-serif')
     parser.add_argument('--fontweight', default='normal')
     parser.add_argument('--fontsize', default=14, type=int)
+    parser.add_argument('--strokewidth', help='stroke width', default=1, type=float)
     parser.add_argument('--beautify', action='store_true')
     parser.add_argument('--json5', action='store_true')
     parser.add_argument('--no-json5', action='store_true')
     parser.add_argument('--compact', action='store_true')
     parser.add_argument('--hflip', help='horizontal flip', action='store_true')
     parser.add_argument('--vflip', help='vertical flip', action='store_true')
+    parser.add_argument('--trim', help='trim long bitfield names', type=float)
+    parser.add_argument('--uneven', help='uneven lanes', action='store_true')
+    parser.add_argument('--legend', help='legend item', action='append', nargs=2, metavar=('NAME', 'TYPE'))
     args = parser.parse_args()
 
     # default is json5, unless forced with --(no-)json5
     if args.json5:
         import json5 as json
     elif args.no_json5:
         import json
@@ -49,13 +55,17 @@
                      lanes=args.lanes,
                      bits=args.bits,
                      fontfamily=args.fontfamily,
                      fontweight=args.fontweight,
                      fontsize=args.fontsize,
                      compact=args.compact,
                      hflip=args.hflip,
-                     vflip=args.vflip)
+                     vflip=args.vflip,
+                     stroke_width=args.stroke_width,
+                     trim=args.trim,
+                     uneven=args.uneven,
+                     legend={key: value for key, value in args.legend} if args.legend else None)
 
     res = jsonml_stringify(res)
     if args.beautify:
         res = beautify(res)
     print(res)
```

### Comparing `bit_field-0.4.0/bit_field/render.py` & `bit_field-1.0.0/bit_field/render.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,52 +3,60 @@
 
 
 def t(x, y):
     return 'translate({}, {})'.format(x, y)
 
 
 def typeStyle(t):
+    return ';fill:' + typeColor(t)
+
+
+def typeColor(t):
     styles = {
         '2': 0,
         '3': 80,
         '4': 170,
         '5': 45,
         '6': 126,
         '7': 215,
     }
     t = str(t)
     if t in styles:
         r, g, b = colorsys.hls_to_rgb(styles[t] / 360, 0.9, 1)
-        return ';fill:rgb({:.0f}, {:.0f}, {:.0f})'.format(r * 255, g * 255, b * 255)
+        return 'rgb({:.0f}, {:.0f}, {:.0f})'.format(r * 255, g * 255, b * 255)
     else:
-        return ';fill:rgb({:.0f}, {:.0f}, {:.0f})'.format(229, 229, 229)
+        return 'rgb({:.0f}, {:.0f}, {:.0f})'.format(229, 229, 229)
 
 
 class Renderer(object):
     def __init__(self,
                  vspace=80,
                  hspace=640,
                  lanes=2,
-                 bits=32,
+                 bits=None,
                  fontsize=14,
                  fontfamily='sans-serif',
                  fontweight='normal',
                  compact=False,
-                 hflip=True,
-                 vflip=True):
+                 hflip=False,
+                 vflip=False,
+                 strokewidth=1,
+                 trim=None,
+                 uneven=False,
+                 legend=None):
         if vspace <= 19:
             raise ValueError(
                 'vspace must be greater than 19, got {}.'.format(vspace))
         if hspace <= 39:
             raise ValueError(
                 'hspace must be greater than 39, got {}.'.format(hspace))
         if lanes <= 0:
             raise ValueError(
                 'lanes must be greater than 0, got {}.'.format(lanes))
-        if bits <= 4:
+        if bits is not None and bits <= 4:
             raise ValueError(
                 'bits must be greater than 4, got {}.'.format(bits))
         if fontsize <= 5:
             raise ValueError(
                 'fontsize must be greater than 5, got {}.'.format(fontsize))
         self.vspace = vspace
         self.hspace = hspace
@@ -56,36 +64,33 @@
         self.bits = bits
         self.fontsize = fontsize
         self.fontfamily = fontfamily
         self.fontweight = fontweight
         self.compact = compact
         self.hflip = hflip
         self.vflip = vflip
+        self.stroke_width = strokewidth
+        self.trim_char_width = trim
+        self.uneven = uneven
+        self.legend = legend
+
+    def get_total_bits(self, desc):
+        return sum(e['bits'] for e in desc)
 
     def render(self, desc):
-        res = ['svg', {
-            'xmlns': 'http://www.w3.org/2000/svg',
-            'width': self.hspace,
-            'height': self.vspace * self.lanes,
-            'viewbox': ' '.join(str(x) for x in [0, 0, self.hspace, self.vspace * self.lanes])
-        }]
+        self.bits = self.bits if self.bits is not None else self.get_total_bits(desc)
 
-        mod = self.bits // self.lanes
+        mod = (self.bits + self.lanes - 1) // self.lanes
         self.mod = mod
         lsb = 0
         msb = self.bits - 1
         for e in desc:
-            if self.vflip:
-                e['msb'] = msb
-                msb -= e['bits']
-                e['lsb'] = msb + 1
-            else:
-                e['lsb'] = lsb
-                lsb += e['bits']
-                e['msb'] = lsb - 1
+            e['lsb'] = lsb
+            lsb += e['bits']
+            e['msb'] = lsb - 1
             e['lsbm'] = e['lsb'] % mod
             e['msbm'] = e['msb'] % mod
             if 'type' not in e:
                 e['type'] = None
 
         max_attr_count = 0
         for e in desc:
@@ -93,175 +98,238 @@
                 if isinstance(e['attr'], list):
                     max_attr_count = max(max_attr_count, len(e['attr']))
                 else:
                     max_attr_count = max(max_attr_count, 1)
 
         if not self.compact:
             self.vlane = self.vspace - self.fontsize * (1.2 + max_attr_count)
+            height = self.vspace * self.lanes  + self.stroke_width / 2
         else:
             self.vlane = self.vspace - self.fontsize * 1.2
+            height = self.vlane * (self.lanes - 1) + self.vspace + self.stroke_width / 2
+        if self.legend:
+            height += self.fontsize * 1.2
+
+        res = ['svg', {
+            'xmlns': 'http://www.w3.org/2000/svg',
+            'width': self.hspace,
+            'height': height,
+            'viewbox': ' '.join(str(x) for x in [0, 0, self.hspace, height])
+        }]
+
+        if self.legend:
+            res.append(self.legend_items())
+
         for i in range(0, self.lanes):
-            if self.hflip != self.vflip:
-                self.lane_index = self.lanes - i - 1
-            else:
+            if self.hflip:
                 self.lane_index = i
+            else:
+                self.lane_index = self.lanes - i - 1
             self.index = i
             res.append(self.lane(desc))
-
         return res
 
+    def legend_items(self):
+        items = ['g', {'transform': t(0, self.stroke_width / 2)}]
+        name_padding = 64
+        square_padding = 20
+        x = self.hspace / 2 - len(self.legend) / 2 * (square_padding + name_padding)
+        for key, value in self.legend.items():
+            items.append(['rect', {
+                'x': x,
+                'width': 12,
+                'height': 12,
+                'fill': typeColor(value),
+                'style': 'stroke:#000; stroke-width:' + str(self.stroke_width) + ';' + typeStyle(value)
+            }])
+            x += square_padding
+            items.append(['text', {
+                'x': x,
+                'font-size': self.fontsize,
+                'font-family': self.fontfamily,
+                'font-weight': self.fontweight,
+                'y': self.fontsize / 1.2,
+            }, key])
+            x += name_padding
+        return items
+
     def lane(self, desc):
-        dy = (self.lanes - self.lane_index - 1) * self.vspace
-        if self.compact and self.lane_index != self.lanes - 1:
-            dy -= (self.lanes - self.lane_index - 2) * (self.fontsize * 1.2)
+        if self.compact:
+            if self.index > 0:
+                dy = (self.index - 1) * self.vlane + self.vspace
+            else:
+                dy = 0
+        else:
+            dy = self.index * self.vspace
+        if self.legend:
+            dy += self.fontsize * 1.2
         res = ['g', {
             'transform': t(0, dy)
         }]
         res.append(self.labels(desc))
         res.append(self.cage(desc))
         return res
 
     def cage(self, desc):
-        stroke_width = 1
-        if not self.compact or self.lane_index == self.lanes - 1:
+        if not self.compact or self.index == 0:
             dy = self.fontsize * 1.2
         else:
             dy = 0
         res = ['g', {
             'stroke': 'black',
-            'stroke-width': stroke_width,
-            'stroke-linecap': 'round',
+            'stroke-width': self.stroke_width,
+            'stroke-linecap': 'butt',
             'transform': t(0, dy)
         }]
-        res.append(self.hline(self.hspace, padding=stroke_width/2))
-        res.append(self.vline(self.vlane))
-        res.append(self.hline(self.hspace, 0, self.vlane, padding=stroke_width/2))
-
-        i, j = self.index * self.mod, self.mod
-        hbit = (self.hspace - stroke_width/2) / self.mod
-        while True:
-            if j == self.mod or any(e['lsb'] == i for e in desc):
-                res.append(self.vline(self.vlane,
-                                      j * hbit))
+
+        skip_count = 0
+        if self.uneven and self.lanes > 1 and self.lane_index == self.lanes - 1:
+            skip_count = self.mod - self.bits % self.mod
+            if skip_count == self.mod:
+                skip_count = 0
+
+        hlen = (self.hspace / self.mod) * (self.mod - skip_count)
+        hpos = 0 if self.vflip else (self.hspace / self.mod) * (skip_count)
+
+        if not self.compact or self.hflip or self.lane_index == 0:
+            res.append(self.hline(hlen, hpos, self.vlane))  # bottom
+        if not self.compact or not self.hflip or self.lane_index == 0:
+            res.append(self.hline(hlen, hpos))  # top
+
+        hbit = (self.hspace - self.stroke_width) / self.mod
+        for bit_pos in range(self.mod):
+            bitm = (bit_pos if self.vflip else self.mod - bit_pos - 1)
+            bit = self.lane_index * self.mod + bitm
+            if bit >= self.bits:
+                continue
+            rpos = bit_pos + 1 if self.vflip else bit_pos
+            lpos = bit_pos if self.vflip else bit_pos + 1
+            if bitm + 1 == self.mod - skip_count:
+                res.append(self.vline(self.vlane, rpos * hbit + self.stroke_width / 2))
+            if bitm == 0:
+                res.append(self.vline(self.vlane, lpos * hbit + self.stroke_width / 2))
+            elif any(e['lsb'] == bit for e in desc):
+                res.append(self.vline(self.vlane, lpos * hbit + self.stroke_width / 2))
             else:
                 res.append(self.vline((self.vlane / 8),
-                                      j * hbit))
+                                      lpos * hbit + self.stroke_width / 2))
                 res.append(self.vline((self.vlane / 8),
-                                      j * hbit, self.vlane * 7 / 8))
-            i += 1
-            j -= 1
-            if j == 0:
-                break
+                                      lpos * hbit + self.stroke_width / 2, self.vlane * 7 / 8))
 
         return res
 
     def labels(self, desc):
         return ['g', {'text-anchor': 'middle'}, self.labelArr(desc)]
 
-    def labelArr(self, desc):
+    def labelArr(self, desc):  # noqa: C901
         step = self.hspace / self.mod
         bits = ['g', {'transform': t(step / 2, self.fontsize)}]
         names = ['g', {'transform': t(step / 2, self.vlane / 2 + self.fontsize / 2)}]
         attrs = ['g', {'transform': t(step / 2, self.vlane + self.fontsize)}]
         blanks = ['g', {'transform': t(0, 0)}]
 
         for e in desc:
             lsbm = 0
             msbm = self.mod - 1
-            lsb = self.index * self.mod
-            msb = (self.index + 1) * self.mod - 1
-            if e['lsb'] // self.mod == self.index:
+            lsb = self.lane_index * self.mod
+            msb = (self.lane_index + 1) * self.mod - 1
+            if e['lsb'] // self.mod == self.lane_index:
                 lsbm = e['lsbm']
                 lsb = e['lsb']
-                if e['msb'] // self.mod == self.index:
+                if e['msb'] // self.mod == self.lane_index:
                     msb = e['msb']
                     msbm = e['msbm']
             else:
-                if e['msb'] // self.mod == self.index:
+                if e['msb'] // self.mod == self.lane_index:
                     msb = e['msb']
                     msbm = e['msbm']
                 elif not (lsb > e['lsb'] and msb < e['msb']):
                     continue
+            msb_pos = msbm if self.vflip else (self.mod - msbm - 1)
+            lsb_pos = lsbm if self.vflip else (self.mod - lsbm - 1)
             if not self.compact:
                 bits.append(['text', {
-                    'x': step * (self.mod - lsbm - 1),
+                    'x': step * lsb_pos,
                     'font-size': self.fontsize,
                     'font-family': self.fontfamily,
                     'font-weight': self.fontweight
-                }, str(self.bits - lsb - 1) if self.vflip else str(lsb)])
+                }, str(lsb)])
                 if lsbm != msbm:
                     bits.append(['text', {
-                        'x': step * (self.mod - msbm - 1),
+                        'x': step * msb_pos,
                         'font-size': self.fontsize,
                         'font-family': self.fontfamily,
                         'font-weight': self.fontweight
-                    }, str(self.bits - msb - 1) if self.vflip else str(msb)])
+                    }, str(msb)])
             if 'name' in e:
                 ltextattrs = {
                     'font-size': self.fontsize,
                     'font-family': self.fontfamily,
                     'font-weight': self.fontweight,
                     'text-anchor': 'middle',
                     'y': 6
                 }
                 if 'rotate' in e:
                     ltextattrs['transform'] = ' rotate({})'.format(e['rotate'])
                 if 'overline' in e and e['overline']:
                     ltextattrs['text-decoration'] = 'overline'
+                available_space = step * (msbm - lsbm + 1)
                 ltext = ['g', {
-                    'transform': t(step * (self.mod - ((msbm + lsbm) / 2) - 1), -6),
-                }, ['text', ltextattrs] + tspan(e['name'])]
+                    'transform': t(step * (msb_pos + lsb_pos) / 2, -6),
+                }, ['text', ltextattrs] + tspan(self.trim_text(e['name'], available_space))]
                 names.append(ltext)
             if 'name' not in e or e['type'] is not None:
                 style = typeStyle(e['type'])
                 blanks.append(['rect', {
                     'style': style,
-                    'x': step * (self.mod - msbm - 1),
-                    'y': 0,
+                    'x': step * (lsb_pos if self.vflip else msb_pos),
+                    'y': self.stroke_width / 2,
                     'width': step * (msbm - lsbm + 1),
-                    'height': self.vlane
+                    'height': self.vlane - self.stroke_width / 2,
+                    'fill': typeColor(e['type']),
                 }])
             if 'attr' in e and not self.compact:
                 if isinstance(e['attr'], list):
                     e_attr = e['attr']
                 else:
                     e_attr = [e['attr']]
                 for i, attribute in enumerate(e_attr):
                     if isinstance(attribute, int):
                         atext = []
                         for biti in range(0, msb - lsb + 1):
                             if (1 << (biti + lsb - e['lsb'])) & attribute == 0:
                                 bit_text = "0"
                             else:
                                 bit_text = "1"
-                            atext+=[['text', {
-                                'x': step * (self.mod - lsbm - 1 - biti),
+                            bit_pos = lsb_pos + biti if self.vflip else (lsb_pos - biti)
+                            atext += [['text', {
+                                'x': step * bit_pos,
                                 'font-size': self.fontsize,
                                 'font-family': self.fontfamily,
                                 'font-weight': self.fontweight,
                             }] + tspan(bit_text)]
                     else:
                         atext = [['text', {
-                            'x': step * (self.mod - ((msbm + lsbm) / 2) - 1),
+                            'x': step * (msb_pos + lsb_pos) / 2,
                             'font-size': self.fontsize,
                             'font-family': self.fontfamily,
                             'font-weight': self.fontweight
                         }] + tspan(attribute)]
                     attrs.append(['g', {
                         'transform': t(0, i*self.fontsize)
                     }, *atext])
-        if not self.compact or self.lane_index == self.lanes - 1:
+        if not self.compact or (self.index == 0):
             if self.compact:
-                for i in range(self.bits // self.lanes):
+                for i in range(self.mod):
                     bits.append(['text', {
-                        'x': step * (self.mod - i - 1),
+                        'x': step * i,
                         'font-size': self.fontsize,
                         'font-family': self.fontfamily,
-                        'font-weight': self.fontweight
-                    }, str(self.bits // self.lanes - i - 1) if self.vflip else str(i)])
+                        'font-weight': self.fontweight,
+                    }, str(i if self.vflip else self.mod - i - 1)])
             res = ['g', {}, bits, ['g', {
                 'transform': t(0, self.fontsize*1.2)
             }, blanks, names, attrs]]
         else:
             res = ['g', {}, blanks, names, attrs]
         return res
 
@@ -270,32 +338,45 @@
         att = {}
         if padding != 0:
             len -= padding
             x += padding/2
         if x != 0:
             att['x1'] = x
         if len != 0:
-            att['x2'] = len
+            att['x2'] = x + len
         if y != 0:
             att['y1'] = y
             att['y2'] = y
         res.append(att)
         return res
 
-    def vline(self, len, x=None, y=None):
+    def vline(self, len, x=None, y=None, stroke=None):
         res = ['line']
         att = {}
         if x is not None:
             att['x1'] = x
             att['x2'] = x
         if y is not None:
             att['y1'] = y
             att['y2'] = y + len
         else:
             att['y2'] = len
+        if stroke:
+            att['stroke'] = stroke
         res.append(att)
         return res
 
+    def trim_text(self, text, available_space):
+        if self.trim_char_width is None:
+            return text
+        text_width = len(text) * self.trim_char_width
+        if text_width <= available_space:
+            return text
+        end = len(text) - int((text_width - available_space) / self.trim_char_width) - 3
+        if end > 0:
+            return text[:end] + '...'
+        return text[:1] + '...'
+
 
 def render(desc, **kwargs):
     renderer = Renderer(**kwargs)
     return renderer.render(desc)
```

### Comparing `bit_field-0.4.0/bit_field/tspan.py` & `bit_field-1.0.0/bit_field/tspan.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,19 +15,20 @@
     '<sup>': {'add': {'baseline-shift': 'super', 'font-size': '.7em'}},
     '</sup>': {'del': {'baseline-shift': 'super', 'font-size': '.7em'}},
     '<tt>': {'add': {'font-family': 'monospace'}},
     '</tt>': {'del': {'font-family': 'monospace'}}
 }
 pattern = '|'.join(re.escape(k) for k in trans.keys())
 
+
 def dump(state):
     att = {}
     for k, v in state.items():
         for kk, vv in v.items():
-            if vv == True:
+            if vv:
                 att[k] = kk
     return att
 
 
 def tspan(str):
     state = {
         'text-decoration': {},
@@ -56,10 +57,11 @@
             for k, v in cmd['del'].items():
                 del state[k][v]
         str = str[m.end(0):]
         if len(str) == 0:
             break
     return res
 
+
 if __name__ == '__main__':
     import sys
     print(tspan(''.join(sys.stdin.readlines())))
```

### Comparing `bit_field-0.4.0/bit_field.egg-info/PKG-INFO` & `bit_field-1.0.0/bit_field.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: bit-field
-Version: 0.4.0
+Version: 1.0.0
 Summary: A bitfield diagram renderer
 Home-page: https://github.com/Arth-ur/bitfield
 Author: Arthur Gay
 License: MIT
 Keywords: bitfield,bytefield,diagram,renderer,svg
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: JSON5
 License-File: LICENSE
 License-File: LICENSE-ORIGINAL
 
 A Python3 port of the javascript [bit-field library](https://github.com/drom/bitfield/) by [Aliaksei Chapyzhenka](https://github.com/drom).
 
+This package is also available as an extension for Sphinx: [sphinxcontrib-bitfield](https://github.com/Arth-ur/sphinxcontrib-bitfield).
+
 ## Install
 
 ```sh
 pip install bit_field
 ```
 
 To install this package with JSON5 support:
@@ -58,16 +59,19 @@
 --vspace     : vertical space - default 80
 --hspace     : horizontal space - default 640
 --lanes      : rectangle lanes - default 2
 --bits       : overall bitwidth - default 32
 --fontfamily : - default sans-serif
 --fontweight : - default normal
 --fontsize   : - default 14
+--strokewidth: - default 1
 --hflip      : horizontal flip
---vflip      : horizontal flip
+--vflip      : vertical flip
+--trim       : horizontal space available for a single character
+--uneven:    : uneven lanes
 
 --beautify   : use xml beautifier
 
 --json5      : force json5 input format (need json5 python module)
 --no-json5   : never use json5 input format
 ```
 
@@ -85,9 +89,7 @@
 ```
 ### alpha.svg
 
 ![Heat Sink](https://raw.githubusercontent.com/Arth-ur/bitfield/master/bit_field/test/alpha.svg?sanitize=true)
 
 ### Licensing
 This work is based on original work by [Aliaksei Chapyzhenka](https://github.com/drom) under the MIT license (see LICENSE-ORIGINAL).
-
-
```

### Comparing `bit_field-0.4.0/setup.cfg` & `bit_field-1.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bit_field
-version = 0.4.0
+version = 1.0.0
 author = Arthur Gay
 description = A bitfield diagram renderer
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Arth-ur/bitfield
 classifiers = 
 	Programming Language :: Python :: 3
```

