# Comparing `tmp/xcpcio_board_spider-0.0.8.tar.gz` & `tmp/xcpcio_board_spider-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcpcio_board_spider-0.0.8.tar", max compression
+gzip compressed data, was "xcpcio_board_spider-0.0.9.tar", max compression
```

## Comparing `xcpcio_board_spider-0.0.8.tar` & `xcpcio_board_spider-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1063 2023-05-05 16:17:38.797640 xcpcio_board_spider-0.0.8/LICENSE
--rw-r--r--   0        0        0      538 2023-05-05 16:17:38.797640 xcpcio_board_spider-0.0.8/README.md
--rw-r--r--   0        0        0     1004 2023-05-05 16:17:38.801640 xcpcio_board_spider-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       40 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/__init__.py
--rw-r--r--   0        0        0       34 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/core/__init__.py
--rw-r--r--   0        0        0      377 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/core/logger.py
--rw-r--r--   0        0        0     1074 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/core/logo.py
--rw-r--r--   0        0        0     1863 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/core/utils.py
--rw-r--r--   0        0        0        0 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/spider/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/spider/domjudge/__init__.py
--rw-r--r--   0        0        0       24 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/spider/domjudge/v2/__init__.py
--rw-r--r--   0        0        0     5319 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/spider/domjudge/v2/domjudge.py
--rw-r--r--   0        0        0      113 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/type/__init__.py
--rw-r--r--   0        0        0      303 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/type/constants.py
--rw-r--r--   0        0        0     3288 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/type/contest.py
--rw-r--r--   0        0        0     1020 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/type/submission.py
--rw-r--r--   0        0        0     1555 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/type/team.py
--rw-r--r--   0        0        0      262 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/type/type.py
--rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 xcpcio_board_spider-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-07 15:28:11.847542 xcpcio_board_spider-0.0.9/LICENSE
+-rw-r--r--   0        0        0      538 2023-05-07 15:28:11.847542 xcpcio_board_spider-0.0.9/README.md
+-rw-r--r--   0        0        0     1004 2023-05-07 15:28:11.851542 xcpcio_board_spider-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-05-07 15:28:11.891542 xcpcio_board_spider-0.0.9/xcpcio_board_spider/__init__.py
+-rw-r--r--   0        0        0       34 2023-05-07 15:28:11.891542 xcpcio_board_spider-0.0.9/xcpcio_board_spider/core/__init__.py
+-rw-r--r--   0        0        0      377 2023-05-07 15:28:11.891542 xcpcio_board_spider-0.0.9/xcpcio_board_spider/core/logger.py
+-rw-r--r--   0        0        0     1074 2023-05-07 15:28:11.891542 xcpcio_board_spider-0.0.9/xcpcio_board_spider/core/logo.py
+-rw-r--r--   0        0        0     1863 2023-05-07 15:28:11.891542 xcpcio_board_spider-0.0.9/xcpcio_board_spider/core/utils.py
+-rw-r--r--   0        0        0        0 2023-05-07 15:28:11.891542 xcpcio_board_spider-0.0.9/xcpcio_board_spider/spider/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 15:28:11.891542 xcpcio_board_spider-0.0.9/xcpcio_board_spider/spider/domjudge/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-07 15:28:11.891542 xcpcio_board_spider-0.0.9/xcpcio_board_spider/spider/domjudge/v2/__init__.py
+-rw-r--r--   0        0        0     5319 2023-05-07 15:28:11.891542 xcpcio_board_spider-0.0.9/xcpcio_board_spider/spider/domjudge/v2/domjudge.py
+-rw-r--r--   0        0        0      113 2023-05-07 15:28:11.891542 xcpcio_board_spider-0.0.9/xcpcio_board_spider/type/__init__.py
+-rw-r--r--   0        0        0      303 2023-05-07 15:28:11.891542 xcpcio_board_spider-0.0.9/xcpcio_board_spider/type/constants.py
+-rw-r--r--   0        0        0     3330 2023-05-07 15:28:11.891542 xcpcio_board_spider-0.0.9/xcpcio_board_spider/type/contest.py
+-rw-r--r--   0        0        0     1020 2023-05-07 15:28:11.895542 xcpcio_board_spider-0.0.9/xcpcio_board_spider/type/submission.py
+-rw-r--r--   0        0        0     1555 2023-05-07 15:28:11.895542 xcpcio_board_spider-0.0.9/xcpcio_board_spider/type/team.py
+-rw-r--r--   0        0        0      262 2023-05-07 15:28:11.895542 xcpcio_board_spider-0.0.9/xcpcio_board_spider/type/type.py
+-rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 xcpcio_board_spider-0.0.9/PKG-INFO
```

### Comparing `xcpcio_board_spider-0.0.8/LICENSE` & `xcpcio_board_spider-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xcpcio_board_spider-0.0.8/README.md` & `xcpcio_board_spider-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `xcpcio_board_spider-0.0.8/pyproject.toml` & `xcpcio_board_spider-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xcpcio-board-spider"
-version = "0.0.8"
+version = "0.0.9"
 description = "XCPCIO Board Spider"
 authors = ["Dup4 <lyuzhi.pan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `xcpcio_board_spider-0.0.8/xcpcio_board_spider/core/logo.py` & `xcpcio_board_spider-0.0.9/xcpcio_board_spider/core/logo.py`

 * *Files identical despite different names*

### Comparing `xcpcio_board_spider-0.0.8/xcpcio_board_spider/core/utils.py` & `xcpcio_board_spider-0.0.9/xcpcio_board_spider/core/utils.py`

 * *Files identical despite different names*

### Comparing `xcpcio_board_spider-0.0.8/xcpcio_board_spider/spider/domjudge/v2/domjudge.py` & `xcpcio_board_spider-0.0.9/xcpcio_board_spider/spider/domjudge/v2/domjudge.py`

 * *Files identical despite different names*

### Comparing `xcpcio_board_spider-0.0.8/xcpcio_board_spider/type/contest.py` & `xcpcio_board_spider-0.0.9/xcpcio_board_spider/type/contest.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
         else:
             self.logo = None
 
     def fill_problem_id(self):
         self.problem_id = [chr(ord('A') + i)
                            for i in range(self.problem_quantity)]
 
+        return self
+
     def fill_balloon_color(self):
         default_balloon_color_list = [
             Color(background_color='rgba(189, 14, 14, 0.7)', color='#fff'),
             Color(background_color='rgba(255, 144, 228, 0.7)', color='#fff'),
             Color(background_color='rgba(255, 255, 255, 0.7)', color='#000'),
             Color(background_color='rgba(38, 185, 60, 0.7)', color='#fff'),
             Color(background_color='rgba(239, 217, 9, 0.7)', color='#000'),
@@ -56,14 +58,16 @@
             Color(background_color='rgba(42, 197, 202, 0.7)', color='#fff'),
             Color(background_color='rgba(142, 56, 54, 0.7)', color='#fff'),
             Color(background_color='rgba(0, 0, 0, 0.7)', color='#fff'),
         ]
 
         self.balloon_color = default_balloon_color_list[:self.problem_quantity]
 
+        return self
+
     @property
     def __json__(self):
         json_obj = {}
 
         json_obj["contest_name"] = self.contest_name
         json_obj["start_time"] = self.start_time
         json_obj["end_time"] = self.end_time
```

### Comparing `xcpcio_board_spider-0.0.8/xcpcio_board_spider/type/submission.py` & `xcpcio_board_spider-0.0.9/xcpcio_board_spider/type/submission.py`

 * *Files identical despite different names*

### Comparing `xcpcio_board_spider-0.0.8/xcpcio_board_spider/type/team.py` & `xcpcio_board_spider-0.0.9/xcpcio_board_spider/type/team.py`

 * *Files identical despite different names*

### Comparing `xcpcio_board_spider-0.0.8/PKG-INFO` & `xcpcio_board_spider-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcpcio-board-spider
-Version: 0.0.8
+Version: 0.0.9
 Summary: XCPCIO Board Spider
 License: MIT
 Author: Dup4
 Author-email: lyuzhi.pan@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

