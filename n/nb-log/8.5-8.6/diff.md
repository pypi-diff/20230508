# Comparing `tmp/nb_log-8.5.tar.gz` & `tmp/nb_log-8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nb_log-8.5.tar", last modified: Fri Apr 28 10:41:41 2023, max compression
+gzip compressed data, was "dist\nb_log-8.6.tar", last modified: Mon May  8 07:37:23 2023, max compression
```

## Comparing `nb_log-8.5.tar` & `nb_log-8.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 10:41:41.000000 nb_log-8.5/
--rw-rw-rw-   0        0        0    27863 2023-04-28 10:41:41.000000 nb_log-8.5/PKG-INFO
--rw-rw-rw-   0        0        0    26926 2022-12-05 09:46:23.000000 nb_log-8.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 10:41:41.000000 nb_log-8.5/nb_log/
--rw-rw-rw-   0        0        0     2369 2023-04-28 10:24:28.000000 nb_log-8.5/nb_log/__init__.py
--rw-rw-rw-   0        0        0    50691 2023-04-28 10:26:55.000000 nb_log-8.5/nb_log/handlers.py
--rw-rw-rw-   0        0        0    49868 2022-09-17 07:28:19.000000 nb_log-8.5/nb_log/handlers0000.py
--rw-rw-rw-   0        0        0      247 2023-04-18 01:17:35.000000 nb_log-8.5/nb_log/helper.py
--rw-rw-rw-   0        0        0    30621 2023-04-18 02:30:56.000000 nb_log-8.5/nb_log/log_manager.py
--rw-rw-rw-   0        0        0     7782 2023-04-18 01:50:08.000000 nb_log-8.5/nb_log/monkey_print.py
--rw-rw-rw-   0        0        0     9455 2023-04-17 07:36:14.000000 nb_log-8.5/nb_log/nb_log_config_default.py
--rw-rw-rw-   0        0        0     7710 2023-04-13 09:47:00.000000 nb_log-8.5/nb_log/set_nb_log_config.py
-drwxrwxrwx   0        0        0        0 2023-04-28 10:41:41.000000 nb_log-8.5/nb_log.egg-info/
--rw-rw-rw-   0        0        0    27863 2023-04-28 10:41:40.000000 nb_log-8.5/nb_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-04-28 10:41:40.000000 nb_log-8.5/nb_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 10:41:40.000000 nb_log-8.5/nb_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2023-04-28 10:41:40.000000 nb_log-8.5/nb_log.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-28 10:41:40.000000 nb_log-8.5/nb_log.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 10:41:41.000000 nb_log-8.5/setup.cfg
--rw-rw-rw-   0        0        0     2325 2023-04-28 10:41:33.000000 nb_log-8.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:37:23.000000 nb_log-8.6/
+-rw-rw-rw-   0        0        0    27863 2023-05-08 07:37:23.000000 nb_log-8.6/PKG-INFO
+-rw-rw-rw-   0        0        0    26926 2022-12-05 09:46:23.000000 nb_log-8.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 07:37:23.000000 nb_log-8.6/nb_log/
+-rw-rw-rw-   0        0        0     2369 2023-04-28 10:24:28.000000 nb_log-8.6/nb_log/__init__.py
+-rw-rw-rw-   0        0        0    50691 2023-04-28 10:26:55.000000 nb_log-8.6/nb_log/handlers.py
+-rw-rw-rw-   0        0        0    49868 2022-09-17 07:28:19.000000 nb_log-8.6/nb_log/handlers0000.py
+-rw-rw-rw-   0        0        0      247 2023-04-18 01:17:35.000000 nb_log-8.6/nb_log/helper.py
+-rw-rw-rw-   0        0        0    30621 2023-04-18 02:30:56.000000 nb_log-8.6/nb_log/log_manager.py
+-rw-rw-rw-   0        0        0     7782 2023-04-18 01:50:08.000000 nb_log-8.6/nb_log/monkey_print.py
+-rw-rw-rw-   0        0        0     9455 2023-04-17 07:36:14.000000 nb_log-8.6/nb_log/nb_log_config_default.py
+-rw-rw-rw-   0        0        0     7710 2023-04-13 09:47:00.000000 nb_log-8.6/nb_log/set_nb_log_config.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:37:23.000000 nb_log-8.6/nb_log.egg-info/
+-rw-rw-rw-   0        0        0    27863 2023-05-08 07:37:23.000000 nb_log-8.6/nb_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-05-08 07:37:23.000000 nb_log-8.6/nb_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 07:37:23.000000 nb_log-8.6/nb_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-05-08 07:37:23.000000 nb_log-8.6/nb_log.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-08 07:37:23.000000 nb_log-8.6/nb_log.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 07:37:23.000000 nb_log-8.6/setup.cfg
+-rw-rw-rw-   0        0        0     2345 2023-05-08 07:37:15.000000 nb_log-8.6/setup.py
```

### Comparing `nb_log-8.5/PKG-INFO` & `nb_log-8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_log
-Version: 8.5
+Version: 8.6
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_log-8.5/README.md` & `nb_log-8.6/README.md`

 * *Files identical despite different names*

### Comparing `nb_log-8.5/nb_log/__init__.py` & `nb_log-8.6/nb_log/__init__.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.5/nb_log/handlers.py` & `nb_log-8.6/nb_log/handlers.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.5/nb_log/handlers0000.py` & `nb_log-8.6/nb_log/handlers0000.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.5/nb_log/log_manager.py` & `nb_log-8.6/nb_log/log_manager.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.5/nb_log/monkey_print.py` & `nb_log-8.6/nb_log/monkey_print.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.5/nb_log/nb_log_config_default.py` & `nb_log-8.6/nb_log/nb_log_config_default.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.5/nb_log/set_nb_log_config.py` & `nb_log-8.6/nb_log/set_nb_log_config.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.5/nb_log.egg-info/PKG-INFO` & `nb_log-8.6/nb_log.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-log
-Version: 8.5
+Version: 8.6
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_log-8.5/setup.py` & `nb_log-8.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,32 +7,33 @@
 #     long_description = fh.read()
 
 # filepath = ((Path(__file__).parent / Path('README.md')).absolute()).as_posix()
 filepath = 'README.md'
 print(filepath)
 
 install_requires = [
-    'pymongo==4.0.2',
+    'pymongo==4.3.3',
     'tomorrow3==1.1.0',
-    'concurrent-log-handler==0.9.19',
+    'concurrent-log-handler==0.9.23',
     'elasticsearch',
     'kafka-python==2.0.2',
     'requests',
     'flask',
     'python-json-logger==0.1.10',
     'nb_filelock',
-    'service-identity'
+    'service-identity',
+    'deprecated',
 ]
 
 if os.name == 'nt':
     install_requires.append('pywin32')
 
 setup(
     name='nb_log',  #
-    version="8.5",
+    version="8.6",
     description=(
         'very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on '
     ),
     keywords=["logging", "logger", "multiprocess file handler", "color handler"],
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
@@ -61,14 +62,14 @@
 """
 打包上传
 python setup.py sdist upload -r pypi
 
 
 
 python setup.py sdist & twine upload dist/nb_log-6.0.tar.gz
-python setup.py sdist & python -m  twine upload dist/nb_log-8.5.tar.gz
+python setup.py sdist & python -m  twine upload dist/nb_log-8.6.tar.gz
 
 twine upload dist/*
 
 
 python -m pip install nb_log --upgrade -i https://pypi.org/simple   # 及时的方式，不用等待 阿里云 豆瓣 同步
 """
```

