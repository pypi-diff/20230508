# Comparing `tmp/thankyou-0.0.2.tar.gz` & `tmp/thankyou-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thankyou-0.0.2.tar", max compression
+gzip compressed data, was "thankyou-0.0.3.tar", max compression
```

## Comparing `thankyou-0.0.2.tar` & `thankyou-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-05-08 08:35:27.761622 thankyou-0.0.2/LICENSE
--rw-r--r--   0        0        0      712 2023-05-08 08:35:27.761622 thankyou-0.0.2/README.md
--rw-r--r--   0        0        0     1185 2023-05-08 08:35:27.761622 thankyou-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       61 2023-05-08 08:35:27.761622 thankyou-0.0.2/thankyou/__init__.py
--rw-r--r--   0        0        0      131 2023-05-08 08:35:27.761622 thankyou-0.0.2/thankyou/tests.py
--rw-r--r--   0        0        0     8940 2023-05-08 08:35:27.761622 thankyou-0.0.2/thankyou/thankyou.py
--rw-r--r--   0        0        0     1713 1970-01-01 00:00:00.000000 thankyou-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-08 10:30:25.845579 thankyou-0.0.3/LICENSE
+-rw-r--r--   0        0        0      824 2023-05-08 10:30:25.845579 thankyou-0.0.3/README.md
+-rw-r--r--   0        0        0     1185 2023-05-08 10:30:25.845579 thankyou-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-05-08 10:30:25.845579 thankyou-0.0.3/thankyou/__init__.py
+-rw-r--r--   0        0        0      256 2023-05-08 10:30:25.845579 thankyou-0.0.3/thankyou/tests.py
+-rw-r--r--   0        0        0     9198 2023-05-08 10:30:25.845579 thankyou-0.0.3/thankyou/thankyou.py
+-rw-r--r--   0        0        0     1825 1970-01-01 00:00:00.000000 thankyou-0.0.3/PKG-INFO
```

### Comparing `thankyou-0.0.2/LICENSE` & `thankyou-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thankyou-0.0.2/pyproject.toml` & `thankyou-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thankyou"
-version = "0.0.2"
+version = "0.0.3"
 description = "Print \"Thank You\" in every known language"
 authors = [
     "Mario Hernandez <yo@mariofix.com>"
 ]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mariofix/thankyou"
```

### Comparing `thankyou-0.0.2/thankyou/thankyou.py` & `thankyou-0.0.3/thankyou/thankyou.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from typing import Union
 import secrets
 
 # Translated list thanks to ChatGPT
-thanks_array = [
+thanks_array: list = [
     ("Afghanistan", "تشکر"),
     ("Albania", "Faleminderit"),
     ("Algeria", "شكرا"),
     ("Andorra", "Gràcies"),
     ("Angola", "Obrigado"),
     ("Antigua and Barbuda", "Thank you"),
     ("Argentina", "Gracias"),
@@ -261,10 +262,17 @@
     ("Shang Dynasty", "谢谢"),
     ("Sumerian Civilization", "واژه های خیر"),
     ("Tang Dynasty", "谢谢"),
     ("Vedic Period India", "धन्यवाद"),
 ]
 
 
-def give_thanks():
+def give_thanks(as_tuple: bool = False) -> Union[str, tuple]:
+    """Returns translated "Thank You (Country)"
+
+    Selects one randomply from a list of tuples using secrets package
+    """
     thanks = secrets.choice(thanks_array)
-    return "{} ({})".format(thanks[1], thanks[0])
+    if not as_tuple:
+        return "{} ({})".format(thanks[1], thanks[0])
+    else:
+        return thanks
```

### Comparing `thankyou-0.0.2/PKG-INFO` & `thankyou-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thankyou
-Version: 0.0.2
+Version: 0.0.3
 Summary: Print "Thank You" in every known language
 Home-page: https://github.com/mariofix/thankyou
 License: MIT
 Keywords: thanks,library,thank
 Author: Mario Hernandez
 Author-email: yo@mariofix.com
 Requires-Python: >=3.8,<4.0
@@ -19,17 +19,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Repository, https://github.com/mariofix/thankyou
 Description-Content-Type: text/markdown
 
-# thanks
+# Thank You
 Python module to print "Thanks/Thank you" in every known language.
 Install it, import it and use it with
 ```python
 from thankyou import give_thanks
 thanks = give_thanks()
 ```
 
+So, why do this?
+Why not I may reply.
+
+It's just a "nicer" way to generate random (sometimes hostile) data.
+
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/mariofix/thankyou/main.svg)](https://results.pre-commit.ci/latest/github/mariofix/thankyou/main) [![Thank You](https://github.com/mariofix/thankyou/actions/workflows/tests.yml/badge.svg)](https://github.com/mariofix/thankyou/actions/workflows/tests.yml) [![PyPI version](https://badge.fury.io/py/thankyou.svg)](https://badge.fury.io/py/thankyou) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

