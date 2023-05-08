# Comparing `tmp/vcsc_data_common-0.1.5.tar.gz` & `tmp/vcsc_data_common-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcsc_data_common-0.1.5.tar", last modified: Fri May  5 07:00:02 2023, max compression
+gzip compressed data, was "vcsc_data_common-0.1.6.tar", last modified: Mon May  8 09:19:34 2023, max compression
```

## Comparing `vcsc_data_common-0.1.5.tar` & `vcsc_data_common-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-05 07:00:02.378660 vcsc_data_common-0.1.5/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-05-05 07:00:02.378763 vcsc_data_common-0.1.5/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.1.5/README.md
--rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.1.5/pyproject.toml
--rw-r--r--   0 pd         (501) staff       (20)      339 2023-05-05 07:00:02.379138 vcsc_data_common-0.1.5/setup.cfg
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-05 07:00:02.375260 vcsc_data_common-0.1.5/vcsc_data_common/
--rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.1.5/vcsc_data_common/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-05 07:00:02.377243 vcsc_data_common-0.1.5/vcsc_data_common/ai_framework/
--rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.1.5/vcsc_data_common/ai_framework/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     4948 2023-03-31 09:44:29.000000 vcsc_data_common-0.1.5/vcsc_data_common/ai_framework/interval_fetching.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-05 07:00:02.377531 vcsc_data_common-0.1.5/vcsc_data_common/live_price_data/
--rw-r--r--   0 pd         (501) staff       (20)     2341 2023-05-04 06:36:10.000000 vcsc_data_common-0.1.5/vcsc_data_common/live_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-05 07:00:02.377834 vcsc_data_common-0.1.5/vcsc_data_common/offline_price_data/
--rw-r--r--   0 pd         (501) staff       (20)      880 2023-03-14 02:58:59.000000 vcsc_data_common-0.1.5/vcsc_data_common/offline_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-05 07:00:02.378116 vcsc_data_common-0.1.5/vcsc_data_common/order/
--rw-r--r--   0 pd         (501) staff       (20)     3647 2023-03-27 04:29:07.000000 vcsc_data_common-0.1.5/vcsc_data_common/order/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-05 07:00:02.378405 vcsc_data_common-0.1.5/vcsc_data_common/portfolio_info/
--rw-r--r--   0 pd         (501) staff       (20)     3476 2023-05-05 06:59:07.000000 vcsc_data_common-0.1.5/vcsc_data_common/portfolio_info/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-05 07:00:02.376747 vcsc_data_common-0.1.5/vcsc_data_common.egg-info/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-05-05 07:00:02.000000 vcsc_data_common-0.1.5/vcsc_data_common.egg-info/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      527 2023-05-05 07:00:02.000000 vcsc_data_common-0.1.5/vcsc_data_common.egg-info/SOURCES.txt
--rw-r--r--   0 pd         (501) staff       (20)        1 2023-05-05 07:00:02.000000 vcsc_data_common-0.1.5/vcsc_data_common.egg-info/dependency_links.txt
--rw-r--r--   0 pd         (501) staff       (20)      140 2023-05-05 07:00:02.000000 vcsc_data_common-0.1.5/vcsc_data_common.egg-info/requires.txt
--rw-r--r--   0 pd         (501) staff       (20)       17 2023-05-05 07:00:02.000000 vcsc_data_common-0.1.5/vcsc_data_common.egg-info/top_level.txt
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-08 09:19:34.400389 vcsc_data_common-0.1.6/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-05-08 09:19:34.402016 vcsc_data_common-0.1.6/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.1.6/README.md
+-rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.1.6/pyproject.toml
+-rw-r--r--   0 pd         (501) staff       (20)      339 2023-05-08 09:19:34.403007 vcsc_data_common-0.1.6/setup.cfg
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-08 09:19:34.395794 vcsc_data_common-0.1.6/vcsc_data_common/
+-rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.1.6/vcsc_data_common/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-08 09:19:34.397682 vcsc_data_common-0.1.6/vcsc_data_common/ai_framework/
+-rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.1.6/vcsc_data_common/ai_framework/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     4948 2023-03-31 09:44:29.000000 vcsc_data_common-0.1.6/vcsc_data_common/ai_framework/interval_fetching.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-08 09:19:34.398183 vcsc_data_common-0.1.6/vcsc_data_common/live_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)     2341 2023-05-04 06:36:10.000000 vcsc_data_common-0.1.6/vcsc_data_common/live_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-08 09:19:34.398531 vcsc_data_common-0.1.6/vcsc_data_common/offline_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)      880 2023-03-14 02:58:59.000000 vcsc_data_common-0.1.6/vcsc_data_common/offline_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-08 09:19:34.398889 vcsc_data_common-0.1.6/vcsc_data_common/order/
+-rw-r--r--   0 pd         (501) staff       (20)     3647 2023-03-27 04:29:07.000000 vcsc_data_common-0.1.6/vcsc_data_common/order/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-08 09:19:34.399806 vcsc_data_common-0.1.6/vcsc_data_common/portfolio_info/
+-rw-r--r--   0 pd         (501) staff       (20)     3660 2023-05-08 09:14:23.000000 vcsc_data_common-0.1.6/vcsc_data_common/portfolio_info/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-08 09:19:34.396747 vcsc_data_common-0.1.6/vcsc_data_common.egg-info/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-05-08 09:19:34.000000 vcsc_data_common-0.1.6/vcsc_data_common.egg-info/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      527 2023-05-08 09:19:34.000000 vcsc_data_common-0.1.6/vcsc_data_common.egg-info/SOURCES.txt
+-rw-r--r--   0 pd         (501) staff       (20)        1 2023-05-08 09:19:34.000000 vcsc_data_common-0.1.6/vcsc_data_common.egg-info/dependency_links.txt
+-rw-r--r--   0 pd         (501) staff       (20)      140 2023-05-08 09:19:34.000000 vcsc_data_common-0.1.6/vcsc_data_common.egg-info/requires.txt
+-rw-r--r--   0 pd         (501) staff       (20)       17 2023-05-08 09:19:34.000000 vcsc_data_common-0.1.6/vcsc_data_common.egg-info/top_level.txt
```

### Comparing `vcsc_data_common-0.1.5/pyproject.toml` & `vcsc_data_common-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.5/vcsc_data_common/ai_framework/interval_fetching.py` & `vcsc_data_common-0.1.6/vcsc_data_common/ai_framework/interval_fetching.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.5/vcsc_data_common/live_price_data/__init__.py` & `vcsc_data_common-0.1.6/vcsc_data_common/live_price_data/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.5/vcsc_data_common/offline_price_data/__init__.py` & `vcsc_data_common-0.1.6/vcsc_data_common/offline_price_data/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.5/vcsc_data_common/order/__init__.py` & `vcsc_data_common-0.1.6/vcsc_data_common/order/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.5/vcsc_data_common/portfolio_info/__init__.py` & `vcsc_data_common-0.1.6/vcsc_data_common/portfolio_info/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,26 +51,31 @@
                 f'update_target_percent_portfolio ==> {response.text}')
         else:
             logging.error(
                 f'update_target_percent_portfolio ==> {response.text}')
             raise Exception('update_target_percent_portfolio failed')
 
         ### hard code backtest môi trường dev ###
-        url = f"http://10.11.0.99:31377/portfolioRatio/updateNewRatio"
+        try:
+            url = f"http://10.11.0.99:31377/portfolioRatio/updateNewRatio"
 
-        payload = json.dumps({
-            "ratio": portfolio_data,
-            "portfolioModel": portfolioModel
-        })
-        headers = {
-            'Content-Type': 'application/json'
-        }
+            payload = json.dumps({
+                "ratio": portfolio_data,
+                "portfolioModel": portfolioModel
+            })
+            headers = {
+                'Content-Type': 'application/json'
+            }
 
-        response = requests.request("POST", url, headers=headers, data=payload)
+            response = requests.request(
+                "POST", url, headers=headers, data=payload)
 
-        if(response.status_code == 200):
-            logging.info(
-                f'update_target_percent_portfolio ==> {response.text}')
-        else:
-            logging.error(
-                f'update_target_percent_portfolio ==> {response.text}')
-            raise Exception('update_target_percent_portfolio failed')
+            if(response.status_code == 200):
+                logging.info(
+                    f'update_target_percent_portfolio ==> {response.text}')
+            else:
+                logging.error(
+                    f'update_target_percent_portfolio ==> {response.text}')
+                raise Exception('update_target_percent_portfolio failed')
+        except:
+            logging.error('fail update dev environment')
+            pass
```

### Comparing `vcsc_data_common-0.1.5/vcsc_data_common.egg-info/SOURCES.txt` & `vcsc_data_common-0.1.6/vcsc_data_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

