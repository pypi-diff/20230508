# Comparing `tmp/smartjs-0.0.9.tar.gz` & `tmp/smartjs-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartjs-0.0.9.tar", max compression
+gzip compressed data, was "smartjs-0.1.0.tar", max compression
```

## Comparing `smartjs-0.0.9.tar` & `smartjs-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      383 2023-05-07 13:22:15.175760 smartjs-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      183 2023-05-05 14:06:40.683599 smartjs-0.0.9/smartjs/__init__.py
--rw-r--r--   0        0        0    13214 2023-05-07 13:14:18.303555 smartjs-0.0.9/smartjs/base.py
--rw-r--r--   0        0        0     2223 2023-05-05 22:02:36.952511 smartjs-0.0.9/smartjs/constants.py
--rw-r--r--   0        0        0     4879 2023-05-07 13:14:18.308482 smartjs-0.0.9/smartjs/elements.py
--rw-r--r--   0        0        0     5805 2023-05-06 22:41:19.600790 smartjs-0.0.9/smartjs/functions.py
--rw-r--r--   0        0        0    11888 2023-05-06 23:09:29.039937 smartjs-0.0.9/smartjs/javascript.py
--rw-r--r--   0        0        0     1660 2023-05-05 21:29:35.092805 smartjs-0.0.9/smartjs/page.py
--rw-r--r--   0        0        0      994 2023-05-07 01:38:04.688449 smartjs-0.0.9/smartjs/path.py
--rw-r--r--   0        0        0     1400 2023-05-06 22:39:05.716015 smartjs-0.0.9/smartjs/style.py
--rw-r--r--   0        0        0      665 2023-05-07 13:22:25.695005 smartjs-0.0.9/setup.py
--rw-r--r--   0        0        0      414 2023-05-07 13:22:25.695231 smartjs-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      383 2023-05-07 23:02:01.983688 smartjs-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-05-05 14:06:40.683599 smartjs-0.1.0/smartjs/__init__.py
+-rw-r--r--   0        0        0    13214 2023-05-07 13:14:18.303555 smartjs-0.1.0/smartjs/base.py
+-rw-r--r--   0        0        0     2223 2023-05-05 22:02:36.952511 smartjs-0.1.0/smartjs/constants.py
+-rw-r--r--   0        0        0     4880 2023-05-07 23:02:01.978824 smartjs-0.1.0/smartjs/elements.py
+-rw-r--r--   0        0        0     5805 2023-05-06 22:41:19.600790 smartjs-0.1.0/smartjs/functions.py
+-rw-r--r--   0        0        0    11888 2023-05-06 23:09:29.039937 smartjs-0.1.0/smartjs/javascript.py
+-rw-r--r--   0        0        0     1660 2023-05-05 21:29:35.092805 smartjs-0.1.0/smartjs/page.py
+-rw-r--r--   0        0        0      994 2023-05-07 01:38:04.688449 smartjs-0.1.0/smartjs/path.py
+-rw-r--r--   0        0        0     1400 2023-05-06 22:39:05.716015 smartjs-0.1.0/smartjs/style.py
+-rw-r--r--   0        0        0      665 2023-05-07 23:02:06.918074 smartjs-0.1.0/setup.py
+-rw-r--r--   0        0        0      414 2023-05-07 23:02:06.918310 smartjs-0.1.0/PKG-INFO
```

### Comparing `smartjs-0.0.9/smartjs/base.py` & `smartjs-0.1.0/smartjs/base.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.9/smartjs/constants.py` & `smartjs-0.1.0/smartjs/constants.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.9/smartjs/elements.py` & `smartjs-0.1.0/smartjs/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
 		if value:
 			args.append(Kwarg('value', value))
 		if id:
 			args.append(Kwarg('id', id))
 		if text:
 			args.append(Text(text))
 		if default:
-			args.append(Arg('checked'))
+			args.append(Arg('selected'))
 		super().__init__(*args)
 
 
 class BaseUniqueElement(BaseElement):
 	@property
 	def post_init_kwargs(self):
 		return dict(id=type(self).__name__.lower())
```

### Comparing `smartjs-0.0.9/smartjs/functions.py` & `smartjs-0.1.0/smartjs/functions.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.9/smartjs/javascript.py` & `smartjs-0.1.0/smartjs/javascript.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.9/smartjs/page.py` & `smartjs-0.1.0/smartjs/page.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.9/smartjs/path.py` & `smartjs-0.1.0/smartjs/path.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.9/smartjs/style.py` & `smartjs-0.1.0/smartjs/style.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.9/setup.py` & `smartjs-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Unidecode>=1.3.6,<2.0.0']
 
 setup_kwargs = {
     'name': 'smartjs',
-    'version': '0.0.9',
+    'version': '0.1.0',
     'description': 'Project for creation of javascript, html and style elements for use in web pages.',
     'long_description': None,
     'author': 'Daniel Victor',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

