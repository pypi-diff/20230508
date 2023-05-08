# Comparing `tmp/custard-1.1.5.tar.gz` & `tmp/custard-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custard-1.1.5.tar", max compression
+gzip compressed data, was "custard-1.1.6.tar", max compression
```

## Comparing `custard-1.1.5.tar` & `custard-1.1.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     5589 2023-04-29 16:20:12.886455 custard-1.1.5/README.md
--rw-r--r--   0        0        0      236 2023-04-29 16:20:12.886455 custard-1.1.5/custard/__init__.py
--rw-r--r--   0        0        0     1192 2023-04-29 16:20:12.886455 custard-1.1.5/custard/core/__init__.py
--rw-r--r--   0        0        0   770290 2023-04-29 16:20:12.886455 custard-1.1.5/custard/core/decode.py
--rw-r--r--   0        0        0    28635 2023-04-29 16:20:12.886455 custard-1.1.5/custard/core/factory.py
--rw-r--r--   0        0        0    13726 2023-04-29 16:20:12.890456 custard-1.1.5/custard/core/functools.py
--rw-r--r--   0        0        0     2976 2023-04-29 16:20:12.890456 custard-1.1.5/custard/core/kerberos.py
--rw-r--r--   0        0        0    25958 2023-04-29 16:20:12.890456 custard-1.1.5/custard/core/processor.py
--rw-r--r--   0        0        0    20274 2023-04-29 16:20:12.890456 custard-1.1.5/custard/core/regular.py
--rw-r--r--   0        0        0    15684 2023-04-29 16:20:12.890456 custard-1.1.5/custard/core/system.py
--rw-r--r--   0        0        0    22041 2023-04-29 16:20:12.890456 custard-1.1.5/custard/core/useragent.py
--rw-r--r--   0        0        0     1607 2023-04-29 16:20:12.890456 custard-1.1.5/custard/core/xml2dict.py
--rw-r--r--   0        0        0     1853 2023-04-29 16:20:12.890456 custard-1.1.5/custard/core/xprint.py
--rw-r--r--   0        0        0      463 2023-04-29 16:20:12.890456 custard-1.1.5/custard/crypto/__init__.py
--rw-r--r--   0        0        0    15682 2023-04-29 16:20:12.890456 custard-1.1.5/custard/crypto/crypto.py
--rw-r--r--   0        0        0     3257 2023-04-29 16:20:12.890456 custard-1.1.5/custard/crypto/streambody.py
--rw-r--r--   0        0        0      323 2023-04-29 16:20:12.890456 custard-1.1.5/custard/curl/__init__.py
--rw-r--r--   0        0        0     5936 2023-04-29 16:20:12.890456 custard-1.1.5/custard/curl/parse.py
--rw-r--r--   0        0        0      291 2023-04-29 16:20:12.890456 custard-1.1.5/custard/hitfilter/__init__.py
--rw-r--r--   0        0        0     2972 2023-04-29 16:20:12.890456 custard-1.1.5/custard/hitfilter/hitfilter.py
--rw-r--r--   0        0        0   761348 2023-04-29 16:20:12.894456 custard-1.1.5/custard/hitfilter/keywords
--rw-r--r--   0        0        0      418 2023-04-29 16:20:12.894456 custard-1.1.5/custard/kaptcha/__init__.py
--rw-r--r--   0        0        0     9386 2023-04-29 16:20:12.894456 custard-1.1.5/custard/kaptcha/captcha.py
--rw-r--r--   0        0        0   171508 2023-04-29 16:20:12.894456 custard-1.1.5/custard/kaptcha/font1.ttf
--rw-r--r--   0        0        0    42452 2023-04-29 16:20:12.894456 custard-1.1.5/custard/kaptcha/font2.ttf
--rw-r--r--   0        0        0    92956 2023-04-29 16:20:12.898455 custard-1.1.5/custard/kaptcha/font3.ttf
--rw-r--r--   0        0        0   314452 2023-04-29 16:20:12.898455 custard-1.1.5/custard/kaptcha/font4.ttf
--rw-r--r--   0        0        0     3411 2023-04-29 16:20:12.898455 custard-1.1.5/custard/limiter/README.md
--rw-r--r--   0        0        0     2584 2023-04-29 16:20:12.898455 custard-1.1.5/custard/limiter/__init__.py
--rw-r--r--   0        0        0     2818 2023-04-29 16:20:12.898455 custard-1.1.5/custard/limiter/depends.py
--rw-r--r--   0        0        0      452 2023-04-29 16:20:12.898455 custard-1.1.5/custard/limiter/enums.py
--rw-r--r--   0        0        0     1705 2023-04-29 16:20:12.898455 custard-1.1.5/custard/limiter/examples/__init__.py
--rw-r--r--   0        0        0     1962 2023-04-29 16:20:12.898455 custard-1.1.5/custard/limiter/examples/test_depends.py
--rw-r--r--   0        0        0      438 2023-04-29 16:20:12.898455 custard-1.1.5/custard/limiter/execres.py
--rw-r--r--   0        0        0     1819 2023-04-29 16:20:12.898455 custard-1.1.5/custard/mock/__init__.py
--rw-r--r--   0        0        0    14336 2023-04-29 16:20:12.898455 custard-1.1.5/custard/mock/mini_racer.py
--rw-r--r--   0        0        0   366292 2023-04-29 16:20:12.902455 custard-1.1.5/custard/mock/mock.min.js
--rw-r--r--   0        0        0   292581 2023-04-29 16:20:12.902455 custard-1.1.5/custard/mock/mock.old.min.js
--rw-r--r--   0        0        0      696 2023-04-29 16:20:12.902455 custard-1.1.5/custard/pagination/__init__.py
--rw-r--r--   0        0        0     4249 2023-04-29 16:20:12.902455 custard-1.1.5/custard/pagination/api.py
--rw-r--r--   0        0        0     1094 2023-04-29 16:20:12.902455 custard-1.1.5/custard/pagination/async_sqlalchemy.py
--rw-r--r--   0        0        0     2741 2023-04-29 16:20:12.902455 custard-1.1.5/custard/pagination/bases.py
--rw-r--r--   0        0        0     1322 2023-04-29 16:20:12.902455 custard-1.1.5/custard/pagination/iterables.py
--rw-r--r--   0        0        0     1437 2023-04-29 16:20:12.902455 custard-1.1.5/custard/pagination/limit_offset.py
--rw-r--r--   0        0        0     1658 2023-04-29 16:20:12.902455 custard-1.1.5/custard/pagination/pagination.py
--rw-r--r--   0        0        0      847 2023-04-29 16:20:12.902455 custard-1.1.5/custard/pagination/paginator.py
--rw-r--r--   0        0        0     1107 2023-04-29 16:20:12.902455 custard-1.1.5/custard/pagination/sync_sqlalchemy.py
--rw-r--r--   0        0        0      990 2023-04-29 16:20:12.902455 custard-1.1.5/custard/swagger/__init__.py
--rw-r--r--   0        0        0      328 2023-04-29 16:20:12.902455 custard-1.1.5/custard/swagger/exception.py
--rw-r--r--   0        0        0     6423 2023-04-29 16:20:12.902455 custard-1.1.5/custard/swagger/swagger.py
--rw-r--r--   0        0        0      584 2023-04-29 16:20:12.902455 custard-1.1.5/custard/swagger/utils.py
--rw-r--r--   0        0        0      644 2023-04-29 16:20:12.902455 custard-1.1.5/custard/time/__init__.py
--rw-r--r--   0        0        0     6299 2023-04-29 16:20:12.902455 custard-1.1.5/custard/time/dafunc.py
--rw-r--r--   0        0        0     1673 2023-04-29 16:20:12.902455 custard-1.1.5/custard/time/exceptions.py
--rw-r--r--   0        0        0     5752 2023-04-29 16:20:12.902455 custard-1.1.5/custard/time/moment.py
--rw-r--r--   0        0        0     1692 2023-04-29 16:20:12.902455 custard-1.1.5/custard/time/stoppable_thread.py
--rw-r--r--   0        0        0      233 2023-04-29 16:20:12.902455 custard-1.1.5/custard/utils/__init__.py
--rw-r--r--   0        0        0   161226 2023-04-29 16:20:12.902455 custard-1.1.5/custard/utils/area_code.py
--rw-r--r--   0        0        0     3895 2023-04-29 16:20:12.902455 custard-1.1.5/custard/utils/configparser.py
--rw-r--r--   0        0        0     3754 2023-04-29 16:20:12.902455 custard-1.1.5/custard/utils/id_cards.py
--rw-r--r--   0        0        0    85077 2023-04-29 16:20:12.906455 custard-1.1.5/custard/utils/jenkins.py
--rw-r--r--   0        0        0    24805 2023-04-29 16:20:12.906455 custard-1.1.5/custard/utils/multi.py
--rw-r--r--   0        0        0     4555 2023-04-29 16:20:12.906455 custard-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     8753 1970-01-01 00:00:00.000000 custard-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     5589 2023-05-08 07:38:47.968252 custard-1.1.6/README.md
+-rw-r--r--   0        0        0      236 2023-05-08 07:38:47.968252 custard-1.1.6/custard/__init__.py
+-rw-r--r--   0        0        0     1192 2023-05-08 07:38:47.968252 custard-1.1.6/custard/core/__init__.py
+-rw-r--r--   0        0        0   770290 2023-05-08 07:38:47.972252 custard-1.1.6/custard/core/decode.py
+-rw-r--r--   0        0        0    28635 2023-05-08 07:38:47.972252 custard-1.1.6/custard/core/factory.py
+-rw-r--r--   0        0        0    13726 2023-05-08 07:38:47.972252 custard-1.1.6/custard/core/functools.py
+-rw-r--r--   0        0        0     2976 2023-05-08 07:38:47.972252 custard-1.1.6/custard/core/kerberos.py
+-rw-r--r--   0        0        0    25958 2023-05-08 07:38:47.972252 custard-1.1.6/custard/core/processor.py
+-rw-r--r--   0        0        0    20274 2023-05-08 07:38:47.972252 custard-1.1.6/custard/core/regular.py
+-rw-r--r--   0        0        0    15703 2023-05-08 07:38:47.972252 custard-1.1.6/custard/core/system.py
+-rw-r--r--   0        0        0    22041 2023-05-08 07:38:47.972252 custard-1.1.6/custard/core/useragent.py
+-rw-r--r--   0        0        0     1607 2023-05-08 07:38:47.972252 custard-1.1.6/custard/core/xml2dict.py
+-rw-r--r--   0        0        0     1853 2023-05-08 07:38:47.972252 custard-1.1.6/custard/core/xprint.py
+-rw-r--r--   0        0        0      463 2023-05-08 07:38:47.972252 custard-1.1.6/custard/crypto/__init__.py
+-rw-r--r--   0        0        0    15682 2023-05-08 07:38:47.972252 custard-1.1.6/custard/crypto/crypto.py
+-rw-r--r--   0        0        0     3257 2023-05-08 07:38:47.972252 custard-1.1.6/custard/crypto/streambody.py
+-rw-r--r--   0        0        0      323 2023-05-08 07:38:47.972252 custard-1.1.6/custard/curl/__init__.py
+-rw-r--r--   0        0        0     5936 2023-05-08 07:38:47.972252 custard-1.1.6/custard/curl/parse.py
+-rw-r--r--   0        0        0      291 2023-05-08 07:38:47.972252 custard-1.1.6/custard/hitfilter/__init__.py
+-rw-r--r--   0        0        0     2972 2023-05-08 07:38:47.972252 custard-1.1.6/custard/hitfilter/hitfilter.py
+-rw-r--r--   0        0        0   761348 2023-05-08 07:38:47.976252 custard-1.1.6/custard/hitfilter/keywords
+-rw-r--r--   0        0        0      418 2023-05-08 07:38:47.976252 custard-1.1.6/custard/kaptcha/__init__.py
+-rw-r--r--   0        0        0     9386 2023-05-08 07:38:47.976252 custard-1.1.6/custard/kaptcha/captcha.py
+-rw-r--r--   0        0        0   171508 2023-05-08 07:38:47.980252 custard-1.1.6/custard/kaptcha/font1.ttf
+-rw-r--r--   0        0        0    42452 2023-05-08 07:38:47.980252 custard-1.1.6/custard/kaptcha/font2.ttf
+-rw-r--r--   0        0        0    92956 2023-05-08 07:38:47.980252 custard-1.1.6/custard/kaptcha/font3.ttf
+-rw-r--r--   0        0        0   314452 2023-05-08 07:38:47.980252 custard-1.1.6/custard/kaptcha/font4.ttf
+-rw-r--r--   0        0        0     3411 2023-05-08 07:38:47.980252 custard-1.1.6/custard/limiter/README.md
+-rw-r--r--   0        0        0     2584 2023-05-08 07:38:47.980252 custard-1.1.6/custard/limiter/__init__.py
+-rw-r--r--   0        0        0     2818 2023-05-08 07:38:47.980252 custard-1.1.6/custard/limiter/depends.py
+-rw-r--r--   0        0        0      452 2023-05-08 07:38:47.980252 custard-1.1.6/custard/limiter/enums.py
+-rw-r--r--   0        0        0     1705 2023-05-08 07:38:47.980252 custard-1.1.6/custard/limiter/examples/__init__.py
+-rw-r--r--   0        0        0     1962 2023-05-08 07:38:47.980252 custard-1.1.6/custard/limiter/examples/test_depends.py
+-rw-r--r--   0        0        0      438 2023-05-08 07:38:47.980252 custard-1.1.6/custard/limiter/execres.py
+-rw-r--r--   0        0        0     1819 2023-05-08 07:38:47.980252 custard-1.1.6/custard/mock/__init__.py
+-rw-r--r--   0        0        0    14336 2023-05-08 07:38:47.980252 custard-1.1.6/custard/mock/mini_racer.py
+-rw-r--r--   0        0        0   366292 2023-05-08 07:38:47.984252 custard-1.1.6/custard/mock/mock.min.js
+-rw-r--r--   0        0        0   292581 2023-05-08 07:38:47.984252 custard-1.1.6/custard/mock/mock.old.min.js
+-rw-r--r--   0        0        0      696 2023-05-08 07:38:47.984252 custard-1.1.6/custard/pagination/__init__.py
+-rw-r--r--   0        0        0     4249 2023-05-08 07:38:47.984252 custard-1.1.6/custard/pagination/api.py
+-rw-r--r--   0        0        0     1094 2023-05-08 07:38:47.984252 custard-1.1.6/custard/pagination/async_sqlalchemy.py
+-rw-r--r--   0        0        0     2741 2023-05-08 07:38:47.984252 custard-1.1.6/custard/pagination/bases.py
+-rw-r--r--   0        0        0     1322 2023-05-08 07:38:47.984252 custard-1.1.6/custard/pagination/iterables.py
+-rw-r--r--   0        0        0     1437 2023-05-08 07:38:47.984252 custard-1.1.6/custard/pagination/limit_offset.py
+-rw-r--r--   0        0        0     1658 2023-05-08 07:38:47.984252 custard-1.1.6/custard/pagination/pagination.py
+-rw-r--r--   0        0        0      847 2023-05-08 07:38:47.984252 custard-1.1.6/custard/pagination/paginator.py
+-rw-r--r--   0        0        0     1107 2023-05-08 07:38:47.984252 custard-1.1.6/custard/pagination/sync_sqlalchemy.py
+-rw-r--r--   0        0        0      990 2023-05-08 07:38:47.984252 custard-1.1.6/custard/swagger/__init__.py
+-rw-r--r--   0        0        0      328 2023-05-08 07:38:47.984252 custard-1.1.6/custard/swagger/exception.py
+-rw-r--r--   0        0        0     6423 2023-05-08 07:38:47.984252 custard-1.1.6/custard/swagger/swagger.py
+-rw-r--r--   0        0        0      584 2023-05-08 07:38:47.984252 custard-1.1.6/custard/swagger/utils.py
+-rw-r--r--   0        0        0      644 2023-05-08 07:38:47.984252 custard-1.1.6/custard/time/__init__.py
+-rw-r--r--   0        0        0     6299 2023-05-08 07:38:47.984252 custard-1.1.6/custard/time/dafunc.py
+-rw-r--r--   0        0        0     1673 2023-05-08 07:38:47.984252 custard-1.1.6/custard/time/exceptions.py
+-rw-r--r--   0        0        0     5752 2023-05-08 07:38:47.984252 custard-1.1.6/custard/time/moment.py
+-rw-r--r--   0        0        0     1692 2023-05-08 07:38:47.984252 custard-1.1.6/custard/time/stoppable_thread.py
+-rw-r--r--   0        0        0      233 2023-05-08 07:38:47.984252 custard-1.1.6/custard/utils/__init__.py
+-rw-r--r--   0        0        0   161226 2023-05-08 07:38:47.984252 custard-1.1.6/custard/utils/area_code.py
+-rw-r--r--   0        0        0     3895 2023-05-08 07:38:47.984252 custard-1.1.6/custard/utils/configparser.py
+-rw-r--r--   0        0        0     3754 2023-05-08 07:38:47.984252 custard-1.1.6/custard/utils/id_cards.py
+-rw-r--r--   0        0        0    85077 2023-05-08 07:38:47.988252 custard-1.1.6/custard/utils/jenkins.py
+-rw-r--r--   0        0        0    24805 2023-05-08 07:38:47.988252 custard-1.1.6/custard/utils/multi.py
+-rw-r--r--   0        0        0     4490 2023-05-08 07:38:47.988252 custard-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     8598 1970-01-01 00:00:00.000000 custard-1.1.6/PKG-INFO
```

### Comparing `custard-1.1.5/README.md` & `custard-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/core/__init__.py` & `custard-1.1.6/custard/core/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/core/decode.py` & `custard-1.1.6/custard/core/decode.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/core/factory.py` & `custard-1.1.6/custard/core/factory.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/core/functools.py` & `custard-1.1.6/custard/core/functools.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/core/kerberos.py` & `custard-1.1.6/custard/core/kerberos.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/core/processor.py` & `custard-1.1.6/custard/core/processor.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/core/regular.py` & `custard-1.1.6/custard/core/regular.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/core/system.py` & `custard-1.1.6/custard/core/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
             >>> root_dir = "../../custard"
             >>> SystemHand.walk(root_dir)
         """
         result = []
         dirs = [os.path.join(root_dir, index) for index in os.listdir(root_dir)]
         for index in dirs:
             for root, dirs, files in os.walk(index, topdown=False):
-                file_path = [os.path.join(root, file) for file in files]
+                file_path = [os.path.join(root, file).replace('\\', '/') for file in files]
                 result += file_path
         return result
 
     @classmethod
     def get_current_path(cls):
         """
         获取当前文件路径
```

### Comparing `custard-1.1.5/custard/core/useragent.py` & `custard-1.1.6/custard/core/useragent.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/core/xml2dict.py` & `custard-1.1.6/custard/core/xml2dict.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/core/xprint.py` & `custard-1.1.6/custard/core/xprint.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/crypto/crypto.py` & `custard-1.1.6/custard/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/crypto/streambody.py` & `custard-1.1.6/custard/crypto/streambody.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/curl/parse.py` & `custard-1.1.6/custard/curl/parse.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/hitfilter/hitfilter.py` & `custard-1.1.6/custard/hitfilter/hitfilter.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/hitfilter/keywords` & `custard-1.1.6/custard/hitfilter/keywords`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/kaptcha/captcha.py` & `custard-1.1.6/custard/kaptcha/captcha.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/kaptcha/font1.ttf` & `custard-1.1.6/custard/kaptcha/font1.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/kaptcha/font2.ttf` & `custard-1.1.6/custard/kaptcha/font2.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/kaptcha/font3.ttf` & `custard-1.1.6/custard/kaptcha/font3.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/kaptcha/font4.ttf` & `custard-1.1.6/custard/kaptcha/font4.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/limiter/README.md` & `custard-1.1.6/custard/limiter/README.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/limiter/__init__.py` & `custard-1.1.6/custard/limiter/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/limiter/depends.py` & `custard-1.1.6/custard/limiter/depends.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/limiter/examples/__init__.py` & `custard-1.1.6/custard/limiter/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/limiter/examples/test_depends.py` & `custard-1.1.6/custard/limiter/examples/test_depends.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/mock/__init__.py` & `custard-1.1.6/custard/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/mock/mini_racer.py` & `custard-1.1.6/custard/mock/mini_racer.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/mock/mock.min.js` & `custard-1.1.6/custard/mock/mock.min.js`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/mock/mock.old.min.js` & `custard-1.1.6/custard/mock/mock.old.min.js`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/pagination/__init__.py` & `custard-1.1.6/custard/pagination/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/pagination/api.py` & `custard-1.1.6/custard/pagination/api.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/pagination/async_sqlalchemy.py` & `custard-1.1.6/custard/pagination/async_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/pagination/bases.py` & `custard-1.1.6/custard/pagination/bases.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/pagination/iterables.py` & `custard-1.1.6/custard/pagination/iterables.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/pagination/limit_offset.py` & `custard-1.1.6/custard/pagination/limit_offset.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/pagination/pagination.py` & `custard-1.1.6/custard/pagination/pagination.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/pagination/paginator.py` & `custard-1.1.6/custard/pagination/paginator.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/pagination/sync_sqlalchemy.py` & `custard-1.1.6/custard/pagination/sync_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/swagger/__init__.py` & `custard-1.1.6/custard/swagger/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/swagger/swagger.py` & `custard-1.1.6/custard/swagger/swagger.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/swagger/utils.py` & `custard-1.1.6/custard/swagger/utils.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/time/__init__.py` & `custard-1.1.6/custard/time/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/time/dafunc.py` & `custard-1.1.6/custard/time/dafunc.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/time/exceptions.py` & `custard-1.1.6/custard/time/exceptions.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/time/moment.py` & `custard-1.1.6/custard/time/moment.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/time/stoppable_thread.py` & `custard-1.1.6/custard/time/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/utils/area_code.py` & `custard-1.1.6/custard/utils/area_code.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/utils/configparser.py` & `custard-1.1.6/custard/utils/configparser.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/utils/id_cards.py` & `custard-1.1.6/custard/utils/id_cards.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/utils/jenkins.py` & `custard-1.1.6/custard/utils/jenkins.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/custard/utils/multi.py` & `custard-1.1.6/custard/utils/multi.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.5/pyproject.toml` & `custard-1.1.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "custard"
-version = "1.1.5"
+version = "1.1.6"
 description = "custard easy to learn, fast to code, ready for production"
 readme = "README.md"
 license = "MIT"
 authors = ["Kamalyes <mryu168@163.com>",]
 
 repository = "https://github.com/kamalyes/custard"
 
@@ -18,57 +18,54 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 mypy = "^1.2.0"
-ruff = "^0.0.263"
+ruff = ">=0.0.263,<0.0.266"
 types-PyYAML="^6.0.12.9"
 types-requests="^2.29.0.0"
 types-urllib3="^1.26.25.11"
 types-python-dateutil="^2.8.19.12"
 types-simplejson="^3.19.0.0"
 pydantic = ">=1.9.1"
-SQLAlchemy = { version = ">=1.3.20,<1.4.39", optional = true }
-Faker = { version = ">=13.6.0,<18.6.0", optional = true }
-fastapi = { version = ">=0.78.0,<0.95.1", optional = true }
+SQLAlchemy = { version = ">=1.3.20,<2.0.13", optional = true }
+Faker = { version = ">=13.6.0,<18.7.0", optional = true }
+fastapi = { version = ">=0.78.0,<0.95.2", optional = true }
 psycopg2-binary = "^2.9.5"
 mkdocs = "^1.4.1"
 mkdocs-material = "^9.1.8"
-pymdown-extensions = "^9.11"
-fontawesome-markdown = "^0.2.6"
 httpx = "^0.24.0"
 asgi-lifespan = "^2.1.0"
 requests = "^2.29.0"
-uvicorn = { version = ">=0.17.6,<0.22.0", optional = true }
+uvicorn = { version = ">=0.17.6,<0.23.0", optional = true }
 Jinja2 = "^3.1.2"
-pypinyin = "^0.39.1"
+pypinyin = ">=0.39.1,<0.49.0"
 pyjwt = "^2.4.0"
 six = "^1.16.0"
 kafka = "^1.3.5"
 contextvars = "^2.4"
-starlette = "^0.19.1"
+starlette = ">=0.19.1,<0.27.0"
 aioredis = "^2.0.1"
 lxml = "^4.9.0"
-redis = "^3.5.3"
-certifi = { version = "<=2021.10.8", optional = true }
+redis = ">=3.5.3,<5.0.0"
+certifi = { version = "<=2023.5.7", optional = true }
 dicttoxml = "^1.7.4"
 crypto = "^1.4.1"
 PyYAML = "^6.0"
-urllib3 = "^1.26.12"
+urllib3 = ">=1.26.12,<3.0.0"
 w3lib = "^2.1.1"
 py_mini_racer="^0.6.0"
 pillow="^9.5.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
```

### Comparing `custard-1.1.5/PKG-INFO` & `custard-1.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custard
-Version: 1.1.5
+Version: 1.1.6
 Summary: custard easy to learn, fast to code, ready for production
 Home-page: https://github.com/kamalyes/custard
 License: MIT
 Author: Kamalyes
 Author-email: mryu168@163.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -14,57 +14,54 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Provides-Extra: all
-Requires-Dist: Faker (>=13.6.0,<18.6.0) ; extra == "all"
+Requires-Dist: Faker (>=13.6.0,<18.7.0) ; extra == "all"
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0) ; extra == "all"
-Requires-Dist: SQLAlchemy (>=1.3.20,<1.4.39) ; extra == "all"
+Requires-Dist: SQLAlchemy (>=1.3.20,<2.0.13) ; extra == "all"
 Requires-Dist: aioredis (>=2.0.1,<3.0.0) ; extra == "all"
 Requires-Dist: asgi-lifespan (>=2.1.0,<3.0.0)
-Requires-Dist: certifi (<=2021.10.8) ; extra == "all"
+Requires-Dist: certifi (<=2023.5.7) ; extra == "all"
 Requires-Dist: contextvars (>=2.4,<3.0) ; extra == "all"
 Requires-Dist: crypto (>=1.4.1,<2.0.0) ; extra == "all"
 Requires-Dist: dicttoxml (>=1.7.4,<2.0.0) ; extra == "all"
-Requires-Dist: fastapi (>=0.78.0,<0.95.1) ; extra == "all"
-Requires-Dist: fontawesome-markdown (>=0.2.6,<0.3.0)
+Requires-Dist: fastapi (>=0.78.0,<0.95.2) ; extra == "all"
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: kafka (>=1.3.5,<2.0.0) ; extra == "all"
 Requires-Dist: lxml (>=4.9.0,<5.0.0) ; extra == "all"
 Requires-Dist: mkdocs (>=1.4.1,<2.0.0) ; extra == "all"
 Requires-Dist: mkdocs-material (>=9.1.8,<10.0.0)
 Requires-Dist: mypy (>=1.2.0,<2.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: py_mini_racer (>=0.6.0,<0.7.0)
 Requires-Dist: pydantic (>=1.9.1) ; extra == "all"
 Requires-Dist: pyjwt (>=2.4.0,<3.0.0) ; extra == "all"
-Requires-Dist: pymdown-extensions (>=9.11,<10.0)
-Requires-Dist: pypinyin (>=0.39.1,<0.40.0) ; extra == "all"
-Requires-Dist: redis (>=3.5.3,<4.0.0) ; extra == "all"
+Requires-Dist: pypinyin (>=0.39.1,<0.49.0) ; extra == "all"
+Requires-Dist: redis (>=3.5.3,<5.0.0) ; extra == "all"
 Requires-Dist: requests (>=2.29.0,<3.0.0) ; extra == "all"
-Requires-Dist: ruff (>=0.0.263,<0.0.264)
+Requires-Dist: ruff (>=0.0.263,<0.0.266)
 Requires-Dist: six (>=1.16.0,<2.0.0) ; extra == "all"
-Requires-Dist: starlette (>=0.19.1,<0.20.0) ; extra == "all"
+Requires-Dist: starlette (>=0.19.1,<0.27.0) ; extra == "all"
 Requires-Dist: types-PyYAML (>=6.0.12.9,<7.0.0.0)
 Requires-Dist: types-python-dateutil (>=2.8.19.12,<3.0.0.0)
 Requires-Dist: types-requests (>=2.29.0.0,<3.0.0.0)
 Requires-Dist: types-simplejson (>=3.19.0.0,<4.0.0.0)
 Requires-Dist: types-urllib3 (>=1.26.25.11,<2.0.0.0)
-Requires-Dist: urllib3 (>=1.26.12,<2.0.0) ; extra == "all"
-Requires-Dist: uvicorn (>=0.17.6,<0.22.0) ; extra == "all"
+Requires-Dist: urllib3 (>=1.26.12,<3.0.0) ; extra == "all"
+Requires-Dist: uvicorn (>=0.17.6,<0.23.0) ; extra == "all"
 Requires-Dist: w3lib (>=2.1.1,<3.0.0) ; extra == "all"
 Project-URL: Repository, https://github.com/kamalyes/custard
 Description-Content-Type: text/markdown
 
 </p>
 <p align="center">
 <a href="https://img.shields.io/badge/Python-3.9.11+-green" target="__blank"><img src="https://img.shields.io/badge/Python-3.9.11+-green" alt="custard preview"></a>
```

#### html2text {}

```diff
@@ -1,49 +1,47 @@
-Metadata-Version: 2.1 Name: custard Version: 1.1.5 Summary: custard easy to
+Metadata-Version: 2.1 Name: custard Version: 1.1.6 Summary: custard easy to
 learn, fast to code, ready for production Home-page: https://github.com/
 kamalyes/custard License: MIT Author: Kamalyes Author-email: mryu168@163.com
 Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 System Administrators Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Topic :: Software Development
-:: Libraries :: Python Modules Classifier: Typing :: Typed Provides-Extra: all
-Requires-Dist: Faker (>=13.6.0,<18.6.0) ; extra == "all" Requires-Dist: Jinja2
-(>=3.1.2,<4.0.0) Requires-Dist: PyYAML (>=6.0,<7.0) ; extra == "all" Requires-
-Dist: SQLAlchemy (>=1.3.20,<1.4.39) ; extra == "all" Requires-Dist: aioredis
-(>=2.0.1,<3.0.0) ; extra == "all" Requires-Dist: asgi-lifespan (>=2.1.0,<3.0.0)
-Requires-Dist: certifi (<=2021.10.8) ; extra == "all" Requires-Dist:
-contextvars (>=2.4,<3.0) ; extra == "all" Requires-Dist: crypto
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Typing :: Typed
+Provides-Extra: all Requires-Dist: Faker (>=13.6.0,<18.7.0) ; extra == "all"
+Requires-Dist: Jinja2 (>=3.1.2,<4.0.0) Requires-Dist: PyYAML (>=6.0,<7.0) ;
+extra == "all" Requires-Dist: SQLAlchemy (>=1.3.20,<2.0.13) ; extra == "all"
+Requires-Dist: aioredis (>=2.0.1,<3.0.0) ; extra == "all" Requires-Dist: asgi-
+lifespan (>=2.1.0,<3.0.0) Requires-Dist: certifi (<=2023.5.7) ; extra == "all"
+Requires-Dist: contextvars (>=2.4,<3.0) ; extra == "all" Requires-Dist: crypto
 (>=1.4.1,<2.0.0) ; extra == "all" Requires-Dist: dicttoxml (>=1.7.4,<2.0.0) ;
-extra == "all" Requires-Dist: fastapi (>=0.78.0,<0.95.1) ; extra == "all"
-Requires-Dist: fontawesome-markdown (>=0.2.6,<0.3.0) Requires-Dist: httpx
-(>=0.24.0,<0.25.0) Requires-Dist: kafka (>=1.3.5,<2.0.0) ; extra == "all"
-Requires-Dist: lxml (>=4.9.0,<5.0.0) ; extra == "all" Requires-Dist: mkdocs
-(>=1.4.1,<2.0.0) ; extra == "all" Requires-Dist: mkdocs-material
+extra == "all" Requires-Dist: fastapi (>=0.78.0,<0.95.2) ; extra == "all"
+Requires-Dist: httpx (>=0.24.0,<0.25.0) Requires-Dist: kafka (>=1.3.5,<2.0.0) ;
+extra == "all" Requires-Dist: lxml (>=4.9.0,<5.0.0) ; extra == "all" Requires-
+Dist: mkdocs (>=1.4.1,<2.0.0) ; extra == "all" Requires-Dist: mkdocs-material
 (>=9.1.8,<10.0.0) Requires-Dist: mypy (>=1.2.0,<2.0.0) Requires-Dist: pillow
 (>=9.5.0,<10.0.0) Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0) Requires-
 Dist: py_mini_racer (>=0.6.0,<0.7.0) Requires-Dist: pydantic (>=1.9.1) ; extra
 == "all" Requires-Dist: pyjwt (>=2.4.0,<3.0.0) ; extra == "all" Requires-Dist:
-pymdown-extensions (>=9.11,<10.0) Requires-Dist: pypinyin (>=0.39.1,<0.40.0) ;
-extra == "all" Requires-Dist: redis (>=3.5.3,<4.0.0) ; extra == "all" Requires-
-Dist: requests (>=2.29.0,<3.0.0) ; extra == "all" Requires-Dist: ruff
-(>=0.0.263,<0.0.264) Requires-Dist: six (>=1.16.0,<2.0.0) ; extra == "all"
-Requires-Dist: starlette (>=0.19.1,<0.20.0) ; extra == "all" Requires-Dist:
-types-PyYAML (>=6.0.12.9,<7.0.0.0) Requires-Dist: types-python-dateutil
-(>=2.8.19.12,<3.0.0.0) Requires-Dist: types-requests (>=2.29.0.0,<3.0.0.0)
-Requires-Dist: types-simplejson (>=3.19.0.0,<4.0.0.0) Requires-Dist: types-
-urllib3 (>=1.26.25.11,<2.0.0.0) Requires-Dist: urllib3 (>=1.26.12,<2.0.0) ;
-extra == "all" Requires-Dist: uvicorn (>=0.17.6,<0.22.0) ; extra == "all"
-Requires-Dist: w3lib (>=2.1.1,<3.0.0) ; extra == "all" Project-URL: Repository,
-https://github.com/kamalyes/custard Description-Content-Type: text/markdown
+pypinyin (>=0.39.1,<0.49.0) ; extra == "all" Requires-Dist: redis
+(>=3.5.3,<5.0.0) ; extra == "all" Requires-Dist: requests (>=2.29.0,<3.0.0) ;
+extra == "all" Requires-Dist: ruff (>=0.0.263,<0.0.266) Requires-Dist: six
+(>=1.16.0,<2.0.0) ; extra == "all" Requires-Dist: starlette (>=0.19.1,<0.27.0)
+; extra == "all" Requires-Dist: types-PyYAML (>=6.0.12.9,<7.0.0.0) Requires-
+Dist: types-python-dateutil (>=2.8.19.12,<3.0.0.0) Requires-Dist: types-
+requests (>=2.29.0.0,<3.0.0.0) Requires-Dist: types-simplejson
+(>=3.19.0.0,<4.0.0.0) Requires-Dist: types-urllib3 (>=1.26.25.11,<2.0.0.0)
+Requires-Dist: urllib3 (>=1.26.12,<3.0.0) ; extra == "all" Requires-Dist:
+uvicorn (>=0.17.6,<0.23.0) ; extra == "all" Requires-Dist: w3lib
+(>=2.1.1,<3.0.0) ; extra == "all" Project-URL: Repository, https://github.com/
+kamalyes/custard Description-Content-Type: text/markdown
  [custard_preview] [custard_preview] [https://img.shields.io/pypi/dm/custard]
 ## ðç®ä»
 custardæ¯ä¸ä¸ªå°èå¨çPythonå·¥å·ç±»åºï¼éè¿éææ¹æ³å°è£ï¼éä½ç¸å³APIçå­¦ä¹ ææ¬ï¼æé«å·¥ä½æçï¼ä½¿Pythonæ¥æå½æ°å¼è¯­è¨è¬çä¼éï¼è®©Pythonè¯­è¨ä¹å¯ä»¥âçççâã
 custardä¸­çå·¥å·æ¹æ³æ¥èªæ¯ä¸ªç¨æ·çç²¾éç»ç¢ï¼å®æ¶µçäºPythonå¼ååºå±ä»£ç ä¸­çæ¹æ¹é¢é¢ï¼å®æ¢æ¯å¤§åé¡¹ç®å¼åä¸­è§£å³å°é®é¢çå©å¨ï¼ä¹æ¯å°åé¡¹ç®ä¸­çæçæå½ï¼
 custardæ¯é¡¹ç®ä¸­âutilâååå¥½çæ¿ä»£ï¼å®èçäºå¼åäººåå¯¹é¡¹ç®ä¸­å¬ç¨ç±»åå¬ç¨å·¥å·æ¹æ³çå°è£æ¶é´ï¼ä½¿å¼åä¸æ³¨äºä¸å¡ï¼åæ¶å¯ä»¥æå¤§éåº¦çé¿åå°è£ä¸å®åå¸¦æ¥çbugã
 ## ðºcustardå¦ä½æ¹åæä»¬çcodingæ¹å¼
 custardçç®æ æ¯ä½¿ç¨ä¸ä¸ªå·¥å·æ¹æ³ä»£æ¿ä¸æ®µå¤æä»£ç ï¼ä»èæå¤§éåº¦çé¿åâå¤å¶ç²è´´âä»£ç çé®é¢ï¼å½»åºæ¹åæä»¬åä»£ç çæ¹å¼ã
```

