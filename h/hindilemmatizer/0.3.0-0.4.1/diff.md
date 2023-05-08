# Comparing `tmp/hindilemmatizer-0.3.0-py3-none-any.whl.zip` & `tmp/hindilemmatizer-0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,12 @@
-Zip file size: 131982 bytes, number of entries: 8
+Zip file size: 6845367 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      156 b- defN 23-May-06 13:08 hindilemmatizer/__init__.py
--rw-r--r--  2.0 unx     2735 b- defN 23-May-06 13:36 hindilemmatizer/lemmatizer.py
--rw-r--r--  2.0 unx   555099 b- defN 23-May-07 18:49 hindilemmatizer/data/data.csv
--rw-r--r--  2.0 unx     1071 b- defN 23-May-07 18:57 hindilemmatizer-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      186 b- defN 23-May-07 18:57 hindilemmatizer-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-07 18:57 hindilemmatizer-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-May-07 18:57 hindilemmatizer-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      682 b- defN 23-May-07 18:57 hindilemmatizer-0.3.0.dist-info/RECORD
-8 files, 560037 bytes uncompressed, 130784 bytes compressed:  76.6%
+-rw-r--r--  2.0 unx     3380 b- defN 23-May-08 17:01 hindilemmatizer/lemmatizer.py
+-rw-r--r--  2.0 unx   555099 b- defN 23-May-08 16:44 hindilemmatizer/data/data.csv
+-rw-r--r--  2.0 unx   228523 b- defN 23-May-08 16:44 hindilemmatizer/data/direct.csv
+-rw-r--r--  2.0 unx 23623710 b- defN 23-May-08 16:44 hindilemmatizer/data/totalWords.txt
+-rw-r--r--  2.0 unx     1071 b- defN 23-May-08 17:08 hindilemmatizer-0.4.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      186 b- defN 23-May-08 17:08 hindilemmatizer-0.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-08 17:08 hindilemmatizer-0.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-May-08 17:08 hindilemmatizer-0.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      868 b- defN 23-May-08 17:08 hindilemmatizer-0.4.1.dist-info/RECORD
+10 files, 24413101 bytes uncompressed, 6843885 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -3,23 +3,29 @@
 
 Filename: hindilemmatizer/lemmatizer.py
 Comment: 
 
 Filename: hindilemmatizer/data/data.csv
 Comment: 
 
-Filename: hindilemmatizer-0.3.0.dist-info/LICENSE
+Filename: hindilemmatizer/data/direct.csv
 Comment: 
 
-Filename: hindilemmatizer-0.3.0.dist-info/METADATA
+Filename: hindilemmatizer/data/totalWords.txt
 Comment: 
 
-Filename: hindilemmatizer-0.3.0.dist-info/WHEEL
+Filename: hindilemmatizer-0.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: hindilemmatizer-0.3.0.dist-info/top_level.txt
+Filename: hindilemmatizer-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: hindilemmatizer-0.3.0.dist-info/RECORD
+Filename: hindilemmatizer-0.4.1.dist-info/WHEEL
+Comment: 
+
+Filename: hindilemmatizer-0.4.1.dist-info/top_level.txt
+Comment: 
+
+Filename: hindilemmatizer-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hindilemmatizer/lemmatizer.py

```diff
@@ -12,14 +12,36 @@
   for row in reader:
     globalPrefixWordsSet.add(row[1])
     globalRootWordsSet.add(row[2])
     globalSuffixWordsSet.add(row[3])
 
   f.close()
 
+
+directRoots = dict()
+
+direct_path = pkg_resources.resource_filename('hindilemmatizer', 'data/direct.csv')
+with open(direct_path, encoding='utf-8') as f:
+  reader=csv.reader(f)
+  for row in reader:
+    directRoots[row[0]] = row[1]
+
+  f.close()
+
+
+totalWords = set()
+
+total_path = pkg_resources.resource_filename('hindilemmatizer', 'data/totalWords.txt')
+with open(total_path, encoding='utf-8') as f:
+  data = f.readlines()
+  for i in range(len(data)):
+    totalWords.add(data[i].strip())
+  f.close()
+
+
 globalPrefixWordsSet.discard("")
 globalRootWordsSet.discard("")
 globalSuffixWordsSet.discard("")
 
 alreadyLemmatizedWords = dict()
 # Here comes real algorithm
 class WordLemmatizer:
@@ -49,26 +71,26 @@
     if(len(self.possibleRootWords)):
       return self.finalReturn()
     
     return self.step2()
   
   def step2(self):
     for l in range(2,len(self.word)):
-      if self.word[l:] in globalSuffixWordsSet and len(self.word[l:])>1:
+      if self.word[l:] in globalSuffixWordsSet and len(self.word[l:])>1 and self.word[:l] in totalWords:
         self.possibleRootWords.add(WordLemmatizer(self.word[:l]).lemmatize())
 
     if(len(self.possibleRootWords)):
       return self.finalReturn()
 
     return self.word
 
   def step3(self):
 
     for r in range(1,len(self.inflectedWord)-1):
-      if self.word[:r] in globalPrefixWordsSet:
+      if self.word[:r] in globalPrefixWordsSet and self.word[r:] in totalWords:
         self.possibleRootWords.add(WordLemmatizer(self.word[r:]).lemmatize())
     if(len(self.possibleRootWords)):
       return self.finalReturn()
 
     return self.word
 
   def finalReturn(self):
@@ -82,14 +104,17 @@
     return self.word
 
 def sanitizeLine(line):
   return re.sub(r'\s+', ' ', re.sub(r'[{}[\]:;?@!#$%^&*()-_\'\"<>\u0964\u0965,]', ' ', line.encode("utf-8").decode("utf-8"))).split()
 
 def processWord(word):
 
+  if word in directRoots:
+    alreadyLemmatizedWords[word] = directRoots[word]
+
   if word in alreadyLemmatizedWords:
     return alreadyLemmatizedWords[word]
 
   lemma= WordLemmatizer(word).lemmatize()
   alreadyLemmatizedWords[word]=lemma
   return lemma
```

## Comparing `hindilemmatizer-0.3.0.dist-info/LICENSE` & `hindilemmatizer-0.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hindilemmatizer-0.3.0.dist-info/RECORD` & `hindilemmatizer-0.4.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 hindilemmatizer/__init__.py,sha256=1ebhI5j8l6U-3JCYQtIS4z3t8yKYRj5fZo2phOWzCP4,156
-hindilemmatizer/lemmatizer.py,sha256=M5qnIQ9Wv4PhAfIiina04bHUKURR49UgQL4hzwclACw,2735
+hindilemmatizer/lemmatizer.py,sha256=by6IdSiK4Y8jP7w2Sj63y9oCyHhW3Ogxu2aO1gU6M2o,3380
 hindilemmatizer/data/data.csv,sha256=54ozpY7FWv-RqYMLTBUKuvqSowvLEfPnEH-gm6GkCQc,555099
-hindilemmatizer-0.3.0.dist-info/LICENSE,sha256=_X30G4gWiaB7S98CDdzGzf2w8z3OXKynaPZxdj9muJw,1071
-hindilemmatizer-0.3.0.dist-info/METADATA,sha256=SkXwBGYwshkQsnlpLuxokz23wPlKzBhh6ZiIk4Sauq0,186
-hindilemmatizer-0.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-hindilemmatizer-0.3.0.dist-info/top_level.txt,sha256=GJC0W0QnJxoX-JKaJf-ARkgFOU-FvckrleigitVFHTg,16
-hindilemmatizer-0.3.0.dist-info/RECORD,,
+hindilemmatizer/data/direct.csv,sha256=CHtL85lBXnetYOeMCONkYWlBLa3XUK62y40RfwqR2_0,228523
+hindilemmatizer/data/totalWords.txt,sha256=qMs56UGMIen-c-_KgEom-pck6UPGeDEtL2aFvQksFBk,23623710
+hindilemmatizer-0.4.1.dist-info/LICENSE,sha256=_X30G4gWiaB7S98CDdzGzf2w8z3OXKynaPZxdj9muJw,1071
+hindilemmatizer-0.4.1.dist-info/METADATA,sha256=K8581-xeRhNpGM9tMPx_G84Cvrvz_t2uqggYAT837sg,186
+hindilemmatizer-0.4.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+hindilemmatizer-0.4.1.dist-info/top_level.txt,sha256=GJC0W0QnJxoX-JKaJf-ARkgFOU-FvckrleigitVFHTg,16
+hindilemmatizer-0.4.1.dist-info/RECORD,,
```

