# Comparing `tmp/manga-ocr-0.1.8.tar.gz` & `tmp/manga-ocr-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\manga-ocr-0.1.8.tar", last modified: Sat Nov  5 12:30:11 2022, max compression
+gzip compressed data, was "dist\manga-ocr-0.1.9.tar", last modified: Sun May  7 22:35:40 2023, max compression
```

## Comparing `manga-ocr-0.1.8.tar` & `manga-ocr-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-11-05 12:30:11.000000 manga-ocr-0.1.8/
--rw-rw-rw-   0        0        0    11558 2022-01-15 17:19:21.000000 manga-ocr-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       28 2022-02-09 19:39:37.000000 manga-ocr-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1771 2022-11-05 12:30:11.000000 manga-ocr-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     6558 2022-11-03 20:56:16.000000 manga-ocr-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2022-11-05 12:30:11.000000 manga-ocr-0.1.8/assets/
--rw-rw-rw-   0        0        0    56623 2022-02-09 19:39:37.000000 manga-ocr-0.1.8/assets/example.jpg
-drwxrwxrwx   0        0        0        0 2022-11-05 12:30:11.000000 manga-ocr-0.1.8/manga_ocr/
--rw-rw-rw-   0        0        0       61 2022-11-05 12:29:40.000000 manga-ocr-0.1.8/manga_ocr/__init__.py
--rw-rw-rw-   0        0        0      127 2022-01-19 22:01:59.000000 manga-ocr-0.1.8/manga_ocr/__main__.py
--rw-rw-rw-   0        0        0     2161 2022-11-03 20:31:42.000000 manga-ocr-0.1.8/manga_ocr/ocr.py
--rw-rw-rw-   0        0        0     3940 2022-03-09 20:14:10.000000 manga-ocr-0.1.8/manga_ocr/run.py
-drwxrwxrwx   0        0        0        0 2022-11-05 12:30:11.000000 manga-ocr-0.1.8/manga_ocr.egg-info/
--rw-rw-rw-   0        0        0     1771 2022-11-05 12:30:10.000000 manga-ocr-0.1.8/manga_ocr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2022-11-05 12:30:10.000000 manga-ocr-0.1.8/manga_ocr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-05 12:30:10.000000 manga-ocr-0.1.8/manga_ocr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2022-11-05 12:30:10.000000 manga-ocr-0.1.8/manga_ocr.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      108 2022-11-05 12:30:10.000000 manga-ocr-0.1.8/manga_ocr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-11-05 12:30:10.000000 manga-ocr-0.1.8/manga_ocr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-05 12:30:11.000000 manga-ocr-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1037 2022-11-05 12:29:39.000000 manga-ocr-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 22:35:40.000000 manga-ocr-0.1.9/
+-rw-rw-rw-   0        0        0    11558 2022-01-15 17:19:21.000000 manga-ocr-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       28 2022-02-09 19:39:37.000000 manga-ocr-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1771 2023-05-07 22:35:40.000000 manga-ocr-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6558 2022-11-03 20:56:16.000000 manga-ocr-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 22:35:40.000000 manga-ocr-0.1.9/assets/
+-rw-rw-rw-   0        0        0    56623 2022-02-09 19:39:37.000000 manga-ocr-0.1.9/assets/example.jpg
+drwxrwxrwx   0        0        0        0 2023-05-07 22:35:40.000000 manga-ocr-0.1.9/manga_ocr/
+-rw-rw-rw-   0        0        0       61 2023-05-07 22:32:48.000000 manga-ocr-0.1.9/manga_ocr/__init__.py
+-rw-rw-rw-   0        0        0      127 2022-01-19 22:01:59.000000 manga-ocr-0.1.9/manga_ocr/__main__.py
+-rw-rw-rw-   0        0        0     2185 2023-05-07 21:52:56.000000 manga-ocr-0.1.9/manga_ocr/ocr.py
+-rw-rw-rw-   0        0        0     3940 2022-03-09 20:14:10.000000 manga-ocr-0.1.9/manga_ocr/run.py
+drwxrwxrwx   0        0        0        0 2023-05-07 22:35:40.000000 manga-ocr-0.1.9/manga_ocr.egg-info/
+-rw-rw-rw-   0        0        0     1771 2023-05-07 22:35:40.000000 manga-ocr-0.1.9/manga_ocr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-05-07 22:35:40.000000 manga-ocr-0.1.9/manga_ocr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 22:35:40.000000 manga-ocr-0.1.9/manga_ocr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-07 22:35:40.000000 manga-ocr-0.1.9/manga_ocr.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       94 2023-05-07 22:35:40.000000 manga-ocr-0.1.9/manga_ocr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-07 22:35:40.000000 manga-ocr-0.1.9/manga_ocr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 22:35:40.000000 manga-ocr-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1011 2023-05-07 22:32:48.000000 manga-ocr-0.1.9/setup.py
```

### Comparing `manga-ocr-0.1.8/LICENSE` & `manga-ocr-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `manga-ocr-0.1.8/PKG-INFO` & `manga-ocr-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manga-ocr
-Version: 0.1.8
+Version: 0.1.9
 Summary: OCR for Japanese manga
 Home-page: https://github.com/kha-white/manga-ocr
 Author: Maciej Budyś
 Author-email: kha-white@mail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `manga-ocr-0.1.8/README.md` & `manga-ocr-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `manga-ocr-0.1.8/assets/example.jpg` & `manga-ocr-0.1.9/assets/example.jpg`

 * *Files identical despite different names*

### Comparing `manga-ocr-0.1.8/manga_ocr/ocr.py` & `manga-ocr-0.1.9/manga_ocr/ocr.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     def __call__(self, img_or_path):
         if isinstance(img_or_path, str) or isinstance(img_or_path, Path):
             img = Image.open(img_or_path)
         elif isinstance(img_or_path, Image.Image):
             img = img_or_path
         else:
-            raise ValueError(f'Invalid value of img_or_path: {img_or_path}')
+            raise ValueError(f'img_or_path must be a path or PIL.Image, instead got: {img_or_path}')
 
         img = img.convert('L').convert('RGB')
 
         x = self._preprocess(img)
         x = self.model.generate(x[None].to(self.model.device), max_length=300)[0].cpu()
         x = self.tokenizer.decode(x, skip_special_tokens=True)
         x = post_process(x)
```

### Comparing `manga-ocr-0.1.8/manga_ocr/run.py` & `manga-ocr-0.1.9/manga_ocr/run.py`

 * *Files identical despite different names*

### Comparing `manga-ocr-0.1.8/manga_ocr.egg-info/PKG-INFO` & `manga-ocr-0.1.9/manga_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manga-ocr
-Version: 0.1.8
+Version: 0.1.9
 Summary: OCR for Japanese manga
 Home-page: https://github.com/kha-white/manga-ocr
 Author: Maciej Budyś
 Author-email: kha-white@mail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `manga-ocr-0.1.8/setup.py` & `manga-ocr-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from setuptools import setup
 
 long_description = (Path(__file__).parent / "README.md").read_text('utf-8').split('# Installation')[0]
 
 setup(
     name="manga-ocr",
-    version='0.1.8',
+    version='0.1.9',
     description="OCR for Japanese manga",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kha-white/manga-ocr",
     author="Maciej Budyś",
     author_email="kha-white@mail.com",
     license="Apache License 2.0",
@@ -22,17 +22,16 @@
         "fire",
         "fugashi",
         "jaconv",
         "loguru",
         "numpy",
         "Pillow",
         "pyperclip",
-        "sentencepiece",
         "torch>=1.0",
-        "transformers>=4.12.5",
+        "transformers>=4.25.0",
         "unidic_lite",
     ],
     entry_points={
         "console_scripts": [
             "manga_ocr=manga_ocr.__main__:main",
         ]
     },
```

