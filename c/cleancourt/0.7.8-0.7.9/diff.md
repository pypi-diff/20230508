# Comparing `tmp/cleancourt-0.7.8.tar.gz` & `tmp/cleancourt-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cleancourt-0.7.8.tar", last modified: Mon Apr 17 19:47:06 2023, max compression
+gzip compressed data, was "dist/cleancourt-0.7.9.tar", last modified: Wed Apr 19 17:19:05 2023, max compression
```

## Comparing `cleancourt-0.7.8.tar` & `cleancourt-0.7.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 19:47:06.000000 cleancourt-0.7.8/
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-04-17 19:46:51.000000 cleancourt-0.7.8/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    15468 2023-04-17 19:47:06.000000 cleancourt-0.7.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    13414 2023-04-17 19:46:51.000000 cleancourt-0.7.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-17 19:47:06.000000 cleancourt-0.7.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1195 2023-04-17 19:46:51.000000 cleancourt-0.7.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 19:47:06.000000 cleancourt-0.7.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 19:47:06.000000 cleancourt-0.7.8/src/cleancourt/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/check_spaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3351 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/clean_data.py
--rw-rw-rw-   0 root         (0) root         (0)     4124 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/compare_companies.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/compute_ngrams.py
--rw-rw-rw-   0 root         (0) root         (0)     9104 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/cosine_similarity.py
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/filter_types.py
--rw-rw-rw-   0 root         (0) root         (0)     5985 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/full_clean_names.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/integrate_output.py
--rw-rw-rw-   0 root         (0) root         (0)     2969 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/parse_names.py
--rw-rw-rw-   0 root         (0) root         (0)     1996 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/separate_parent_company.py
--rw-rw-rw-   0 root         (0) root         (0)      832 2023-04-17 19:46:51.000000 cleancourt-0.7.8/src/cleancourt/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 19:47:06.000000 cleancourt-0.7.8/src/cleancourt.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15468 2023-04-17 19:47:06.000000 cleancourt-0.7.8/src/cleancourt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      623 2023-04-17 19:47:06.000000 cleancourt-0.7.8/src/cleancourt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 19:47:06.000000 cleancourt-0.7.8/src/cleancourt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-04-17 19:47:06.000000 cleancourt-0.7.8/src/cleancourt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-17 19:47:06.000000 cleancourt-0.7.8/src/cleancourt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:19:05.000000 cleancourt-0.7.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2023-04-19 17:18:50.000000 cleancourt-0.7.9/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    15468 2023-04-19 17:19:05.000000 cleancourt-0.7.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    13414 2023-04-19 17:18:50.000000 cleancourt-0.7.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-19 17:19:05.000000 cleancourt-0.7.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1195 2023-04-19 17:18:50.000000 cleancourt-0.7.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:19:05.000000 cleancourt-0.7.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:19:05.000000 cleancourt-0.7.9/src/cleancourt/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/check_spaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3351 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/clean_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4124 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/compare_companies.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/compute_ngrams.py
+-rw-rw-rw-   0 root         (0) root         (0)     9104 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/cosine_similarity.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/filter_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     5985 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/full_clean_names.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/integrate_output.py
+-rw-rw-rw-   0 root         (0) root         (0)     3226 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/parse_names.py
+-rw-rw-rw-   0 root         (0) root         (0)     2047 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/separate_parent_company.py
+-rw-rw-rw-   0 root         (0) root         (0)      832 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:19:05.000000 cleancourt-0.7.9/src/cleancourt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15468 2023-04-19 17:19:05.000000 cleancourt-0.7.9/src/cleancourt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      623 2023-04-19 17:19:05.000000 cleancourt-0.7.9/src/cleancourt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 17:19:05.000000 cleancourt-0.7.9/src/cleancourt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-04-19 17:19:05.000000 cleancourt-0.7.9/src/cleancourt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-19 17:19:05.000000 cleancourt-0.7.9/src/cleancourt.egg-info/top_level.txt
```

### Comparing `cleancourt-0.7.8/LICENSE.txt` & `cleancourt-0.7.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.8/PKG-INFO` & `cleancourt-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleancourt
-Version: 0.7.8
+Version: 0.7.9
 Summary: a library for cleaning court docket entries
 Home-page: UNKNOWN
 Author: Logan Pratico
 Author-email: praticol@lsc.gov
 License: UNKNOWN
 Description: 
         # cleancourt
```

### Comparing `cleancourt-0.7.8/README.md` & `cleancourt-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.8/setup.py` & `cleancourt-0.7.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def get_file_text(file_name):
     with open(os.path.join(here, file_name)) as in_file:
         return in_file.read()
 
 
 setup(
     name="cleancourt",
-    version="0.7.8",
+    version="0.7.9",
     description="a library for cleaning court docket entries",
     author="Logan Pratico",
     author_email="praticol@lsc.gov",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.9",
```

### Comparing `cleancourt-0.7.8/src/cleancourt/__init__.py` & `cleancourt-0.7.9/src/cleancourt/__init__.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.8/src/cleancourt/check_spaces.py` & `cleancourt-0.7.9/src/cleancourt/check_spaces.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.8/src/cleancourt/clean_data.py` & `cleancourt-0.7.9/src/cleancourt/clean_data.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.8/src/cleancourt/compare_companies.py` & `cleancourt-0.7.9/src/cleancourt/compare_companies.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.8/src/cleancourt/cosine_similarity.py` & `cleancourt-0.7.9/src/cleancourt/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.8/src/cleancourt/filter_types.py` & `cleancourt-0.7.9/src/cleancourt/filter_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,17 +19,20 @@
     # Probable people performs poorly on bank names. Working to update training dataset but this is a quick fix for now
 
     try:
         val = pp.tag(name)
         return (
             (val[1] != "Person")
             or 'CorporationNameOrganization' in val[0]
+            or 'CorporationNameBranchIdentifier' in val[0]
+            or 'CorporationLegalType' in val[0]
             or ("|and|" in name)
             or (name.count(" ") == 0)
             or (re.search(" bank$", name))
+            or 'citibank' in name
             or ("bennington crossing" in name)
         ) and not name[0].isdigit()
     except:
         return True
 
 
 def filter_people(name):
@@ -41,14 +44,17 @@
     """
 
     try:
         val = pp.tag(name)
         return (
             (val[1] == "Person")
             and 'CorporationNameOrganization' not in val[0]
+            and 'CorporationNameBranchIdentifier' not in val[0]
+            and 'CorporationLegalType' not in val[0]
+            and 'citibank' not in name
             and ("|and|" not in name)
             and (name.count(" ") != 0)
             and not (re.search(" bank$", name))
             and ("bennington crossing" not in name)
         )
     except:
         return False
```

### Comparing `cleancourt-0.7.8/src/cleancourt/full_clean_names.py` & `cleancourt-0.7.9/src/cleancourt/full_clean_names.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.8/src/cleancourt/integrate_output.py` & `cleancourt-0.7.9/src/cleancourt/integrate_output.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.8/src/cleancourt/parse_names.py` & `cleancourt-0.7.9/src/cleancourt/parse_names.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,16 +43,23 @@
                 prefOther = val[0]["PrefixOther"]
             except KeyError:
                 prefOther = ""
 
 
             try: # Update 0.7.8 first names are sometimes parsed as SuffixOther in probablepeople. this attempts to correct for that error
                 sufOther = val[0]["SuffixOther"]
+                if sufOther == 'dds' or sufOther == 'md':
+                    sufOtherEnd = sufOther
+                else:
+                    sufOtherEnd = ""
+
             except KeyError:
                 sufOther = ""
+                sufOtherEnd = ""
+
 
             try:
                 first = val[0]["GivenName"]
             except KeyError:
                 first = ""
 
             try:
@@ -94,12 +101,14 @@
                 + middleI
                 + " "
                 + last
                 + " " 
                 + lastI
                 + " "
                 + suffix
+                + " " 
+                + sufOtherEnd
             )
 
             names_dict[name] = re.sub(" +", " ", full_name.strip()) # Strip any extra white spaces
 
     return names_dict
```

### Comparing `cleancourt-0.7.8/src/cleancourt/separate_parent_company.py` & `cleancourt-0.7.9/src/cleancourt/separate_parent_company.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import re
 from tqdm import tqdm
 
 
 def remove_company_connector(string):
     string = re.sub(
-        "(.+) as a? ?management agent for (.+)", "\\2 /-/ \\1", string
+        "(.+) as a? ?management agent for (.{4,})", "\\2 /-/ \\1", string
     )  # Remove any appareance of as management agent for
-    string = re.sub("(.+) successor in interest to (.+)", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) [as ]?assignee of (.+)", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) [as ]?managing agent for (.+)", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) [as ]?m/a for (.+)", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) by (.+) as managing agent$", "\\1 /-/ \\2", string)
+    string = re.sub("(.+) successor in interest to (.{4,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) [as ]?assignee of (.{4,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) [as ]?managing agent for (.{4,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) [as ]?m/a for (.{4,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.{4,}) by (.+) as managing agent$", "\\1 /-/ \\2", string)
     string = re.sub(
-        "(.+) a[^A-z]?s[^A-z]?o[^A-z]? (.+)", "\\2 /-/ \\1", string
+        "(.+) a[^A-z]?s[^A-z]?o[^A-z]? (.{4,})", "\\2 /-/ \\1", string
     )  # Remove any appearance of a.s.o. and what follows
     string = re.sub(
-        "(.+) d[^A-z]?b[^A-z]?a[^A-z]? (.+)", "\\2 /-/ \\1", string
+        "(.+) d[^A-z]?b[^A-z]?a[^A-z]? (.{4,})", "\\2 /-/ \\1", string
     )  # Remove any appearance of d.b.a and what follows
-    string = re.sub("(.+) as agent for (.+)", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) agent for (.+)", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) as mg agent for (.+)", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) mg agt (.+)", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) as managing for (.+)", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) asset\.? management for (.+)", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) doing business as (.+)", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) owner of (.+)", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) trustee of (.+)", "\\1 /-/ \\2", string)
+    string = re.sub("(.+) as agent for (.{4,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) agent for (.{4,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) as mg agent for (.{4,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) mg agt (.{4,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) as managing for (.{4,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) asset\.? management for (.{4,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) doing business as (.{4,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) owner of (.{4,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.{4,}) trustee of (.+)", "\\1 /-/ \\2", string)
 
     return string
 
 
 def separate_company_names(names):
     plaintiffs = []
     plaintiff_parents = []
```

### Comparing `cleancourt-0.7.8/src/cleancourt/test_utils.py` & `cleancourt-0.7.9/src/cleancourt/test_utils.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.8/src/cleancourt.egg-info/PKG-INFO` & `cleancourt-0.7.9/src/cleancourt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleancourt
-Version: 0.7.8
+Version: 0.7.9
 Summary: a library for cleaning court docket entries
 Home-page: UNKNOWN
 Author: Logan Pratico
 Author-email: praticol@lsc.gov
 License: UNKNOWN
 Description: 
         # cleancourt
```

### Comparing `cleancourt-0.7.8/src/cleancourt.egg-info/SOURCES.txt` & `cleancourt-0.7.9/src/cleancourt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

