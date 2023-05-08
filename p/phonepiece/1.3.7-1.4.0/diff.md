# Comparing `tmp/phonepiece-1.3.7.tar.gz` & `tmp/phonepiece-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/phonepiece-1.3.7.tar", last modified: Tue Feb 14 03:40:35 2023, max compression
+gzip compressed data, was "dist/phonepiece-1.4.0.tar", last modified: Mon May  8 07:39:00 2023, max compression
```

## Comparing `phonepiece-1.3.7.tar` & `phonepiece-1.4.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-02-14 03:40:35.000000 phonepiece-1.3.7/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    22240 2022-11-27 22:18:32.000000 phonepiece-1.3.7/LICENSE.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      266 2023-02-14 03:40:35.000000 phonepiece-1.3.7/PKG-INFO
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     6041 2023-01-27 22:35:07.000000 phonepiece-1.3.7/README.md
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-02-14 03:40:34.000000 phonepiece-1.3.7/phonepiece/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       47 2022-09-01 15:22:55.000000 phonepiece-1.3.7/phonepiece/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      798 2022-11-28 20:55:03.000000 phonepiece-1.3.7/phonepiece/arpa.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-02-14 03:40:34.000000 phonepiece-1.3.7/phonepiece/bin/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:48:28.000000 phonepiece-1.3.7/phonepiece/bin/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1404 2022-09-08 18:19:22.000000 phonepiece-1.3.7/phonepiece/bin/download_model.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1479 2023-01-06 00:58:31.000000 phonepiece-1.3.7/phonepiece/bin/update_model.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      248 2022-11-28 19:48:04.000000 phonepiece-1.3.7/phonepiece/config.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-02-14 03:40:35.000000 phonepiece-1.3.7/phonepiece/data/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 18:20:26.000000 phonepiece-1.3.7/phonepiece/data/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      256 2021-06-23 15:57:09.000000 phonepiece-1.3.7/phonepiece/data/arpabet.csv
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     4351 2022-11-28 17:35:17.000000 phonepiece-1.3.7/phonepiece/data/ipa-xsampa.csv
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)   363488 2022-11-28 17:35:17.000000 phonepiece-1.3.7/phonepiece/data/ipa_all.csv
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7452 2023-02-14 03:40:22.000000 phonepiece-1.3.7/phonepiece/data/ipa_base.csv
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)   232037 2020-03-04 19:47:15.000000 phonepiece-1.3.7/phonepiece/data/language.tsv
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)   175859 2020-06-27 15:14:04.000000 phonepiece-1.3.7/phonepiece/data/phoible-segments-features.tsv
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      559 2022-11-23 19:56:36.000000 phonepiece-1.3.7/phonepiece/data/pinyin2ipa.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)   575995 2021-07-28 15:08:54.000000 phonepiece-1.3.7/phonepiece/data/tree.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     8547 2021-03-25 20:42:14.000000 phonepiece-1.3.7/phonepiece/edit_distance.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2115 2023-01-20 20:59:52.000000 phonepiece-1.3.7/phonepiece/epitran.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9113 2023-02-14 03:40:22.000000 phonepiece-1.3.7/phonepiece/inventory.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7098 2023-02-14 03:40:22.000000 phonepiece-1.3.7/phonepiece/ipa.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      757 2022-11-27 21:51:35.000000 phonepiece-1.3.7/phonepiece/iso.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2171 2022-11-27 22:16:15.000000 phonepiece-1.3.7/phonepiece/lexicon.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     4257 2023-01-23 20:09:34.000000 phonepiece-1.3.7/phonepiece/pinyin.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1380 2022-12-01 18:53:21.000000 phonepiece-1.3.7/phonepiece/timit.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2373 2022-08-31 22:28:12.000000 phonepiece-1.3.7/phonepiece/tree.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5613 2023-01-29 19:56:05.000000 phonepiece-1.3.7/phonepiece/unit.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1255 2022-11-28 20:51:39.000000 phonepiece-1.3.7/phonepiece/utils.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-02-14 03:40:34.000000 phonepiece-1.3.7/phonepiece.egg-info/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      266 2023-02-14 03:40:34.000000 phonepiece-1.3.7/phonepiece.egg-info/PKG-INFO
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      941 2023-02-14 03:40:34.000000 phonepiece-1.3.7/phonepiece.egg-info/SOURCES.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        1 2023-02-14 03:40:34.000000 phonepiece-1.3.7/phonepiece.egg-info/dependency_links.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       30 2023-02-14 03:40:34.000000 phonepiece-1.3.7/phonepiece.egg-info/requires.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       11 2023-02-14 03:40:34.000000 phonepiece-1.3.7/phonepiece.egg-info/top_level.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       38 2023-02-14 03:40:35.000000 phonepiece-1.3.7/setup.cfg
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      491 2023-02-14 03:40:22.000000 phonepiece-1.3.7/setup.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-02-14 03:40:35.000000 phonepiece-1.3.7/test/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      589 2023-01-20 21:23:48.000000 phonepiece-1.3.7/test/test_epitran.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1048 2023-01-29 19:58:17.000000 phonepiece-1.3.7/test/test_inventory.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1684 2023-02-14 03:40:22.000000 phonepiece-1.3.7/test/test_ipa.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      221 2023-01-06 00:52:08.000000 phonepiece-1.3.7/test/test_lexicon.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 07:39:00.000000 phonepiece-1.4.0/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    22240 2022-11-27 22:18:32.000000 phonepiece-1.4.0/LICENSE.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      266 2023-05-08 07:39:00.000000 phonepiece-1.4.0/PKG-INFO
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     6709 2023-05-08 07:38:53.000000 phonepiece-1.4.0/README.md
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 07:39:00.000000 phonepiece-1.4.0/phonepiece/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       47 2022-09-01 15:22:55.000000 phonepiece-1.4.0/phonepiece/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1896 2023-04-26 09:50:41.000000 phonepiece-1.4.0/phonepiece/arpa.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 07:39:00.000000 phonepiece-1.4.0/phonepiece/bin/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:48:28.000000 phonepiece-1.4.0/phonepiece/bin/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1404 2022-09-08 18:19:22.000000 phonepiece-1.4.0/phonepiece/bin/download_model.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     4402 2023-05-08 07:38:53.000000 phonepiece-1.4.0/phonepiece/bin/eval_distance.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1479 2023-01-06 00:58:31.000000 phonepiece-1.4.0/phonepiece/bin/update_model.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      248 2022-11-28 19:48:04.000000 phonepiece-1.4.0/phonepiece/config.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 07:39:00.000000 phonepiece-1.4.0/phonepiece/data/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 18:20:26.000000 phonepiece-1.4.0/phonepiece/data/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      256 2021-06-23 15:57:09.000000 phonepiece-1.4.0/phonepiece/data/arpabet.csv
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     4351 2022-11-28 17:35:17.000000 phonepiece-1.4.0/phonepiece/data/ipa-xsampa.csv
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)   363488 2022-11-28 17:35:17.000000 phonepiece-1.4.0/phonepiece/data/ipa_all.csv
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7452 2023-02-14 03:40:22.000000 phonepiece-1.4.0/phonepiece/data/ipa_base.csv
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)   232037 2020-03-04 19:47:15.000000 phonepiece-1.4.0/phonepiece/data/language.tsv
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)   175859 2020-06-27 15:14:04.000000 phonepiece-1.4.0/phonepiece/data/phoible-segments-features.tsv
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      559 2022-11-23 19:56:36.000000 phonepiece-1.4.0/phonepiece/data/pinyin2ipa.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)   575995 2021-07-28 15:08:54.000000 phonepiece-1.4.0/phonepiece/data/tree.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9598 2023-05-08 07:38:53.000000 phonepiece-1.4.0/phonepiece/distance.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2116 2023-05-08 07:38:53.000000 phonepiece-1.4.0/phonepiece/epitran.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9245 2023-05-08 07:38:53.000000 phonepiece-1.4.0/phonepiece/inventory.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7268 2023-05-08 07:38:53.000000 phonepiece-1.4.0/phonepiece/ipa.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3577 2023-05-08 07:38:53.000000 phonepiece-1.4.0/phonepiece/lang.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2731 2023-05-08 07:38:53.000000 phonepiece-1.4.0/phonepiece/lexicon.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     4257 2023-01-23 20:09:34.000000 phonepiece-1.4.0/phonepiece/pinyin.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1398 2023-02-17 19:39:59.000000 phonepiece-1.4.0/phonepiece/timit.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5613 2023-01-29 19:56:05.000000 phonepiece-1.4.0/phonepiece/unit.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1602 2023-05-08 07:38:53.000000 phonepiece-1.4.0/phonepiece/utils.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 07:39:00.000000 phonepiece-1.4.0/phonepiece.egg-info/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      266 2023-05-08 07:39:00.000000 phonepiece-1.4.0/phonepiece.egg-info/PKG-INFO
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      972 2023-05-08 07:39:00.000000 phonepiece-1.4.0/phonepiece.egg-info/SOURCES.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        1 2023-05-08 07:39:00.000000 phonepiece-1.4.0/phonepiece.egg-info/dependency_links.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       43 2023-05-08 07:39:00.000000 phonepiece-1.4.0/phonepiece.egg-info/requires.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       11 2023-05-08 07:39:00.000000 phonepiece-1.4.0/phonepiece.egg-info/top_level.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       38 2023-05-08 07:39:00.000000 phonepiece-1.4.0/setup.cfg
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      491 2023-05-08 07:38:53.000000 phonepiece-1.4.0/setup.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 07:39:00.000000 phonepiece-1.4.0/test/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      265 2023-05-08 07:38:53.000000 phonepiece-1.4.0/test/test_distance.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      589 2023-01-20 21:23:48.000000 phonepiece-1.4.0/test/test_epitran.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1048 2023-01-29 19:58:17.000000 phonepiece-1.4.0/test/test_inventory.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1684 2023-02-14 03:40:22.000000 phonepiece-1.4.0/test/test_ipa.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      221 2023-01-06 00:52:08.000000 phonepiece-1.4.0/test/test_lexicon.py
```

### Comparing `phonepiece-1.3.7/LICENSE.txt` & `phonepiece-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `phonepiece-1.3.7/README.md` & `phonepiece-1.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -92,28 +92,56 @@
              'ʌ': ['ʌ'],
              'ʒ': ['ʒ'],
              'θ': ['θ'],
              '<blk>': ['<blk>'],
              '<eos>': ['<eos>']})
 ```
 
-### Phonetics Utilities
+### Phone Tokenization
 
-This lib also provides a few phonetics utilities, for example, IPA manipulations
+This lib also provides a tokenizer which splits a concatenated IPA string into separate IPAs
 
 ```python
 In [1]: from phonepiece.ipa import read_ipa                                                         
 
 In [2]: ipa = read_ipa()                                                                            
 
 In [3]: ipa.tokenize('kʰæt')                                                                        
 Out[3]: ['kʰ', 'æ', 't']
+```
+
+### Phonological Distance
+
+The `phonological_distance` is an augmented edit distance, it takes phonological distance into account as well.
+
+```python
+In [1]: from phonepiece.distance import phonological_distance
+
+In [2]: phonological_distance('a', 'b')
+Out[2]: 0.5862068965517241
+
+In [3]: phonological_distance('a', 'e')
+Out[3]: 0.03448275862068961
+
+In [4]: phonological_distance('a', 'bc')
+Out[4]: 1.5862068965517242
+```
+
+### Lexicon Lookup
+
+It also includes many lexicon dictionaries, you can look up pronunciation of a particular word (if it exists)
+The output phonemes are consistent with its language's inventory phoneme space
+
+```
+In [1]: from phonepiece.lexicon import read_lexicon
+
+In [2]: eng = read_lexicon('eng')
 
-In [4]: ipa.similarity('a', 'e')                                                                    
-Out[4]: 0.9655172413793104
+In [3]: eng['hello']
+Out[3]: ['h', 'ʌ', 'l', 'o', 'w']
 ```
 
 ## Models
 
 | model | # supported languages |                                                                          description                                                                          |
 | :----: |:---------------------:|:-------------------------------------------------------------------------------------------------------------------------------------------------------------:|
 | phoible |          ~2k          | phone/phoneme databases extracted from [Phoible](https://phoible.org/) [1]. Allophone information is from [Allovera](https://github.com/dmort27/allovera) [3] |
```

### Comparing `phonepiece-1.3.7/phonepiece/bin/download_model.py` & `phonepiece-1.4.0/phonepiece/bin/download_model.py`

 * *Files identical despite different names*

### Comparing `phonepiece-1.3.7/phonepiece/bin/update_model.py` & `phonepiece-1.4.0/phonepiece/bin/update_model.py`

 * *Files identical despite different names*

### Comparing `phonepiece-1.3.7/phonepiece/data/ipa-xsampa.csv` & `phonepiece-1.4.0/phonepiece/data/ipa-xsampa.csv`

 * *Files identical despite different names*

### Comparing `phonepiece-1.3.7/phonepiece/data/ipa_all.csv` & `phonepiece-1.4.0/phonepiece/data/ipa_all.csv`

 * *Files identical despite different names*

### Comparing `phonepiece-1.3.7/phonepiece/data/ipa_base.csv` & `phonepiece-1.4.0/phonepiece/data/ipa_base.csv`

 * *Files identical despite different names*

### Comparing `phonepiece-1.3.7/phonepiece/data/language.tsv` & `phonepiece-1.4.0/phonepiece/data/language.tsv`

 * *Files identical despite different names*

### Comparing `phonepiece-1.3.7/phonepiece/data/phoible-segments-features.tsv` & `phonepiece-1.4.0/phonepiece/data/phoible-segments-features.tsv`

 * *Files identical despite different names*

### Comparing `phonepiece-1.3.7/phonepiece/data/pinyin2ipa.txt` & `phonepiece-1.4.0/phonepiece/data/pinyin2ipa.txt`

 * *Files identical despite different names*

### Comparing `phonepiece-1.3.7/phonepiece/data/tree.txt` & `phonepiece-1.4.0/phonepiece/data/tree.txt`

 * *Files identical despite different names*

### Comparing `phonepiece-1.3.7/phonepiece/edit_distance.py` & `phonepiece-1.4.0/phonepiece/distance.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import sys
+from phonepiece.ipa import read_ipa
+import editdistance
 
 def print_result(string_lst, out=None):
 
     res = ""
     for str in string_lst:
         res += '{0: >5}'.format(str)
 
@@ -38,18 +40,14 @@
     # dp update
     for i in range(1, len_b+1):
         for j in range(1, len_a+1):
             index_a = j-1
             index_b = i-1
             cost = 0 if string_a[index_a] == string_b[index_b] else 1
 
-            dx = 0
-            dy = 0
-            mincost = 0
-
             if dp[i-1][j][0] < dp[i][j-1][0]:
                 dx = -1
                 dy = 0
                 mincost = dp[i-1][j][0] + 1
             else:
                 dx = 0
                 dy = -1
@@ -85,14 +83,17 @@
         cy += dy
 
     best_start_index = cy
     best_end_index -= 1
 
     return mincost, best_start_index, best_end_index
 
+def fast_edit_distance(string_a, string_b):
+    return editdistance.distance(string_a, string_b)
+
 def edit_distance(string_a, string_b, utt_id='utt_id', verbose=False, out=None):
 
     # length of each string
     len_a = len(string_a)
     len_b = len(string_b)
 
     # dp table
@@ -174,16 +175,18 @@
         cur_node = prev_node
 
 
     if verbose:
 
         if out is None:
             out = sys.stdout
+
         out.write("-"*80+'\n')
-        out.write(f"UTT: {utt_id} - add {add_cnt}, del {del_cnt}, sub {sub_cnt}\n")
+        out.write(f"UTT: {utt_id}\n")
+        out.write(f"ERR {dp[len_b][len_a]}: ADD {add_cnt}, DEL {del_cnt}, SUB {sub_cnt}\n")
         hyp_lst.append("HYP: ")
         ref_lst.append("REF: ")
         ops_lst.append("OPS: ")
 
         hyp_lst.reverse()
         ref_lst.reverse()
         ops_lst.reverse()
@@ -191,15 +194,50 @@
         print_result(ref_lst, out)
         print_result(hyp_lst, out)
         print_result(ops_lst, out)
 
     return dp[len_b][len_a], add_cnt, del_cnt, sub_cnt, add_lst, del_lst, sub_lst
 
 
-def wer(string_a, string_b):
+def phonological_distance(string_a, string_b):
+
+    if ' '  in string_a:
+        string_a = string_a.split(' ')
+
+    if ' ' in string_b:
+        string_b = string_b.split(' ')
+
+    ipa = read_ipa()
+
+    # length of each string
+    len_a = len(string_a)
+    len_b = len(string_b)
+
+    # dp table
+    dp = [[0 for x in range(len_a+1)] for y in range(len_b+1)]
+
+    # initialize first row and first column
+    for i in range(len_a+1):
+        dp[0][i] = i
+
+    for i in range(len_b+1):
+        dp[i][0] = i
+
+    # dp update
+    for i in range(1, len_b+1):
+        for j in range(1, len_a+1):
+            index_a = j-1
+            index_b = i-1
+            sub_cost = ipa.distance(string_a[index_a], string_b[index_b])
+            dp[i][j] = min(dp[i-1][j-1]+sub_cost, min(dp[i-1][j]+1, dp[i][j-1]+1))
+
+    return dp[len_b][len_a]
+
+
+def naive_edit_distance(string_a, string_b):
 
     # length of each string
     len_a = len(string_a)
     len_b = len(string_b)
 
     # dp table
     dp = [[0 for x in range(len_a+1)] for y in range(len_b+1)]
@@ -218,15 +256,14 @@
             index_b = i-1
             cost = 0.0 if string_a[index_a] == string_b[index_b] else 1.0
             dp[i][j] = min(dp[i-1][j-1]+cost, min(dp[i-1][j]+1, dp[i][j-1]+1))
 
     return dp[len_b][len_a]
 
 
-
 def group_edit_distance(string_b, string_a, grp_dict, grp_err, grp_cnt):
     # length of each string
     len_a = len(string_a)
     len_b = len(string_b)
 
     # dp table
     dp = [[0 for x in range(len_a + 1)] for y in range(len_b + 1)]
@@ -292,34 +329,34 @@
     ans = dict()
     hyp = dict()
 
     grp_set = dict()
     grp_err = dict()
     grp_cnt = dict()
 
-    for line in open(ans_path):
+    for line in open(ans_path, 'r', encoding='utf-8'):
         utt_id, sent = line.split(' ', 1)
         words = sent.split()
 
         if '<unk>' in words:
             continue
 
         ans[utt_id] = words
 
 
-    for line in open(hyp_path):
+    for line in open(hyp_path, 'r', encoding='utf-8'):
         utt_id, sent = line.split(' ', 1)
         words = sent.split()
 
         if '<unk>' in words:
             continue
 
         hyp[utt_id] = words
 
-    for i, line in enumerate(open(grp_path)):
+    for i, line in enumerate(open(grp_path, 'r', encoding='utf-8')):
         phonemes = line.split()
 
         for phone in phonemes:
             grp_set[phone] = i
             grp_err[i] = 0
             grp_cnt[i] = 0
```

### Comparing `phonepiece-1.3.7/phonepiece/epitran.py` & `phonepiece-1.4.0/phonepiece/epitran.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from phonepiece.iso import normalize_lang_id
+from phonepiece.lang import normalize_lang_id
 from phonepiece.config import PhonePieceConfig
 from collections import defaultdict
 import unicodedata
 import csv
 from phonepiece.utils import load_lang_dir
 import re
 from phonepiece.ipa import read_ipa
```

### Comparing `phonepiece-1.3.7/phonepiece/inventory.py` & `phonepiece-1.4.0/phonepiece/inventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from phonepiece.config import *
 from phonepiece.unit import read_unit, write_unit, create_unit
 from phonepiece.ipa import read_ipa
-from phonepiece.iso import normalize_lang_id
+from phonepiece.lang import normalize_lang_id
 from collections import defaultdict
 from phonepiece.utils import load_lang_dir
 
 
 def read_inventory(lang_id_or_path, model_name='latest', base=False):
     """
     read inventory of the lang_id from a prebuilt inventory model or a customized local path
@@ -62,16 +62,19 @@
         fields = line.strip().split()
         phoneme = fields[0]
 
         for phone in fields[1:]:
             if base:
                 phone = ipa.compute_base_phone(phone)
 
-            phone2phoneme[phone].append(phoneme)
-            phoneme2phone[phoneme].append(phone)
+            if phoneme not in phone2phoneme[phone]:
+                phone2phoneme[phone].append(phoneme)
+
+            if phone not in phoneme2phone[phoneme]:
+                phoneme2phone[phoneme].append(phone)
 
     # blk and eos would be considered as phone/phonemes as well
     phone2phoneme['<blk>'] = ['<blk>']
     phone2phoneme['<eos>'] = ['<eos>']
     phoneme2phone['<blk>'] = ['<blk>']
     phoneme2phone['<eos>'] = ['<eos>']
 
@@ -110,15 +113,15 @@
     for k,v in inv.phone2phoneme.items():
         for phoneme in v:
             if phoneme not in allophone:
                 allophone[phoneme] = []
 
             allophone[phoneme].append(k)
 
-    w = open(inv_path / 'allophone.txt', 'w')
+    w = open(inv_path / 'allophone.txt', 'w', encoding='utf-8')
 
     for phoneme in inv.phoneme.elems[1:-1]:
         w.write(phoneme+' '+' '.join(allophone[phoneme])+'\n')
 
     w.close()
```

### Comparing `phonepiece-1.3.7/phonepiece/ipa.py` & `phonepiece-1.4.0/phonepiece/ipa.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     ('Y', 'ʏ'),
     ('ɚ', 'ə˞'),
     ('ɝ', 'ɜ˞'),
     ('ә', 'ə'),
     ('ˈ', ''),
     ('tʃ', 't͡ʃ'),
     ('dʒ','d͡ʒ'),
+    ('N', 'n'), # special handling for JPN N
     # tones: ˩˨˧˦˥
     ('˩', ''),
     ('˨', ''),
     ('˧', ''),
     ('˦', ''),
     ('˥', ''),
 ]
@@ -39,15 +40,15 @@
 
     feature_file = PhonePieceConfig.data_path / f'ipa_all.csv'
 
     feature_map = {'0': 0, '-': -1, '+': 1}
 
     phone2feature = {}
 
-    with open(feature_file) as csvfile:
+    with open(feature_file, 'r', encoding='utf-8') as csvfile:
         reader = csv.reader(csvfile)
 
         # This skips the first row of the CSV file.
         next(reader)
 
         for row in reader:
             phone = unicodedata.normalize('NFD', row[0])
@@ -60,15 +61,15 @@
        1,1,1,0.5,0.25,0.25,0.25,0.125,0.125,0.125,0.125,0.25,0.25,0.125,0.25,0.25,0.25,0.25,0.25,0.25,0.25,0.125,0,0
     ]
 
     assert len(weights) == 24
 
     base_phone_file = PhonePieceConfig.data_path / f'ipa_base.csv'
     base_phones = []
-    with open(base_phone_file) as csvfile:
+    with open(base_phone_file, 'r', encoding='utf-8') as csvfile:
         reader = csv.reader(csvfile)
 
         # This skips the first row of the CSV file.
         next(reader)
 
         for row in reader:
             phone = unicodedata.normalize('NFD', row[0])
@@ -137,15 +138,14 @@
                 if canonical_form is None:
                     canonical_form = min_phone
 
                 assert canonical_form is not None
                 for phone in phones:
                     self.canonical_phone[phone] = canonical_form
 
-
     def normalize(self, orig_phone):
         norm_phone = unicodedata.normalize('NFD', orig_phone)
 
         # normalize some easy mistakes
         for rule in _norm_rules:
             norm_phone = norm_phone.replace(rule[0], rule[1])
 
@@ -213,14 +213,19 @@
             return 0
 
         f1 = self.phone2feature[p1]
         f2 = self.phone2feature[p2]
 
         return 1.0 - np.sum(np.abs(f1 - f2) * self.weights) / np.sum(self.weights) / 2.0
 
+
+    def distance(self, p1, p2):
+        return 1.0 - self.similarity(p1, p2)
+
+
     def most_similar(self, target_phone, phone_cands, verbose=False):
 
         max_phone = phone_cands[0]
         min_distance = 1000000
 
         if target_phone in phone_cands:
             return target_phone
```

### Comparing `phonepiece-1.3.7/phonepiece/lexicon.py` & `phonepiece-1.4.0/phonepiece/lexicon.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from collections import defaultdict
 from phonepiece.utils import load_lang_dir
-from phonepiece.iso import normalize_lang_id
+from phonepiece.lang import normalize_lang_id
 from phonepiece.inventory import read_inventory
+from phonepiece.utils import import_with_auto_install
+from phonepiece.arpa import ArpaConverter
 
 
 def read_lexicon(lang_id, model_name='latest'):
 
     """
     read lexicon of the lang_id from a prebuilt inventory model or a customized local path
 
@@ -22,20 +24,33 @@
     # load or download lang dir
     lang_dir = load_lang_dir(lang_id, model_name)
 
     inventory = read_inventory(lang_id, model_name)
 
     lexicon_path = lang_dir / 'lexicon.txt'
 
-    # empty lexicon
-    if not lexicon_path.exists():
+    # special handling for English
+    if lang_id == 'eng':
+        cmudict_module = import_with_auto_install('cmudict', 'cmudict')
+        cmudict = cmudict_module.dict()
+        converter = ArpaConverter()
+        word2phoneme = {}
+        for word in cmudict:
+            arpa = cmudict[word][0]
+            ipas = converter.convert(arpa)
+            word2phoneme[word] = ipas
+
+        return Lexicon(lang_id, inventory, word2phoneme)
+
+    elif not lexicon_path.exists():
+        # empty lexicon
         return Lexicon(lang_id, inventory, {})
 
     word2phoneme = {}
-    for line in open(str(lexicon_path), 'r'):
+    for line in open(str(lexicon_path), 'r', encoding='utf-8'):
         fields = line.strip().split('\t')
 
         # wrongly formatted lines
         if len(fields) != 2 or len(fields[0]) == 0 or len(fields[1]) == 0:
             continue
 
         # to lower by default
```

### Comparing `phonepiece-1.3.7/phonepiece/pinyin.py` & `phonepiece-1.4.0/phonepiece/pinyin.py`

 * *Files identical despite different names*

### Comparing `phonepiece-1.3.7/phonepiece/timit.py` & `phonepiece-1.4.0/phonepiece/timit.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     def __init__(self):
 
         timit_path = PhonePieceConfig.data_path / 'timit.txt'
 
         self.timit_map = {}
 
-        with open(timit_path, 'r') as f:
+        with open(timit_path, 'r', encoding='utf-8') as f:
             for line in f:
                 fields = line.strip().split()
 
                 if fields[1] != 'nan':
                     self.timit_map[fields[0]] = fields[2]
                 else:
                     self.timit_map[fields[0]] = ''
```

### Comparing `phonepiece-1.3.7/phonepiece/unit.py` & `phonepiece-1.4.0/phonepiece/unit.py`

 * *Files identical despite different names*

### Comparing `phonepiece-1.3.7/phonepiece/utils.py` & `phonepiece-1.4.0/phonepiece/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 from phonepiece.config import *
 from phonepiece.bin.download_model import download_model
-from phonepiece.iso import normalize_lang_id
+from phonepiece.lang import normalize_lang_id
+import pip
+import importlib
+
+def import_with_auto_install(package, package_name):
+    try:
+        return importlib.import_module(package)
+    except ImportError:
+        pip.main(['install', package_name])
+    return importlib.import_module(package)
 
 
 def load_lang_dir(lang_id, model_name='latest'):
     """
     make sure lang_dir is properly downloaded or loaded
 
     :param lang_id: a 3 char or 2 char iso id
@@ -29,10 +38,11 @@
         lang_dir = PhonePieceConfig.data_path / 'model' / model_name / lang_id
 
         # if not exists, we try to download the model
         if not lang_dir.exists():
             download_model(model_name)
 
         if not lang_dir.exists():
-            raise ValueError(f"could not download or read {model_name} inventory")
+            print(f"warning: could not download or read {lang_id} inventory, using eng instead")
+            lang_dir = PhonePieceConfig.data_path / 'model' / model_name / 'eng'
 
     return lang_dir
```

### Comparing `phonepiece-1.3.7/phonepiece.egg-info/SOURCES.txt` & `phonepiece-1.4.0/phonepiece.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 LICENSE.txt
 README.md
 setup.py
 phonepiece/__init__.py
 phonepiece/arpa.py
 phonepiece/config.py
-phonepiece/edit_distance.py
+phonepiece/distance.py
 phonepiece/epitran.py
 phonepiece/inventory.py
 phonepiece/ipa.py
-phonepiece/iso.py
+phonepiece/lang.py
 phonepiece/lexicon.py
 phonepiece/pinyin.py
 phonepiece/timit.py
-phonepiece/tree.py
 phonepiece/unit.py
 phonepiece/utils.py
 phonepiece.egg-info/PKG-INFO
 phonepiece.egg-info/SOURCES.txt
 phonepiece.egg-info/dependency_links.txt
 phonepiece.egg-info/requires.txt
 phonepiece.egg-info/top_level.txt
 phonepiece/bin/__init__.py
 phonepiece/bin/download_model.py
+phonepiece/bin/eval_distance.py
 phonepiece/bin/update_model.py
 phonepiece/data/__init__.py
 phonepiece/data/arpabet.csv
 phonepiece/data/ipa-xsampa.csv
 phonepiece/data/ipa_all.csv
 phonepiece/data/ipa_base.csv
 phonepiece/data/language.tsv
 phonepiece/data/phoible-segments-features.tsv
 phonepiece/data/pinyin2ipa.txt
 phonepiece/data/tree.txt
+test/test_distance.py
 test/test_epitran.py
 test/test_inventory.py
 test/test_ipa.py
 test/test_lexicon.py
```

### Comparing `phonepiece-1.3.7/test/test_epitran.py` & `phonepiece-1.4.0/test/test_epitran.py`

 * *Files identical despite different names*

### Comparing `phonepiece-1.3.7/test/test_inventory.py` & `phonepiece-1.4.0/test/test_inventory.py`

 * *Files identical despite different names*

### Comparing `phonepiece-1.3.7/test/test_ipa.py` & `phonepiece-1.4.0/test/test_ipa.py`

 * *Files identical despite different names*

