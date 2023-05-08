# Comparing `tmp/pytranslations-0.0.1.tar.gz` & `tmp/pytranslations-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytranslations-0.0.1.tar", last modified: Mon May  8 08:31:00 2023, max compression
+gzip compressed data, was "pytranslations-0.0.2.tar", last modified: Mon May  8 09:16:22 2023, max compression
```

## Comparing `pytranslations-0.0.1.tar` & `pytranslations-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 08:31:00.067120 pytranslations-0.0.1/
--rw-rw-rw-   0        0        0     1065 2023-05-08 07:25:45.000000 pytranslations-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      561 2023-05-08 08:31:00.067120 pytranslations-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-05-07 21:26:59.000000 pytranslations-0.0.1/README.md
--rw-rw-rw-   0        0        0      110 2023-05-08 07:59:35.000000 pytranslations-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      671 2023-05-08 08:31:00.069115 pytranslations-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      227 2023-05-08 08:30:22.000000 pytranslations-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:31:00.013865 pytranslations-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 08:31:00.053117 pytranslations-0.0.1/src/pytranslations/
--rw-rw-rw-   0        0        0       40 2023-05-08 08:26:55.000000 pytranslations-0.0.1/src/pytranslations/__init__.py
--rw-rw-rw-   0        0        0     4591 2023-05-08 08:30:42.000000 pytranslations-0.0.1/src/pytranslations/translations.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:31:00.066126 pytranslations-0.0.1/src/pytranslations.egg-info/
--rw-rw-rw-   0        0        0      561 2023-05-08 08:30:59.000000 pytranslations-0.0.1/src/pytranslations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-05-08 08:31:00.000000 pytranslations-0.0.1/src/pytranslations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 08:30:59.000000 pytranslations-0.0.1/src/pytranslations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-08 08:30:59.000000 pytranslations-0.0.1/src/pytranslations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 09:16:22.593319 pytranslations-0.0.2/
+-rw-rw-rw-   0        0        0     1065 2023-05-08 07:25:45.000000 pytranslations-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2358 2023-05-08 09:16:22.594320 pytranslations-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1811 2023-05-08 09:14:12.000000 pytranslations-0.0.2/README.md
+-rw-rw-rw-   0        0        0      110 2023-05-08 07:59:35.000000 pytranslations-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      671 2023-05-08 09:16:22.597321 pytranslations-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      227 2023-05-08 09:15:37.000000 pytranslations-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:16:22.519330 pytranslations-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 09:16:22.572314 pytranslations-0.0.2/src/pytranslations/
+-rw-rw-rw-   0        0        0       40 2023-05-08 08:26:55.000000 pytranslations-0.0.2/src/pytranslations/__init__.py
+-rw-rw-rw-   0        0        0     4820 2023-05-08 09:10:36.000000 pytranslations-0.0.2/src/pytranslations/translations.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:16:22.592311 pytranslations-0.0.2/src/pytranslations.egg-info/
+-rw-rw-rw-   0        0        0     2358 2023-05-08 09:16:22.000000 pytranslations-0.0.2/src/pytranslations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-05-08 09:16:22.000000 pytranslations-0.0.2/src/pytranslations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 09:16:22.000000 pytranslations-0.0.2/src/pytranslations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-08 09:16:22.000000 pytranslations-0.0.2/src/pytranslations.egg-info/top_level.txt
```

### Comparing `pytranslations-0.0.1/LICENSE` & `pytranslations-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytranslations-0.0.1/setup.cfg` & `pytranslations-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7974 7261 6e73 6c61 7469 6f6e   = pytranslation
 00000020: 730d 0a76 6572 7369 6f6e 203d 2030 2e30  s..version = 0.0
-00000030: 2e31 0d0a 6175 7468 6f72 203d 2057 796d  .1..author = Wym
+00000030: 2e32 0d0a 6175 7468 6f72 203d 2057 796d  .2..author = Wym
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2064 6577 7265 6174 6f72 3240 676d 6169   dewreator2@gmai
 00000060: 6c2e 636f 6d0d 0a64 6573 6372 6970 7469  l.com..descripti
 00000070: 6f6e 203d 2041 206c 6967 6874 7765 6967  on = A lightweig
 00000080: 6874 206c 6962 7261 7279 2074 6f20 6861  ht library to ha
 00000090: 6e64 6c65 2074 7261 6e73 6c61 7469 6f6e  ndle translation
 000000a0: 730d 0a6c 6f6e 675f 6465 7363 7269 7074  s..long_descript
```

### Comparing `pytranslations-0.0.1/src/pytranslations/translations.py` & `pytranslations-0.0.2/src/pytranslations/translations.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     pass
 
 class Translations:
 
     def __init__(self) -> None:
         self.language_codes: list[str] = []
         self.users_languages: dict = {}
-        self.default_language: str = ""
+        self.default_language: str | None = None
         self.translations: dict = {}
     
 
     def get_translations_from_json(self, json_str: str):
         """
             Get translations from a JSON string
         """
@@ -116,16 +116,19 @@
         return self.users_languages[user_id]
 
 
     def add_user(self, user_id, language = None):
 
         if len(self.language_codes) == 0:
             raise InvalidSetupError("You must first set the translations data! Use get_translations_from_json()")
-        if language not in self.language_codes:
-            raise NoLanguageDataError(f"Can not set language to {language}: this language is not on the available languages list")
         
         if language:
+            if language not in self.language_codes:
+                raise NoLanguageDataError(f"Can not set language to {language}: this language is not on the available languages list")
             self.users_languages[user_id] = language
-    
+        else:
+            if not self.default_language:
+                raise InvalidSetupError(f"You need to set the default language first!")
+            self.users_languages[user_id] = self.default_language    
 
     def set_users_languages(self, language_dict): 
         self.users_languages = language_dict
```

