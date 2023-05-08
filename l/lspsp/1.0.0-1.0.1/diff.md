# Comparing `tmp/lspsp-1.0.0.tar.gz` & `tmp/lspsp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lspsp-1.0.0.tar", last modified: Mon May  8 01:24:23 2023, max compression
+gzip compressed data, was "lspsp-1.0.1.tar", last modified: Mon May  8 02:53:26 2023, max compression
```

## Comparing `lspsp-1.0.0.tar` & `lspsp-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:24:23.304874 lspsp-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 01:24:23.304874 lspsp-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 01:24:07.000000 lspsp-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 01:24:07.000000 lspsp-1.0.0/config.json.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:24:23.300874 lspsp-1.0.0/lspsp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 01:24:07.000000 lspsp-1.0.0/lspsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-08 01:24:07.000000 lspsp-1.0.0/lspsp/lspmon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-08 01:24:07.000000 lspsp-1.0.0/lspsp/lspnotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-08 01:24:07.000000 lspsp-1.0.0/lspsp/lspsp.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 01:24:07.000000 lspsp-1.0.0/lspsp/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:24:23.300874 lspsp-1.0.0/lspsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 01:24:23.000000 lspsp-1.0.0/lspsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-08 01:24:23.000000 lspsp-1.0.0/lspsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 01:24:23.000000 lspsp-1.0.0/lspsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-08 01:24:23.000000 lspsp-1.0.0/lspsp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-08 01:24:23.000000 lspsp-1.0.0/lspsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 01:24:23.000000 lspsp-1.0.0/lspsp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:24:23.304874 lspsp-1.0.0/resource/
--rw-r--r--   0 runner    (1001) docker     (123)    55908 2023-05-08 01:24:07.000000 lspsp-1.0.0/resource/mail.html
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 01:24:23.304874 lspsp-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-08 01:24:07.000000 lspsp-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 02:53:26.990557 lspsp-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 02:53:14.000000 lspsp-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 02:53:26.990557 lspsp-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 02:53:14.000000 lspsp-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 02:53:14.000000 lspsp-1.0.1/config.json.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 02:53:26.990557 lspsp-1.0.1/lspsp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 02:53:14.000000 lspsp-1.0.1/lspsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-08 02:53:14.000000 lspsp-1.0.1/lspsp/lspmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-08 02:53:14.000000 lspsp-1.0.1/lspsp/lspnotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-08 02:53:14.000000 lspsp-1.0.1/lspsp/lspsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 02:53:14.000000 lspsp-1.0.1/lspsp/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 02:53:26.990557 lspsp-1.0.1/lspsp/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)    55908 2023-05-08 02:53:14.000000 lspsp-1.0.1/lspsp/resource/mail.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 02:53:26.990557 lspsp-1.0.1/lspsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 02:53:26.000000 lspsp-1.0.1/lspsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-08 02:53:26.000000 lspsp-1.0.1/lspsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 02:53:26.000000 lspsp-1.0.1/lspsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-08 02:53:26.000000 lspsp-1.0.1/lspsp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-08 02:53:26.000000 lspsp-1.0.1/lspsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 02:53:26.000000 lspsp-1.0.1/lspsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 02:53:26.990557 lspsp-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-08 02:53:14.000000 lspsp-1.0.1/setup.py
```

### Comparing `lspsp-1.0.0/lspsp/lspmon.py` & `lspsp-1.0.1/lspsp/lspmon.py`

 * *Files identical despite different names*

### Comparing `lspsp-1.0.0/lspsp/lspnotify.py` & `lspsp-1.0.1/lspsp/lspnotify.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from email.header import Header
 from email.mime.text import MIMEText
 import logging
 import smtplib
 from jinja2 import Environment, FileSystemLoader
+import os
 
 
 class LspNotify:
     def __init__(self) -> None:
         self._logger = logging.getLogger(__name__)
 
     def mail(self, config, content):
-        env = Environment(loader=FileSystemLoader('./resource'))
+        root = os.path.dirname(__file__)
+        path = os.path.join(root, 'resource')
+        env = Environment(loader=FileSystemLoader(path))
         template = env.get_template('mail.html')
         html_content = template.render(content=content)
 
         message = MIMEText(str(html_content), 'html', 'utf-8')
         message['From'] = '%s <%s>' % (
             Header(config['name'], 'utf-8').encode(), config['usn'])
         message['To'] = config['recv']
```

### Comparing `lspsp-1.0.0/lspsp/lspsp.py` & `lspsp-1.0.1/lspsp/lspsp.py`

 * *Files identical despite different names*

### Comparing `lspsp-1.0.0/resource/mail.html` & `lspsp-1.0.1/lspsp/resource/mail.html`

 * *Files identical despite different names*

### Comparing `lspsp-1.0.0/setup.py` & `lspsp-1.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="lspsp",
-    version="1.0.0",
+    version="1.0.1",
     license='GPL',
     description='LSPSP.ME Monitor',
     long_description='LSPSP.ME Monitor Service',
     packages=find_packages(),
     include_package_data=True,
     platforms="any",
     install_requires=[
@@ -20,11 +20,10 @@
     scripts=[],
     entry_points={
         'console_scripts': [
             'lspsp = lspsp.main:main'
         ]
     },
     data_files=[
-        ('/etc/lspsp', ['config.json.template']),
-        ('/etc/lspsp/resource', ['resource/mail.html'])
+        ('etc/lspsp', ['config.json.template'])
     ]
 )
```

