# Comparing `tmp/goatl-0.6.2.tar.gz` & `tmp/goatl-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goatl-0.6.2.tar", max compression
+gzip compressed data, was "goatl-0.6.3.tar", max compression
```

## Comparing `goatl-0.6.2.tar` & `goatl-0.6.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1096 2023-05-01 13:53:20.360927 goatl-0.6.2/LICENSE
--rw-r--r--   0        0        0     3785 2023-05-02 13:11:06.002245 goatl-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     5145 2023-05-02 12:58:41.812269 goatl-0.6.2/README.md
--rw-r--r--   0        0        0      478 2023-05-01 21:17:22.000540 goatl-0.6.2/src/goatl/__init__.py
--rw-r--r--   0        0        0    14789 2023-05-02 13:10:44.939654 goatl-0.6.2/src/goatl/core.py
--rw-r--r--   0        0        0     1478 2023-05-01 20:22:33.439577 goatl-0.6.2/src/goatl/utils.py
--rw-r--r--   0        0        0     5734 2023-05-02 13:13:08.063660 goatl-0.6.2/setup.py
--rw-r--r--   0        0        0     5859 2023-05-02 13:13:08.063660 goatl-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-05-01 13:53:20.360927 goatl-0.6.3/LICENSE
+-rw-r--r--   0        0        0     3785 2023-05-08 09:24:51.326186 goatl-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     5055 2023-05-08 06:58:15.715743 goatl-0.6.3/README.md
+-rw-r--r--   0        0        0      478 2023-05-01 21:17:22.000540 goatl-0.6.3/src/goatl/__init__.py
+-rw-r--r--   0        0        0    14717 2023-05-08 09:23:27.660461 goatl-0.6.3/src/goatl/core.py
+-rw-r--r--   0        0        0     1478 2023-05-01 20:22:33.439577 goatl-0.6.3/src/goatl/utils.py
+-rw-r--r--   0        0        0     5644 2023-05-08 09:25:06.363175 goatl-0.6.3/setup.py
+-rw-r--r--   0        0        0     5771 2023-05-08 09:25:06.363175 goatl-0.6.3/PKG-INFO
```

### Comparing `goatl-0.6.2/LICENSE` & `goatl-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `goatl-0.6.2/pyproject.toml` & `goatl-0.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "goatl"
-version = "0.6.2"
+version = "0.6.3"
 description = "The goat logger"
 readme = "README.md"
 authors = ["goatl <EytanDn@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/EytanDn/goatl"
 homepage = "https://github.com/EytanDn/goatl"
```

### Comparing `goatl-0.6.2/README.md` & `goatl-0.6.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# goatl
+<div align="center">
+<img src="assets/images/goatlbanner.png" alt="goatl logo"/>
 
-```
-some body please prompt midjourney for "Cartoonish goat scribing on a long scroll oil painting, --ar  2:1"
-and make abanner for here.
-```
+</div>
+
+---
 
-##
+# goatl
 
 <div align="center">
 
 [![Build status](https://github.com/EytanDn/goatl/workflows/build/badge.svg?branch=master&event=push)](https://github.com/EytanDn/goatl/actions?query=workflow%3Abuild)
 [![Python Version](https://img.shields.io/pypi/pyversions/goatl.svg)](https://pypi.org/project/goatl/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/EytanDn/goatl/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
@@ -71,15 +71,15 @@
     return x*2
 
 foo(1, 2)
 # ... INFO - foo called with args: (1, 2), kwargs: {}
 # ... DEBUG - foo returned: 3
 bar()
 # ... DEBUG - bar called with args: (), kwargs: {}
-# ... INFO - bar returned: hello world
+# ... DEBUG - bar returned: hello world
 baz(3)
 # ... DEBUG - baz called with args: (3,), kwargs: {}
 # ... INFO - baz returned: 6
 ```
 
 ### as a class decorator
 
@@ -110,16 +110,14 @@
 ### configurations shortcuts
 
 ```python
 file_formatter = log.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 log.addFileHandler("foo.log", fmt=file_formatter)
 log.addStreamHandler(fmt="%(levelname)s - %(message)s")
 log.basicConfig(...)
-log.setFormat(...)
-log.setLevel(...)
 ```
 
 ### logging interface #not implemented yet
 
 I do plan to implement goatl's interaction with logging through an interface
 such that it will be possible to use goatl with any logging backend.
```

### Comparing `goatl-0.6.2/src/goatl/core.py` & `goatl-0.6.3/src/goatl/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -338,20 +338,22 @@
 setattr(log, "StreamHandler", logging.StreamHandler)
 
 
 def _add_stdout_handler(fmt: Union[logging.Formatter, str]=None,
                       logger: Optional[logging.Logger]=None, 
                       level: Optional[int]=logging.INFO):
     """shortcut to add a stdout handler to the root logger"""
-    assert logger is None or isinstance(logger, logging.Logger), \
-                                    "logger must be a logging.Logger"
+    if logger is not None:
+        assert isinstance(logger, logging.Logger), \
+                "logger must be a logging.Logger"
     assert isinstance(level, int) or level in levels, \
-                                    "level must be an int or a log.level"
-    assert not isinstance(fmt,(logging.Formatter, str, type(None))), \
-                                    "fmt must be a logging.Formatter or a string"
+                "level must be an int or a log.level"
+    if fmt is not None:
+        assert isinstance(fmt,(logging.Formatter, str)), \
+                "fmt must be a logging.Formatter or a string"
     
     handler = logging.StreamHandler(stream=sys.stdout)
     if logger is None:
         logger = logging.getLogger()
         
     if isinstance(fmt, str):
         handler.setFormatter(logging.Formatter(fmt))
@@ -368,22 +370,25 @@
                       fmt: Union[logging.Formatter, str]=None,
                       logger: Optional[logging.Logger]=None, 
                       level: Optional[int]=logging.DEBUG):
     """shortcut to add a file handler to the root logger
     if filename is not provided, it will be set to the name of the current script 
     with a .log extension 
     """
-    assert filename is None or isinstance(filename, str), \
-                                    "filename must be a string"
-    assert logger is None or isinstance(logger, logging.Logger), \
-                                    "logger must be a logging.Logger"
+    if filename is not None:
+        assert isinstance(filename, str), \
+                "filename must be a string"
+    if logger is not None:
+        assert isinstance(logger, logging.Logger), \
+                "logger must be a logging.Logger"
     assert isinstance(level, int) or level in levels, \
-                                    "level must be an int or a log.level"
-    assert not isinstance(fmt,(logging.Formatter, str, type(None))), \
-                                    "fmt must be a logging.Formatter or a string"
+                "level must be an int or a log.level"
+    if fmt is not None:
+        assert isinstance(fmt,(logging.Formatter, str)), \
+                "fmt must be a logging.Formatter or a string"
                     
     filename = filename or os.path.splitext(os.path.basename(sys.argv[0]))[0]
     filename = filename.replace(" ", "_") + ".log"
     handler = logging.FileHandler(filename=filename)
     if isinstance(fmt, str):
         handler.setFormatter(logging.Formatter(fmt))
     elif isinstance(fmt, logging.Formatter):
```

### Comparing `goatl-0.6.2/src/goatl/utils.py` & `goatl-0.6.3/src/goatl/utils.py`

 * *Files identical despite different names*

### Comparing `goatl-0.6.2/setup.py` & `goatl-0.6.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 ['goatl']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'goatl',
-    'version': '0.6.2',
+    'version': '0.6.3',
     'description': 'The goat logger',
-    'long_description': '# goatl\n\n```\nsome body please prompt midjourney for "Cartoonish goat scribing on a long scroll oil painting, --ar  2:1"\nand make abanner for here.\n```\n\n##\n\n<div align="center">\n\n[![Build status](https://github.com/EytanDn/goatl/workflows/build/badge.svg?branch=master&event=push)](https://github.com/EytanDn/goatl/actions?query=workflow%3Abuild)\n[![Python Version](https://img.shields.io/pypi/pyversions/goatl.svg)](https://pypi.org/project/goatl/)\n[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/EytanDn/goatl/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n![Coverage Report](assets/images/coverage.svg)\n\n</div>\n\n## Installation\n\n```bash\npip install -U goatl\n```\n\nor install with `Poetry`\n\n```bash\npoetry add goatl\n```\n\n## Purpose\n\ngoatl provides a simple and easy to use logging interface for python projects.\nby replacing repetitive boilerplate code with a simple function call:\nthe magic "log" function.\n\n```python\nfrom goatl import log\n```\n\ngoatl usage is all about the log\n\n## Usage\n\n### as a function\n\n```python\nlog("hello world")\n# 2020-07-19 16:00:00,000 - goatl - INFO - hello world\nlog.debug("hello world?")\n# 2020-07-19 16:00:00,000 - goatl - DEBUG - hello world?\nlog.info("do you know the answer of {} + {}?", 41, 1)\n# 2020-07-19 16:00:00,000 - goatl - INFO - do you know the answer of 41 + 1?\n```\n\n### as a method decorator\n\n```python\n@log\ndef foo(x, y):\n    return x + y\n\n@log.debug\ndef bar():\n    return "hello world"\n\n@log.debug(return_level=log.info)\ndef baz(x):\n    return x*2\n\nfoo(1, 2)\n# ... INFO - foo called with args: (1, 2), kwargs: {}\n# ... DEBUG - foo returned: 3\nbar()\n# ... DEBUG - bar called with args: (), kwargs: {}\n# ... INFO - bar returned: hello world\nbaz(3)\n# ... DEBUG - baz called with args: (3,), kwargs: {}\n# ... INFO - baz returned: 6\n```\n\n### as a class decorator\n\n```python\n@log\nclass Foo:\n    def __init__(self, x):\n        self.x = x\n\n    def bar(self, y):\n        return self.x + y\n\n    @log.warn\n    def baz(self):\n        return self.x * 2\n\n\nfoo = Foo(1)\n# ... INFO - Instantiated Foo with args: (1,), kwargs: {}\nfoo.bar(2)\n# ... INFO - Foo.bar called with args: (2,), kwargs: {}\n# ... DEBUG - Foo.bar returned: 3\nfoo.baz()\n# ... WARNING - Foo.baz called with args: (), kwargs: {}\n# ... WARNING - Foo.baz returned: 2\n```\n\n### configurations shortcuts\n\n```python\nfile_formatter = log.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")\nlog.addFileHandler("foo.log", fmt=file_formatter)\nlog.addStreamHandler(fmt="%(levelname)s - %(message)s")\nlog.basicConfig(...)\nlog.setFormat(...)\nlog.setLevel(...)\n```\n\n### logging interface #not implemented yet\n\nI do plan to implement goatl\'s interaction with logging through an interface\nsuch that it will be possible to use goatl with any logging backend.\n\n```python\nlog.setBackend(logging)\nlog.setBackend(loguru)\nlogger = log.getLogger("foo")\n```\n\n## core concepts\n\nIn order to justify the existence of goatl,\nit must fulfill three important core concepts:\n\n1. Unobtrusive - it should not interfere\\* with the existing code.\n2. Ease of use - using it should be intuitive and pythonic.\n3. Clean - the amount of code added to the existing code should be minimal.\n\n<sub>\\* - logging will always carry a performative cost, goatl will aim at keeping it to a minimum.</sub>\n\n### means\n\nextensive testing of goatl must be implemented to ensure that it does not interfere with the existing code.\nit should be tested by wrapping other popular libraries and modules with goatl.\nthis will ensure that goatl does not interfere with the existing code.\nperformance tests should be implemented to measure the performance cost of goatl,\nit should not exceed a reasonable threshold, in comparison to adding logging manually.\n\n### main features\n\nthe log function provides an easy interace for:\n\n- out of and in context log calls\n- wrapping existing functions with log calls\n- wrapping existing classes with log calls\n- wrapping existing modules with log calls #not implemented yet, is this even possible?\n- logging configuration #not implemented yet\n- support multiple logging backends #not implemented yet\n\nall in an intuitive and pythonic way.\n\n## Releases\n\nYou can see the list of available releases on the [GitHub Releases](https://github.com/EytanDn/goatl/releases) page.\n\n## License\n\n[![License](https://img.shields.io/github/license/Eytandn/goatl)](https://github.com/EytanDn/goatl/blob/master/LICENSE)\n\nThis project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/eytandn/goatl/blob/master/LICENSE) for more details.\n\n## Citation\n\n```bibtex\n@misc{goatl,\n  author = {goatl},\n  title = {goat logger},\n  year = {2023},\n  publisher = {GitHub},\n  journal = {GitHub repository},\n  howpublished = {\\url{https://github.com/EytanDn/goatl}}\n}\n```\n',
+    'long_description': '<div align="center">\n<img src="assets/images/goatlbanner.png" alt="goatl logo"/>\n\n</div>\n\n---\n\n# goatl\n\n<div align="center">\n\n[![Build status](https://github.com/EytanDn/goatl/workflows/build/badge.svg?branch=master&event=push)](https://github.com/EytanDn/goatl/actions?query=workflow%3Abuild)\n[![Python Version](https://img.shields.io/pypi/pyversions/goatl.svg)](https://pypi.org/project/goatl/)\n[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/EytanDn/goatl/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n![Coverage Report](assets/images/coverage.svg)\n\n</div>\n\n## Installation\n\n```bash\npip install -U goatl\n```\n\nor install with `Poetry`\n\n```bash\npoetry add goatl\n```\n\n## Purpose\n\ngoatl provides a simple and easy to use logging interface for python projects.\nby replacing repetitive boilerplate code with a simple function call:\nthe magic "log" function.\n\n```python\nfrom goatl import log\n```\n\ngoatl usage is all about the log\n\n## Usage\n\n### as a function\n\n```python\nlog("hello world")\n# 2020-07-19 16:00:00,000 - goatl - INFO - hello world\nlog.debug("hello world?")\n# 2020-07-19 16:00:00,000 - goatl - DEBUG - hello world?\nlog.info("do you know the answer of {} + {}?", 41, 1)\n# 2020-07-19 16:00:00,000 - goatl - INFO - do you know the answer of 41 + 1?\n```\n\n### as a method decorator\n\n```python\n@log\ndef foo(x, y):\n    return x + y\n\n@log.debug\ndef bar():\n    return "hello world"\n\n@log.debug(return_level=log.info)\ndef baz(x):\n    return x*2\n\nfoo(1, 2)\n# ... INFO - foo called with args: (1, 2), kwargs: {}\n# ... DEBUG - foo returned: 3\nbar()\n# ... DEBUG - bar called with args: (), kwargs: {}\n# ... DEBUG - bar returned: hello world\nbaz(3)\n# ... DEBUG - baz called with args: (3,), kwargs: {}\n# ... INFO - baz returned: 6\n```\n\n### as a class decorator\n\n```python\n@log\nclass Foo:\n    def __init__(self, x):\n        self.x = x\n\n    def bar(self, y):\n        return self.x + y\n\n    @log.warn\n    def baz(self):\n        return self.x * 2\n\n\nfoo = Foo(1)\n# ... INFO - Instantiated Foo with args: (1,), kwargs: {}\nfoo.bar(2)\n# ... INFO - Foo.bar called with args: (2,), kwargs: {}\n# ... DEBUG - Foo.bar returned: 3\nfoo.baz()\n# ... WARNING - Foo.baz called with args: (), kwargs: {}\n# ... WARNING - Foo.baz returned: 2\n```\n\n### configurations shortcuts\n\n```python\nfile_formatter = log.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")\nlog.addFileHandler("foo.log", fmt=file_formatter)\nlog.addStreamHandler(fmt="%(levelname)s - %(message)s")\nlog.basicConfig(...)\n```\n\n### logging interface #not implemented yet\n\nI do plan to implement goatl\'s interaction with logging through an interface\nsuch that it will be possible to use goatl with any logging backend.\n\n```python\nlog.setBackend(logging)\nlog.setBackend(loguru)\nlogger = log.getLogger("foo")\n```\n\n## core concepts\n\nIn order to justify the existence of goatl,\nit must fulfill three important core concepts:\n\n1. Unobtrusive - it should not interfere\\* with the existing code.\n2. Ease of use - using it should be intuitive and pythonic.\n3. Clean - the amount of code added to the existing code should be minimal.\n\n<sub>\\* - logging will always carry a performative cost, goatl will aim at keeping it to a minimum.</sub>\n\n### means\n\nextensive testing of goatl must be implemented to ensure that it does not interfere with the existing code.\nit should be tested by wrapping other popular libraries and modules with goatl.\nthis will ensure that goatl does not interfere with the existing code.\nperformance tests should be implemented to measure the performance cost of goatl,\nit should not exceed a reasonable threshold, in comparison to adding logging manually.\n\n### main features\n\nthe log function provides an easy interace for:\n\n- out of and in context log calls\n- wrapping existing functions with log calls\n- wrapping existing classes with log calls\n- wrapping existing modules with log calls #not implemented yet, is this even possible?\n- logging configuration #not implemented yet\n- support multiple logging backends #not implemented yet\n\nall in an intuitive and pythonic way.\n\n## Releases\n\nYou can see the list of available releases on the [GitHub Releases](https://github.com/EytanDn/goatl/releases) page.\n\n## License\n\n[![License](https://img.shields.io/github/license/Eytandn/goatl)](https://github.com/EytanDn/goatl/blob/master/LICENSE)\n\nThis project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/eytandn/goatl/blob/master/LICENSE) for more details.\n\n## Citation\n\n```bibtex\n@misc{goatl,\n  author = {goatl},\n  title = {goat logger},\n  year = {2023},\n  publisher = {GitHub},\n  journal = {GitHub repository},\n  howpublished = {\\url{https://github.com/EytanDn/goatl}}\n}\n```\n',
     'author': 'goatl',
     'author_email': 'EytanDn@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/EytanDn/goatl',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `goatl-0.6.2/PKG-INFO` & `goatl-0.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goatl
-Version: 0.6.2
+Version: 0.6.3
 Summary: The goat logger
 Home-page: https://github.com/EytanDn/goatl
 License: MIT
 Keywords: logging,logger,log,goat,goatl,goatlogger,goat-logger,goat-logging,goat-log
 Author: goatl
 Author-email: EytanDn@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -17,22 +17,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Repository, https://github.com/EytanDn/goatl
 Description-Content-Type: text/markdown
 
-# goatl
+<div align="center">
+<img src="assets/images/goatlbanner.png" alt="goatl logo"/>
 
-```
-some body please prompt midjourney for "Cartoonish goat scribing on a long scroll oil painting, --ar  2:1"
-and make abanner for here.
-```
+</div>
+
+---
 
-##
+# goatl
 
 <div align="center">
 
 [![Build status](https://github.com/EytanDn/goatl/workflows/build/badge.svg?branch=master&event=push)](https://github.com/EytanDn/goatl/actions?query=workflow%3Abuild)
 [![Python Version](https://img.shields.io/pypi/pyversions/goatl.svg)](https://pypi.org/project/goatl/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/EytanDn/goatl/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
@@ -94,15 +94,15 @@
     return x*2
 
 foo(1, 2)
 # ... INFO - foo called with args: (1, 2), kwargs: {}
 # ... DEBUG - foo returned: 3
 bar()
 # ... DEBUG - bar called with args: (), kwargs: {}
-# ... INFO - bar returned: hello world
+# ... DEBUG - bar returned: hello world
 baz(3)
 # ... DEBUG - baz called with args: (3,), kwargs: {}
 # ... INFO - baz returned: 6
 ```
 
 ### as a class decorator
 
@@ -133,16 +133,14 @@
 ### configurations shortcuts
 
 ```python
 file_formatter = log.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 log.addFileHandler("foo.log", fmt=file_formatter)
 log.addStreamHandler(fmt="%(levelname)s - %(message)s")
 log.basicConfig(...)
-log.setFormat(...)
-log.setLevel(...)
 ```
 
 ### logging interface #not implemented yet
 
 I do plan to implement goatl's interaction with logging through an interface
 such that it will be possible to use goatl with any logging backend.
```

