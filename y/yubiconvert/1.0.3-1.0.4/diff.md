# Comparing `tmp/yubiconvert-1.0.3.tar.gz` & `tmp/yubiconvert-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yubiconvert-1.0.3.tar", last modified: Mon May  8 04:31:31 2023, max compression
+gzip compressed data, was "yubiconvert-1.0.4.tar", last modified: Mon May  8 07:27:26 2023, max compression
```

## Comparing `yubiconvert-1.0.3.tar` & `yubiconvert-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 darshan.patel   (502) staff       (20)        0 2023-05-08 04:31:31.769988 yubiconvert-1.0.3/
--rw-r--r--   0 darshan.patel   (502) staff       (20)     1071 2023-04-05 10:16:57.000000 yubiconvert-1.0.3/LICENSE
--rw-r--r--   0 darshan.patel   (502) staff       (20)     2540 2023-05-08 04:31:31.769767 yubiconvert-1.0.3/PKG-INFO
--rw-r--r--   0 darshan.patel   (502) staff       (20)     1679 2023-04-05 10:16:57.000000 yubiconvert-1.0.3/README.md
--rw-r--r--   0 darshan.patel   (502) staff       (20)       38 2023-05-08 04:31:31.770037 yubiconvert-1.0.3/setup.cfg
--rw-r--r--   0 darshan.patel   (502) staff       (20)      975 2023-05-08 04:31:12.000000 yubiconvert-1.0.3/setup.py
-drwxr-xr-x   0 darshan.patel   (502) staff       (20)        0 2023-05-08 04:31:31.765088 yubiconvert-1.0.3/yubiconvert/
--rw-r--r--   0 darshan.patel   (502) staff       (20)        0 2023-04-05 10:16:57.000000 yubiconvert-1.0.3/yubiconvert/__init__.py
--rw-r--r--   0 darshan.patel   (502) staff       (20)    11503 2023-05-08 04:30:23.000000 yubiconvert-1.0.3/yubiconvert/yubiconvert.py
-drwxr-xr-x   0 darshan.patel   (502) staff       (20)        0 2023-05-08 04:31:31.769431 yubiconvert-1.0.3/yubiconvert.egg-info/
--rw-r--r--   0 darshan.patel   (502) staff       (20)     2540 2023-05-08 04:31:31.000000 yubiconvert-1.0.3/yubiconvert.egg-info/PKG-INFO
--rw-r--r--   0 darshan.patel   (502) staff       (20)      251 2023-05-08 04:31:31.000000 yubiconvert-1.0.3/yubiconvert.egg-info/SOURCES.txt
--rw-r--r--   0 darshan.patel   (502) staff       (20)        1 2023-05-08 04:31:31.000000 yubiconvert-1.0.3/yubiconvert.egg-info/dependency_links.txt
--rw-r--r--   0 darshan.patel   (502) staff       (20)        5 2023-05-08 04:31:31.000000 yubiconvert-1.0.3/yubiconvert.egg-info/requires.txt
--rw-r--r--   0 darshan.patel   (502) staff       (20)       12 2023-05-08 04:31:31.000000 yubiconvert-1.0.3/yubiconvert.egg-info/top_level.txt
+drwxr-xr-x   0 darshan.patel   (502) staff       (20)        0 2023-05-08 07:27:26.524585 yubiconvert-1.0.4/
+-rw-r--r--   0 darshan.patel   (502) staff       (20)     1071 2023-04-05 10:16:57.000000 yubiconvert-1.0.4/LICENSE
+-rw-r--r--   0 darshan.patel   (502) staff       (20)     2540 2023-05-08 07:27:26.524338 yubiconvert-1.0.4/PKG-INFO
+-rw-r--r--   0 darshan.patel   (502) staff       (20)     1679 2023-04-05 10:16:57.000000 yubiconvert-1.0.4/README.md
+-rw-r--r--   0 darshan.patel   (502) staff       (20)       38 2023-05-08 07:27:26.524655 yubiconvert-1.0.4/setup.cfg
+-rw-r--r--   0 darshan.patel   (502) staff       (20)      975 2023-05-08 07:26:56.000000 yubiconvert-1.0.4/setup.py
+drwxr-xr-x   0 darshan.patel   (502) staff       (20)        0 2023-05-08 07:27:26.521088 yubiconvert-1.0.4/yubiconvert/
+-rw-r--r--   0 darshan.patel   (502) staff       (20)        0 2023-04-05 10:16:57.000000 yubiconvert-1.0.4/yubiconvert/__init__.py
+-rw-r--r--   0 darshan.patel   (502) staff       (20)    11355 2023-05-08 07:27:00.000000 yubiconvert-1.0.4/yubiconvert/yubiconvert.py
+drwxr-xr-x   0 darshan.patel   (502) staff       (20)        0 2023-05-08 07:27:26.523934 yubiconvert-1.0.4/yubiconvert.egg-info/
+-rw-r--r--   0 darshan.patel   (502) staff       (20)     2540 2023-05-08 07:27:26.000000 yubiconvert-1.0.4/yubiconvert.egg-info/PKG-INFO
+-rw-r--r--   0 darshan.patel   (502) staff       (20)      251 2023-05-08 07:27:26.000000 yubiconvert-1.0.4/yubiconvert.egg-info/SOURCES.txt
+-rw-r--r--   0 darshan.patel   (502) staff       (20)        1 2023-05-08 07:27:26.000000 yubiconvert-1.0.4/yubiconvert.egg-info/dependency_links.txt
+-rw-r--r--   0 darshan.patel   (502) staff       (20)        5 2023-05-08 07:27:26.000000 yubiconvert-1.0.4/yubiconvert.egg-info/requires.txt
+-rw-r--r--   0 darshan.patel   (502) staff       (20)       12 2023-05-08 07:27:26.000000 yubiconvert-1.0.4/yubiconvert.egg-info/top_level.txt
```

### Comparing `yubiconvert-1.0.3/LICENSE` & `yubiconvert-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yubiconvert-1.0.3/PKG-INFO` & `yubiconvert-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yubiconvert
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python module that can convert numeric words to their numerical form effortlessly
 Home-page: https://github.com/Yubi2Community/yubiconvert
 Author: Yubi Data Science Team
 Author-email: data@go-yubi.com
 License: MIT
 Description: # YubiConvert
```

### Comparing `yubiconvert-1.0.3/README.md` & `yubiconvert-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `yubiconvert-1.0.3/setup.py` & `yubiconvert-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "function to open file"
     return open(os.path.join(os.path.dirname(__file__), fname))
 
 
 setup(
     name="yubiconvert",
     packages=["yubiconvert"],  # this must be the same as the name above
-    version="1.0.3",
+    version="1.0.4",
     license="MIT",
     description="Python module that can convert numeric words to their numerical form effortlessly",
     author="Yubi Data Science Team",
     author_email="data@go-yubi.com",
     url="https://github.com/Yubi2Community/yubiconvert",
     keywords=[
         "numbers",
```

### Comparing `yubiconvert-1.0.3/yubiconvert/yubiconvert.py` & `yubiconvert-1.0.4/yubiconvert/yubiconvert.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,18 +47,24 @@
 common_place_names = {
     "dozen": 12,
     "score": 20,
     "hundred": 100,
     "hundreds": 100,
     "gross": 144,
     "thousand": 1_000,
-    "thousands": 1_000
+    "thousands": 1_000,
 }
 
-indian_place_names = {"lakh": 1_00_000,"lakhs": 1_00_000 ,"lac": 1_00_000, "crore": 1_00_00_000, "crores": 1_00_00_000}
+indian_place_names = {
+    "lakh": 1_00_000,
+    "lakhs": 1_00_000,
+    "lac": 1_00_000,
+    "crore": 1_00_00_000,
+    "crores": 1_00_00_000,
+}
 us_place_names = {
     "million": 1_000_000,
     "billion": 1_000_000_000,
     "trillion": 1_000_000_000_000,
     "quadrillion": 1_000_000_000_000_000,
     "quintillion": 1_000_000_000_000_000_000,
     "sextillion": 1_000_000_000_000_000_000_000,
@@ -222,15 +228,17 @@
         int/float: numeric value of input string
     """
     if not isinstance(phrase, str):
         raise ValueError(
             "Type of input is not string! Please enter a valid number word (eg. 'two million twenty three thousand and forty nine')"
         )
     phrase = phrase.lower()
-    phrase = phrase.replace("rupees", "rupee").replace('paise','paisa').replace('only','')
+    phrase = (
+        phrase.replace("rupees", "rupee").replace("paise", "paisa").replace("only", "")
+    )
     count_indian_standards = 0
     count_us_standards = 0
     for i in phrase.split():
         if i in indian_place_abbrev or i in indian_place_names:
             count_indian_standards += 1
         elif i in us_place_abbrev or i in us_place_names:
             count_us_standards += 1
@@ -308,21 +316,15 @@
     """
     if not isinstance(text, str):
         raise ValueError("Only String format is supported")
     text = " ".join([number_to_word.get(i, i) for i in text.lower().strip().split(" ")])
     if text.find("-") not in [-1, 0]:
         text = text.replace("-", " ")
     tagged_number_words = " ".join([f"{i}/CD" for i in word_to_number])
-    tagged_number_words += (
-<<<<<<< HEAD
-        " a/CD and/CD &/CD rs/CD rupee/CD rupees/CD paisa/CD cent/CD cents/CD paise/CD only/CD"
-=======
-        " a/CD and/CD &/CD rs/CD rupee/CD rupees/CD paisa/CD cent/CD cents/CD paise/CD"
->>>>>>> 7c2b760 (Added a word paise to handle fracitonal amount)
-    )
+    tagged_number_words += " a/CD and/CD &/CD rs/CD rupee/CD rupees/CD paisa/CD cent/CD cents/CD paise/CD only/CD"
     tagged_number_words_tuples = [
         nltk.tag.str2tuple(t) for t in tagged_number_words.split()
     ]
     my_tagger = nltk.UnigramTagger(
         [tagged_number_words_tuples], backoff=nltk.DefaultTagger("IGNORE")
     )
 
@@ -341,8 +343,7 @@
 
             num = _word_to_num(" ".join(ut))
             regex = re.compile(re.escape(" ".join(ut)), re.IGNORECASE)
             text = regex.sub(str(num), text, 1)
         except Exception as exp:
             raise exp
     return text
-
```

### Comparing `yubiconvert-1.0.3/yubiconvert.egg-info/PKG-INFO` & `yubiconvert-1.0.4/yubiconvert.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yubiconvert
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python module that can convert numeric words to their numerical form effortlessly
 Home-page: https://github.com/Yubi2Community/yubiconvert
 Author: Yubi Data Science Team
 Author-email: data@go-yubi.com
 License: MIT
 Description: # YubiConvert
```

