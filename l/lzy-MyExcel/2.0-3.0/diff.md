# Comparing `tmp/lzy-MyExcel-2.0.tar.gz` & `tmp/lzy-MyExcel-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\lzy-MyExcel-2.0.tar", last modified: Wed Mar 23 06:50:31 2022, max compression
+gzip compressed data, was "lzy-MyExcel-3.0.tar", last modified: Mon May  8 00:08:47 2023, max compression
```

## Comparing `lzy-MyExcel-2.0.tar` & `lzy-MyExcel-3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2022-03-23 06:50:31.000000 lzy-MyExcel-2.0/
--rw-rw-rw-   0        0        0     3433 2022-03-23 06:45:27.000000 lzy-MyExcel-2.0/MyExcel.py
--rw-rw-rw-   0        0        0      197 2022-03-23 06:50:31.000000 lzy-MyExcel-2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-03-23 06:50:31.000000 lzy-MyExcel-2.0/lzy_MyExcel.egg-info/
--rw-rw-rw-   0        0        0      197 2022-03-23 06:50:31.000000 lzy-MyExcel-2.0/lzy_MyExcel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2022-03-23 06:50:31.000000 lzy-MyExcel-2.0/lzy_MyExcel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-23 06:50:31.000000 lzy-MyExcel-2.0/lzy_MyExcel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-03-23 06:50:31.000000 lzy-MyExcel-2.0/lzy_MyExcel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-03-23 06:50:31.000000 lzy-MyExcel-2.0/setup.cfg
--rw-rw-rw-   0        0        0      203 2022-03-23 06:50:14.000000 lzy-MyExcel-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 00:08:47.705675 lzy-MyExcel-3.0/
+-rw-rw-rw-   0        0        0     3522 2023-05-08 00:03:15.000000 lzy-MyExcel-3.0/MyExcel.py
+-rw-rw-rw-   0        0        0       83 2023-05-08 00:08:47.704678 lzy-MyExcel-3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-08 00:08:47.703681 lzy-MyExcel-3.0/lzy_MyExcel.egg-info/
+-rw-rw-rw-   0        0        0       83 2023-05-08 00:08:47.000000 lzy-MyExcel-3.0/lzy_MyExcel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-05-08 00:08:47.000000 lzy-MyExcel-3.0/lzy_MyExcel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 00:08:47.000000 lzy-MyExcel-3.0/lzy_MyExcel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-08 00:08:47.000000 lzy-MyExcel-3.0/lzy_MyExcel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 00:08:47.705675 lzy-MyExcel-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      209 2023-05-08 00:06:49.000000 lzy-MyExcel-3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lzy-MyExcel-2.0/MyExcel.py` & `lzy-MyExcel-3.0/MyExcel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 import re
+
 import openpyxl
-from openpyxl.utils import get_column_letter
 from openpyxl.utils import column_index_from_string
+from openpyxl.utils import get_column_letter
 
 
 class MyExcel:
     def __init__(self, **kwargs):
         self.filepath = kwargs.get('filepath')
         self.workbook = openpyxl.load_workbook(filename=self.filepath, data_only=kwargs.get('data_only'))
 
-    def read_sheet(self, **kwargs):
+    def read_sheet(self, close=True, **kwargs):
         if kwargs.get('sheet_name'):
             self.active_sheet = self.workbook[kwargs.get('sheet_name')]
         else:
             self.active_sheet = self.workbook.active
         coordinate = kwargs.get('coordinate')
         start_column = int(column_index_from_string(re.findall(r'([a-z]+)\d+:([a-z]+)\d+', coordinate, re.I)[0][0]))
         end_column = int(column_index_from_string(re.findall(r'([a-z]+)\d+:([a-z]+)\d+', coordinate, re.I)[0][1]))
         start_row = int(re.findall(r'[a-z]+(\d+):[a-z]+(\d+)', coordinate, re.I)[0][0])
         end_row = int(re.findall(r'[a-z]+(\d+):[a-z]+(\d+)', coordinate, re.I)[0][1])
         value_list = []
         if kwargs.get('iter').lower() == 'row':
             for row_cell in self.active_sheet.iter_rows(min_row=start_row, max_row=end_row, min_col=start_column,
                                                         max_col=end_column):
-                if kwargs.get('value')== True:
+                if kwargs.get('value') == True:
                     value_list.append([cell.value for cell in row_cell])
                 else:
                     value_list.append([cell for cell in row_cell])
         elif kwargs.get('iter').lower() == 'column':
             for column_cell in self.active_sheet.iter_cols(min_row=start_row, max_row=end_row, min_col=start_column,
                                                            max_col=end_column):
-                if kwargs.get('value')== True:
-                    value_list.append([cell.value for cell in  column_cell])
+                if kwargs.get('value') == True:
+                    value_list.append([cell.value for cell in column_cell])
                 else:
                     value_list.append([cell for cell in column_cell])
-        self.workbook.close()
+        if close:
+            self.workbook.close()
         return value_list
 
-    def write_sheet(self, **kwargs):
+    def write_sheet(self, save_close=True, **kwargs):
         if kwargs.get('sheet_name'):
             self.active_sheet = self.workbook[kwargs.get('sheet_name')]
         else:
             self.active_sheet = self.workbook.active
         coordinate = kwargs.get('coordinate')
         start_column = int(column_index_from_string(re.findall(r'([a-z]+)', coordinate, re.I)[0]))
         start_row = int(re.findall(r'(\d+)', coordinate, re.I)[0])
         for row in range(len(kwargs.get('list'))):
             for column in range(len(kwargs.get('list')[row])):
                 self.active_sheet.cell(row + start_row, column + start_column).value = kwargs.get('list')[row][column]
-        self.workbook.save(self.filepath)
-        self.workbook.close()
+        if save_close:
+            self.workbook.save(self.filepath)
+            self.workbook.close()
 
     def max_row_or_column(self, **kwargs):
         if kwargs.get('sheet_name'):
             self.active_sheet = self.workbook[kwargs.get('sheet_name')]
         else:
             self.active_sheet = self.workbook.active
         if kwargs.get('value'):
             if kwargs.get('value').isdigit():
                 return max((bb.column for bb in self.active_sheet[kwargs.get('value')] if bb.value))
             elif kwargs.get('value').isalpha():
                 return max((bb.row for bb in self.active_sheet[kwargs.get('value')] if bb.value))
         else:
-            return get_column_letter(self.active_sheet.max_column), self.active_sheet.max_row
+            return get_column_letter(self.active_sheet.max_column), self.active_sheet.max_row
```

