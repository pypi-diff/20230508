# Comparing `tmp/FicImage-1.0.0.tar.gz` & `tmp/FicImage-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FicImage-1.0.0.tar", last modified: Mon May  8 15:55:39 2023, max compression
+gzip compressed data, was "FicImage-1.0.1.tar", last modified: Mon May  8 16:26:47 2023, max compression
```

## Comparing `FicImage-1.0.0.tar` & `FicImage-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 15:55:39.277870 FicImage-1.0.0/
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     1075 2023-04-28 12:48:04.000000 FicImage-1.0.0/LICENSE
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     7307 2023-05-08 15:55:39.273870 FicImage-1.0.0/PKG-INFO
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     5264 2023-05-07 15:48:12.000000 FicImage-1.0.0/README.md
--rw-rw-r--   0 nonso     (1000) nonso     (1001)      921 2023-05-08 15:43:35.000000 FicImage-1.0.0/pyproject.toml
--rw-rw-r--   0 nonso     (1000) nonso     (1001)       38 2023-05-08 15:55:39.277870 FicImage-1.0.0/setup.cfg
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     1281 2023-05-08 15:55:20.000000 FicImage-1.0.0/setup.py
-drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 15:55:38.985866 FicImage-1.0.0/src/
-drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 15:55:39.237870 FicImage-1.0.0/src/FicImage/
--rw-rw-r--   0 nonso     (1000) nonso     (1001)        0 2023-05-06 04:09:38.000000 FicImage-1.0.0/src/FicImage/__init__.py
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     5275 2023-05-05 16:21:24.000000 FicImage-1.0.0/src/FicImage/image.py
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     3729 2023-05-08 15:18:02.000000 FicImage-1.0.0/src/FicImage/main.py
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     2286 2023-05-08 15:18:02.000000 FicImage-1.0.0/src/FicImage/utils.py
-drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 15:55:39.273870 FicImage-1.0.0/src/FicImage.egg-info/
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     7307 2023-05-08 15:55:38.000000 FicImage-1.0.0/src/FicImage.egg-info/PKG-INFO
--rw-rw-r--   0 nonso     (1000) nonso     (1001)      349 2023-05-08 15:55:38.000000 FicImage-1.0.0/src/FicImage.egg-info/SOURCES.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)        1 2023-05-08 15:55:38.000000 FicImage-1.0.0/src/FicImage.egg-info/dependency_links.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)       52 2023-05-08 15:55:38.000000 FicImage-1.0.0/src/FicImage.egg-info/entry_points.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)      182 2023-05-08 15:55:38.000000 FicImage-1.0.0/src/FicImage.egg-info/requires.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)        9 2023-05-08 15:55:38.000000 FicImage-1.0.0/src/FicImage.egg-info/top_level.txt
+drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 16:26:47.143530 FicImage-1.0.1/
+drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 16:26:47.143530 FicImage-1.0.1/FicImage/
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)        0 2023-05-06 04:09:38.000000 FicImage-1.0.1/FicImage/__init__.py
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     5275 2023-05-05 16:21:24.000000 FicImage-1.0.1/FicImage/image.py
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     3721 2023-05-08 16:20:33.000000 FicImage-1.0.1/FicImage/main.py
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     2277 2023-05-08 16:20:33.000000 FicImage-1.0.1/FicImage/utils.py
+drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 16:26:47.143530 FicImage-1.0.1/FicImage.egg-info/
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     7307 2023-05-08 16:26:47.000000 FicImage-1.0.1/FicImage.egg-info/PKG-INFO
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)      309 2023-05-08 16:26:47.000000 FicImage-1.0.1/FicImage.egg-info/SOURCES.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)        1 2023-05-08 16:26:47.000000 FicImage-1.0.1/FicImage.egg-info/dependency_links.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)       48 2023-05-08 16:26:47.000000 FicImage-1.0.1/FicImage.egg-info/entry_points.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)      182 2023-05-08 16:26:47.000000 FicImage-1.0.1/FicImage.egg-info/requires.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)        9 2023-05-08 16:26:47.000000 FicImage-1.0.1/FicImage.egg-info/top_level.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     1075 2023-04-28 12:48:04.000000 FicImage-1.0.1/LICENSE
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     7307 2023-05-08 16:26:47.143530 FicImage-1.0.1/PKG-INFO
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     5264 2023-05-07 15:48:12.000000 FicImage-1.0.1/README.md
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)      921 2023-05-08 16:26:37.000000 FicImage-1.0.1/pyproject.toml
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)       38 2023-05-08 16:26:47.143530 FicImage-1.0.1/setup.cfg
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     1243 2023-05-08 16:26:37.000000 FicImage-1.0.1/setup.py
```

### Comparing `FicImage-1.0.0/LICENSE` & `FicImage-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FicImage-1.0.0/PKG-INFO` & `FicImage-1.0.1/FicImage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FicImage
-Version: 1.0.0
+Version: 1.0.1
 Summary: FicImage is an application designed to enhance the reading experience of FicHub epubs.
 Home-page: https://github.com/Jemeni11/FicImage
 Author: Emmanuel C. Jemeni
 Author-email: "Emmanuel C. Jemeni" <jemenichinonso11@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Emmanuel C. Jemeni
```

### Comparing `FicImage-1.0.0/README.md` & `FicImage-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `FicImage-1.0.0/pyproject.toml` & `FicImage-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "FicImage"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Emmanuel C. Jemeni", email="jemenichinonso11@gmail.com" }
 ]
 description = "FicImage is an application designed to enhance the reading experience of FicHub epubs."
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
```

### Comparing `FicImage-1.0.0/setup.py` & `FicImage-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="FicImage",
-	version="1.0.0",
+	version="1.0.1",
 	author="Emmanuel C. Jemeni",
 	author_email="jemenichinonso11@gmail.com",
 	description="FicImage is an application designed to enhance the reading experience of FicHub epubs.",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/Jemeni11/FicImage",
 	project_urls={
 		"Bug Tracker": "https://github.com/Jemeni11/FicImage/issues",
 	},
 	entry_points={
 		'console_scripts': [
-			'ficimage=src.FicImage.main:main'
+			'ficimage=FicImage.main:main'
 		]
 	},
 	install_requires=[
 		'beautifulsoup4==4.12.2',
 		'certifi==2022.12.7',
 		'charset-normalizer==3.1.0',
 		'EbookLib==0.18',
@@ -37,11 +37,10 @@
 	classifiers=[
 		"Development Status :: 5 - Production/Stable",
 		"Programming Language :: Python :: 3",
 		"License :: OSI Approved :: MIT License",
 		"Operating System :: OS Independent",
 		"Topic :: Internet :: WWW/HTTP",
 	],
-	package_dir={"": "src"},
-	packages=setuptools.find_packages(where="src"),
+	packages=setuptools.find_packages('.'),
 	python_requires=">=3.6"
 )
```

### Comparing `FicImage-1.0.0/src/FicImage/image.py` & `FicImage-1.0.1/FicImage/image.py`

 * *Files identical despite different names*

### Comparing `FicImage-1.0.0/src/FicImage/main.py` & `FicImage-1.0.1/FicImage/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import ebooklib
 from ebooklib import epub
 from bs4 import BeautifulSoup
-from src.FicImage.image import get_image_from_url
-from src.FicImage.utils import config_check, load_config_json, default_ficimage_settings
+from FicImage.image import get_image_from_url
+from FicImage.utils import config_check, load_config_json, default_ficimage_settings
 
 
 def main(path_to_epub: str, config_file_path: str = None) -> None:
 	"""
 	This function updates the FicHub epub file with images.
 	:param path_to_epub: The path to the FicHub epub file.
 	:param config_file_path: The path to the ficimage.json file.
```

### Comparing `FicImage-1.0.0/src/FicImage/utils.py` & `FicImage-1.0.1/FicImage/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 	:param directory_path: A string or None
 	:return: A tuple containing a boolean and a string
 	"""
 	if directory_path is None:
 		current_dir = os.getcwd()
 		print(f"[Config File Check]: No directory was passed, checking current directory '{current_dir}'")
 		
-		file_path = os.path.join(current_dir, "../../ficimage.json")
+		file_path = os.path.join(current_dir, "../ficimage.json")
 		
 		if os.path.isfile(file_path):
 			print(f"[Config File Check]: ficimage.json found in current directory!")
 			return True, current_dir
 		
 		directory_path = os.path.expanduser("~")
 		print(f"[Config File Check]: ficimage.json not found in current directory, checking '{directory_path}'")
 	
-	file_path = os.path.join(directory_path, "../../ficimage.json")
+	file_path = os.path.join(directory_path, "../ficimage.json")
 	
 	is_file = os.path.isfile(file_path)
 	print(f"[Config File Check]: "
 	      f"{'ficimage.json found!' if is_file else 'ficimage.json not found, using default config settings'}")
 	
 	return is_file, directory_path
 
@@ -38,15 +38,15 @@
 def load_config_json(ficimage_path: str) -> dict:
 	"""
 	Loads ficimage.json. Calls `sys.exit` if there's a JSONDecodeError.
 	:param ficimage_path: The path to ficimage.json.
 	:return: A dict containing the data stored inside ficimage.json
 	"""
 	try:
-		with open(os.path.join(ficimage_path, "../../ficimage.json"), 'r') as f:
+		with open(os.path.join(ficimage_path, "../ficimage.json"), 'r') as f:
 			return json.load(f)
 	except json.decoder.JSONDecodeError:
 		sys.exit("[Loading Config JSON]: Invalid JSON in Config File")
 
 
 def default_ficimage_settings() -> dict:
 	"""
```

### Comparing `FicImage-1.0.0/src/FicImage.egg-info/PKG-INFO` & `FicImage-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FicImage
-Version: 1.0.0
+Version: 1.0.1
 Summary: FicImage is an application designed to enhance the reading experience of FicHub epubs.
 Home-page: https://github.com/Jemeni11/FicImage
 Author: Emmanuel C. Jemeni
 Author-email: "Emmanuel C. Jemeni" <jemenichinonso11@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Emmanuel C. Jemeni
```

