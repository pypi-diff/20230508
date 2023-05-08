# Comparing `tmp/python-office-0.3.8.tar.gz` & `tmp/python-office-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-office-0.3.8.tar", last modified: Sun Apr  9 06:16:37 2023, max compression
+gzip compressed data, was "python-office-0.3.9.tar", last modified: Sun Apr  9 06:59:59 2023, max compression
```

## Comparing `python-office-0.3.8.tar` & `python-office-0.3.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 06:16:37.031092 python-office-0.3.8/
--rw-rw-rw-   0        0        0    11558 2023-04-05 07:52:22.000000 python-office-0.3.8/LICENSE
--rw-rw-rw-   0        0        0    10590 2023-04-09 06:16:37.032112 python-office-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0    10005 2023-04-05 07:52:22.000000 python-office-0.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 06:16:36.821881 python-office-0.3.8/office/
--rw-rw-rw-   0        0        0      883 2023-04-05 07:52:22.000000 python-office-0.3.8/office/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:16:36.873497 python-office-0.3.8/office/api/
--rw-rw-rw-   0        0        0       17 2023-04-05 07:52:22.000000 python-office-0.3.8/office/api/__init__.py
--rw-rw-rw-   0        0        0      277 2023-04-05 07:52:22.000000 python-office-0.3.8/office/api/email.py
--rw-rw-rw-   0        0        0     2145 2023-04-05 07:52:22.000000 python-office-0.3.8/office/api/excel.py
--rw-rw-rw-   0        0        0     2658 2023-04-08 15:34:44.000000 python-office-0.3.8/office/api/file.py
--rw-rw-rw-   0        0        0     1978 2023-04-05 07:52:22.000000 python-office-0.3.8/office/api/image.py
--rw-rw-rw-   0        0        0      465 2023-04-05 07:52:22.000000 python-office-0.3.8/office/api/markdown.py
--rw-rw-rw-   0        0        0      271 2023-04-05 07:52:22.000000 python-office-0.3.8/office/api/ocr.py
--rw-rw-rw-   0        0        0     1828 2023-04-09 06:14:30.000000 python-office-0.3.8/office/api/pdf.py
--rw-rw-rw-   0        0        0      729 2023-04-05 07:52:22.000000 python-office-0.3.8/office/api/ppt.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:16:36.878012 python-office-0.3.8/office/api/testApi/
--rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.8/office/api/testApi/__init__.py
--rw-rw-rw-   0        0        0      508 2023-04-05 07:52:22.000000 python-office-0.3.8/office/api/testApi/ruiming.py
--rw-rw-rw-   0        0        0     1135 2023-04-05 07:52:22.000000 python-office-0.3.8/office/api/tools.py
--rw-rw-rw-   0        0        0      523 2023-04-05 07:52:22.000000 python-office-0.3.8/office/api/video.py
--rw-rw-rw-   0        0        0      289 2023-04-05 07:52:22.000000 python-office-0.3.8/office/api/web.py
--rw-rw-rw-   0        0        0      737 2023-04-05 07:52:22.000000 python-office-0.3.8/office/api/wechat.py
--rw-rw-rw-   0        0        0     1224 2023-04-05 07:52:22.000000 python-office-0.3.8/office/api/word.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:16:36.882018 python-office-0.3.8/office/cli/
--rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.8/office/cli/__init__.py
--rw-rw-rw-   0        0        0     3956 2023-04-05 07:52:22.000000 python-office-0.3.8/office/cli/main.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:16:36.884019 python-office-0.3.8/office/core/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:16:36.889722 python-office-0.3.8/office/core/TestTypes/
--rw-rw-rw-   0        0        0     4262 2023-04-05 07:52:22.000000 python-office-0.3.8/office/core/TestTypes/RuimingType.py
--rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.8/office/core/TestTypes/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.8/office/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:16:36.892714 python-office-0.3.8/office/lib/
--rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:16:36.897218 python-office-0.3.8/office/lib/conf/
--rw-rw-rw-   0        0        0       19 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/conf/CONST.py
--rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/conf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:16:36.903510 python-office-0.3.8/office/lib/decorator_utils/
--rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/decorator_utils/__init__.py
--rw-rw-rw-   0        0        0     6250 2023-04-08 15:27:05.000000 python-office-0.3.8/office/lib/decorator_utils/instruction_url.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:16:36.908011 python-office-0.3.8/office/lib/excel/
--rw-rw-rw-   0        0        0     3890 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/excel/SplitExcel.py
--rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/excel/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:16:36.914059 python-office-0.3.8/office/lib/image/
--rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/image/__init__.py
--rw-rw-rw-   0        0        0     2822 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/image/add_watermark_service.py
--rw-rw-rw-   0        0        0     2237 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/image/eliminate_background.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:16:36.918591 python-office-0.3.8/office/lib/pdf/
--rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/pdf/__init__.py
--rw-rw-rw-   0        0        0     1970 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/pdf/add_watermark_service.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:16:36.924128 python-office-0.3.8/office/lib/ppt/
--rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/ppt/__init__.py
--rw-rw-rw-   0        0        0     1140 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/ppt/ppt2pdf_service.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:16:36.948744 python-office-0.3.8/office/lib/tools/
--rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/tools/__init__.py
--rw-rw-rw-   0        0        0     1128 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/tools/lottery8ticket.py
--rw-rw-rw-   0        0        0     7247 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/tools/pwd4wifi_service.py
--rw-rw-rw-   0        0        0    14160 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/tools/qoute_dict_create_article.py
--rw-rw-rw-   0        0        0    77907 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/tools/weather_city_code.py
--rw-rw-rw-   0        0        0     1004 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/tools/weather_service.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:16:36.962305 python-office-0.3.8/office/lib/utils/
--rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/utils/__init__.py
--rw-rw-rw-   0        0        0     1062 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/utils/except_utils.py
--rw-rw-rw-   0        0        0     1472 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/utils/pandas_mem.py
--rw-rw-rw-   0        0        0      272 2023-04-05 07:52:22.000000 python-office-0.3.8/office/lib/utils/time_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:16:36.990942 python-office-0.3.8/python_office.egg-info/
--rw-rw-rw-   0        0        0    10590 2023-04-09 06:16:36.000000 python-office-0.3.8/python_office.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2021 2023-04-09 06:16:36.000000 python-office-0.3.8/python_office.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 06:16:36.000000 python-office-0.3.8/python_office.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-08 15:28:20.000000 python-office-0.3.8/python_office.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      116 2023-04-09 06:16:36.000000 python-office-0.3.8/python_office.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-09 06:16:36.000000 python-office-0.3.8/python_office.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      894 2023-04-09 06:16:37.034107 python-office-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0      428 2023-04-05 07:52:22.000000 python-office-0.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:16:36.995455 python-office-0.3.8/tests/
--rw-rw-rw-   0        0        0      379 2023-04-05 07:52:22.000000 python-office-0.3.8/tests/__init__.py
--rw-rw-rw-   0        0        0      460 2023-04-05 07:52:23.000000 python-office-0.3.8/tests/test_main.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:16:37.029577 python-office-0.3.8/tests/test_unit/
--rw-rw-rw-   0        0        0        0 2023-04-05 07:52:23.000000 python-office-0.3.8/tests/test_unit/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-05 07:52:23.000000 python-office-0.3.8/tests/test_unit/test_dev.py
--rw-rw-rw-   0        0        0     2168 2023-04-05 07:52:23.000000 python-office-0.3.8/tests/test_unit/test_excel.py
--rw-rw-rw-   0        0        0     1271 2023-04-08 15:28:39.000000 python-office-0.3.8/tests/test_unit/test_file.py
--rw-rw-rw-   0        0        0      782 2023-04-05 07:52:23.000000 python-office-0.3.8/tests/test_unit/test_image.py
--rw-rw-rw-   0        0        0      684 2023-04-05 07:52:23.000000 python-office-0.3.8/tests/test_unit/test_markdown.py
--rw-rw-rw-   0        0        0     2032 2023-04-05 07:52:23.000000 python-office-0.3.8/tests/test_unit/test_pdf.py
--rw-rw-rw-   0        0        0      355 2023-04-05 07:52:23.000000 python-office-0.3.8/tests/test_unit/test_ppt.py
--rw-rw-rw-   0        0        0      946 2023-04-05 07:52:23.000000 python-office-0.3.8/tests/test_unit/test_ruiming.py
--rw-rw-rw-   0        0        0      193 2023-04-05 07:52:23.000000 python-office-0.3.8/tests/test_unit/test_search_by_content.py
--rw-rw-rw-   0        0        0      824 2023-04-05 07:52:23.000000 python-office-0.3.8/tests/test_unit/test_tools.py
--rw-rw-rw-   0        0        0        0 2023-04-05 07:52:23.000000 python-office-0.3.8/tests/test_unit/test_video.py
--rw-rw-rw-   0        0        0      295 2023-04-05 07:52:23.000000 python-office-0.3.8/tests/test_unit/test_wechat.py
--rw-rw-rw-   0        0        0      232 2023-04-05 07:52:23.000000 python-office-0.3.8/tests/test_unit/test_word.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:59.258170 python-office-0.3.9/
+-rw-rw-rw-   0        0        0    11558 2023-04-05 07:52:22.000000 python-office-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0    10590 2023-04-09 06:59:59.259171 python-office-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0    10005 2023-04-05 07:52:22.000000 python-office-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:59.099333 python-office-0.3.9/office/
+-rw-rw-rw-   0        0        0      926 2023-04-09 06:35:53.000000 python-office-0.3.9/office/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:59.126381 python-office-0.3.9/office/api/
+-rw-rw-rw-   0        0        0       17 2023-04-05 07:52:22.000000 python-office-0.3.9/office/api/__init__.py
+-rw-rw-rw-   0        0        0      277 2023-04-05 07:52:22.000000 python-office-0.3.9/office/api/email.py
+-rw-rw-rw-   0        0        0     2145 2023-04-05 07:52:22.000000 python-office-0.3.9/office/api/excel.py
+-rw-rw-rw-   0        0        0     2658 2023-04-08 15:34:44.000000 python-office-0.3.9/office/api/file.py
+-rw-rw-rw-   0        0        0     1978 2023-04-05 07:52:22.000000 python-office-0.3.9/office/api/image.py
+-rw-rw-rw-   0        0        0      465 2023-04-05 07:52:22.000000 python-office-0.3.9/office/api/markdown.py
+-rw-rw-rw-   0        0        0      271 2023-04-05 07:52:22.000000 python-office-0.3.9/office/api/ocr.py
+-rw-rw-rw-   0        0        0     1828 2023-04-09 06:14:30.000000 python-office-0.3.9/office/api/pdf.py
+-rw-rw-rw-   0        0        0      729 2023-04-05 07:52:22.000000 python-office-0.3.9/office/api/ppt.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:59.130896 python-office-0.3.9/office/api/testApi/
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.9/office/api/testApi/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-04-05 07:52:22.000000 python-office-0.3.9/office/api/testApi/ruiming.py
+-rw-rw-rw-   0        0        0     1135 2023-04-05 07:52:22.000000 python-office-0.3.9/office/api/tools.py
+-rw-rw-rw-   0        0        0      523 2023-04-05 07:52:22.000000 python-office-0.3.9/office/api/video.py
+-rw-rw-rw-   0        0        0      289 2023-04-05 07:52:22.000000 python-office-0.3.9/office/api/web.py
+-rw-rw-rw-   0        0        0      737 2023-04-05 07:52:22.000000 python-office-0.3.9/office/api/wechat.py
+-rw-rw-rw-   0        0        0     1224 2023-04-05 07:52:22.000000 python-office-0.3.9/office/api/word.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:59.134897 python-office-0.3.9/office/cli/
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.9/office/cli/__init__.py
+-rw-rw-rw-   0        0        0     3956 2023-04-05 07:52:22.000000 python-office-0.3.9/office/cli/main.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:59.137907 python-office-0.3.9/office/core/
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:59.141437 python-office-0.3.9/office/core/TestTypes/
+-rw-rw-rw-   0        0        0     4262 2023-04-05 07:52:22.000000 python-office-0.3.9/office/core/TestTypes/RuimingType.py
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.9/office/core/TestTypes/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.9/office/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:59.143441 python-office-0.3.9/office/lib/
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:59.148440 python-office-0.3.9/office/lib/conf/
+-rw-rw-rw-   0        0        0       19 2023-04-09 06:35:08.000000 python-office-0.3.9/office/lib/conf/CONST.py
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/conf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:59.154637 python-office-0.3.9/office/lib/decorator_utils/
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/decorator_utils/__init__.py
+-rw-rw-rw-   0        0        0     6250 2023-04-08 15:27:05.000000 python-office-0.3.9/office/lib/decorator_utils/instruction_url.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:59.158640 python-office-0.3.9/office/lib/excel/
+-rw-rw-rw-   0        0        0     3890 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/excel/SplitExcel.py
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/excel/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:59.167166 python-office-0.3.9/office/lib/image/
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/image/__init__.py
+-rw-rw-rw-   0        0        0     2822 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/image/add_watermark_service.py
+-rw-rw-rw-   0        0        0     2237 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/image/eliminate_background.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:59.171702 python-office-0.3.9/office/lib/pdf/
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/pdf/__init__.py
+-rw-rw-rw-   0        0        0     1970 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/pdf/add_watermark_service.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:59.174701 python-office-0.3.9/office/lib/ppt/
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/ppt/__init__.py
+-rw-rw-rw-   0        0        0     1140 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/ppt/ppt2pdf_service.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:59.188246 python-office-0.3.9/office/lib/tools/
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/tools/__init__.py
+-rw-rw-rw-   0        0        0     1128 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/tools/lottery8ticket.py
+-rw-rw-rw-   0        0        0     7247 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/tools/pwd4wifi_service.py
+-rw-rw-rw-   0        0        0    14160 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/tools/qoute_dict_create_article.py
+-rw-rw-rw-   0        0        0    77907 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/tools/weather_city_code.py
+-rw-rw-rw-   0        0        0     1004 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/tools/weather_service.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:59.197761 python-office-0.3.9/office/lib/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/utils/__init__.py
+-rw-rw-rw-   0        0        0     1062 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/utils/except_utils.py
+-rw-rw-rw-   0        0        0     1472 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/utils/pandas_mem.py
+-rw-rw-rw-   0        0        0      272 2023-04-05 07:52:22.000000 python-office-0.3.9/office/lib/utils/time_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:59.222827 python-office-0.3.9/python_office.egg-info/
+-rw-rw-rw-   0        0        0    10590 2023-04-09 06:59:59.000000 python-office-0.3.9/python_office.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2021 2023-04-09 06:59:59.000000 python-office-0.3.9/python_office.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 06:59:59.000000 python-office-0.3.9/python_office.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-09 06:33:00.000000 python-office-0.3.9/python_office.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      116 2023-04-09 06:59:59.000000 python-office-0.3.9/python_office.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-09 06:59:59.000000 python-office-0.3.9/python_office.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      894 2023-04-09 06:59:59.262172 python-office-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      428 2023-04-05 07:52:22.000000 python-office-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:59.227371 python-office-0.3.9/tests/
+-rw-rw-rw-   0        0        0      379 2023-04-05 07:52:22.000000 python-office-0.3.9/tests/__init__.py
+-rw-rw-rw-   0        0        0      460 2023-04-05 07:52:23.000000 python-office-0.3.9/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:59.256150 python-office-0.3.9/tests/test_unit/
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:52:23.000000 python-office-0.3.9/tests/test_unit/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:52:23.000000 python-office-0.3.9/tests/test_unit/test_dev.py
+-rw-rw-rw-   0        0        0     2168 2023-04-05 07:52:23.000000 python-office-0.3.9/tests/test_unit/test_excel.py
+-rw-rw-rw-   0        0        0     1271 2023-04-08 15:28:39.000000 python-office-0.3.9/tests/test_unit/test_file.py
+-rw-rw-rw-   0        0        0      782 2023-04-05 07:52:23.000000 python-office-0.3.9/tests/test_unit/test_image.py
+-rw-rw-rw-   0        0        0      684 2023-04-05 07:52:23.000000 python-office-0.3.9/tests/test_unit/test_markdown.py
+-rw-rw-rw-   0        0        0     2032 2023-04-05 07:52:23.000000 python-office-0.3.9/tests/test_unit/test_pdf.py
+-rw-rw-rw-   0        0        0      355 2023-04-05 07:52:23.000000 python-office-0.3.9/tests/test_unit/test_ppt.py
+-rw-rw-rw-   0        0        0      946 2023-04-05 07:52:23.000000 python-office-0.3.9/tests/test_unit/test_ruiming.py
+-rw-rw-rw-   0        0        0      193 2023-04-05 07:52:23.000000 python-office-0.3.9/tests/test_unit/test_search_by_content.py
+-rw-rw-rw-   0        0        0      824 2023-04-05 07:52:23.000000 python-office-0.3.9/tests/test_unit/test_tools.py
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:52:23.000000 python-office-0.3.9/tests/test_unit/test_video.py
+-rw-rw-rw-   0        0        0      295 2023-04-05 07:52:23.000000 python-office-0.3.9/tests/test_unit/test_wechat.py
+-rw-rw-rw-   0        0        0      232 2023-04-05 07:52:23.000000 python-office-0.3.9/tests/test_unit/test_word.py
```

### Comparing `python-office-0.3.8/LICENSE` & `python-office-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/PKG-INFO` & `python-office-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-office
-Version: 0.3.8
+Version: 0.3.9
 Summary: python for office
 Home-page: https://github.com/CoderWanFeng/python-office
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: Apache-2.0 license
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/python-office/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/python-office/blob/master/README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-office Version: 0.3.8 Summary: python for
+Metadata-Version: 2.1 Name: python-office Version: 0.3.9 Summary: python for
 office Home-page: https://github.com/CoderWanFeng/python-office Author:
 CoderWanFeng Author-email: 1957875073@qq.com License: Apache-2.0 license
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/python-office/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/python-office/blob/
 master/README.md Project-URL: Source Code, https://github.com/CoderWanFeng/
 python-office Platform: any Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE
```

### Comparing `python-office-0.3.8/README.md` & `python-office-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/api/excel.py` & `python-office-0.3.9/office/api/excel.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/api/file.py` & `python-office-0.3.9/office/api/file.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/api/image.py` & `python-office-0.3.9/office/api/image.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/api/pdf.py` & `python-office-0.3.9/office/api/pdf.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/api/ppt.py` & `python-office-0.3.9/office/api/ppt.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/api/tools.py` & `python-office-0.3.9/office/api/tools.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/api/video.py` & `python-office-0.3.9/office/api/video.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/api/wechat.py` & `python-office-0.3.9/office/api/wechat.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/api/word.py` & `python-office-0.3.9/office/api/word.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/cli/main.py` & `python-office-0.3.9/office/cli/main.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/core/TestTypes/RuimingType.py` & `python-office-0.3.9/office/core/TestTypes/RuimingType.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/lib/decorator_utils/instruction_url.py` & `python-office-0.3.9/office/lib/decorator_utils/instruction_url.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/lib/excel/SplitExcel.py` & `python-office-0.3.9/office/lib/excel/SplitExcel.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/lib/image/add_watermark_service.py` & `python-office-0.3.9/office/lib/image/add_watermark_service.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/lib/image/eliminate_background.py` & `python-office-0.3.9/office/lib/image/eliminate_background.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/lib/pdf/add_watermark_service.py` & `python-office-0.3.9/office/lib/pdf/add_watermark_service.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/lib/ppt/ppt2pdf_service.py` & `python-office-0.3.9/office/lib/ppt/ppt2pdf_service.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/lib/tools/lottery8ticket.py` & `python-office-0.3.9/office/lib/tools/lottery8ticket.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/lib/tools/pwd4wifi_service.py` & `python-office-0.3.9/office/lib/tools/pwd4wifi_service.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/lib/tools/qoute_dict_create_article.py` & `python-office-0.3.9/office/lib/tools/qoute_dict_create_article.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/lib/tools/weather_city_code.py` & `python-office-0.3.9/office/lib/tools/weather_city_code.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/lib/tools/weather_service.py` & `python-office-0.3.9/office/lib/tools/weather_service.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/lib/utils/except_utils.py` & `python-office-0.3.9/office/lib/utils/except_utils.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/office/lib/utils/pandas_mem.py` & `python-office-0.3.9/office/lib/utils/pandas_mem.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/python_office.egg-info/PKG-INFO` & `python-office-0.3.9/python_office.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-office
-Version: 0.3.8
+Version: 0.3.9
 Summary: python for office
 Home-page: https://github.com/CoderWanFeng/python-office
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: Apache-2.0 license
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/python-office/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/python-office/blob/master/README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-office Version: 0.3.8 Summary: python for
+Metadata-Version: 2.1 Name: python-office Version: 0.3.9 Summary: python for
 office Home-page: https://github.com/CoderWanFeng/python-office Author:
 CoderWanFeng Author-email: 1957875073@qq.com License: Apache-2.0 license
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/python-office/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/python-office/blob/
 master/README.md Project-URL: Source Code, https://github.com/CoderWanFeng/
 python-office Platform: any Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE
```

### Comparing `python-office-0.3.8/python_office.egg-info/SOURCES.txt` & `python-office-0.3.9/python_office.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/setup.cfg` & `python-office-0.3.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7974 686f 6e2d 6f66 6669 6365   = python-office
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 332e  ..version = 0.3.
-00000030: 380d 0a64 6573 6372 6970 7469 6f6e 203d  8..description =
+00000030: 390d 0a64 6573 6372 6970 7469 6f6e 203d  9..description =
 00000040: 2070 7974 686f 6e20 666f 7220 6f66 6669   python for offi
 00000050: 6365 0d0a 6c6f 6e67 5f64 6573 6372 6970  ce..long_descrip
 00000060: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000070: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 00000080: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
 00000090: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
 000000a0: 6b64 6f77 6e0d 0a75 726c 203d 2068 7474  kdown..url = htt
```

### Comparing `python-office-0.3.8/tests/test_unit/test_excel.py` & `python-office-0.3.9/tests/test_unit/test_excel.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/tests/test_unit/test_file.py` & `python-office-0.3.9/tests/test_unit/test_file.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/tests/test_unit/test_image.py` & `python-office-0.3.9/tests/test_unit/test_image.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/tests/test_unit/test_markdown.py` & `python-office-0.3.9/tests/test_unit/test_markdown.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/tests/test_unit/test_pdf.py` & `python-office-0.3.9/tests/test_unit/test_pdf.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/tests/test_unit/test_ruiming.py` & `python-office-0.3.9/tests/test_unit/test_ruiming.py`

 * *Files identical despite different names*

### Comparing `python-office-0.3.8/tests/test_unit/test_tools.py` & `python-office-0.3.9/tests/test_unit/test_tools.py`

 * *Files identical despite different names*

