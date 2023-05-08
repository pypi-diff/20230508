# Comparing `tmp/pypipr-0.1.8.tar.gz` & `tmp/pypipr-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypipr-0.1.8.tar", max compression
+gzip compressed data, was "pypipr-0.1.9.tar", max compression
```

## Comparing `pypipr-0.1.8.tar` & `pypipr-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2022-10-11 16:47:36.486008 pypipr-0.1.8/pypipr/__init__.py
--rw-r--r--   0        0        0     1816 2022-10-14 15:45:39.479083 pypipr-0.1.8/pypipr/iconsole.py
--rw-r--r--   0        0        0      199 2022-10-14 15:23:12.870383 pypipr-0.1.8/pypipr/iconstant.py
--rw-r--r--   0        0        0      315 2022-10-14 15:23:37.319991 pypipr-0.1.8/pypipr/idatetime.py
--rw-r--r--   0        0        0      252 2022-10-14 15:24:05.627645 pypipr-0.1.8/pypipr/pypipr.py
--rw-r--r--   0        0        0      342 2022-10-14 15:50:19.525672 pypipr-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1746 2022-10-14 15:42:50.506147 pypipr-0.1.8/README.md
--rw-r--r--   0        0        0     2381 1970-01-01 00:00:00.000000 pypipr-0.1.8/setup.py
--rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 pypipr-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-10-11 16:47:36.486008 pypipr-0.1.9/pypipr/__init__.py
+-rw-r--r--   0        0        0     1816 2022-10-14 15:45:39.479083 pypipr-0.1.9/pypipr/iconsole.py
+-rw-r--r--   0        0        0      199 2022-10-14 15:23:12.870383 pypipr-0.1.9/pypipr/iconstant.py
+-rw-r--r--   0        0        0      315 2022-10-14 15:23:37.319991 pypipr-0.1.9/pypipr/idatetime.py
+-rw-r--r--   0        0        0      252 2022-10-14 15:24:05.627645 pypipr-0.1.9/pypipr/pypipr.py
+-rw-r--r--   0        0        0      358 2022-10-14 15:54:43.270169 pypipr-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1746 2022-10-14 15:42:50.506147 pypipr-0.1.9/README.md
+-rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 pypipr-0.1.9/setup.py
+-rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 pypipr-0.1.9/PKG-INFO
```

### Comparing `pypipr-0.1.8/pypipr/iconsole.py` & `pypipr-0.1.9/pypipr/iconsole.py`

 * *Files identical despite different names*

### Comparing `pypipr-0.1.8/README.md` & `pypipr-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pypipr-0.1.8/setup.py` & `pypipr-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['pypipr']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pytest>=7.1.3,<8.0.0', 'pytz>=2022.4,<2023.0']
+['getch>=1.0,<2.0', 'pytest>=7.1.3,<8.0.0', 'pytz>=2022.4,<2023.0']
 
 setup_kwargs = {
     'name': 'pypipr',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'The Python Package Index Project',
     'long_description': '# About\nThe Python Package Index Project (pypipr)\n\n\n# Setup\nInstall with pip\n```\npython -m pip install pypipr\n```\n\nTest with\n```python\nfrom pypipr.pypipr import Pypipr\nPypipr.test_print()\n```\n\n\n# Pypipr Class\n`test_print()` memastikan module sudah terinstal dan dapat dijalankan\n```python\nfrom pypipr.pypipr import Pypipr\nPypipr.test_print()\n```\n\n\n# iconsole\n`@Log()` / `Log decorator` akan melakukan print ke console. Mempermudah pembuatan log karena tidak perlu mengubah fungsi yg sudah ada. Berguna untuk memberikan informasi proses program yg sedang berjalan.\n\n```python\nfrom pypipr.iconsole import log\n\n@log("Calling some function")\ndef some_function():\n    ...\n    return\n```\n\n\n`print_colorize()` print ke console dengan warna\n\n```python\nfrom pypipr.iconsole import print_colorize\nprint_colorize("Print some text")\n```\n\n\n`input_char()` meminta masukan satu huruf tanpa menekan enter. Char tidak ditampilkan.\n\n```python\nfrom pypipr.iconsole import input_char\ninput_char("Input Char without print : ")\n```\n\n\n`input_char()` meminta masukan satu huruf tanpa menekan enter. Char ditampilkan.\n\n```python\nfrom pypipr.iconsole import input_char_echo\ninput_char_echo("Input Char n : ")\n```\n\n\n# idatetime\n`datetime_now()` memudahkan dalam membuat tanggal dan waktu untuk suatu timezone\n\n```python\nfrom pypipr.idatetime import datetime_now\ndatetime_now("Asia/Jakarta")\ndatetime_now("GMT")\ndatetime_now("Etc/GMT+7")\n```\n\n\n# iconstant\n`WINDOWS` True apabila berjalan di platform Windows\n\n```python\nfrom pypipr.iconstant import WINDOWS\nprint(WINDOWS)\n```\n\n`LINUX` True apabila berjalan di platform Linux\n\n```python\nfrom pypipr.iconstant import LINUX\nprint(LINUX)\n```\n',
     'author': 'ufiapjj',
     'author_email': 'ufiapjj@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pypipr-0.1.8/PKG-INFO` & `pypipr-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pypipr
-Version: 0.1.8
+Version: 0.1.9
 Summary: The Python Package Index Project
 Author: ufiapjj
 Author-email: ufiapjj@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: getch (>=1.0,<2.0)
 Requires-Dist: pytest (>=7.1.3,<8.0.0)
 Requires-Dist: pytz (>=2022.4,<2023.0)
 Description-Content-Type: text/markdown
 
 # About
 The Python Package Index Project (pypipr)
```

