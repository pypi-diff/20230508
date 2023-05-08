# Comparing `tmp/krx_rigger-0.0.8.tar.gz` & `tmp/krx_rigger-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/krx_rigger-0.0.8.tar", last modified: Thu May  4 05:58:53 2023, max compression
+gzip compressed data, was "dist/krx_rigger-0.0.9.tar", last modified: Thu May  4 06:33:05 2023, max compression
```

## Comparing `krx_rigger-0.0.8.tar` & `krx_rigger-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-04 05:58:53.000000 krx_rigger-0.0.8/
--rw-r--r--   0 nezah      (501) staff       (20)      430 2023-05-04 05:58:53.000000 krx_rigger-0.0.8/PKG-INFO
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-04 05:58:53.000000 krx_rigger-0.0.8/krx_rigger.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      430 2023-05-04 05:58:53.000000 krx_rigger-0.0.8/krx_rigger.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      196 2023-05-04 05:58:53.000000 krx_rigger-0.0.8/krx_rigger.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)        4 2023-05-04 05:58:53.000000 krx_rigger-0.0.8/krx_rigger.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-04 05:58:53.000000 krx_rigger-0.0.8/krx_rigger.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 krx_rigger-0.0.8/LICENSE
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-04 05:58:53.000000 krx_rigger-0.0.8/test/
--rw-r--r--   0 nezah      (501) staff       (20)      436 2023-05-03 14:12:55.000000 krx_rigger-0.0.8/test/test_list.py
--rw-r--r--   0 nezah      (501) staff       (20)       40 2023-05-03 13:45:03.000000 krx_rigger-0.0.8/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      550 2023-05-04 05:58:52.000000 krx_rigger-0.0.8/setup.py
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-04 05:58:53.000000 krx_rigger-0.0.8/setup.cfg
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-04 05:58:53.000000 krx_rigger-0.0.8/krx/
--rw-r--r--   0 nezah      (501) staff       (20)     7644 2023-05-04 05:58:36.000000 krx_rigger-0.0.8/krx/__init__.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-04 06:33:05.000000 krx_rigger-0.0.9/
+-rw-r--r--   0 nezah      (501) staff       (20)      430 2023-05-04 06:33:05.000000 krx_rigger-0.0.9/PKG-INFO
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-04 06:33:05.000000 krx_rigger-0.0.9/krx_rigger.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      430 2023-05-04 06:33:05.000000 krx_rigger-0.0.9/krx_rigger.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      196 2023-05-04 06:33:05.000000 krx_rigger-0.0.9/krx_rigger.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        4 2023-05-04 06:33:05.000000 krx_rigger-0.0.9/krx_rigger.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-04 06:33:05.000000 krx_rigger-0.0.9/krx_rigger.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 krx_rigger-0.0.9/LICENSE
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-04 06:33:05.000000 krx_rigger-0.0.9/test/
+-rw-r--r--   0 nezah      (501) staff       (20)      436 2023-05-03 14:12:55.000000 krx_rigger-0.0.9/test/test_list.py
+-rw-r--r--   0 nezah      (501) staff       (20)       40 2023-05-03 13:45:03.000000 krx_rigger-0.0.9/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      550 2023-05-04 06:33:04.000000 krx_rigger-0.0.9/setup.py
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-04 06:33:05.000000 krx_rigger-0.0.9/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-04 06:33:05.000000 krx_rigger-0.0.9/krx/
+-rw-r--r--   0 nezah      (501) staff       (20)     7754 2023-05-04 06:33:04.000000 krx_rigger-0.0.9/krx/__init__.py
```

### Comparing `krx_rigger-0.0.8/LICENSE` & `krx_rigger-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `krx_rigger-0.0.8/setup.py` & `krx_rigger-0.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krx_rigger",
-    version="0.0.8",
+    version="0.0.9",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="krx web crawler wrapper",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/krx_rigger",
     packages=setuptools.find_packages(),
```

### Comparing `krx_rigger-0.0.8/krx/__init__.py` & `krx_rigger-0.0.9/krx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,17 +187,21 @@
         link_script = links[1].get("onclick")
         doc_id = extract_kid(link_script)
         tds = tr.select("td")
         time = tds[0].text
         org = tds[3].text
         imgs = tds[1].select("img")
         remarks = [img['alt'] for img in imgs]
+        fonts = tds[2].select("font")
+        etcs = [font.text for font in fonts]
+
         return {
             "dt": dt,
             "time": time,
             "company": company,
             "company_id": company_id,
             "doc_id": doc_id,
             "title": title,
             "org": org,
-            "remarks": remarks
+            "remarks": remarks,
+            "etcs": etcs
         }
```

