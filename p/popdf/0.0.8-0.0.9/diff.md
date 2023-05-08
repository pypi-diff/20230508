# Comparing `tmp/popdf-0.0.8.tar.gz` & `tmp/popdf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popdf-0.0.8.tar", last modified: Sun Apr  9 06:17:20 2023, max compression
+gzip compressed data, was "popdf-0.0.9.tar", last modified: Mon May  8 13:59:55 2023, max compression
```

## Comparing `popdf-0.0.8.tar` & `popdf-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 06:17:20.462427 popdf-0.0.8/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 popdf-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     5244 2023-04-09 06:17:20.463421 popdf-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4719 2023-04-02 05:09:27.000000 popdf-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 06:17:20.408811 popdf-0.0.8/popdf/
--rw-rw-rw-   0        0        0       29 2023-04-06 14:38:32.000000 popdf-0.0.8/popdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:17:20.434396 popdf-0.0.8/popdf/api/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 popdf-0.0.8/popdf/api/__init__.py
--rw-rw-rw-   0        0        0     1663 2023-04-09 06:14:30.000000 popdf-0.0.8/popdf/api/pdf.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:17:20.438389 popdf-0.0.8/popdf/core/
--rw-rw-rw-   0        0        0     8595 2023-04-09 06:14:30.000000 popdf-0.0.8/popdf/core/PDFType.py
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 popdf-0.0.8/popdf/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:17:20.439392 popdf-0.0.8/popdf/lib/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 popdf-0.0.8/popdf/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:17:20.449908 popdf-0.0.8/popdf/lib/pdf/
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 popdf-0.0.8/popdf/lib/pdf/__init__.py
--rw-rw-rw-   0        0        0     2111 2023-03-24 15:13:04.000000 popdf-0.0.8/popdf/lib/pdf/add_watermark_service.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:17:20.431384 popdf-0.0.8/popdf.egg-info/
--rw-rw-rw-   0        0        0     5244 2023-04-09 06:17:20.000000 popdf-0.0.8/popdf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-04-09 06:17:20.000000 popdf-0.0.8/popdf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 06:17:20.000000 popdf-0.0.8/popdf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-09 06:17:20.000000 popdf-0.0.8/popdf.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       70 2023-04-09 06:17:20.000000 popdf-0.0.8/popdf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-09 06:17:20.000000 popdf-0.0.8/popdf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      776 2023-04-09 06:17:20.465949 popdf-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 popdf-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:17:20.461420 popdf-0.0.8/tests/
--rw-rw-rw-   0        0        0      181 2022-09-17 08:11:22.000000 popdf-0.0.8/tests/__init__.py
--rw-rw-rw-   0        0        0     2089 2023-04-03 15:21:41.000000 popdf-0.0.8/tests/test_pdf.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:59:55.688208 popdf-0.0.9/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 popdf-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5244 2023-05-08 13:59:55.689205 popdf-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4719 2023-04-02 05:09:27.000000 popdf-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 13:59:55.647428 popdf-0.0.9/popdf/
+-rw-rw-rw-   0        0        0       29 2023-04-06 14:38:32.000000 popdf-0.0.9/popdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:59:55.672552 popdf-0.0.9/popdf/api/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 popdf-0.0.9/popdf/api/__init__.py
+-rw-rw-rw-   0        0        0     1692 2023-05-08 13:54:55.000000 popdf-0.0.9/popdf/api/pdf.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:59:55.677079 popdf-0.0.9/popdf/core/
+-rw-rw-rw-   0        0        0     8947 2023-05-08 13:58:47.000000 popdf-0.0.9/popdf/core/PDFType.py
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 popdf-0.0.9/popdf/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:59:55.679078 popdf-0.0.9/popdf/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 popdf-0.0.9/popdf/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:59:55.684077 popdf-0.0.9/popdf/lib/pdf/
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 popdf-0.0.9/popdf/lib/pdf/__init__.py
+-rw-rw-rw-   0        0        0     2111 2023-03-24 15:13:04.000000 popdf-0.0.9/popdf/lib/pdf/add_watermark_service.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:59:55.668548 popdf-0.0.9/popdf.egg-info/
+-rw-rw-rw-   0        0        0     5244 2023-05-08 13:59:55.000000 popdf-0.0.9/popdf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-05-08 13:59:55.000000 popdf-0.0.9/popdf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 13:59:55.000000 popdf-0.0.9/popdf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-08 13:48:46.000000 popdf-0.0.9/popdf.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       70 2023-05-08 13:59:55.000000 popdf-0.0.9/popdf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-08 13:59:55.000000 popdf-0.0.9/popdf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      776 2023-05-08 13:59:55.691209 popdf-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 popdf-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:59:55.687209 popdf-0.0.9/tests/
+-rw-rw-rw-   0        0        0      181 2022-09-17 08:11:22.000000 popdf-0.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0     2089 2023-04-03 15:21:41.000000 popdf-0.0.9/tests/test_pdf.py
```

### Comparing `popdf-0.0.8/LICENSE` & `popdf-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `popdf-0.0.8/PKG-INFO` & `popdf-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popdf
-Version: 0.0.8
+Version: 0.0.9
 Summary: pip install popdf
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/popdf/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/popdf/blob/master/README.md
```

### Comparing `popdf-0.0.8/README.md` & `popdf-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `popdf-0.0.8/popdf/api/pdf.py` & `popdf-0.0.9/popdf/api/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     output_file_name：指定添加了水印的文件名称，可以不指定，默认是：添加了水印的文件.pdf
     """
     mainPDF.add_watermark_by_parameters(pdf_file, mark_str, output_path, output_file_name)
 
 
 # txt转pdf
 # @except_dec()
-def txt2pdf(path: str, res_pdf='txt2pdf.pdf'):
-    mainPDF.file2pdf(path, res_pdf)
+def txt2pdf(path: str, res_pdf='txt2pdf.pdf',output_path=r'./'):
+    mainPDF.txt2pdf(path, res_pdf,output_path)
 
 
 # PDF加密
 # @except_dec()
 def encrypt4pdf(path, password, output_path):
     mainPDF.encrypt4pdf(path, password, output_path)
```

### Comparing `popdf-0.0.8/popdf/core/PDFType.py` & `popdf-0.0.9/popdf/core/PDFType.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 '''
 @Author  ：B站/抖音/微博/小红书/公众号，都叫：程序员晚枫
 @WeChat     ：CoderWanFeng
 @Blog      ：www.python-office.com
 @Date    ：2023/4/3 23:05
 @Description     ：
 '''
+import os
+from pathlib import Path
 
-from fpdf import FPDF
+import fitz  # fitz就是pip install PyMuPDF
 import pikepdf
 from PyPDF2 import PdfReader, PdfWriter  # PdfFileReader, PdfFileWriter,
+from fpdf import FPDF
 from pdf2docx import Converter
-import os
-from pathlib import Path
-import fitz  # fitz就是pip install PyMuPDF
-from pofile import get_files
+from pofile import get_files, mkdir
 from poprogress import simple_progress
 
 from popdf.lib.pdf import add_watermark_service
 
 
 class MainPDF():
 
@@ -52,25 +52,31 @@
             _out_pdf_file = Path(_input_pdf_file.parent).absolute() / output_file_name  # '添加了水印的文件.pdf'
 
         _temp_pdf = _input_pdf_file.parent / '32012356985422-watermark.pdf'  # 水印文件
         add_watermark_service.create_watermark(_temp_pdf, str(mark_str))  # 水印文件
         add_watermark_service.pdf_add_watermark(_input_pdf_file, _temp_pdf, _out_pdf_file)
         print(f"水印添加结束，请打开电脑上的这个位置，查看结果文件：{_out_pdf_file}")
 
-    def file2pdf(self, file_type, path, res_pdf='file2pdf.pdf'):
-        if file_type == 'txt':
+    def txt2pdf(self, path, res_pdf='file2pdf.pdf', output_path=r'./'):
+        abs_path = Path(path).absolute()
+        suffix = '.txt'
+        txt_list = get_files(path=str(abs_path), suffix=suffix)
+        exsit, abs_output_path = mkdir(output_path)
+        for index, txt in simple_progress(enumerate(txt_list)):
             pdf = FPDF()
             pdf.add_page()  # Add a page
             pdf.set_font("Arial", size=15)  # set style and size of font
-            f = open(path, "r")  # open the text file in read mode
+            file_content = open(txt, "r")  # open the text file in read mode
             # insert the texts in pdf
-            for x in f:
-                pdf.cell(50, 5, txt=x, ln=1, align='C')
-            # pdf.output("path where you want to store pdf file\\file_name.pdf")
-            pdf.output(res_pdf)
+            for content in file_content:
+                pdf.cell(50, 5, txt=content, ln=1, align='C')
+            if index==0:
+                pdf.output(os.path.join(abs_output_path, res_pdf))
+            else:
+                pdf.output(os.path.join(abs_output_path, f'{str(index)} - {res_pdf}'))
 
     def pdf2docx(self, file_path, output_path):
         word_name = os.path.basename(file_path)[:-4] + '.docx'
         word_path = Path(output_path) / word_name
         cv = Converter(file_path)
         cv.convert(word_path)
         cv.close()
@@ -138,15 +144,15 @@
 
     #         if not os.path.exists(out_dir):  # 判断存放图片的文件夹是否存在
     #             os.makedirs(out_dir)  # 若图片文件夹不存在就创建
 
     #         pix.writePNG(out_dir + '/' + 'images_%s.png' % pg)  # 将图片写入指定的文件夹内
     #     print(f'PDF转换Image完成，图片在你指定的output文件夹{out_dir}，如果没有指定，默认是PDF同一个文件夹')
 
-    def pdf2imgs(self, pdf_path: str, out_dir=".") -> None:
+    def pdf2imgs(self, pdf_path: str, out_dir="./") -> None:
         pdf_file_list = get_files(pdf_path, suffix='.pdf')
         print('PDF开始转换，你可以加入交流群唠唠嗑：http://www.python4office.cn/wechat-group/')
         for pdf_file in simple_progress(pdf_file_list):
             pdfDoc = fitz.open(pdf_file)
             if pdfDoc.page_count > 50:
                 print('少年，你的PDF页数有点多哟，请耐心等待~')
             for pg in simple_progress(range(pdfDoc.page_count)):
```

### Comparing `popdf-0.0.8/popdf/lib/pdf/add_watermark_service.py` & `popdf-0.0.9/popdf/lib/pdf/add_watermark_service.py`

 * *Files identical despite different names*

### Comparing `popdf-0.0.8/popdf.egg-info/PKG-INFO` & `popdf-0.0.9/popdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popdf
-Version: 0.0.8
+Version: 0.0.9
 Summary: pip install popdf
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/popdf/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/popdf/blob/master/README.md
```

### Comparing `popdf-0.0.8/setup.cfg` & `popdf-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f70 6466 0d0a 7665 7273 696f   = popdf..versio
-00000020: 6e20 3d20 302e 302e 380d 0a64 6573 6372  n = 0.0.8..descr
+00000020: 6e20 3d20 302e 302e 390d 0a64 6573 6372  n = 0.0.9..descr
 00000030: 6970 7469 6f6e 203d 2070 6970 2069 6e73  iption = pip ins
 00000040: 7461 6c6c 2070 6f70 6466 0d0a 6c6f 6e67  tall popdf..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
```

### Comparing `popdf-0.0.8/tests/test_pdf.py` & `popdf-0.0.9/tests/test_pdf.py`

 * *Files identical despite different names*

