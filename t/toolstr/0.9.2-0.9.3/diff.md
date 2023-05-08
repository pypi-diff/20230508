# Comparing `tmp/toolstr-0.9.2.tar.gz` & `tmp/toolstr-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolstr-0.9.2.tar", last modified: Mon Apr 24 06:18:02 2023, max compression
+gzip compressed data, was "toolstr-0.9.3.tar", last modified: Mon May  8 06:50:24 2023, max compression
```

## Comparing `toolstr-0.9.2.tar` & `toolstr-0.9.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0       80 2023-01-01 01:26:00.835967 toolstr-0.9.2/.gitignore
--rw-r--r--   0        0        0     1084 2022-12-09 18:24:40.520680 toolstr-0.9.2/LICENSE
--rw-r--r--   0        0        0     8107 2022-12-09 18:24:40.520919 toolstr-0.9.2/README.md
--rw-r--r--   0        0        0      611 2022-12-12 20:01:41.098721 toolstr-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      245 2023-04-24 06:17:40.740773 toolstr-0.9.2/toolstr/__init__.py
--rw-r--r--   0        0        0      475 2022-12-09 18:24:40.521992 toolstr-0.9.2/toolstr/charts/README.md
--rw-r--r--   0        0        0      134 2022-12-09 18:24:40.522217 toolstr-0.9.2/toolstr/charts/__init__.py
--rw-r--r--   0        0        0    12629 2022-12-09 18:24:40.522525 toolstr-0.9.2/toolstr/charts/braille_utils.py
--rw-r--r--   0        0        0     2412 2022-12-09 18:24:40.522810 toolstr-0.9.2/toolstr/charts/char_dicts.py
--rw-r--r--   0        0        0     3763 2022-12-09 18:24:40.523072 toolstr-0.9.2/toolstr/charts/grid_utils.py
--rw-r--r--   0        0        0     2247 2022-12-09 18:24:40.523333 toolstr-0.9.2/toolstr/charts/line_utils.py
--rw-r--r--   0        0        0     3682 2022-12-12 20:14:13.660011 toolstr-0.9.2/toolstr/charts/plot_utils.py
--rw-r--r--   0        0        0     7038 2022-12-09 18:24:40.524040 toolstr-0.9.2/toolstr/charts/raster_utils.py
--rw-r--r--   0        0        0     8161 2022-12-12 20:13:58.305050 toolstr-0.9.2/toolstr/charts/render_utils.py
--rw-r--r--   0        0        0     2523 2022-12-09 18:24:40.524620 toolstr-0.9.2/toolstr/charts/sextant_utils.py
--rw-r--r--   0        0        0      186 2023-04-24 03:18:32.307974 toolstr-0.9.2/toolstr/formats/__init__.py
--rw-r--r--   0        0        0     1964 2022-12-09 18:24:40.525217 toolstr-0.9.2/toolstr/formats/bullet_formats.py
--rw-r--r--   0        0        0     1997 2022-12-09 18:24:40.525609 toolstr-0.9.2/toolstr/formats/column_formats.py
--rw-r--r--   0        0        0     7280 2023-03-27 19:55:46.509117 toolstr-0.9.2/toolstr/formats/datatype_formats.py
--rw-r--r--   0        0        0     3143 2022-12-12 07:53:13.190851 toolstr-0.9.2/toolstr/formats/positional_formats.py
--rw-r--r--   0        0        0     2191 2022-12-09 18:24:40.526344 toolstr-0.9.2/toolstr/formats/rich_formats.py
--rw-r--r--   0        0        0     3167 2023-04-24 06:16:05.352543 toolstr-0.9.2/toolstr/formats/template_formats.py
--rw-r--r--   0        0        0       61 2022-12-09 18:24:40.526678 toolstr-0.9.2/toolstr/outlines/__init__.py
--rw-r--r--   0        0        0     9083 2022-12-09 18:24:40.526924 toolstr-0.9.2/toolstr/outlines/outline_chars.py
--rw-r--r--   0        0        0     7033 2022-12-09 18:24:40.527200 toolstr-0.9.2/toolstr/outlines/outline_printing.py
--rw-r--r--   0        0        0        0 2022-12-09 18:24:40.527329 toolstr-0.9.2/toolstr/py.typed
--rw-r--r--   0        0        0     2402 2022-12-12 03:10:49.782218 toolstr-0.9.2/toolstr/spec.py
--rw-r--r--   0        0        0       28 2022-12-12 20:09:48.083313 toolstr-0.9.2/toolstr/summaries/__init__.py
--rw-r--r--   0        0        0     6158 2023-04-05 16:58:38.202042 toolstr-0.9.2/toolstr/summaries/set_summary.py
--rw-r--r--   0        0        0       89 2022-12-09 18:24:40.527921 toolstr-0.9.2/toolstr/tables/__init__.py
--rw-r--r--   0        0        0     5083 2022-12-09 18:24:40.528163 toolstr-0.9.2/toolstr/tables/multiline_tables.py
--rw-r--r--   0        0        0     2983 2023-04-24 06:16:44.834292 toolstr-0.9.2/toolstr/tables/table_adapters.py
--rw-r--r--   0        0        0    33607 2023-03-22 21:23:07.773603 toolstr-0.9.2/toolstr/tables/table_utils.py
--rw-r--r--   0        0        0     8721 1970-01-01 00:00:00.000000 toolstr-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0       80 2023-01-01 01:26:00.835967 toolstr-0.9.3/.gitignore
+-rw-r--r--   0        0        0     1084 2022-12-09 18:24:40.520680 toolstr-0.9.3/LICENSE
+-rw-r--r--   0        0        0     8107 2022-12-09 18:24:40.520919 toolstr-0.9.3/README.md
+-rw-r--r--   0        0        0      611 2022-12-12 20:01:41.098721 toolstr-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      245 2023-05-08 06:49:41.584123 toolstr-0.9.3/toolstr/__init__.py
+-rw-r--r--   0        0        0      475 2022-12-09 18:24:40.521992 toolstr-0.9.3/toolstr/charts/README.md
+-rw-r--r--   0        0        0      134 2022-12-09 18:24:40.522217 toolstr-0.9.3/toolstr/charts/__init__.py
+-rw-r--r--   0        0        0    12629 2022-12-09 18:24:40.522525 toolstr-0.9.3/toolstr/charts/braille_utils.py
+-rw-r--r--   0        0        0     2412 2022-12-09 18:24:40.522810 toolstr-0.9.3/toolstr/charts/char_dicts.py
+-rw-r--r--   0        0        0     3763 2022-12-09 18:24:40.523072 toolstr-0.9.3/toolstr/charts/grid_utils.py
+-rw-r--r--   0        0        0     2247 2022-12-09 18:24:40.523333 toolstr-0.9.3/toolstr/charts/line_utils.py
+-rw-r--r--   0        0        0     3682 2022-12-12 20:14:13.660011 toolstr-0.9.3/toolstr/charts/plot_utils.py
+-rw-r--r--   0        0        0     7038 2022-12-09 18:24:40.524040 toolstr-0.9.3/toolstr/charts/raster_utils.py
+-rw-r--r--   0        0        0     8161 2022-12-12 20:13:58.305050 toolstr-0.9.3/toolstr/charts/render_utils.py
+-rw-r--r--   0        0        0     2523 2022-12-09 18:24:40.524620 toolstr-0.9.3/toolstr/charts/sextant_utils.py
+-rw-r--r--   0        0        0      186 2023-04-24 03:18:32.307974 toolstr-0.9.3/toolstr/formats/__init__.py
+-rw-r--r--   0        0        0     1964 2022-12-09 18:24:40.525217 toolstr-0.9.3/toolstr/formats/bullet_formats.py
+-rw-r--r--   0        0        0     1997 2022-12-09 18:24:40.525609 toolstr-0.9.3/toolstr/formats/column_formats.py
+-rw-r--r--   0        0        0     7280 2023-03-27 19:55:46.509117 toolstr-0.9.3/toolstr/formats/datatype_formats.py
+-rw-r--r--   0        0        0     3143 2022-12-12 07:53:13.190851 toolstr-0.9.3/toolstr/formats/positional_formats.py
+-rw-r--r--   0        0        0     2191 2022-12-09 18:24:40.526344 toolstr-0.9.3/toolstr/formats/rich_formats.py
+-rw-r--r--   0        0        0     3167 2023-04-24 06:16:05.352543 toolstr-0.9.3/toolstr/formats/template_formats.py
+-rw-r--r--   0        0        0       61 2022-12-09 18:24:40.526678 toolstr-0.9.3/toolstr/outlines/__init__.py
+-rw-r--r--   0        0        0     9083 2022-12-09 18:24:40.526924 toolstr-0.9.3/toolstr/outlines/outline_chars.py
+-rw-r--r--   0        0        0     7358 2023-05-08 06:14:15.635867 toolstr-0.9.3/toolstr/outlines/outline_printing.py
+-rw-r--r--   0        0        0        0 2022-12-09 18:24:40.527329 toolstr-0.9.3/toolstr/py.typed
+-rw-r--r--   0        0        0     2402 2022-12-12 03:10:49.782218 toolstr-0.9.3/toolstr/spec.py
+-rw-r--r--   0        0        0       28 2022-12-12 20:09:48.083313 toolstr-0.9.3/toolstr/summaries/__init__.py
+-rw-r--r--   0        0        0     6158 2023-04-05 16:58:38.202042 toolstr-0.9.3/toolstr/summaries/set_summary.py
+-rw-r--r--   0        0        0       89 2022-12-09 18:24:40.527921 toolstr-0.9.3/toolstr/tables/__init__.py
+-rw-r--r--   0        0        0     5083 2022-12-09 18:24:40.528163 toolstr-0.9.3/toolstr/tables/multiline_tables.py
+-rw-r--r--   0        0        0     2983 2023-04-24 06:16:44.834292 toolstr-0.9.3/toolstr/tables/table_adapters.py
+-rw-r--r--   0        0        0    33607 2023-03-22 21:23:07.773603 toolstr-0.9.3/toolstr/tables/table_utils.py
+-rw-r--r--   0        0        0     8721 1970-01-01 00:00:00.000000 toolstr-0.9.3/PKG-INFO
```

### Comparing `toolstr-0.9.2/LICENSE` & `toolstr-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/README.md` & `toolstr-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/pyproject.toml` & `toolstr-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/toolstr/charts/braille_utils.py` & `toolstr-0.9.3/toolstr/charts/braille_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/toolstr/charts/char_dicts.py` & `toolstr-0.9.3/toolstr/charts/char_dicts.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/toolstr/charts/grid_utils.py` & `toolstr-0.9.3/toolstr/charts/grid_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/toolstr/charts/line_utils.py` & `toolstr-0.9.3/toolstr/charts/line_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/toolstr/charts/plot_utils.py` & `toolstr-0.9.3/toolstr/charts/plot_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/toolstr/charts/raster_utils.py` & `toolstr-0.9.3/toolstr/charts/raster_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/toolstr/charts/render_utils.py` & `toolstr-0.9.3/toolstr/charts/render_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/toolstr/charts/sextant_utils.py` & `toolstr-0.9.3/toolstr/charts/sextant_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/toolstr/formats/bullet_formats.py` & `toolstr-0.9.3/toolstr/formats/bullet_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/toolstr/formats/column_formats.py` & `toolstr-0.9.3/toolstr/formats/column_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/toolstr/formats/datatype_formats.py` & `toolstr-0.9.3/toolstr/formats/datatype_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/toolstr/formats/positional_formats.py` & `toolstr-0.9.3/toolstr/formats/positional_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/toolstr/formats/rich_formats.py` & `toolstr-0.9.3/toolstr/formats/rich_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/toolstr/formats/template_formats.py` & `toolstr-0.9.3/toolstr/formats/template_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/toolstr/outlines/outline_chars.py` & `toolstr-0.9.3/toolstr/outlines/outline_chars.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/toolstr/outlines/outline_printing.py` & `toolstr-0.9.3/toolstr/outlines/outline_printing.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     left_border: typing.Optional[bool] = None,
     right_border: typing.Optional[bool] = None,
     pad: typing.Optional[int] = None,
     upper_pad: typing.Optional[int] = None,
     lower_pad: typing.Optional[int] = None,
     left_pad: typing.Optional[int] = None,
     right_pad: typing.Optional[int] = None,
+    text_style: str | None = None,
     style: str | None = None,
     indent: str | int | None = None,
     **border_style: typing.Any,
 ) -> None:
 
     string = get_outlined_text(
         text=text,
@@ -64,14 +65,15 @@
         left_border=left_border,
         right_border=right_border,
         pad=pad,
         upper_pad=upper_pad,
         lower_pad=lower_pad,
         left_pad=left_pad,
         right_pad=right_pad,
+        text_style=text_style,
         style=style,
         **border_style,
     )
 
     if indent is not None:
         string = formats.indent_block(block=string, indent=indent)
 
@@ -83,14 +85,15 @@
     *,
     width: typing.Optional[int] = None,
     justify: typing.Optional[spec.HorizontalJustification] = None,
     upper_pad: int = 0,
     lower_pad: int = 0,
     left_pad: int = 1,
     right_pad: int = 1,
+    text_style: str | None = None,
     style: str | None = None,
     **border_style: typing.Any,
 ) -> None:
     print_outlined_text(
         text,
         width=width,
         justify=justify,
@@ -98,37 +101,40 @@
         lower_border=True,
         left_border=True,
         right_border=True,
         upper_pad=upper_pad,
         lower_pad=lower_pad,
         left_pad=left_pad,
         right_pad=right_pad,
+        text_style=text_style,
         style=style,
         **border_style,
     )
 
 
 def print_header(
     text: str,
     *,
     width: typing.Optional[int] = None,
     justify: typing.Optional[spec.HorizontalJustification] = None,
     pad: int = 0,
+    text_style: str | None = None,
     style: str | None = None,
     **border_style: typing.Any,
 ) -> None:
     print_outlined_text(
         text,
         width=width,
         justify=justify,
         pad=pad,
         upper_border=False,
         lower_border=True,
         left_border=False,
         right_border=False,
+        text_style=text_style,
         style=style,
         **border_style,
     )
 
 
 def get_outlined_text(
     text: str,
@@ -140,14 +146,15 @@
     left_border: typing.Optional[bool] = None,
     right_border: typing.Optional[bool] = None,
     pad: typing.Optional[int] = None,
     upper_pad: typing.Optional[int] = None,
     lower_pad: typing.Optional[int] = None,
     left_pad: typing.Optional[int] = None,
     right_pad: typing.Optional[int] = None,
+    text_style: str | None = None,
     style: str | None = None,
     **border_style: typing.Any,
 ) -> str:
 
     # set defaults
     if justify is None:
         justify = 'left'
@@ -239,14 +246,18 @@
             middle_left_prefix
             + left_pad_str
             + line
             + right_pad_str
             + middle_right_postfix
         )
         line = line.rstrip()
+
+        if text_style is not None:
+            line = formats.add_style(line, text_style)
+
         outlined += line + '\n'
 
     # add lower border
     if lower_border:
         outlined += (
             lower_left_prefix
             + (text_width + pad_width) * border_chars['horizontal']
```

### Comparing `toolstr-0.9.2/toolstr/spec.py` & `toolstr-0.9.3/toolstr/spec.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/toolstr/summaries/set_summary.py` & `toolstr-0.9.3/toolstr/summaries/set_summary.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/toolstr/tables/multiline_tables.py` & `toolstr-0.9.3/toolstr/tables/multiline_tables.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/toolstr/tables/table_adapters.py` & `toolstr-0.9.3/toolstr/tables/table_adapters.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/toolstr/tables/table_utils.py` & `toolstr-0.9.3/toolstr/tables/table_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.2/PKG-INFO` & `toolstr-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolstr
-Version: 0.9.2
+Version: 0.9.3
 Summary: toolstr is a suite of str processing tools, including formatting and drawing
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: tooltime>=0.1.4
 Requires-Dist: typing-extensions>=4.0.0
 Requires-Dist: scikit-image>=0.19.2 ; extra == "full"
 Requires-Dist: rich>=12.1.0 ; extra == "full"
```

