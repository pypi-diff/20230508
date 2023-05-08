# Comparing `tmp/balladeer-0.8.0.tar.gz` & `tmp/balladeer-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balladeer-0.8.0.tar", last modified: Sun Oct 24 14:52:59 2021, max compression
+gzip compressed data, was "balladeer-0.9.0.tar", last modified: Sun Oct 24 16:07:47 2021, max compression
```

## Comparing `balladeer-0.8.0.tar` & `balladeer-0.9.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 boss      (1000) boss      (1000)        0 2021-10-24 14:52:59.384487 balladeer-0.8.0/
--rw-rw-r--   0 boss      (1000) boss      (1000)      204 2021-10-24 14:49:15.000000 balladeer-0.8.0/CHANGELOG.rst
--rw-rw-r--   0 boss      (1000) boss      (1000)    35141 2021-06-06 14:07:36.000000 balladeer-0.8.0/LICENSE
--rw-rw-r--   0 boss      (1000) boss      (1000)      118 2021-06-06 14:07:36.000000 balladeer-0.8.0/MANIFEST.in
--rw-rw-r--   0 boss      (1000) boss      (1000)      907 2021-10-24 14:52:59.384487 balladeer-0.8.0/PKG-INFO
--rw-rw-r--   0 boss      (1000) boss      (1000)      344 2021-06-06 14:07:36.000000 balladeer-0.8.0/README.rst
-drwxrwxr-x   0 boss      (1000) boss      (1000)        0 2021-10-24 14:52:59.380487 balladeer-0.8.0/balladeer/
--rw-rw-r--   0 boss      (1000) boss      (1000)     1138 2021-10-24 14:50:38.000000 balladeer-0.8.0/balladeer/__init__.py
-drwxrwxr-x   0 boss      (1000) boss      (1000)        0 2021-10-24 14:52:59.380487 balladeer-0.8.0/balladeer/doc/
--rw-rw-r--   0 boss      (1000) boss      (1000)        0 2021-10-17 11:45:12.000000 balladeer-0.8.0/balladeer/doc/index.rst
--rw-rw-r--   0 boss      (1000) boss      (1000)     2581 2021-10-22 12:33:23.000000 balladeer-0.8.0/balladeer/drama.py
--rw-rw-r--   0 boss      (1000) boss      (1000)     3351 2021-10-24 13:24:05.000000 balladeer-0.8.0/balladeer/gesture.py
--rw-rw-r--   0 boss      (1000) boss      (1000)     1596 2021-10-23 10:32:34.000000 balladeer-0.8.0/balladeer/speech.py
--rw-rw-r--   0 boss      (1000) boss      (1000)     3134 2021-10-22 08:15:46.000000 balladeer-0.8.0/balladeer/story.py
-drwxrwxr-x   0 boss      (1000) boss      (1000)        0 2021-10-24 14:52:59.384487 balladeer-0.8.0/balladeer/test/
--rw-rw-r--   0 boss      (1000) boss      (1000)        0 2021-06-06 14:07:36.000000 balladeer-0.8.0/balladeer/test/__init__.py
--rw-rw-r--   0 boss      (1000) boss      (1000)     2632 2021-10-22 10:29:04.000000 balladeer-0.8.0/balladeer/test/test_drama.py
--rw-rw-r--   0 boss      (1000) boss      (1000)     5035 2021-10-24 13:27:47.000000 balladeer-0.8.0/balladeer/test/test_gesture.py
--rw-rw-r--   0 boss      (1000) boss      (1000)     1399 2021-10-23 10:03:57.000000 balladeer-0.8.0/balladeer/test/test_speech.py
--rw-rw-r--   0 boss      (1000) boss      (1000)     2462 2021-10-23 10:26:10.000000 balladeer-0.8.0/balladeer/types.py
-drwxrwxr-x   0 boss      (1000) boss      (1000)        0 2021-10-24 14:52:59.384487 balladeer-0.8.0/balladeer.egg-info/
--rw-rw-r--   0 boss      (1000) boss      (1000)      907 2021-10-24 14:52:59.000000 balladeer-0.8.0/balladeer.egg-info/PKG-INFO
--rw-rw-r--   0 boss      (1000) boss      (1000)      583 2021-10-24 14:52:59.000000 balladeer-0.8.0/balladeer.egg-info/SOURCES.txt
--rw-rw-r--   0 boss      (1000) boss      (1000)        1 2021-10-24 14:52:59.000000 balladeer-0.8.0/balladeer.egg-info/dependency_links.txt
--rw-rw-r--   0 boss      (1000) boss      (1000)       58 2021-10-24 14:52:59.000000 balladeer-0.8.0/balladeer.egg-info/requires.txt
--rw-rw-r--   0 boss      (1000) boss      (1000)       10 2021-10-24 14:52:59.000000 balladeer-0.8.0/balladeer.egg-info/top_level.txt
--rw-rw-r--   0 boss      (1000) boss      (1000)        1 2021-10-17 14:32:28.000000 balladeer-0.8.0/balladeer.egg-info/zip-safe
-drwxrwxr-x   0 boss      (1000) boss      (1000)        0 2021-10-24 14:52:59.380487 balladeer-0.8.0/build/
-drwxrwxr-x   0 boss      (1000) boss      (1000)        0 2021-10-24 14:52:59.380487 balladeer-0.8.0/build/lib/
-drwxrwxr-x   0 boss      (1000) boss      (1000)        0 2021-10-24 14:52:59.380487 balladeer-0.8.0/build/lib/balladeer/
-drwxrwxr-x   0 boss      (1000) boss      (1000)        0 2021-10-24 14:52:59.380487 balladeer-0.8.0/build/lib/balladeer/doc/
--rw-rw-r--   0 boss      (1000) boss      (1000)        0 2021-10-17 11:45:12.000000 balladeer-0.8.0/build/lib/balladeer/doc/index.rst
--rw-rw-r--   0 boss      (1000) boss      (1000)       38 2021-10-24 14:52:59.384487 balladeer-0.8.0/setup.cfg
--rw-rw-r--   0 boss      (1000) boss      (1000)     1881 2021-10-20 13:47:52.000000 balladeer-0.8.0/setup.py
+drwxrwxr-x   0 boss      (1000) boss      (1000)        0 2021-10-24 16:07:47.506843 balladeer-0.9.0/
+-rw-rw-r--   0 boss      (1000) boss      (1000)      204 2021-10-24 14:49:15.000000 balladeer-0.9.0/CHANGELOG.rst
+-rw-rw-r--   0 boss      (1000) boss      (1000)    35141 2021-06-06 14:07:36.000000 balladeer-0.9.0/LICENSE
+-rw-rw-r--   0 boss      (1000) boss      (1000)      118 2021-06-06 14:07:36.000000 balladeer-0.9.0/MANIFEST.in
+-rw-rw-r--   0 boss      (1000) boss      (1000)      907 2021-10-24 16:07:47.506843 balladeer-0.9.0/PKG-INFO
+-rw-rw-r--   0 boss      (1000) boss      (1000)      344 2021-06-06 14:07:36.000000 balladeer-0.9.0/README.rst
+drwxrwxr-x   0 boss      (1000) boss      (1000)        0 2021-10-24 16:07:47.502843 balladeer-0.9.0/balladeer/
+-rw-rw-r--   0 boss      (1000) boss      (1000)     1138 2021-10-24 16:05:11.000000 balladeer-0.9.0/balladeer/__init__.py
+drwxrwxr-x   0 boss      (1000) boss      (1000)        0 2021-10-24 16:07:47.502843 balladeer-0.9.0/balladeer/doc/
+-rw-rw-r--   0 boss      (1000) boss      (1000)        0 2021-10-17 11:45:12.000000 balladeer-0.9.0/balladeer/doc/index.rst
+-rw-rw-r--   0 boss      (1000) boss      (1000)     2581 2021-10-22 12:33:23.000000 balladeer-0.9.0/balladeer/drama.py
+-rw-rw-r--   0 boss      (1000) boss      (1000)     3402 2021-10-24 15:59:59.000000 balladeer-0.9.0/balladeer/gesture.py
+-rw-rw-r--   0 boss      (1000) boss      (1000)     1596 2021-10-23 10:32:34.000000 balladeer-0.9.0/balladeer/speech.py
+-rw-rw-r--   0 boss      (1000) boss      (1000)     3134 2021-10-22 08:15:46.000000 balladeer-0.9.0/balladeer/story.py
+drwxrwxr-x   0 boss      (1000) boss      (1000)        0 2021-10-24 16:07:47.506843 balladeer-0.9.0/balladeer/test/
+-rw-rw-r--   0 boss      (1000) boss      (1000)        0 2021-06-06 14:07:36.000000 balladeer-0.9.0/balladeer/test/__init__.py
+-rw-rw-r--   0 boss      (1000) boss      (1000)     2632 2021-10-22 10:29:04.000000 balladeer-0.9.0/balladeer/test/test_drama.py
+-rw-rw-r--   0 boss      (1000) boss      (1000)     5086 2021-10-24 16:03:54.000000 balladeer-0.9.0/balladeer/test/test_gesture.py
+-rw-rw-r--   0 boss      (1000) boss      (1000)     1399 2021-10-23 10:03:57.000000 balladeer-0.9.0/balladeer/test/test_speech.py
+-rw-rw-r--   0 boss      (1000) boss      (1000)     2462 2021-10-23 10:26:10.000000 balladeer-0.9.0/balladeer/types.py
+drwxrwxr-x   0 boss      (1000) boss      (1000)        0 2021-10-24 16:07:47.502843 balladeer-0.9.0/balladeer.egg-info/
+-rw-rw-r--   0 boss      (1000) boss      (1000)      907 2021-10-24 16:07:47.000000 balladeer-0.9.0/balladeer.egg-info/PKG-INFO
+-rw-rw-r--   0 boss      (1000) boss      (1000)      583 2021-10-24 16:07:47.000000 balladeer-0.9.0/balladeer.egg-info/SOURCES.txt
+-rw-rw-r--   0 boss      (1000) boss      (1000)        1 2021-10-24 16:07:47.000000 balladeer-0.9.0/balladeer.egg-info/dependency_links.txt
+-rw-rw-r--   0 boss      (1000) boss      (1000)       58 2021-10-24 16:07:47.000000 balladeer-0.9.0/balladeer.egg-info/requires.txt
+-rw-rw-r--   0 boss      (1000) boss      (1000)       10 2021-10-24 16:07:47.000000 balladeer-0.9.0/balladeer.egg-info/top_level.txt
+-rw-rw-r--   0 boss      (1000) boss      (1000)        1 2021-10-17 14:32:28.000000 balladeer-0.9.0/balladeer.egg-info/zip-safe
+drwxrwxr-x   0 boss      (1000) boss      (1000)        0 2021-10-24 16:07:47.498843 balladeer-0.9.0/build/
+drwxrwxr-x   0 boss      (1000) boss      (1000)        0 2021-10-24 16:07:47.502843 balladeer-0.9.0/build/lib/
+drwxrwxr-x   0 boss      (1000) boss      (1000)        0 2021-10-24 16:07:47.502843 balladeer-0.9.0/build/lib/balladeer/
+drwxrwxr-x   0 boss      (1000) boss      (1000)        0 2021-10-24 16:07:47.502843 balladeer-0.9.0/build/lib/balladeer/doc/
+-rw-rw-r--   0 boss      (1000) boss      (1000)        0 2021-10-17 11:45:12.000000 balladeer-0.9.0/build/lib/balladeer/doc/index.rst
+-rw-rw-r--   0 boss      (1000) boss      (1000)       38 2021-10-24 16:07:47.506843 balladeer-0.9.0/setup.cfg
+-rw-rw-r--   0 boss      (1000) boss      (1000)     1881 2021-10-20 13:47:52.000000 balladeer-0.9.0/setup.py
```

### Comparing `balladeer-0.8.0/LICENSE` & `balladeer-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `balladeer-0.8.0/PKG-INFO` & `balladeer-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balladeer
-Version: 0.8.0
+Version: 0.9.0
 Summary: Web-enabled interactive fiction in Python.
 Home-page: https://github.com/tundish/balladeer
 Author: D E Haynes
 Author-email: tundish@gigeconomy.org.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `balladeer-0.8.0/balladeer/__init__.py` & `balladeer-0.9.0/balladeer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 from balladeer.drama import Drama
 from balladeer.gesture import Gesture
 from balladeer.gesture import Hand
 from balladeer.gesture import Head
 from balladeer.speech import Article
 from balladeer.speech import Name
```

### Comparing `balladeer-0.8.0/balladeer/drama.py` & `balladeer-0.9.0/balladeer/drama.py`

 * *Files identical despite different names*

### Comparing `balladeer-0.8.0/balladeer/gesture.py` & `balladeer-0.9.0/balladeer/gesture.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,7 +92,11 @@
         else:
             return []
 
     def __call__(self, strategy=None, **kwargs):
         strategy = strategy or random.choice
         event, state = strategy(self.transitions)
         return self, event, state
+
+    def __str__(self):
+        return self.label
+
```

### Comparing `balladeer-0.8.0/balladeer/speech.py` & `balladeer-0.9.0/balladeer/speech.py`

 * *Files identical despite different names*

### Comparing `balladeer-0.8.0/balladeer/story.py` & `balladeer-0.9.0/balladeer/story.py`

 * *Files identical despite different names*

### Comparing `balladeer-0.8.0/balladeer/test/test_drama.py` & `balladeer-0.9.0/balladeer/test/test_drama.py`

 * *Files identical despite different names*

### Comparing `balladeer-0.8.0/balladeer/test/test_gesture.py` & `balladeer-0.9.0/balladeer/test/test_gesture.py`

 * *Files 7% similar despite different names*

```diff
@@ -107,17 +107,17 @@
         self.assertIs(a.propose, b.propose)  # Lest we forget
 
     def test_simple(self):
         g = Gesture("simple", head=Head([
             Phrase(Verb("make"), Name("tea")),
             Phrase(Verb("make"), Name("brew")),
         ]))
-        self.assertIn("make tea", str(g))
-        self.assertIn("\n", str(g))
-        self.assertIn("make brew", str(g))
+        self.assertEqual("simple", str(g))
+        self.assertEqual("make", g.head.propose[0].verb.imperative)
+        self.assertEqual("tea", g.head.propose[0].name.noun)
 
     def test_brew(self):
         brew = self.create_brew()
         while not (brew.passed or brew.failed):
             gesture, event, state = brew()
             gesture.state = state
```

### Comparing `balladeer-0.8.0/balladeer/test/test_speech.py` & `balladeer-0.9.0/balladeer/test/test_speech.py`

 * *Files identical despite different names*

### Comparing `balladeer-0.8.0/balladeer/types.py` & `balladeer-0.9.0/balladeer/types.py`

 * *Files identical despite different names*

### Comparing `balladeer-0.8.0/balladeer.egg-info/PKG-INFO` & `balladeer-0.9.0/balladeer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balladeer
-Version: 0.8.0
+Version: 0.9.0
 Summary: Web-enabled interactive fiction in Python.
 Home-page: https://github.com/tundish/balladeer
 Author: D E Haynes
 Author-email: tundish@gigeconomy.org.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `balladeer-0.8.0/balladeer.egg-info/SOURCES.txt` & `balladeer-0.9.0/balladeer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `balladeer-0.8.0/setup.py` & `balladeer-0.9.0/setup.py`

 * *Files identical despite different names*

