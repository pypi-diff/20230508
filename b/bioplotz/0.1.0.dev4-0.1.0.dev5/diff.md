# Comparing `tmp/bioplotz-0.1.0.dev4.tar.gz` & `tmp/bioplotz-0.1.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioplotz-0.1.0.dev4.tar", last modified: Fri May  5 02:19:41 2023, max compression
+gzip compressed data, was "bioplotz-0.1.0.dev5.tar", last modified: Mon May  8 07:23:09 2023, max compression
```

## Comparing `bioplotz-0.1.0.dev4.tar` & `bioplotz-0.1.0.dev5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-05 02:19:41.540094 bioplotz-0.1.0.dev4/
--rw-r--r--   0 zsc       (1000) users      (100)     1305 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev4/LICENSE
--rw-r--r--   0 zsc       (1000) users      (100)       67 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev4/MANIFEST.in
--rw-r--r--   0 zsc       (1000) users      (100)    13845 2023-05-05 02:19:41.540094 bioplotz-0.1.0.dev4/PKG-INFO
--rw-r--r--   0 zsc       (1000) users      (100)    13548 2023-05-05 02:18:26.000000 bioplotz-0.1.0.dev4/README.md
-drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-05 02:19:41.540094 bioplotz-0.1.0.dev4/bioplotz/
--rw-r--r--   0 zsc       (1000) users      (100)      225 2023-05-05 02:19:11.000000 bioplotz-0.1.0.dev4/bioplotz/__init__.py
--rw-r--r--   0 zsc       (1000) users      (100)    10185 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev4/bioplotz/chromosome.py
--rw-r--r--   0 zsc       (1000) users      (100)     2477 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev4/bioplotz/genecluster.py
--rwxr-xr-x   0 zsc       (1000) users      (100)     6110 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev4/bioplotz/manhattan.py
--rw-r--r--   0 zsc       (1000) users      (100)     4579 2023-05-05 02:16:04.000000 bioplotz-0.1.0.dev4/bioplotz/mulitalign.py
-drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-05 02:19:41.540094 bioplotz-0.1.0.dev4/bioplotz.egg-info/
--rw-r--r--   0 zsc       (1000) users      (100)    13845 2023-05-05 02:19:41.000000 bioplotz-0.1.0.dev4/bioplotz.egg-info/PKG-INFO
--rw-r--r--   0 zsc       (1000) users      (100)      310 2023-05-05 02:19:41.000000 bioplotz-0.1.0.dev4/bioplotz.egg-info/SOURCES.txt
--rw-r--r--   0 zsc       (1000) users      (100)        1 2023-05-05 02:19:41.000000 bioplotz-0.1.0.dev4/bioplotz.egg-info/dependency_links.txt
--rw-r--r--   0 zsc       (1000) users      (100)       24 2023-05-05 02:19:41.000000 bioplotz-0.1.0.dev4/bioplotz.egg-info/requires.txt
--rw-r--r--   0 zsc       (1000) users      (100)        9 2023-05-05 02:19:41.000000 bioplotz-0.1.0.dev4/bioplotz.egg-info/top_level.txt
--rw-r--r--   0 zsc       (1000) users      (100)       38 2023-05-05 02:19:41.540094 bioplotz-0.1.0.dev4/setup.cfg
--rw-r--r--   0 zsc       (1000) users      (100)      643 2023-05-05 02:19:05.000000 bioplotz-0.1.0.dev4/setup.py
+drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-08 07:23:09.505732 bioplotz-0.1.0.dev5/
+-rw-r--r--   0 zsc       (1000) users      (100)     1305 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev5/LICENSE
+-rw-r--r--   0 zsc       (1000) users      (100)       67 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev5/MANIFEST.in
+-rw-r--r--   0 zsc       (1000) users      (100)    13845 2023-05-08 07:23:09.505732 bioplotz-0.1.0.dev5/PKG-INFO
+-rw-r--r--   0 zsc       (1000) users      (100)    13548 2023-05-05 02:18:26.000000 bioplotz-0.1.0.dev5/README.md
+drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-08 07:23:09.501732 bioplotz-0.1.0.dev5/bioplotz/
+-rw-r--r--   0 zsc       (1000) users      (100)      225 2023-05-08 07:21:48.000000 bioplotz-0.1.0.dev5/bioplotz/__init__.py
+-rw-r--r--   0 zsc       (1000) users      (100)    10185 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev5/bioplotz/chromosome.py
+-rw-r--r--   0 zsc       (1000) users      (100)     2477 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev5/bioplotz/genecluster.py
+-rwxr-xr-x   0 zsc       (1000) users      (100)     6110 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev5/bioplotz/manhattan.py
+-rw-r--r--   0 zsc       (1000) users      (100)     4706 2023-05-08 07:20:31.000000 bioplotz-0.1.0.dev5/bioplotz/mulitalign.py
+drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-08 07:23:09.505732 bioplotz-0.1.0.dev5/bioplotz.egg-info/
+-rw-r--r--   0 zsc       (1000) users      (100)    13845 2023-05-08 07:23:09.000000 bioplotz-0.1.0.dev5/bioplotz.egg-info/PKG-INFO
+-rw-r--r--   0 zsc       (1000) users      (100)      310 2023-05-08 07:23:09.000000 bioplotz-0.1.0.dev5/bioplotz.egg-info/SOURCES.txt
+-rw-r--r--   0 zsc       (1000) users      (100)        1 2023-05-08 07:23:09.000000 bioplotz-0.1.0.dev5/bioplotz.egg-info/dependency_links.txt
+-rw-r--r--   0 zsc       (1000) users      (100)       24 2023-05-08 07:23:09.000000 bioplotz-0.1.0.dev5/bioplotz.egg-info/requires.txt
+-rw-r--r--   0 zsc       (1000) users      (100)        9 2023-05-08 07:23:09.000000 bioplotz-0.1.0.dev5/bioplotz.egg-info/top_level.txt
+-rw-r--r--   0 zsc       (1000) users      (100)       38 2023-05-08 07:23:09.505732 bioplotz-0.1.0.dev5/setup.cfg
+-rw-r--r--   0 zsc       (1000) users      (100)      643 2023-05-08 07:21:45.000000 bioplotz-0.1.0.dev5/setup.py
```

### Comparing `bioplotz-0.1.0.dev4/LICENSE` & `bioplotz-0.1.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev4/PKG-INFO` & `bioplotz-0.1.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioplotz
-Version: 0.1.0.dev4
+Version: 0.1.0.dev5
 Summary: A python package for drawing some bioinformatic pictures.
 Home-page: https://github.com/sc-zhang/bioplotz
 Author: Shengcheng Zhang
 Author-email: zsc-zhang@foxmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bioplotz-0.1.0.dev4/README.md` & `bioplotz-0.1.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev4/bioplotz/chromosome.py` & `bioplotz-0.1.0.dev5/bioplotz/chromosome.py`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev4/bioplotz/genecluster.py` & `bioplotz-0.1.0.dev5/bioplotz/genecluster.py`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev4/bioplotz/manhattan.py` & `bioplotz-0.1.0.dev5/bioplotz/manhattan.py`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev4/bioplotz/mulitalign.py` & `bioplotz-0.1.0.dev5/bioplotz/mulitalign.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,18 @@
                  base_per_line: int = 80,
                  highlight_positions: list = None,
                  highlight_color: any = 'green'):
         self.__data = data
         self.__match_color = match_color
         self.__mismatch_color = mismatch_color
         self.__base_per_line = base_per_line
-        self.__highlight_positions = set(highlight_positions)
+        if highlight_positions:
+            self.__highlight_positions = set(highlight_positions)
+        else:
+            self.__highlight_positions = None
         self.__highlight_color = highlight_color
 
     @staticmethod
     def __rainbow_text(x, y, strings, colors, ax=None, **kwargs):
         """
         Take a list of *strings* and *colors* and place them next to each
         other, with text strings[i] being shown in colors[i].
@@ -87,15 +90,15 @@
 
             for k in range(sp, ep):
                 cur_set = set()
                 for j in sorted(self.__data):
                     cur_set.add(self.__data[j][k])
                 if len(cur_set) > 1:
                     colors[k - sp] = self.__mismatch_color
-                if k in self.__highlight_positions:
+                if self.__highlight_positions and k in self.__highlight_positions:
                     colors[k - sp] = self.__highlight_color
             for j in range(seq_cnt):
                 gid = seq_list[j]
                 y_ticks.append(i * (seq_cnt + 2) + j + 1)
                 y_labels.append(gid)
                 self.__rainbow_text(0, i * (seq_cnt + 2) + j + 1, self.__data[gid][sp: ep], colors, **kwargs)
         ax.set_ylim(0, total_row_cnt)
```

### Comparing `bioplotz-0.1.0.dev4/bioplotz.egg-info/PKG-INFO` & `bioplotz-0.1.0.dev5/bioplotz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioplotz
-Version: 0.1.0.dev4
+Version: 0.1.0.dev5
 Summary: A python package for drawing some bioinformatic pictures.
 Home-page: https://github.com/sc-zhang/bioplotz
 Author: Shengcheng Zhang
 Author-email: zsc-zhang@foxmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bioplotz-0.1.0.dev4/setup.py` & `bioplotz-0.1.0.dev5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='bioplotz',
-    version='0.1.0.dev4',
+    version='0.1.0.dev5',
     packages=['bioplotz'],
     url='https://github.com/sc-zhang/bioplotz',
     license='',
     author='Shengcheng Zhang',
     author_email='zsc-zhang@foxmail.com',
     description='A python package for drawing some bioinformatic pictures.',
     long_description=long_description,
```

