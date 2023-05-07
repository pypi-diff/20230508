# Comparing `tmp/akellogpt-0.0.3.tar.gz` & `tmp/akellogpt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akellogpt-0.0.3.tar", last modified: Sat May  6 02:27:53 2023, max compression
+gzip compressed data, was "akellogpt-0.0.4.tar", last modified: Sun May  7 23:35:58 2023, max compression
```

## Comparing `akellogpt-0.0.3.tar` & `akellogpt-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 02:27:53.742904 akellogpt-0.0.3/
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)     1075 2023-05-05 23:21:08.000000 akellogpt-0.0.3/LICENSE
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)      495 2023-05-06 02:27:53.742760 akellogpt-0.0.3/PKG-INFO
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)     1603 2023-05-06 00:30:29.000000 akellogpt-0.0.3/README.md
-drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 02:27:53.739843 akellogpt-0.0.3/akellogpt/
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)        0 2023-05-05 23:21:08.000000 akellogpt-0.0.3/akellogpt/__init__.py
-drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 02:27:53.740981 akellogpt-0.0.3/akellogpt/common/
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)        0 2023-05-05 23:21:08.000000 akellogpt-0.0.3/akellogpt/common/__init__.py
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)      693 2023-05-06 00:30:29.000000 akellogpt-0.0.3/akellogpt/common/api.py
-drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 02:27:53.741504 akellogpt-0.0.3/akellogpt/screening/
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)     3383 2023-05-06 01:52:00.000000 akellogpt-0.0.3/akellogpt/screening/__init__.py
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)      412 2023-05-06 00:30:29.000000 akellogpt-0.0.3/akellogpt/screening/mental_health.py
-drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 02:27:53.742122 akellogpt-0.0.3/akellogpt/screening/yaml/
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)      883 2023-05-05 23:21:08.000000 akellogpt-0.0.3/akellogpt/screening/yaml/gad7.yaml
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)     1342 2023-05-05 23:21:08.000000 akellogpt-0.0.3/akellogpt/screening/yaml/phq9.yaml
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)     1972 2023-05-05 23:21:08.000000 akellogpt-0.0.3/akellogpt/screening/yaml/sbq-r.yaml
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)       77 2023-05-06 00:30:29.000000 akellogpt-0.0.3/akellogpt/settings.py
-drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 02:27:53.742553 akellogpt-0.0.3/akellogpt/test/
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)        0 2023-05-05 23:21:08.000000 akellogpt-0.0.3/akellogpt/test/__init__.py
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)      649 2023-05-06 00:30:29.000000 akellogpt-0.0.3/akellogpt/test/test_gad7.py
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)      668 2023-05-06 00:30:29.000000 akellogpt-0.0.3/akellogpt/test/test_phq9.py
-drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 02:27:53.740707 akellogpt-0.0.3/akellogpt.egg-info/
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)      495 2023-05-06 02:27:53.000000 akellogpt-0.0.3/akellogpt.egg-info/PKG-INFO
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)      545 2023-05-06 02:27:53.000000 akellogpt-0.0.3/akellogpt.egg-info/SOURCES.txt
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)        1 2023-05-06 02:27:53.000000 akellogpt-0.0.3/akellogpt.egg-info/dependency_links.txt
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)       26 2023-05-06 02:27:53.000000 akellogpt-0.0.3/akellogpt.egg-info/requires.txt
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)       10 2023-05-06 02:27:53.000000 akellogpt-0.0.3/akellogpt.egg-info/top_level.txt
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)       38 2023-05-06 02:27:53.742945 akellogpt-0.0.3/setup.cfg
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)      911 2023-05-06 02:27:06.000000 akellogpt-0.0.3/setup.py
+drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-07 23:35:58.229385 akellogpt-0.0.4/
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)     1075 2023-05-05 23:21:08.000000 akellogpt-0.0.4/LICENSE
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)      495 2023-05-07 23:35:58.229241 akellogpt-0.0.4/PKG-INFO
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)     1603 2023-05-07 23:34:16.000000 akellogpt-0.0.4/README.md
+drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-07 23:35:58.226777 akellogpt-0.0.4/akellogpt/
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)        0 2023-05-05 23:21:08.000000 akellogpt-0.0.4/akellogpt/__init__.py
+drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-07 23:35:58.227642 akellogpt-0.0.4/akellogpt/common/
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)        0 2023-05-05 23:21:08.000000 akellogpt-0.0.4/akellogpt/common/__init__.py
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)     1660 2023-05-07 23:34:16.000000 akellogpt-0.0.4/akellogpt/common/api.py
+drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-07 23:35:58.227906 akellogpt-0.0.4/akellogpt/screening/
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)     4440 2023-05-07 23:34:16.000000 akellogpt-0.0.4/akellogpt/screening/__init__.py
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)      412 2023-05-07 05:13:51.000000 akellogpt-0.0.4/akellogpt/screening/mental_health.py
+drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-07 23:35:58.228614 akellogpt-0.0.4/akellogpt/screening/yaml/
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)      883 2023-05-05 23:21:08.000000 akellogpt-0.0.4/akellogpt/screening/yaml/gad7.yaml
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)     1342 2023-05-05 23:21:08.000000 akellogpt-0.0.4/akellogpt/screening/yaml/phq9.yaml
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)     1972 2023-05-05 23:21:08.000000 akellogpt-0.0.4/akellogpt/screening/yaml/sbq-r.yaml
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)       66 2023-05-07 23:34:16.000000 akellogpt-0.0.4/akellogpt/settings.py
+drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-07 23:35:58.229057 akellogpt-0.0.4/akellogpt/test/
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)        0 2023-05-05 23:21:08.000000 akellogpt-0.0.4/akellogpt/test/__init__.py
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)      663 2023-05-07 23:34:16.000000 akellogpt-0.0.4/akellogpt/test/test_gad7.py
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)      682 2023-05-07 23:34:16.000000 akellogpt-0.0.4/akellogpt/test/test_phq9.py
+drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-07 23:35:58.227413 akellogpt-0.0.4/akellogpt.egg-info/
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)      495 2023-05-07 23:35:58.000000 akellogpt-0.0.4/akellogpt.egg-info/PKG-INFO
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)      545 2023-05-07 23:35:58.000000 akellogpt-0.0.4/akellogpt.egg-info/SOURCES.txt
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)        1 2023-05-07 23:35:58.000000 akellogpt-0.0.4/akellogpt.egg-info/dependency_links.txt
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)       26 2023-05-07 23:35:58.000000 akellogpt-0.0.4/akellogpt.egg-info/requires.txt
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)       10 2023-05-07 23:35:58.000000 akellogpt-0.0.4/akellogpt.egg-info/top_level.txt
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)       38 2023-05-07 23:35:58.229422 akellogpt-0.0.4/setup.cfg
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)      911 2023-05-07 23:34:16.000000 akellogpt-0.0.4/setup.py
```

### Comparing `akellogpt-0.0.3/LICENSE` & `akellogpt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `akellogpt-0.0.3/README.md` & `akellogpt-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -43,12 +43,12 @@
 ```
 
 # Future work
 We will be expanding akello-gpt to support Workflows
 
 # Contributing to akello-gtp
 1. Fork it
-2. Create your feature branch (git checkout -b my-new-feature).
-3 Commit your changes (git commit -am 'Added some feature')
+2. Create your feature branch (git checkout -b my-new-feature)
+3. Commit your changes (git commit -am 'Added some feature')
 4. Push to the branch (git push origin my-new-feature)
 5. Create new Pull Request
 6. Tests are in akellogpt/test. To run the tests: python setup.py test
```

### Comparing `akellogpt-0.0.3/akellogpt/screening/yaml/gad7.yaml` & `akellogpt-0.0.4/akellogpt/screening/yaml/gad7.yaml`

 * *Files identical despite different names*

### Comparing `akellogpt-0.0.3/akellogpt/screening/yaml/phq9.yaml` & `akellogpt-0.0.4/akellogpt/screening/yaml/phq9.yaml`

 * *Files identical despite different names*

### Comparing `akellogpt-0.0.3/akellogpt/screening/yaml/sbq-r.yaml` & `akellogpt-0.0.4/akellogpt/screening/yaml/sbq-r.yaml`

 * *Files identical despite different names*

### Comparing `akellogpt-0.0.3/akellogpt/test/test_gad7.py` & `akellogpt-0.0.4/akellogpt/test/test_gad7.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,17 +14,16 @@
     """
 
     @responses.activate
     def test_gad7_object(self):
         """
         Test loading the GAD7 object
         """
-        responses.add(responses.POST, API_URL,
-                      json={'score': 3}, status=200)
-        gad7 = GAD7(akello_api_token='<token>')
+        responses.add(responses.POST, f'{API_URL}/akello-gpt', json={'score': 3}, status=200)
+        gad7 = GAD7(api_token='<token>', account_id='', user_id='')
         gad7.score_screener()
         assert len(gad7.questions) == 7
         assert gad7.score > 0
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `akellogpt-0.0.3/akellogpt/test/test_phq9.py` & `akellogpt-0.0.4/akellogpt/test/test_phq9.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,17 +13,16 @@
     Unit tests for PHQ9 Screener
     """
     @responses.activate
     def test_phq9_object(self):
         """
         Simple test to load the PHQ9 object
         """
-        responses.add(responses.POST, API_URL,
-                      json={'score': 3}, status=200)
-        phq9 = PHQ9(akello_api_token='<token>')
+        responses.add(responses.POST, f'{API_URL}/akello-gpt', json={'score': 3}, status=200)
+        phq9 = PHQ9(api_token='<token>', account_id='', user_id='')
         phq9.score_screener()
         assert len(phq9.questions) == 9
         assert phq9.score > 0
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `akellogpt-0.0.3/akellogpt.egg-info/SOURCES.txt` & `akellogpt-0.0.4/akellogpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akellogpt-0.0.3/setup.py` & `akellogpt-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'ChatGPT for healthcare applications'
 LONG_DESCRIPTION = 'Akello GPT helps ensure deterministic results for healthcare applications '
 
 setup(
     name="akellogpt",
     version=VERSION,
     description=DESCRIPTION,
```

