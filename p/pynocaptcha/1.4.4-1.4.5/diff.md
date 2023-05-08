# Comparing `tmp/pynocaptcha-1.4.4.tar.gz` & `tmp/pynocaptcha-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pynocaptcha-1.4.4.tar", last modified: Mon Apr 24 03:56:25 2023, max compression
+gzip compressed data, was "dist/pynocaptcha-1.4.5.tar", last modified: Mon May  8 09:27:27 2023, max compression
```

## Comparing `pynocaptcha-1.4.4.tar` & `pynocaptcha-1.4.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-24 03:56:25.000000 pynocaptcha-1.4.4/
--rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-04-24 03:56:25.000000 pynocaptcha-1.4.4/PKG-INFO
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-24 03:56:25.000000 pynocaptcha-1.4.4/pynocaptcha/
--rw-r--r--   0 esbiya     (501) staff       (20)      508 2023-04-23 09:05:33.000000 pynocaptcha-1.4.4/pynocaptcha/__init__.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-24 03:56:25.000000 pynocaptcha-1.4.4/pynocaptcha/crackers/
--rw-r--r--   0 esbiya     (501) staff       (20)      722 2023-04-23 09:55:53.000000 pynocaptcha-1.4.4/pynocaptcha/crackers/akamai.py
--rw-r--r--   0 esbiya     (501) staff       (20)     4502 2023-04-24 03:56:03.000000 pynocaptcha-1.4.4/pynocaptcha/crackers/base.py
--rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.4.4/pynocaptcha/crackers/cloudflare.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.4.4/pynocaptcha/crackers/hcaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1488 2023-04-23 14:39:24.000000 pynocaptcha-1.4.4/pynocaptcha/crackers/incapsula.py
--rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.4.4/pynocaptcha/crackers/recaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-04-24 03:56:23.000000 pynocaptcha-1.4.4/setup.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-08 09:27:27.000000 pynocaptcha-1.4.5/
+-rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-05-08 09:27:27.000000 pynocaptcha-1.4.5/PKG-INFO
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-08 09:27:27.000000 pynocaptcha-1.4.5/pynocaptcha/
+-rw-r--r--   0 esbiya     (501) staff       (20)      508 2023-04-23 09:05:33.000000 pynocaptcha-1.4.5/pynocaptcha/__init__.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-08 09:27:27.000000 pynocaptcha-1.4.5/pynocaptcha/crackers/
+-rw-r--r--   0 esbiya     (501) staff       (20)      961 2023-05-08 09:19:50.000000 pynocaptcha-1.4.5/pynocaptcha/crackers/akamai.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     4550 2023-05-08 09:21:35.000000 pynocaptcha-1.4.5/pynocaptcha/crackers/base.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.4.5/pynocaptcha/crackers/cloudflare.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.4.5/pynocaptcha/crackers/hcaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1488 2023-04-23 14:39:24.000000 pynocaptcha-1.4.5/pynocaptcha/crackers/incapsula.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.4.5/pynocaptcha/crackers/recaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-05-08 09:20:08.000000 pynocaptcha-1.4.5/setup.py
```

### Comparing `pynocaptcha-1.4.4/PKG-INFO` & `pynocaptcha-1.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pynocaptcha
-Version: 1.4.4
+Version: 1.4.5
 Summary: nocaptcha.io api
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: nocaptcha.io python api
 Keywords: nocaptcha
```

### Comparing `pynocaptcha-1.4.4/pynocaptcha/crackers/akamai.py` & `pynocaptcha-1.4.5/pynocaptcha/crackers/akamai.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     cracker_version = "v2"    
 
     """
     recaptcha universal cracker
     :param href: 触发验证的页面地址
     :param api: akamai 提交 sensor_data 的地址
     :param telemetry: 是否 headers 中的 telemetry 参数验证形式, 默认 false
+    :param _abck: 请求 href 首页返回的 cookie _abck 值, 传了 api 参数必须传该值
+    :param bm_sz: 请求 href 首页返回的 cookie bm_sz 值, 传了 api 参数必须传该值
     调用示例:
     cracker = AkamaiV2Cracker(
         user_token="xxx",
         href="xxx",
         api="xxx",
         
         # debug=True,
@@ -26,8 +28,10 @@
     
     # 必传参数
     must_check_params = ["href"]
     # 默认可选参数
     option_params = {
         "api": "",
         "telemetry": False,
+        "_abck": None,
+        "bm_sz": None
     }
```

### Comparing `pynocaptcha-1.4.4/pynocaptcha/crackers/base.py` & `pynocaptcha-1.4.5/pynocaptcha/crackers/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         if self.proxy:
             self.wanda_args["proxy"] = self.proxy
         
         while 1:
             if self.retry_times < self.max_retry_times:
                 try:
                     resp = requests.post(
-                        f"http://api.nocaptcha.io/api/wanda/{self.cracker_name}/{self.cracker_version}", 
+                        f"http://{'xn--fjqs46frol.com' if self.internal else 'api.nocaptcha.io' }/api/wanda/{self.cracker_name}/{self.cracker_version}", 
                         headers=headers, json=self.wanda_args, timeout=self.timeout
                     ).json()
                     break
                 except Exception as e:
                     if self.debug:
                         logger.error(e)
                     self.retry_times += 1
```

### Comparing `pynocaptcha-1.4.4/pynocaptcha/crackers/cloudflare.py` & `pynocaptcha-1.4.5/pynocaptcha/crackers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.4/pynocaptcha/crackers/hcaptcha.py` & `pynocaptcha-1.4.5/pynocaptcha/crackers/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.4/pynocaptcha/crackers/incapsula.py` & `pynocaptcha-1.4.5/pynocaptcha/crackers/incapsula.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.4/pynocaptcha/crackers/recaptcha.py` & `pynocaptcha-1.4.5/pynocaptcha/crackers/recaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.4/setup.py` & `pynocaptcha-1.4.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 
 setup(
     name='pynocaptcha',
-    version='1.4.4',
+    version='1.4.5',
     description='nocaptcha.io api',
     long_description='nocaptcha.io python api',
     install_requires=["pyhttpx", "loguru"],
     license='MIT',
     packages=["pynocaptcha/crackers", "pynocaptcha"],
     package_dir={'pynocaptcha': 'pynocaptcha'},
     platforms=["all"],
```

