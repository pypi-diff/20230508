# Comparing `tmp/robotframework_difflibext-0.0.4-py3-none-any.whl.zip` & `tmp/robotframework_difflibext-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3682 bytes, number of entries: 8
+Zip file size: 3719 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       72 b- defN 23-Feb-24 06:44 DiffLibExt/__init__.py
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-24 09:20 DiffLibExt/__version__.py
--rw-r--r--  2.0 unx     2750 b- defN 23-Apr-24 09:20 DiffLibExt/difflibext.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Apr-24 09:21 robotframework_difflibext-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      490 b- defN 23-Apr-24 09:21 robotframework_difflibext-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 09:21 robotframework_difflibext-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-24 09:21 robotframework_difflibext-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      713 b- defN 23-Apr-24 09:21 robotframework_difflibext-0.0.4.dist-info/RECORD
-8 files, 5215 bytes uncompressed, 2412 bytes compressed:  53.7%
+-rw-r--r--  2.0 unx       22 b- defN 23-May-08 05:46 DiffLibExt/__version__.py
+-rw-r--r--  2.0 unx     2848 b- defN 23-May-08 05:41 DiffLibExt/difflibext.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-May-08 05:47 robotframework_difflibext-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      490 b- defN 23-May-08 05:47 robotframework_difflibext-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-08 05:47 robotframework_difflibext-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-08 05:47 robotframework_difflibext-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      713 b- defN 23-May-08 05:47 robotframework_difflibext-0.0.5.dist-info/RECORD
+8 files, 5313 bytes uncompressed, 2449 bytes compressed:  53.9%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: DiffLibExt/__version__.py
 Comment: 
 
 Filename: DiffLibExt/difflibext.py
 Comment: 
 
-Filename: robotframework_difflibext-0.0.4.dist-info/LICENSE
+Filename: robotframework_difflibext-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: robotframework_difflibext-0.0.4.dist-info/METADATA
+Filename: robotframework_difflibext-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: robotframework_difflibext-0.0.4.dist-info/WHEEL
+Filename: robotframework_difflibext-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: robotframework_difflibext-0.0.4.dist-info/top_level.txt
+Filename: robotframework_difflibext-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: robotframework_difflibext-0.0.4.dist-info/RECORD
+Filename: robotframework_difflibext-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## DiffLibExt/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.4"
+__version__ = "0.0.5"
```

## DiffLibExt/difflibext.py

```diff
@@ -9,15 +9,16 @@
 
 
 class DiffLibExt:
     ROBOT_LIBRARY_SCOPE = "GLOBAL"
     ROBOT_LIBRARY_DOC_FORMAT = "ROBOT"
     DIFF_OUT_DIR_NAME = "__diff__"
 
-    def __init__(self):
+    def __init__(self, line_wrap_len: int = 100):
+        self.line_wrap_len = line_wrap_len
         self._builtin_lib = BuiltIn()
 
     @keyword
     def file_should_be_equal(self, expected_file_path: str, actual_file_path: str):
         try:
             expected_file_text = Path(expected_file_path).read_text(encoding="utf8")
         except UnicodeDecodeError as e:
@@ -28,15 +29,15 @@
         except UnicodeDecodeError as e:
             raise AssertionError(f"{actual_file_path} is not a text file.") from e
 
         if expected_file_text != actual_file_text:
             self._report_diff(expected_file_text, actual_file_text)
 
     def _report_diff(self, expected_text: str, actual_text: str):
-        html_diff = difflib.HtmlDiff().make_file(
+        html_diff = difflib.HtmlDiff(wrapcolumn=self.line_wrap_len).make_file(
             expected_text.splitlines(),
             actual_text.splitlines(),
             fromdesc="Expected:",
             todesc="Actual:",
         )
         output_dir = self._builtin_lib.get_variable_value("${OUTPUT DIR}")
         pabot_out_regex = r".*(\\|\/)(pabot_results(\\|\/)\d+$)"
```

## Comparing `robotframework_difflibext-0.0.4.dist-info/LICENSE` & `robotframework_difflibext-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `robotframework_difflibext-0.0.4.dist-info/RECORD` & `robotframework_difflibext-0.0.5.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 DiffLibExt/__init__.py,sha256=Va4HbB9lNClbBulDlHRJLIo1MAtctg0-Q-UBMwWBboI,72
-DiffLibExt/__version__.py,sha256=1mptEzQihbdyqqzMgdns_j5ZGK9gz7hR2bsgA_TnjO4,22
-DiffLibExt/difflibext.py,sha256=7LWXItNdRZH9BAfYKYogOgWp5xTZ-oSeIuVIBLKK-ew,2750
-robotframework_difflibext-0.0.4.dist-info/LICENSE,sha256=iTbHssklwr0rKR85nlkPEww1zlvDV8fgwEkTQofHia8,1065
-robotframework_difflibext-0.0.4.dist-info/METADATA,sha256=OrFMFSGz1M8mDhuO2J4B00dLDJAbgiLFp_vz2zBkyf8,490
-robotframework_difflibext-0.0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-robotframework_difflibext-0.0.4.dist-info/top_level.txt,sha256=Wm28sfRPl6iPErXg5G9BD_qFLpkvlN6Cqbuv2weQp18,11
-robotframework_difflibext-0.0.4.dist-info/RECORD,,
+DiffLibExt/__version__.py,sha256=S7u1lbuWmM3A3ajykBialmPoJUK6Jg-WmNqM-9OZFdk,22
+DiffLibExt/difflibext.py,sha256=wejNntOFcpezx9zXLdmk6gwywJJKncojMbiMiEU0u0U,2848
+robotframework_difflibext-0.0.5.dist-info/LICENSE,sha256=iTbHssklwr0rKR85nlkPEww1zlvDV8fgwEkTQofHia8,1065
+robotframework_difflibext-0.0.5.dist-info/METADATA,sha256=G_xWgmh0SmQ4t-SuRaOZGANmf05liHlyMjPYlx80QYg,490
+robotframework_difflibext-0.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+robotframework_difflibext-0.0.5.dist-info/top_level.txt,sha256=Wm28sfRPl6iPErXg5G9BD_qFLpkvlN6Cqbuv2weQp18,11
+robotframework_difflibext-0.0.5.dist-info/RECORD,,
```

