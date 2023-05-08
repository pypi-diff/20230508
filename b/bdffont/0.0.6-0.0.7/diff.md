# Comparing `tmp/bdffont-0.0.6.tar.gz` & `tmp/bdffont-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdffont-0.0.6.tar", last modified: Sat May  6 08:41:47 2023, max compression
+gzip compressed data, was "bdffont-0.0.7.tar", last modified: Mon May  8 07:42:13 2023, max compression
```

## Comparing `bdffont-0.0.6.tar` & `bdffont-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:41:47.890764 bdffont-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-06 08:41:31.000000 bdffont-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-06 08:41:47.890764 bdffont-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-06 08:41:31.000000 bdffont-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-06 08:41:31.000000 bdffont-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 08:41:47.890764 bdffont-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:41:47.886763 bdffont-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:41:47.890764 bdffont-0.0.6/src/bdffont/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-06 08:41:31.000000 bdffont-0.0.6/src/bdffont/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-06 08:41:31.000000 bdffont-0.0.6/src/bdffont/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-05-06 08:41:31.000000 bdffont-0.0.6/src/bdffont/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-05-06 08:41:31.000000 bdffont-0.0.6/src/bdffont/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-05-06 08:41:31.000000 bdffont-0.0.6/src/bdffont/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-06 08:41:31.000000 bdffont-0.0.6/src/bdffont/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:41:47.890764 bdffont-0.0.6/src/bdffont.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-06 08:41:47.000000 bdffont-0.0.6/src/bdffont.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-06 08:41:47.000000 bdffont-0.0.6/src/bdffont.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:41:47.000000 bdffont-0.0.6/src/bdffont.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-06 08:41:47.000000 bdffont-0.0.6/src/bdffont.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:41:47.890764 bdffont-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-06 08:41:31.000000 bdffont-0.0.6/tests/test_damaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-06 08:41:31.000000 bdffont-0.0.6/tests/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-06 08:41:31.000000 bdffont-0.0.6/tests/test_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:42:13.065421 bdffont-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 07:41:54.000000 bdffont-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-08 07:42:13.065421 bdffont-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-08 07:41:54.000000 bdffont-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-08 07:41:54.000000 bdffont-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 07:42:13.065421 bdffont-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:42:13.061421 bdffont-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:42:13.065421 bdffont-0.0.7/src/bdffont/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-08 07:41:54.000000 bdffont-0.0.7/src/bdffont/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-08 07:41:54.000000 bdffont-0.0.7/src/bdffont/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-08 07:41:54.000000 bdffont-0.0.7/src/bdffont/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-05-08 07:41:54.000000 bdffont-0.0.7/src/bdffont/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-08 07:41:54.000000 bdffont-0.0.7/src/bdffont/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-08 07:41:54.000000 bdffont-0.0.7/src/bdffont/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:42:13.065421 bdffont-0.0.7/src/bdffont.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-08 07:42:13.000000 bdffont-0.0.7/src/bdffont.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-08 07:42:13.000000 bdffont-0.0.7/src/bdffont.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 07:42:13.000000 bdffont-0.0.7/src/bdffont.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 07:42:13.000000 bdffont-0.0.7/src/bdffont.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:42:13.065421 bdffont-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-08 07:41:54.000000 bdffont-0.0.7/tests/test_damaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-08 07:41:54.000000 bdffont-0.0.7/tests/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-05-08 07:41:54.000000 bdffont-0.0.7/tests/test_type.py
```

### Comparing `bdffont-0.0.6/LICENSE` & `bdffont-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.6/PKG-INFO` & `bdffont-0.0.7/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: bdffont
-Version: 0.0.6
-Summary: A library for manipulating '.bdf' format fonts.
-Author: TakWolf
-Maintainer: TakWolf
-License: MIT License
-Project-URL: homepage, https://github.com/TakWolf/bdffont
-Project-URL: source, https://github.com/TakWolf/bdffont
-Project-URL: issues, https://github.com/TakWolf/bdffont/issues
-Keywords: bdf,font
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # BdfFont
 
 [![PyPI](https://img.shields.io/pypi/v/bdffont)](https://pypi.org/project/bdffont/)
 
 BdfFont is a library for manipulating [`.bdf` format fonts](https://en.wikipedia.org/wiki/Glyph_Bitmap_Distribution_Format), written in Python.
 
 ## Installation
@@ -29,24 +11,34 @@
 ```
 
 ## Usage
 
 ```python
 import os
 
-import bdffont
-from bdffont import BdfGlyph
-from examples import assets_dir, outputs_dir
+from bdffont import BdfFont, BdfProperties, BdfGlyph
+from examples import outputs_dir
 
 
 def main():
-    font = bdffont.load_bdf(os.path.join(assets_dir, 'example.bdf'))
-    font.name = 'my-new-font'
-    font.bounding_box_size = 16, 16
-    font.bounding_box_offset = 0, -2
+    font = BdfFont(
+        name='my-font',
+        point_size=16,
+        dpi_xy=(75, 75),
+        bounding_box_size=(16, 16),
+        bounding_box_offset=(0, -2),
+        properties=BdfProperties({
+            'PARAM_1': 1,
+            'PARAM_2': '2',
+        }),
+        comments=[
+            'This is a comment.',
+            'This is a comment, too.',
+        ],
+    )
     font.properties.font_version = '1.0.0'
     font.properties.font_ascent = 7
     font.properties.font_descent = 2
     font.properties.x_height = 5
     font.properties.cap_height = 7
     font.add_glyph(BdfGlyph(
         name='A',
@@ -70,15 +62,15 @@
             [0, 1, 0, 0, 0, 0, 1, 0],
             [0, 1, 0, 0, 0, 0, 1, 0],
             [0, 1, 0, 0, 0, 0, 1, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
         ],
     ))
-    font.save(os.path.join(outputs_dir, 'example-output.bdf'))
+    font.save(os.path.join(outputs_dir, 'my-font.bdf'), optimize_bitmap=True)
 
 
 if __name__ == '__main__':
     main()
 ```
 
 ## References
```

### Comparing `bdffont-0.0.6/pyproject.toml` & `bdffont-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bdffont"
-version = "0.0.6"
+version = "0.0.7"
 description = "A library for manipulating '.bdf' format fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `bdffont-0.0.6/src/bdffont/error.py` & `bdffont-0.0.7/src/bdffont/error.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 
 class BdfException(Exception):
     pass
 
 
 class BdfGlyphExists(BdfException):
-    code_point: int
-
     def __init__(self, code_point: int):
         self.code_point = code_point
         super().__init__(f"Glyph '{code_point}' already exists")
 
 
 class BdfMissingLine(BdfException):
-    word: str
-
     def __init__(self, word: str):
         self.word = word
         super().__init__(f"Missing line '{word}'")
 
 
 class BdfValueIncorrect(BdfException):
-    word: str
-
     def __init__(self, word: str):
         self.word = word
         super().__init__(f"'{word}' value incorrect")
 
 
+class BdfIllegalBitmap(BdfException):
+    pass
+
+
 class BdfIllegalPropertiesKey(BdfException):
     pass
 
 
 class BdfIllegalPropertiesValue(BdfException):
     pass
```

### Comparing `bdffont-0.0.6/src/bdffont/font.py` & `bdffont-0.0.7/src/bdffont/font.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,71 +2,55 @@
 
 from bdffont.properties import BdfProperties
 from bdffont.glyph import BdfGlyph
 from bdffont.error import BdfGlyphExists
 
 
 class BdfFont:
-    # The BDF Specification version.
-    spec_version: str
-
-    # Either the 'X logical font description' or some private font name.
-    # https://en.wikipedia.org/wiki/X_logical_font_description
-    # Example: -Adobe-Helvetica-Bold-R-Normal--24-240-75-75-P-65-ISO8859-1
-    name: str
-
-    # The point size of the characters.
-    point_size: int
-
-    # The x resolution, and the y resolution of the device for which these characters were intended.
-    dpi_x: int
-    dpi_y: int
-
-    # The width in x, height in y, and the x and y displacement of the lower left corner from the origin
-    # of the character.
-    bounding_box_width: int
-    bounding_box_height: int
-    bounding_box_offset_x: int
-    bounding_box_offset_y: int
-
-    # Some optional extended properties.
-    properties: BdfProperties
-
-    # Glyph objects using code point indexing.
-    code_point_to_glyph: dict[int, BdfGlyph]
-
-    # Comments.
-    comments: list[str]
-
     def __init__(
             self,
             name: str,
             point_size: int,
             dpi_xy: tuple[int, int],
             bounding_box_size: tuple[int, int],
             bounding_box_offset: tuple[int, int],
             properties: BdfProperties = None,
-            glyphs: list[BdfGlyph] = None,
             comments: list[str] = None,
     ):
+        """
+        :param name:
+            Either the 'X logical font description' or some private font name.
+            Like: -Adobe-Helvetica-Bold-R-Normal--24-240-75-75-P-65-ISO8859-1
+            https://en.wikipedia.org/wiki/X_logical_font_description
+        :param point_size:
+            The point size of the characters.
+        :param dpi_xy:
+            The x resolution, and the y resolution of the device for which these characters were intended.
+        :param bounding_box_size:
+            The width in x, height in y of the character.
+        :param bounding_box_offset:
+            The x and y displacement of the lower left corner from the origin of the character.
+        :param properties:
+            Some optional extended properties.
+        :param comments:
+            The comments.
+        """
         self.spec_version = '2.1'
         self.name = name
         self.point_size = point_size
         self.dpi_x, self.dpi_y = dpi_xy
         self.bounding_box_width, self.bounding_box_height = bounding_box_size
         self.bounding_box_offset_x, self.bounding_box_offset_y = bounding_box_offset
         if properties is None:
             properties = BdfProperties()
         self.properties = properties
-        if glyphs is None:
-            glyphs = []
-        self.code_point_to_glyph = {glyph.code_point: glyph for glyph in glyphs}
         if comments is None:
             comments = []
         self.comments = comments
+        self.code_point_to_glyph = {}
 
     @property
     def dpi_xy(self) -> tuple[int, int]:
         return self.dpi_x, self.dpi_y
 
     @dpi_xy.setter
     def dpi_xy(self, value: tuple[int, int]):
@@ -92,29 +76,41 @@
     def bounding_box(self) -> tuple[int, int, int, int]:
         return self.bounding_box_width, self.bounding_box_height, self.bounding_box_offset_x, self.bounding_box_offset_y
 
     @bounding_box.setter
     def bounding_box(self, value: tuple[int, int, int, int]):
         self.bounding_box_width, self.bounding_box_height, self.bounding_box_offset_x, self.bounding_box_offset_y = value
 
+    def get_glyphs_count(self) -> int:
+        return len(self.code_point_to_glyph)
+
     def get_glyph(self, code_point: int) -> BdfGlyph | None:
         return self.code_point_to_glyph.get(code_point, None)
 
+    def get_orderly_glyphs(self) -> list[BdfGlyph]:
+        glyphs = list(self.code_point_to_glyph.values())
+        glyphs.sort(key=lambda glyph: glyph.code_point)
+        return glyphs
+
     def add_glyph(self, glyph: BdfGlyph):
         if glyph.code_point in self.code_point_to_glyph:
             raise BdfGlyphExists(glyph.code_point)
         self.code_point_to_glyph[glyph.code_point] = glyph
 
+    def add_glyphs(self, glyphs: list[BdfGlyph]):
+        for glyph in glyphs:
+            self.add_glyph(glyph)
+
     def set_glyph(self, glyph: BdfGlyph):
         self.code_point_to_glyph[glyph.code_point] = glyph
 
     def remove_glyph(self, code_point: int) -> BdfGlyph | None:
         return self.code_point_to_glyph.pop(code_point, None)
 
-    def encode(self) -> list[str]:
+    def encode(self, optimize_bitmap: bool = False) -> list[str]:
         lines = [
             f'STARTFONT {self.spec_version}',
         ]
         for comment in self.comments:
             lines.append(f'COMMENT {comment}')
         lines.append(f'FONT {self.name}')
         lines.append(f'SIZE {self.point_size} {self.dpi_x} {self.dpi_y}')
@@ -125,34 +121,37 @@
             lines.append(f'COMMENT {comment}')
         for word, value in self.properties.items():
             if isinstance(value, str):
                 value = f'"{value}"'
             lines.append(f'{word} {value}')
         lines.append('ENDPROPERTIES')
 
-        alphabet = list(self.code_point_to_glyph.items())
-        alphabet.sort()
-        lines.append(f'CHARS {len(alphabet)}')
-        for code_point, glyph in alphabet:
+        lines.append(f'CHARS {self.get_glyphs_count()}')
+        for glyph in self.get_orderly_glyphs():
             lines.append(f'STARTCHAR {glyph.name}')
             for comment in glyph.comments:
                 lines.append(f'COMMENT {comment}')
-            lines.append(f'ENCODING {code_point}')
+            lines.append(f'ENCODING {glyph.code_point}')
             lines.append(f'SWIDTH {glyph.scalable_width_x} {glyph.scalable_width_y}')
             lines.append(f'DWIDTH {glyph.device_width_x} {glyph.device_width_y}')
-            lines.append(f'BBX {glyph.bounding_box_width} {glyph.bounding_box_height} {glyph.bounding_box_offset_x} {glyph.bounding_box_offset_y}')
+            (bounding_box_width, bounding_box_height), (bounding_box_offset_x, bounding_box_offset_y), bitmap = glyph.get_8bit_aligned_bitmap(optimize_bitmap)
+            lines.append(f'BBX {bounding_box_width} {bounding_box_height} {bounding_box_offset_x} {bounding_box_offset_y}')
             lines.append('BITMAP')
-            for bitmap_row in glyph.get_padded_bitmap():
+            for bitmap_row in bitmap:
                 hex_format = '{:0' + str(len(bitmap_row) // 4) + 'X}'
                 lines.append(hex_format.format(int(''.join(map(str, bitmap_row)), 2)))
             lines.append('ENDCHAR')
 
         lines.append('ENDFONT')
         lines.append('')
         return lines
 
-    def encode_str(self) -> str:
-        return '\n'.join(self.encode())
+    def encode_str(self, optimize_bitmap: bool = False) -> str:
+        return '\n'.join(self.encode(optimize_bitmap))
 
-    def save(self, file_path: str | bytes | os.PathLike[str] | os.PathLike[bytes]):
+    def save(
+            self,
+            file_path: str | bytes | os.PathLike[str] | os.PathLike[bytes],
+            optimize_bitmap: bool = False,
+    ):
         with open(file_path, 'w', encoding='utf-8') as file:
-            file.write(self.encode_str())
+            file.write(self.encode_str(optimize_bitmap))
```

### Comparing `bdffont-0.0.6/src/bdffont/glyph.py` & `bdffont-0.0.7/src/bdffont/glyph.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,51 @@
+from bdffont.error import BdfIllegalBitmap
 
-class BdfGlyph:
-    # Up to 14 characters (no blanks) of descriptive name of the glyph.
-    name: str
-
-    # Code point in Unicode.
-    code_point: int
-
-    # The scalable width in x and y of character. Scalable widths are in units of 1/1000th of the size of
-    # the character. If the size of the character is p points, the width information must be scaled by p/1000
-    # to get the width of the character in printer’s points. This width information should be considered as a
-    # vector indicating the position of the next character’s origin relative to the origin of this character.
-    # To convert the scalable width to the width in device pixels, multiply s_width times p/1000 times r/72,
-    # where r is the device resolution in pixels per inch. The result is a real number giving the ideal print
-    # width in device pixels. The actual device width must of course be an integral number of device pixels and
-    # is given in the next entry. The s_width y value should always be zero for a standard X font.
-    scalable_width_x: int
-    scalable_width_y: int
-
-    # The width in x and y of the character in device units. Like the s_width, this width information is a vector
-    # indicating the position of the next character’s origin relative to the origin of this character. Note that
-    # the d_width of a given "hand-tuned" WYSIWYG glyph may deviate slightly from its ideal device-independent width
-    # given by s_width in order to improve its typographic characteristics on a display. The d_width y value should
-    # always be zero for a standard X font.
-    device_width_x: int
-    device_width_y: int
-
-    # The width in x, height in y, and the x and y displacement of the lower left corner from the origin
-    # of the character.
-    bounding_box_width: int
-    bounding_box_height: int
-    bounding_box_offset_x: int
-    bounding_box_offset_y: int
-
-    # The bitmap object.
-    bitmap: list[list[int]]
-
-    # Comments.
-    comments: list[str]
 
+class BdfGlyph:
     def __init__(
             self,
             name: str,
             code_point: int,
             scalable_width: tuple[int, int],
             device_width: tuple[int, int],
             bounding_box_size: tuple[int, int],
             bounding_box_offset: tuple[int, int],
             bitmap: list[list[int]] = None,
             comments: list[str] = None,
     ):
+        """
+        :param name:
+            Up to 14 characters (no blanks) of descriptive name of the glyph.
+        :param code_point:
+            Code point in Unicode.
+        :param scalable_width:
+            The scalable width in x and y of character. Scalable widths are in units of 1/1000th of the size of the
+            character. If the size of the character is p points, the width information must be scaled by p/1000 to
+            get the width of the character in printer’s points. This width information should be considered as a vector
+            indicating the position of the next character’s origin relative to the origin of this character.
+            To convert the scalable width to the width in device pixels, multiply scalable_width times p/1000 times
+            r/72, where r is the device resolution in pixels per inch. The result is a real number giving the ideal
+            print width in device pixels. The actual device width must of course be an integral number of device pixels
+            and is given in the next entry. The scalable_width y value should always be zero for a standard X font.
+        :param device_width:
+            The width in x and y of the character in device units. Like the scalable_width, this width information is
+            a vector indicating the position of the next character’s origin relative to the origin of this character.
+            Note that the device_width of a given "hand-tuned" WYSIWYG glyph may deviate slightly from its ideal
+            device-independent width given by scalable_width in order to improve its typographic characteristics on a
+            display. The device_width y value should always be zero for a standard X font.
+        :param bounding_box_size:
+            The width in x, height in y of the character.
+        :param bounding_box_offset:
+            The x and y displacement of the lower left corner from the origin of the character.
+        :param bitmap:
+            The bitmap object.
+        :param comments:
+            The comments.
+        """
         self.name = name
         self.code_point = code_point
         self.scalable_width_x, self.scalable_width_y = scalable_width
         self.device_width_x, self.device_width_y = device_width
         self.bounding_box_width, self.bounding_box_height = bounding_box_size
         self.bounding_box_offset_x, self.bounding_box_offset_y = bounding_box_offset
         if bitmap is None:
@@ -98,22 +91,77 @@
     def bounding_box(self) -> tuple[int, int, int, int]:
         return self.bounding_box_width, self.bounding_box_height, self.bounding_box_offset_x, self.bounding_box_offset_y
 
     @bounding_box.setter
     def bounding_box(self, value: tuple[int, int, int, int]):
         self.bounding_box_width, self.bounding_box_height, self.bounding_box_offset_x, self.bounding_box_offset_y = value
 
-    def get_padded_bitmap(self) -> list[list[int]]:
-        padded_bitmap = []
+    def check_bitmap_validity(self):
+        if len(self.bitmap) != self.bounding_box_height:
+            raise BdfIllegalBitmap("Glyph bitmap height not equals 'bounding_box_height'")
         for bitmap_row in self.bitmap:
-            padded_bitmap_row = []
-            for alpha in bitmap_row:
-                if alpha == 0:
-                    padded_bitmap_row.append(0)
+            if len(bitmap_row) != self.bounding_box_width:
+                raise BdfIllegalBitmap("Glyph bitmap width not equals 'bounding_box_width'")
+
+    def get_8bit_aligned_bitmap(self, optimize_bitmap: bool = False) -> tuple[tuple[int, int], tuple[int, int], list[list[int]]]:
+        self.check_bitmap_validity()
+        bounding_box_width = self.bounding_box_width
+        bounding_box_height = self.bounding_box_height
+        bounding_box_offset_x = self.bounding_box_offset_x
+        bounding_box_offset_y = self.bounding_box_offset_y
+        bitmap = [[color for color in bitmap_row] for bitmap_row in self.bitmap]
+
+        if optimize_bitmap:
+            # Top
+            while bounding_box_height > 0:
+                for color in bitmap[0]:
+                    if color != 0:
+                        break
+                else:
+                    bitmap.pop(0)
+                    bounding_box_height -= 1
+                    continue
+                break
+            # Bottom
+            while bounding_box_height > 0:
+                for color in bitmap[-1]:
+                    if color != 0:
+                        break
+                else:
+                    bitmap.pop()
+                    bounding_box_height -= 1
+                    bounding_box_offset_y += 1
+                    continue
+                break
+            # Left
+            while bounding_box_width > 0:
+                for bitmap_row in bitmap:
+                    color = bitmap_row[0]
+                    if color != 0:
+                        break
                 else:
-                    padded_bitmap_row.append(1)
-            remainder = len(bitmap_row) % 8
-            if remainder > 0:
+                    for bitmap_row in bitmap:
+                        bitmap_row.pop(0)
+                    bounding_box_width -= 1
+                    bounding_box_offset_x += 1
+                    continue
+                break
+            # Right
+            while bounding_box_width > 0:
+                for bitmap_row in bitmap:
+                    color = bitmap_row[-1]
+                    if color != 0:
+                        break
+                else:
+                    for bitmap_row in bitmap:
+                        bitmap_row.pop()
+                    bounding_box_width -= 1
+                    continue
+                break
+
+        remainder = bounding_box_width % 8
+        if remainder > 0:
+            for bitmap_row in bitmap:
                 for _ in range(8 - remainder):
-                    padded_bitmap_row.append(0)
-            padded_bitmap.append(padded_bitmap_row)
-        return padded_bitmap
+                    bitmap_row.append(0)
+
+        return (bounding_box_width, bounding_box_height), (bounding_box_offset_x, bounding_box_offset_y), bitmap
```

### Comparing `bdffont-0.0.6/src/bdffont/parser.py` & `bdffont-0.0.7/src/bdffont/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import re
 from typing import Iterator
 
 from bdffont.font import BdfFont
 from bdffont.properties import BdfProperties
 from bdffont.glyph import BdfGlyph
-from bdffont.error import BdfGlyphExists, BdfMissingLine, BdfValueIncorrect
+from bdffont.error import BdfMissingLine, BdfValueIncorrect
 
 
 def _next_word_line(lines: Iterator[str]) -> tuple[str, str | None] | None:
     while True:
         try:
             line = next(lines)
         except StopIteration:
@@ -39,38 +39,36 @@
         try:
             value = int(tail)
         except ValueError:
             value = tail
     return value
 
 
-def _decode_properties_segment(lines: Iterator[str], count: int) -> BdfProperties:
+def _decode_properties_segment(lines: Iterator[str], count: int, strict_mode: bool) -> BdfProperties:
     properties = BdfProperties()
     while line_params := _next_word_line(lines):
         word, tail = line_params
         if word == 'ENDPROPERTIES':
-            if count != len(properties):
+            if strict_mode and count != len(properties):
                 raise BdfValueIncorrect('STARTPROPERTIES')
             return properties
         elif word == 'COMMENT':
             properties.comments.append(tail)
         else:
             properties[word] = _convert_tail_to_properties_value(tail)
     raise BdfMissingLine('ENDPROPERTIES')
 
 
-def _decode_bitmap_segment(lines: Iterator[str], comments: list[str]) -> list[list[int]]:
+def _decode_bitmap_segment(lines: Iterator[str]) -> list[list[int]]:
     bitmap = []
     while line_params := _next_word_line(lines):
         word, tail = line_params
         if word == 'ENDCHAR':
             return bitmap
-        elif word == 'COMMENT':
-            comments.append(tail)
-        elif word != '':
+        else:
             bin_format = '{:0' + str(len(word) * 4) + 'b}'
             bitmap.append([int(c) for c in bin_format.format(int(word, 16))])
     raise BdfMissingLine('ENDCHAR')
 
 
 def _decode_glyph_segment(lines: Iterator[str], name: str) -> BdfGlyph:
     code_point = None
@@ -94,87 +92,107 @@
             tokens = _convert_tail_to_ints(tail)
             bounding_box_size = tokens[0], tokens[1]
             bounding_box_offset = tokens[2], tokens[3]
         elif word == 'COMMENT':
             comments.append(tail)
         elif word == 'BITMAP' or word == 'ENDCHAR':
             if word == 'BITMAP':
-                bitmap = _decode_bitmap_segment(lines, comments)
+                bitmap = _decode_bitmap_segment(lines)
             if code_point is None:
                 raise BdfMissingLine('ENCODING')
             if scalable_width is None:
                 raise BdfMissingLine('SWIDTH')
             if device_width is None:
                 raise BdfMissingLine('DWIDTH')
             if bounding_box_size is None or bounding_box_offset is None:
                 raise BdfMissingLine('BBX')
-            return BdfGlyph(name, code_point, scalable_width, device_width, bounding_box_size, bounding_box_offset, bitmap, comments)
+            for bitmap_row in bitmap:
+                while len(bitmap_row) > bounding_box_size[0]:
+                    bitmap_row.pop()
+            return BdfGlyph(
+                name,
+                code_point,
+                scalable_width,
+                device_width,
+                bounding_box_size,
+                bounding_box_offset,
+                bitmap,
+                comments,
+            )
     raise BdfMissingLine('ENDCHAR')
 
 
-def _decode_font_segment(lines: Iterator[str]) -> BdfFont:
+def _decode_font_segment(lines: Iterator[str], strict_mode: bool) -> BdfFont:
     name = None
     point_size = None
     dpi_xy = None
     bounding_box_size = None
     bounding_box_offset = None
     properties = None
-    glyph_count = None
+    glyphs_count = None
     glyphs = []
-    alphabet = set()
     comments = []
     while line_params := _next_word_line(lines):
         word, tail = line_params
         if word == 'FONT':
             name = tail
         elif word == 'SIZE':
             tokens = _convert_tail_to_ints(tail)
             point_size = tokens[0]
             dpi_xy = tokens[1], tokens[2]
         elif word == 'FONTBOUNDINGBOX':
             tokens = _convert_tail_to_ints(tail)
             bounding_box_size = tokens[0], tokens[1]
             bounding_box_offset = tokens[2], tokens[3]
         elif word == 'STARTPROPERTIES':
-            properties = _decode_properties_segment(lines, int(tail))
+            properties = _decode_properties_segment(lines, int(tail), strict_mode)
         elif word == 'CHARS':
-            glyph_count = int(tail)
+            glyphs_count = int(tail)
         elif word == 'STARTCHAR':
-            glyph = _decode_glyph_segment(lines, tail)
-            if glyph.code_point in alphabet:
-                raise BdfGlyphExists(glyph.code_point)
-            glyphs.append(glyph)
-            alphabet.add(glyph.code_point)
+            glyphs.append(_decode_glyph_segment(lines, tail))
         elif word == 'COMMENT':
             comments.append(tail)
         elif word == 'ENDFONT':
             if name is None:
                 raise BdfMissingLine('FONT')
             if point_size is None or dpi_xy is None:
                 raise BdfMissingLine('SIZE')
             if bounding_box_size is None or bounding_box_offset is None:
                 raise BdfMissingLine('FONTBOUNDINGBOX')
-            if glyph_count is None:
+            if glyphs_count is None:
                 raise BdfMissingLine('CHARS')
-            if glyph_count != len(glyphs) or glyph_count != len(alphabet):
+            if strict_mode and glyphs_count != len(glyphs):
                 raise BdfValueIncorrect('CHARS')
-            return BdfFont(name, point_size, dpi_xy, bounding_box_size, bounding_box_offset, properties, glyphs, comments)
+            font = BdfFont(
+                name,
+                point_size,
+                dpi_xy,
+                bounding_box_size,
+                bounding_box_offset,
+                properties,
+                comments,
+            )
+            font.add_glyphs(glyphs)
+            return font
     raise BdfMissingLine('ENDFONT')
 
 
-def decode_bdf(lines: Iterator[str]) -> BdfFont:
+def decode_bdf(lines: Iterator[str], strict_mode: bool = False) -> BdfFont:
     while line_params := _next_word_line(lines):
         word, tail = line_params
         if word == 'STARTFONT':
-            font = _decode_font_segment(lines)
+            font = _decode_font_segment(lines, strict_mode)
             font.spec_version = tail
             return font
     raise BdfMissingLine('STARTFONT')
 
 
-def decode_bdf_str(text: str) -> BdfFont:
-    return decode_bdf(iter(text.split('\n')))
+def decode_bdf_str(text: str, strict_mode: bool = False) -> BdfFont:
+    return decode_bdf(iter(text.split('\n')), strict_mode)
 
 
-def load_bdf(file_path: str | bytes | os.PathLike[str] | os.PathLike[bytes]) -> BdfFont:
+def load_bdf(
+        file_path: str | bytes | os.PathLike[str] | os.PathLike[bytes],
+        strict_mode: bool = False,
+) -> BdfFont:
     with open(file_path, 'r', encoding='utf-8') as file:
-        return decode_bdf(iter(file.readlines()))
+        return decode_bdf(iter(file.readlines()), strict_mode)
```

### Comparing `bdffont-0.0.6/tests/test_damaged.py` & `bdffont-0.0.7/tests/test_damaged.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,69 +3,94 @@
 import pytest
 
 import bdffont
 from bdffont.error import BdfMissingLine, BdfValueIncorrect
 from tests import assets_dir
 
 
-def load_damaged_bdf(file_name: str):
+def load_damaged_bdf(file_name: str, strict_mode: bool = False):
     file_path = os.path.join(assets_dir, 'damaged', file_name)
-    bdffont.load_bdf(file_path)
+    bdffont.load_bdf(file_path, strict_mode=strict_mode)
 
 
 def test_not_a_bdf():
-    with pytest.raises(Exception) as info:
+    with pytest.raises(BdfMissingLine) as info:
         load_damaged_bdf('not_a_bdf.bdf')
-    assert info.type == BdfMissingLine
     assert info.value.word == 'STARTFONT'
 
 
 def test_no_line_font():
-    with pytest.raises(Exception) as info:
+    with pytest.raises(BdfMissingLine) as info:
         load_damaged_bdf('no_line_font.bdf')
-    assert info.type == BdfMissingLine
     assert info.value.word == 'FONT'
 
 
 def test_no_line_size():
-    with pytest.raises(Exception) as info:
+    with pytest.raises(BdfMissingLine) as info:
         load_damaged_bdf('no_line_size.bdf')
-    assert info.type == BdfMissingLine
     assert info.value.word == 'SIZE'
 
 
 def test_no_line_fontboundingbox():
-    with pytest.raises(Exception) as info:
+    with pytest.raises(BdfMissingLine) as info:
         load_damaged_bdf('no_line_fontboundingbox.bdf')
-    assert info.type == BdfMissingLine
     assert info.value.word == 'FONTBOUNDINGBOX'
 
 
 def test_no_line_end_properties():
     with pytest.raises(Exception):
         load_damaged_bdf('no_line_end_properties.bdf')
 
 
+def test_no_line_chars():
+    with pytest.raises(BdfMissingLine) as info:
+        load_damaged_bdf('no_line_chars.bdf')
+    assert info.value.word == 'CHARS'
+
+
+def test_no_line_encoding():
+    with pytest.raises(BdfMissingLine) as info:
+        load_damaged_bdf('no_line_encoding.bdf')
+    assert info.value.word == 'ENCODING'
+
+
+def test_no_line_swidth():
+    with pytest.raises(BdfMissingLine) as info:
+        load_damaged_bdf('no_line_swidth.bdf')
+    assert info.value.word == 'SWIDTH'
+
+
+def test_no_line_dwidth():
+    with pytest.raises(BdfMissingLine) as info:
+        load_damaged_bdf('no_line_dwidth.bdf')
+    assert info.value.word == 'DWIDTH'
+
+
+def test_no_line_bbx():
+    with pytest.raises(BdfMissingLine) as info:
+        load_damaged_bdf('no_line_bbx.bdf')
+    assert info.value.word == 'BBX'
+
+
 def test_no_line_end_char():
     with pytest.raises(Exception):
         load_damaged_bdf('no_line_end_char.bdf')
 
 
 def test_no_line_end_font():
-    with pytest.raises(Exception) as info:
+    with pytest.raises(BdfMissingLine) as info:
         load_damaged_bdf('no_line_end_font.bdf')
-    assert info.type == BdfMissingLine
     assert info.value.word == 'ENDFONT'
 
 
 def test_incorrect_properties_count():
-    with pytest.raises(Exception) as info:
-        load_damaged_bdf('incorrect_properties_count.bdf')
-    assert info.type == BdfValueIncorrect
+    load_damaged_bdf('incorrect_properties_count.bdf')
+    with pytest.raises(BdfValueIncorrect) as info:
+        load_damaged_bdf('incorrect_properties_count.bdf', strict_mode=True)
     assert info.value.word == 'STARTPROPERTIES'
 
 
 def test_incorrect_chars_count():
-    with pytest.raises(Exception) as info:
-        load_damaged_bdf('incorrect_chars_count.bdf')
-    assert info.type == BdfValueIncorrect
+    load_damaged_bdf('incorrect_chars_count.bdf')
+    with pytest.raises(BdfValueIncorrect) as info:
+        load_damaged_bdf('incorrect_chars_count.bdf', strict_mode=True)
     assert info.value.word == 'CHARS'
```

### Comparing `bdffont-0.0.6/tests/test_demo.py` & `bdffont-0.0.7/tests/test_demo.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     font = bdffont.decode_bdf_str(bdf_text)
     return font, bdf_text
 
 
 def test_example():
     font, bdf_text = load_bdf('example.bdf')
     assert font.encode_str() == bdf_text
+    assert font.encode_str(optimize_bitmap=True) == bdf_text
     assert font.spec_version == '2.1'
     assert font.name == '-Adobe-Helvetica-Bold-R-Normal--24-240-75-75-P-65-ISO8859-1'
     assert font.point_size == 24
     assert font.dpi_x == 75
     assert font.dpi_y == 75
     assert font.dpi_xy == (75, 75)
     assert font.bounding_box_width == 9
@@ -45,15 +46,15 @@
     assert font.properties['CHARSET_REGISTRY'] == 'ISO8859'
     assert font.properties['CHARSET_ENCODING'] == '1'
     assert font.properties['MIN_SPACE'] == 4
     assert font.properties.font_ascent == 21
     assert font.properties.font_descent == 7
     assert font.properties.copyright == 'Copyright (c) 1987 Adobe Systems, Inc.'
     assert font.properties.notice == 'Helvetica is a registered trademark of Linotype Inc.'
-    assert len(font.code_point_to_glyph) == 2
+    assert font.get_glyphs_count() == 2
     glyph = font.get_glyph(39)
     assert glyph.name == 'quoteright'
     assert glyph.code_point == 39
     assert glyph.scalable_width_x == 223
     assert glyph.scalable_width_y == 0
     assert glyph.scalable_width == (223, 0)
     assert glyph.device_width_x == 5
@@ -64,27 +65,27 @@
     assert glyph.bounding_box_size == (4, 6)
     assert glyph.bounding_box_offset_x == 2
     assert glyph.bounding_box_offset_y == 12
     assert glyph.bounding_box_offset == (2, 12)
     assert glyph.bounding_box == (4, 6, 2, 12)
     assert len(glyph.bitmap) == 6
     glyph_data = [
-        '_###____',
-        '_###____',
-        '_###____',
-        '_##_____',
-        '###_____',
-        '##______',
+        '_###',
+        '_###',
+        '_###',
+        '_##_',
+        '###_',
+        '##__',
     ]
     for i, bitmap_row in enumerate(glyph.bitmap):
         assert ''.join(map(str, bitmap_row)).replace('0', '_').replace('1', '#') == glyph_data[i]
-    font.save(os.path.join(outputs_dir, 'example-output.bdf'))
+    font.save(os.path.join(outputs_dir, 'example-output.bdf'), optimize_bitmap=True)
 
 
 def test_unifont():
     font = load_bdf('unifont-15.0.01.bdf')[0]
-    font.save(os.path.join(outputs_dir, 'unifont-output.bdf'))
+    font.save(os.path.join(outputs_dir, 'unifont-output.bdf'), optimize_bitmap=True)
 
 
 def test_galmuri9():
     font = load_bdf('galmuri9.bdf')[0]
-    font.save(os.path.join(outputs_dir, 'galmuri9-output.bdf'))
+    font.save(os.path.join(outputs_dir, 'galmuri9-output.bdf'), optimize_bitmap=True)
```

