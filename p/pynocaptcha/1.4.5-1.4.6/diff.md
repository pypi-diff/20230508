# Comparing `tmp/pynocaptcha-1.4.5.tar.gz` & `tmp/pynocaptcha-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pynocaptcha-1.4.5.tar", last modified: Mon May  8 09:27:27 2023, max compression
+gzip compressed data, was "dist/pynocaptcha-1.4.6.tar", last modified: Mon May  8 09:33:31 2023, max compression
```

## Comparing `pynocaptcha-1.4.5.tar` & `pynocaptcha-1.4.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-08 09:27:27.000000 pynocaptcha-1.4.5/
--rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-05-08 09:27:27.000000 pynocaptcha-1.4.5/PKG-INFO
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-08 09:27:27.000000 pynocaptcha-1.4.5/pynocaptcha/
--rw-r--r--   0 esbiya     (501) staff       (20)      508 2023-04-23 09:05:33.000000 pynocaptcha-1.4.5/pynocaptcha/__init__.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-08 09:27:27.000000 pynocaptcha-1.4.5/pynocaptcha/crackers/
--rw-r--r--   0 esbiya     (501) staff       (20)      961 2023-05-08 09:19:50.000000 pynocaptcha-1.4.5/pynocaptcha/crackers/akamai.py
--rw-r--r--   0 esbiya     (501) staff       (20)     4550 2023-05-08 09:21:35.000000 pynocaptcha-1.4.5/pynocaptcha/crackers/base.py
--rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.4.5/pynocaptcha/crackers/cloudflare.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.4.5/pynocaptcha/crackers/hcaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1488 2023-04-23 14:39:24.000000 pynocaptcha-1.4.5/pynocaptcha/crackers/incapsula.py
--rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.4.5/pynocaptcha/crackers/recaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-05-08 09:20:08.000000 pynocaptcha-1.4.5/setup.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-08 09:33:31.000000 pynocaptcha-1.4.6/
+-rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-05-08 09:33:31.000000 pynocaptcha-1.4.6/PKG-INFO
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-08 09:33:31.000000 pynocaptcha-1.4.6/pynocaptcha/
+-rw-r--r--   0 esbiya     (501) staff       (20)      508 2023-04-23 09:05:33.000000 pynocaptcha-1.4.6/pynocaptcha/__init__.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-08 09:33:31.000000 pynocaptcha-1.4.6/pynocaptcha/crackers/
+-rw-r--r--   0 esbiya     (501) staff       (20)      961 2023-05-08 09:19:50.000000 pynocaptcha-1.4.6/pynocaptcha/crackers/akamai.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     4622 2023-05-08 09:32:03.000000 pynocaptcha-1.4.6/pynocaptcha/crackers/base.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.4.6/pynocaptcha/crackers/cloudflare.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.4.6/pynocaptcha/crackers/hcaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1488 2023-04-23 14:39:24.000000 pynocaptcha-1.4.6/pynocaptcha/crackers/incapsula.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.4.6/pynocaptcha/crackers/recaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-05-08 09:32:12.000000 pynocaptcha-1.4.6/setup.py
```

### Comparing `pynocaptcha-1.4.5/PKG-INFO` & `pynocaptcha-1.4.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pynocaptcha
-Version: 1.4.5
+Version: 1.4.6
 Summary: nocaptcha.io api
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: nocaptcha.io python api
 Keywords: nocaptcha
```

### Comparing `pynocaptcha-1.4.5/pynocaptcha/crackers/akamai.py` & `pynocaptcha-1.4.6/pynocaptcha/crackers/akamai.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.5/pynocaptcha/crackers/base.py` & `pynocaptcha-1.4.6/pynocaptcha/crackers/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         user_agent: str = None,
         proxy: str = None, 
         timeout: int = 30,
         debug: bool = False,
         check_useful: bool = False,
         max_retry_times: int = 3,
         internal=True,
+        internal_api=True,
         show_ad=True,
         **kwargs
     ) -> None:
         """
         :param user_token: nocaptcha.io 用户 token
         :param developer_id: nocaptcha.io 用户上级代理 token
         :param user_agent: 请求流程使用 ua
@@ -57,14 +58,15 @@
         self.proxy = proxy
         self.timeout = timeout
         self.debug = debug
         self.check_useful = check_useful
         self.retry_times = 0
         self.max_retry_times = max_retry_times
 
+        self.internal_api = internal_api
         self.wanda_args = {
             "internal": internal
         }
         for k in self.must_check_params:
             _v = kwargs.get(k)
             if not hasattr(self, k) or getattr(self, k) is None:
                 setattr(self, k, _v)
@@ -100,15 +102,15 @@
         if self.proxy:
             self.wanda_args["proxy"] = self.proxy
         
         while 1:
             if self.retry_times < self.max_retry_times:
                 try:
                     resp = requests.post(
-                        f"http://{'xn--fjqs46frol.com' if self.internal else 'api.nocaptcha.io' }/api/wanda/{self.cracker_name}/{self.cracker_version}", 
+                        f"http://{'xn--fjqs46frol.com' if self.internal_api else 'api.nocaptcha.io' }/api/wanda/{self.cracker_name}/{self.cracker_version}", 
                         headers=headers, json=self.wanda_args, timeout=self.timeout
                     ).json()
                     break
                 except Exception as e:
                     if self.debug:
                         logger.error(e)
                     self.retry_times += 1
```

### Comparing `pynocaptcha-1.4.5/pynocaptcha/crackers/cloudflare.py` & `pynocaptcha-1.4.6/pynocaptcha/crackers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.5/pynocaptcha/crackers/hcaptcha.py` & `pynocaptcha-1.4.6/pynocaptcha/crackers/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.5/pynocaptcha/crackers/incapsula.py` & `pynocaptcha-1.4.6/pynocaptcha/crackers/incapsula.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.5/pynocaptcha/crackers/recaptcha.py` & `pynocaptcha-1.4.6/pynocaptcha/crackers/recaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.5/setup.py` & `pynocaptcha-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 
 setup(
     name='pynocaptcha',
-    version='1.4.5',
+    version='1.4.6',
     description='nocaptcha.io api',
     long_description='nocaptcha.io python api',
     install_requires=["pyhttpx", "loguru"],
     license='MIT',
     packages=["pynocaptcha/crackers", "pynocaptcha"],
     package_dir={'pynocaptcha': 'pynocaptcha'},
     platforms=["all"],
```

