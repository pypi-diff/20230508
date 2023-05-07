# Comparing `tmp/pyBibX-2.9.8.tar.gz` & `tmp/pyBibX-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyBibX-2.9.8.tar", last modified: Sat May  6 13:59:50 2023, max compression
+gzip compressed data, was "dist\pyBibX-2.9.9.tar", last modified: Sun May  7 23:37:03 2023, max compression
```

## Comparing `pyBibX-2.9.8.tar` & `pyBibX-2.9.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 13:59:50.000000 pyBibX-2.9.8/
--rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-2.9.8/LICENSE
--rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-2.9.8/MANIFEST.in
--rw-rw-rw-   0        0        0     9590 2023-05-06 13:59:50.000000 pyBibX-2.9.8/PKG-INFO
--rw-rw-rw-   0        0        0     9147 2023-05-06 13:56:24.000000 pyBibX-2.9.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 13:59:50.000000 pyBibX-2.9.8/pyBibX/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.8/pyBibX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:59:50.000000 pyBibX-2.9.8/pyBibX/base/
--rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-2.9.8/pyBibX/base/__init__.py
--rw-rw-rw-   0        0        0   264479 2023-05-06 13:57:56.000000 pyBibX-2.9.8/pyBibX/base/pbx.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:59:50.000000 pyBibX-2.9.8/pyBibX/base/stws/
--rw-rw-rw-   0        0        0     1287 2017-07-30 20:46:06.000000 pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Arabic.txt
--rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Bengali.txt
--rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Bulgarian.txt
--rw-rw-rw-   0        0        0     1518 2017-07-30 20:46:06.000000 pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Czech.txt
--rw-rw-rw-   0        0        0     4212 2017-08-01 12:33:33.000000 pyBibX-2.9.8/pyBibX/base/stws/Stopwords-English.txt
--rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Finnish.txt
--rw-rw-rw-   0        0        0     3234 2017-07-30 20:46:06.000000 pyBibX-2.9.8/pyBibX/base/stws/Stopwords-French.txt
--rw-rw-rw-   0        0        0     4350 2017-07-30 20:46:06.000000 pyBibX-2.9.8/pyBibX/base/stws/Stopwords-German.txt
--rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Hindi.txt
--rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Hungarian.txt
--rw-rw-rw-   0        0        0     2379 2017-07-30 20:46:06.000000 pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Italian.txt
--rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Marathi.txt
--rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Persian.txt
--rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Polish.txt
--rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Portuguese-br.txt
--rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Romanian.txt
--rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Russian.txt
--rw-rw-rw-   0        0        0     2420 2017-08-01 12:33:16.000000 pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Spanish.txt
--rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Swedish.txt
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.8/pyBibX/base/stws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:59:50.000000 pyBibX-2.9.8/pyBibX.egg-info/
--rw-rw-rw-   0        0        0     9590 2023-05-06 13:59:47.000000 pyBibX-2.9.8/pyBibX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1047 2023-05-06 13:59:48.000000 pyBibX-2.9.8/pyBibX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 13:59:47.000000 pyBibX-2.9.8/pyBibX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      210 2023-05-06 13:59:47.000000 pyBibX-2.9.8/pyBibX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-06 13:59:47.000000 pyBibX-2.9.8/pyBibX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 13:59:47.000000 pyBibX-2.9.8/pyBibX.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-05-06 13:59:50.000000 pyBibX-2.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1082 2023-05-06 13:56:38.000000 pyBibX-2.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 23:37:03.000000 pyBibX-2.9.9/
+-rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-2.9.9/LICENSE
+-rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-2.9.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     9608 2023-05-07 23:37:03.000000 pyBibX-2.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0     9165 2023-05-06 14:18:32.000000 pyBibX-2.9.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 23:37:02.000000 pyBibX-2.9.9/pyBibX/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.9/pyBibX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 23:37:02.000000 pyBibX-2.9.9/pyBibX/base/
+-rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-2.9.9/pyBibX/base/__init__.py
+-rw-rw-rw-   0        0        0   264479 2023-05-06 13:57:56.000000 pyBibX-2.9.9/pyBibX/base/pbx.py
+drwxrwxrwx   0        0        0        0 2023-05-07 23:37:03.000000 pyBibX-2.9.9/pyBibX/base/stws/
+-rw-rw-rw-   0        0        0     1287 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Arabic.txt
+-rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Bengali.txt
+-rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Bulgarian.txt
+-rw-rw-rw-   0        0        0     1518 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Czech.txt
+-rw-rw-rw-   0        0        0     4212 2017-08-01 12:33:33.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-English.txt
+-rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Finnish.txt
+-rw-rw-rw-   0        0        0     3234 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-French.txt
+-rw-rw-rw-   0        0        0     4350 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-German.txt
+-rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Hindi.txt
+-rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Hungarian.txt
+-rw-rw-rw-   0        0        0     2379 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Italian.txt
+-rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Marathi.txt
+-rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Persian.txt
+-rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Polish.txt
+-rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Portuguese-br.txt
+-rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Romanian.txt
+-rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Russian.txt
+-rw-rw-rw-   0        0        0     2420 2017-08-01 12:33:16.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Spanish.txt
+-rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Swedish.txt
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.9/pyBibX/base/stws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 23:37:02.000000 pyBibX-2.9.9/pyBibX.egg-info/
+-rw-rw-rw-   0        0        0     9608 2023-05-07 23:37:01.000000 pyBibX-2.9.9/pyBibX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1047 2023-05-07 23:37:02.000000 pyBibX-2.9.9/pyBibX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 23:37:01.000000 pyBibX-2.9.9/pyBibX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      210 2023-05-07 23:37:01.000000 pyBibX-2.9.9/pyBibX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-07 23:37:01.000000 pyBibX-2.9.9/pyBibX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-07 23:37:01.000000 pyBibX-2.9.9/pyBibX.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-05-07 23:37:03.000000 pyBibX-2.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     1082 2023-05-06 14:26:46.000000 pyBibX-2.9.9/setup.py
```

### Comparing `pyBibX-2.9.8/LICENSE` & `pyBibX-2.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/PKG-INFO` & `pyBibX-2.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 2.9.8
+Version: 2.9.9
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,17 +13,17 @@
 
 ## Introduction
 
 A Bibliometric and Scientometric python library that uses the raw files generated by **Scopus** (.bib files), **WOS (Web of Science)** (.bib files), and **PubMed** (.txt files) scientific databases. Also, Powered with Advanced AI Technologies for Analyzing Bibliometric, Scientometric Outcomes, and Textual Data
 
 To export the correct file formats from Scopus, Web of Science, and PubMed, follow these steps:
 
-a) Scopus: Search, select articles, click "Export," choose "BibTeX," select all fields, click "Export" again.
-b) WoS: Search, select articles, click "Export," choose "Save to Other File Formats," select "BibTeX," select all fields, click "Send."
-c) PubMed: Search, select articles, click "Save," choose "PubMed" format, click "Save" to download a .txt file. 
+- a) **Scopus**: Search, select articles, click "Export," choose "BibTeX," select all fields, click "Export" again.
+- b) **WoS**: Search, select articles, click "Export," choose "Save to Other File Formats," select "BibTeX," select all fields, click "Send."
+- c) **PubMed**: Search, select articles, click "Save," choose "PubMed" format, click "Save" to download a .txt file. 
 
 General Capabilities:
 - a) Works with **Scopus** (.bib files), **WOS** (.bib files) and **PubMed** (.txt files) databases 
 - b) Identification and Removal of duplicates
 - c) Identification of documents per type
 - d) Generates an **EDA (Exploratory Data Analysis)** Report: Publications Timespan, Total Number of Countries, Total Number of Institutions, Total Number of Sources, Total Number of References, Total Number of Languages (and also the number of docs for each language), Total Number of Documents, Average Documents per Author, Average Documents per Institution, Average Documents per Source, Average Documents per Year, Total Number of Authors, Total Number of Authors Keywords, Total Number of Authors Keywords Plus, Total Single-Authored Documents, Total Multi-Authored Documents, Average Collaboration Index, Max H-Index, Total Number of Citations, Average Citations per Author, Average Citations per Institution, Average Citations per Document, Average Citations per Source
 - e) Creates an **ID (Identification)** for each Document, Authors, Sources, Institutions, Countries, Authors' Keywords, Keywords Plus. The IDs can be used in graphs/plots to obtain a cleaner visualization
```

### Comparing `pyBibX-2.9.8/README.md` & `pyBibX-2.9.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 ## Introduction
 
 A Bibliometric and Scientometric python library that uses the raw files generated by **Scopus** (.bib files), **WOS (Web of Science)** (.bib files), and **PubMed** (.txt files) scientific databases. Also, Powered with Advanced AI Technologies for Analyzing Bibliometric, Scientometric Outcomes, and Textual Data
 
 To export the correct file formats from Scopus, Web of Science, and PubMed, follow these steps:
 
-a) Scopus: Search, select articles, click "Export," choose "BibTeX," select all fields, click "Export" again.
-b) WoS: Search, select articles, click "Export," choose "Save to Other File Formats," select "BibTeX," select all fields, click "Send."
-c) PubMed: Search, select articles, click "Save," choose "PubMed" format, click "Save" to download a .txt file. 
+- a) **Scopus**: Search, select articles, click "Export," choose "BibTeX," select all fields, click "Export" again.
+- b) **WoS**: Search, select articles, click "Export," choose "Save to Other File Formats," select "BibTeX," select all fields, click "Send."
+- c) **PubMed**: Search, select articles, click "Save," choose "PubMed" format, click "Save" to download a .txt file. 
 
 General Capabilities:
 - a) Works with **Scopus** (.bib files), **WOS** (.bib files) and **PubMed** (.txt files) databases 
 - b) Identification and Removal of duplicates
 - c) Identification of documents per type
 - d) Generates an **EDA (Exploratory Data Analysis)** Report: Publications Timespan, Total Number of Countries, Total Number of Institutions, Total Number of Sources, Total Number of References, Total Number of Languages (and also the number of docs for each language), Total Number of Documents, Average Documents per Author, Average Documents per Institution, Average Documents per Source, Average Documents per Year, Total Number of Authors, Total Number of Authors Keywords, Total Number of Authors Keywords Plus, Total Single-Authored Documents, Total Multi-Authored Documents, Average Collaboration Index, Max H-Index, Total Number of Citations, Average Citations per Author, Average Citations per Institution, Average Citations per Document, Average Citations per Source
 - e) Creates an **ID (Identification)** for each Document, Authors, Sources, Institutions, Countries, Authors' Keywords, Keywords Plus. The IDs can be used in graphs/plots to obtain a cleaner visualization
```

### Comparing `pyBibX-2.9.8/pyBibX/base/pbx.py` & `pyBibX-2.9.9/pyBibX/base/pbx.py`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Arabic.txt` & `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Arabic.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Bengali.txt` & `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Bengali.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Bulgarian.txt` & `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Bulgarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Czech.txt` & `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Czech.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/pyBibX/base/stws/Stopwords-English.txt` & `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-English.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Finnish.txt` & `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Finnish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/pyBibX/base/stws/Stopwords-French.txt` & `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-French.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/pyBibX/base/stws/Stopwords-German.txt` & `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-German.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Hindi.txt` & `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Hindi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Hungarian.txt` & `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Hungarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Italian.txt` & `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Italian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Marathi.txt` & `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Marathi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Persian.txt` & `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Persian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Polish.txt` & `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Polish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Portuguese-br.txt` & `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Portuguese-br.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Romanian.txt` & `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Romanian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Russian.txt` & `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Russian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Spanish.txt` & `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Spanish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/pyBibX/base/stws/Stopwords-Swedish.txt` & `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Swedish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/pyBibX.egg-info/PKG-INFO` & `pyBibX-2.9.9/pyBibX.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 2.9.8
+Version: 2.9.9
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,17 +13,17 @@
 
 ## Introduction
 
 A Bibliometric and Scientometric python library that uses the raw files generated by **Scopus** (.bib files), **WOS (Web of Science)** (.bib files), and **PubMed** (.txt files) scientific databases. Also, Powered with Advanced AI Technologies for Analyzing Bibliometric, Scientometric Outcomes, and Textual Data
 
 To export the correct file formats from Scopus, Web of Science, and PubMed, follow these steps:
 
-a) Scopus: Search, select articles, click "Export," choose "BibTeX," select all fields, click "Export" again.
-b) WoS: Search, select articles, click "Export," choose "Save to Other File Formats," select "BibTeX," select all fields, click "Send."
-c) PubMed: Search, select articles, click "Save," choose "PubMed" format, click "Save" to download a .txt file. 
+- a) **Scopus**: Search, select articles, click "Export," choose "BibTeX," select all fields, click "Export" again.
+- b) **WoS**: Search, select articles, click "Export," choose "Save to Other File Formats," select "BibTeX," select all fields, click "Send."
+- c) **PubMed**: Search, select articles, click "Save," choose "PubMed" format, click "Save" to download a .txt file. 
 
 General Capabilities:
 - a) Works with **Scopus** (.bib files), **WOS** (.bib files) and **PubMed** (.txt files) databases 
 - b) Identification and Removal of duplicates
 - c) Identification of documents per type
 - d) Generates an **EDA (Exploratory Data Analysis)** Report: Publications Timespan, Total Number of Countries, Total Number of Institutions, Total Number of Sources, Total Number of References, Total Number of Languages (and also the number of docs for each language), Total Number of Documents, Average Documents per Author, Average Documents per Institution, Average Documents per Source, Average Documents per Year, Total Number of Authors, Total Number of Authors Keywords, Total Number of Authors Keywords Plus, Total Single-Authored Documents, Total Multi-Authored Documents, Average Collaboration Index, Max H-Index, Total Number of Citations, Average Citations per Author, Average Citations per Institution, Average Citations per Document, Average Citations per Source
 - e) Creates an **ID (Identification)** for each Document, Authors, Sources, Institutions, Countries, Authors' Keywords, Keywords Plus. The IDs can be used in graphs/plots to obtain a cleaner visualization
```

### Comparing `pyBibX-2.9.8/pyBibX.egg-info/SOURCES.txt` & `pyBibX-2.9.9/pyBibX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.8/setup.py` & `pyBibX-2.9.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyBibX',
-    version='2.9.8',
+    version='2.9.9',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyBibX',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

