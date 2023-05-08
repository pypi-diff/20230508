# Comparing `tmp/html_msg-1.0.0.tar.gz` & `tmp/html_msg-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_msg-1.0.0.tar", last modified: Mon May  8 15:39:04 2023, max compression
+gzip compressed data, was "html_msg-1.0.1.tar", last modified: Mon May  8 16:56:38 2023, max compression
```

## Comparing `html_msg-1.0.0.tar` & `html_msg-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 15:39:04.267928 html_msg-1.0.0/
--rw-rw-rw-   0        0        0     1095 2023-05-06 11:32:57.000000 html_msg-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      405 2023-05-08 15:39:04.267928 html_msg-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-05-08 15:29:13.000000 html_msg-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 15:39:04.249531 html_msg-1.0.0/html_msg/
--rw-rw-rw-   0        0        0      187 2023-05-06 12:17:26.000000 html_msg-1.0.0/html_msg/__init__.py
--rw-rw-rw-   0        0        0    12353 2023-05-06 11:56:05.000000 html_msg-1.0.0/html_msg/html_message.py
--rw-rw-rw-   0        0        0    14922 2023-05-06 11:55:20.000000 html_msg-1.0.0/html_msg/html_table.py
-drwxrwxrwx   0        0        0        0 2023-05-08 15:39:04.266955 html_msg-1.0.0/html_msg.egg-info/
--rw-rw-rw-   0        0        0      405 2023-05-08 15:39:04.000000 html_msg-1.0.0/html_msg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-05-08 15:39:04.000000 html_msg-1.0.0/html_msg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 15:39:04.000000 html_msg-1.0.0/html_msg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-08 15:39:04.000000 html_msg-1.0.0/html_msg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-08 15:39:04.000000 html_msg-1.0.0/html_msg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 15:39:04.268926 html_msg-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      779 2023-05-08 15:39:01.000000 html_msg-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:56:38.560555 html_msg-1.0.1/
+-rw-rw-rw-   0        0        0     1095 2023-05-06 11:32:57.000000 html_msg-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      332 2023-05-08 16:56:38.559558 html_msg-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2023-05-08 15:29:13.000000 html_msg-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 16:56:38.549716 html_msg-1.0.1/html_msg/
+-rw-rw-rw-   0        0        0       95 2023-05-08 16:50:14.000000 html_msg-1.0.1/html_msg/__init__.py
+-rw-rw-rw-   0        0        0    12353 2023-05-06 11:56:05.000000 html_msg-1.0.1/html_msg/html_message.py
+-rw-rw-rw-   0        0        0    14922 2023-05-06 11:55:20.000000 html_msg-1.0.1/html_msg/html_table.py
+drwxrwxrwx   0        0        0        0 2023-05-08 16:56:38.559558 html_msg-1.0.1/html_msg.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-05-08 16:56:38.000000 html_msg-1.0.1/html_msg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-05-08 16:56:38.000000 html_msg-1.0.1/html_msg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 16:56:38.000000 html_msg-1.0.1/html_msg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-08 16:56:38.000000 html_msg-1.0.1/html_msg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-08 16:56:38.000000 html_msg-1.0.1/html_msg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 16:56:38.560555 html_msg-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      781 2023-05-08 16:52:26.000000 html_msg-1.0.1/setup.py
```

### Comparing `html_msg-1.0.0/LICENSE.txt` & `html_msg-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html_msg-1.0.0/html_msg/html_message.py` & `html_msg-1.0.1/html_msg/html_message.py`

 * *Files identical despite different names*

### Comparing `html_msg-1.0.0/html_msg/html_table.py` & `html_msg-1.0.1/html_msg/html_table.py`

 * *Files identical despite different names*

### Comparing `html_msg-1.0.0/setup.py` & `html_msg-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 
 
 setup_args = dict(
     name='html_msg',
-    version='1.0.0',
+    version='1.0.1',
     description='This tool allows to create HTML message via simple methods, \
         even if you dont now HTML',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n',
     license='MIT',
     packages=find_packages(),
     author='Sirakan Bagdasarian',
     author_email='bsirak@bk.ru',
     keywords=['HTML', 'Message'],
-    url='https://github.com/',
-    download_url='https://pypi.org/project/'
+    #url='https://github.com/',
+    #download_url='https://pypi.org/project/'
 )
 
 install_requires = [
     'IPython',
     'pandas'
 ]
```

