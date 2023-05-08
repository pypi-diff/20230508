# Comparing `tmp/djlint-1.9.4.tar.gz` & `tmp/djlint-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djlint-1.9.4.tar", max compression
+gzip compressed data, was "djlint-1.9.5.tar", max compression
```

## Comparing `djlint-1.9.4.tar` & `djlint-1.9.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    34916 2022-08-02 16:48:50.834585 djlint-1.9.4/LICENSE
--rw-r--r--   0        0        0     5246 2022-08-02 16:48:50.834585 djlint-1.9.4/README.md
--rw-r--r--   0        0        0     1763 2022-08-02 16:49:20.387112 djlint-1.9.4/pyproject.toml
--rw-r--r--   0        0        0     7278 2022-08-02 16:48:50.898586 djlint-1.9.4/src/djlint/__init__.py
--rw-r--r--   0        0        0       78 2022-08-02 16:48:50.898586 djlint-1.9.4/src/djlint/__main__.py
--rw-r--r--   0        0        0       14 2022-08-02 16:48:50.898586 djlint-1.9.4/src/djlint/formatter/__init__.py
--rw-r--r--   0        0        0     9068 2022-08-02 16:48:50.898586 djlint-1.9.4/src/djlint/formatter/attributes.py
--rw-r--r--   0        0        0     1058 2022-08-02 16:48:50.898586 djlint-1.9.4/src/djlint/formatter/compress.py
--rw-r--r--   0        0        0     5475 2022-08-02 16:48:50.898586 djlint-1.9.4/src/djlint/formatter/condense.py
--rw-r--r--   0        0        0     1191 2022-08-02 16:48:50.898586 djlint-1.9.4/src/djlint/formatter/css.py
--rw-r--r--   0        0        0     2925 2022-08-02 16:48:50.898586 djlint-1.9.4/src/djlint/formatter/expand.py
--rw-r--r--   0        0        0     8411 2022-08-02 16:48:50.898586 djlint-1.9.4/src/djlint/formatter/indent.py
--rw-r--r--   0        0        0     1196 2022-08-02 16:48:50.898586 djlint-1.9.4/src/djlint/formatter/js.py
--rw-r--r--   0        0        0     3583 2022-08-02 16:48:50.898586 djlint-1.9.4/src/djlint/helpers.py
--rw-r--r--   0        0        0     5004 2022-08-02 16:48:50.898586 djlint-1.9.4/src/djlint/lint.py
--rw-r--r--   0        0        0     5464 2022-08-02 16:48:50.898586 djlint-1.9.4/src/djlint/output.py
--rw-r--r--   0        0        0     1235 2022-08-02 16:48:50.898586 djlint-1.9.4/src/djlint/reformat.py
--rw-r--r--   0        0        0     8362 2022-08-02 16:48:50.898586 djlint-1.9.4/src/djlint/rules.yaml
--rw-r--r--   0        0        0    21371 2022-08-02 16:48:50.898586 djlint-1.9.4/src/djlint/settings.py
--rw-r--r--   0        0        0     2819 2022-08-02 16:48:50.898586 djlint-1.9.4/src/djlint/src.py
--rw-r--r--   0        0        0     6659 2022-08-02 16:50:10.028563 djlint-1.9.4/setup.py
--rw-r--r--   0        0        0     6629 2022-08-02 16:50:10.029176 djlint-1.9.4/PKG-INFO
+-rw-r--r--   0        0        0    34916 2022-08-16 12:56:32.182479 djlint-1.9.5/LICENSE
+-rw-r--r--   0        0        0     5246 2022-08-16 12:56:32.182479 djlint-1.9.5/README.md
+-rw-r--r--   0        0        0     1763 2022-08-16 12:57:07.582351 djlint-1.9.5/pyproject.toml
+-rw-r--r--   0        0        0     7278 2022-08-16 12:56:32.254479 djlint-1.9.5/src/djlint/__init__.py
+-rw-r--r--   0        0        0       78 2022-08-16 12:56:32.254479 djlint-1.9.5/src/djlint/__main__.py
+-rw-r--r--   0        0        0       14 2022-08-16 12:56:32.254479 djlint-1.9.5/src/djlint/formatter/__init__.py
+-rw-r--r--   0        0        0     9056 2022-08-16 12:56:32.258479 djlint-1.9.5/src/djlint/formatter/attributes.py
+-rw-r--r--   0        0        0     1058 2022-08-16 12:56:32.258479 djlint-1.9.5/src/djlint/formatter/compress.py
+-rw-r--r--   0        0        0     5475 2022-08-16 12:56:32.258479 djlint-1.9.5/src/djlint/formatter/condense.py
+-rw-r--r--   0        0        0     1191 2022-08-16 12:56:32.258479 djlint-1.9.5/src/djlint/formatter/css.py
+-rw-r--r--   0        0        0     2925 2022-08-16 12:56:32.258479 djlint-1.9.5/src/djlint/formatter/expand.py
+-rw-r--r--   0        0        0     8411 2022-08-16 12:56:32.258479 djlint-1.9.5/src/djlint/formatter/indent.py
+-rw-r--r--   0        0        0     1196 2022-08-16 12:56:32.258479 djlint-1.9.5/src/djlint/formatter/js.py
+-rw-r--r--   0        0        0     3583 2022-08-16 12:56:32.258479 djlint-1.9.5/src/djlint/helpers.py
+-rw-r--r--   0        0        0     5004 2022-08-16 12:56:32.258479 djlint-1.9.5/src/djlint/lint.py
+-rw-r--r--   0        0        0     5464 2022-08-16 12:56:32.258479 djlint-1.9.5/src/djlint/output.py
+-rw-r--r--   0        0        0     1235 2022-08-16 12:56:32.258479 djlint-1.9.5/src/djlint/reformat.py
+-rw-r--r--   0        0        0     8362 2022-08-16 12:56:32.258479 djlint-1.9.5/src/djlint/rules.yaml
+-rw-r--r--   0        0        0    21371 2022-08-16 12:56:32.258479 djlint-1.9.5/src/djlint/settings.py
+-rw-r--r--   0        0        0     2819 2022-08-16 12:56:32.258479 djlint-1.9.5/src/djlint/src.py
+-rw-r--r--   0        0        0     6659 2022-08-16 12:58:31.678224 djlint-1.9.5/setup.py
+-rw-r--r--   0        0        0     6629 2022-08-16 12:58:31.678899 djlint-1.9.5/PKG-INFO
```

### Comparing `djlint-1.9.4/LICENSE` & `djlint-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `djlint-1.9.4/README.md` & `djlint-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `djlint-1.9.4/pyproject.toml` & `djlint-1.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 
 [tool]
 
 [tool.poetry]
 name="djlint"
-version="1.9.4"
+version="1.9.5"
 description="HTML Template Linter and Formatter"
 license="GPL-3.0-or-later"
 authors=["Christopher Pickering <cpickering@rhc.net>"]
 maintainers=["Christopher Pickering <cpickering@rhc.net>"]
 readme="README.md"
 repository="https://github.com/Riverside-Healthcare/djlint"
 documentation="https://djlint.com"
```

### Comparing `djlint-1.9.4/src/djlint/__init__.py` & `djlint-1.9.5/src/djlint/__init__.py`

 * *Files identical despite different names*

### Comparing `djlint-1.9.4/src/djlint/formatter/attributes.py` & `djlint-1.9.5/src/djlint/formatter/attributes.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,30 +37,29 @@
             list(
                 re.finditer(
                     re.compile(r"^<\w+\b\s*", re.M), attributes.splitlines()[0].strip()
                 )
             )
         )[-1]
 
-        start_test = (
-            list(
-                re.finditer(
-                    re.compile(
-                        r"^.*?(?=" + config.template_indent + r")", re.I | re.X | re.M
-                    ),
-                    attributes.splitlines()[0].strip(),
-                )
+        start_test_list = list(
+            re.finditer(
+                re.compile(
+                    r"^.*?(?=" + config.template_indent + r")", re.I | re.X | re.M
+                ),
+                attributes.splitlines()[0].strip(),
             )
-            + list(
-                re.finditer(
-                    re.compile(r"^<\w+\b\s*[^\"']+?[\"']", re.M),
-                    attributes.splitlines()[0].strip(),
-                )
+        ) + list(
+            re.finditer(
+                re.compile(r"^<\w+\b\s*[^\"']+?[\"']", re.M),
+                attributes.splitlines()[0].strip(),
             )
-        )[-1]
+        )
+
+        start_test = start_test_list[-1] if start_test_list else None
 
         base_indent = len(attr_name.group())
 
         indent = 0
         indented = ""
         indent_adder = 0
```

### Comparing `djlint-1.9.4/src/djlint/formatter/compress.py` & `djlint-1.9.5/src/djlint/formatter/compress.py`

 * *Files identical despite different names*

### Comparing `djlint-1.9.4/src/djlint/formatter/condense.py` & `djlint-1.9.5/src/djlint/formatter/condense.py`

 * *Files identical despite different names*

### Comparing `djlint-1.9.4/src/djlint/formatter/css.py` & `djlint-1.9.5/src/djlint/formatter/css.py`

 * *Files identical despite different names*

### Comparing `djlint-1.9.4/src/djlint/formatter/expand.py` & `djlint-1.9.5/src/djlint/formatter/expand.py`

 * *Files identical despite different names*

### Comparing `djlint-1.9.4/src/djlint/formatter/indent.py` & `djlint-1.9.5/src/djlint/formatter/indent.py`

 * *Files identical despite different names*

### Comparing `djlint-1.9.4/src/djlint/formatter/js.py` & `djlint-1.9.5/src/djlint/formatter/js.py`

 * *Files identical despite different names*

### Comparing `djlint-1.9.4/src/djlint/helpers.py` & `djlint-1.9.5/src/djlint/helpers.py`

 * *Files identical despite different names*

### Comparing `djlint-1.9.4/src/djlint/lint.py` & `djlint-1.9.5/src/djlint/lint.py`

 * *Files identical despite different names*

### Comparing `djlint-1.9.4/src/djlint/output.py` & `djlint-1.9.5/src/djlint/output.py`

 * *Files identical despite different names*

### Comparing `djlint-1.9.4/src/djlint/reformat.py` & `djlint-1.9.5/src/djlint/reformat.py`

 * *Files identical despite different names*

### Comparing `djlint-1.9.4/src/djlint/rules.yaml` & `djlint-1.9.5/src/djlint/rules.yaml`

 * *Files identical despite different names*

### Comparing `djlint-1.9.4/src/djlint/settings.py` & `djlint-1.9.5/src/djlint/settings.py`

 * *Files identical despite different names*

### Comparing `djlint-1.9.4/src/djlint/src.py` & `djlint-1.9.5/src/djlint/src.py`

 * *Files identical despite different names*

### Comparing `djlint-1.9.4/setup.py` & `djlint-1.9.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 {':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['djlint = djlint:main']}
 
 setup_kwargs = {
     'name': 'djlint',
-    'version': '1.9.4',
+    'version': '1.9.5',
     'description': 'HTML Template Linter and Formatter',
     'long_description': '\n<h1 align="center">\n  <br>\n  <a href="https://www.djlint.com"><img src="https://raw.githubusercontent.com/Riverside-Healthcare/djLint/master/docs/src/static/img/icon.png" alt="djLint Logo" width="270"></a>\n  <br>\n</h1>\n<h3 align="center">🙏 Passed 100k downloads! Thank you! 🙏</h3>\n<h4 align="center">The missing formatter and linter for HTML templates.</h4>\n\n<p align="center">\n    <a href="https://twitter.com/intent/tweet?text=djLint%20%7C%20The%20missing%20formatter%20and%20linter%20for%20HTML%20templates.&url=https://djlint.com/&hashtags=djlint,html-templates,django,jinja,developers"><img alt="tweet" src="https://img.shields.io/twitter/url/http/shields.io.svg?style=social" /></a>\n    <a href="https://discord.gg/taghAqebzU">\n     <img src="https://badgen.net/discord/online-members/taghAqebzU?icon=discord&label" alt="Discord Chat">\n   </a>\n    </p>\n    <p align="center">\n   <a href="https://codecov.io/gh/Riverside-Healthcare/djlint">\n     <img src="https://codecov.io/gh/Riverside-Healthcare/djlint/branch/master/graph/badge.svg?token=eNTG721BAA" alt="Codecov Status">\n   </a>\n   <a href="https://www.codacy.com/gh/Riverside-Healthcare/djlint/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Riverside-Healthcare/djlint&amp;utm_campaign=Badge_Grade">\n     <img src="https://app.codacy.com/project/badge/Grade/dba6338b0e7a4de896b45b382574f369" alt="Codacy Status">\n   </a>\n   <a href="https://pepy.tech/project/djlint">\n     <img src="https://pepy.tech/badge/djlint" alt="Downloads">\n   </a>\n   <a href="https://www.npmjs.com/package/djlint">\n       <img alt="npm" src="https://img.shields.io/npm/dt/djlint?label=npm%20downloads">\n   </a>\n   <a href="https://pypi.org/project/djlint/">\n     <img src="https://img.shields.io/pypi/v/djlint" alt="Pypi Download">\n   </a>\n</p>\n\n<h4 align="center"><a href="https://www.djlint.com">How to use</a> • <a href="https://www.djlint.com/ru/">Как пользоваться</a> • <a href="https://www.djlint.com/fr/">Utilisation</a></h4>\n<h4 align="center">What lang are you using?</h4>\n\n<p align="center">\n   <a href="https://djlint.com/docs/languages/django/">Django</a> • <a href="https://djlint.com/docs/languages/jinja/">Jinja</a> • <a href="https://djlint.com/docs/languages/nunjucks/">Nunjucks</a> • <a href="https://djlint.com/docs/languages/twig/">Twig</a> • <a href="https://djlint.com/docs/languages/handlebars/">Handlebars</a> • <a href="https://djlint.com/docs/languages/mustach/">Mustache</a> • <a href="https://djlint.com/docs/languages/golang/">GoLang</a> • <a href="https://djlint.com/docs/languages/angular/">Angular</a>\n</p>\n\n<p align="center">\n  <img src="https://github.com/Riverside-Healthcare/djLint/blob/aa9097660d4a2e840450de5456f656c42bc7dd34/docs/src/static/img/demo-min.gif" alt="demo" width="600">\n</p>\n\n## 🤔 For What?\n\nOnce upon a time all the other programming languages had a formatter and linter. Css, javascript, python, the c suite, typescript, ruby, php, go, swift, and you know the others. The cool kids on the block.\n\nHTML templates were left out there on their own, in the cold, unformatted and unlinted :( The dirty corner in your repository. Something had to change.\n\n**djLint is a community build project to and add consistency to html templates.**\n\n## ✨ How?\n\nGrab it with `pip`\n\n```bash\npip install djlint\n```\n\n*Or with the npm experimental install - Note, this requires python and pip to be on your system path.*\n\n```bash\nnpm i djlint\n```\n\nLint your project\n\n```bash\ndjlint . --extension=html.j2 --lint\n```\nCheck your format\n\n```bash\ndjlint . --extension=html.j2 --check\n```\nFix my format!\n```bash\ndjlint . --extension=html.j2 --reformat\n```\n\n## 💙 Like it?\n\nAdd a badge to your projects ```readme.md```:\n\n```md\n[![Code style: djlint](https://img.shields.io/badge/html%20style-djlint-blue.svg)](https://www.djlint.com)\n```\n\nAdd a badge to your ```readme.rst```:\n\n```rst\n.. image:: https://img.shields.io/badge/html%20style-djlint-blue.svg\n   :target: https://www.djlint.com\n```\nLooks like this:\n\n[![djLint](https://img.shields.io/badge/html%20style-djLint-blue.svg)](https://github.com/Riverside-Healthcare/djlint)\n\n\n## 🛠️ Can I help?\n\nYes! \n\n*Would you like to add a rule to the linter?* Take a look at the [linter docs](https://djlint.com/docs/linter/) and [source code](https://github.com/Riverside-Healthcare/djLint/blob/master/src/djlint/rules.yaml)\n\n*Are you a regex pro?* Benchmark and submit a pr with improved regex for the [linter rules](https://github.com/Riverside-Healthcare/djLint/blob/master/src/djlint/rules.yaml)\n\n**⚠️ Help Needed! ⚠️** *Good with python?* djLint was an experimental project and is catching on with other devs. Help out with a rewrite of the formatter to improve speed and html style for edge cases. Contribute on the [2.0 branch](https://github.com/Riverside-Healthcare/djLint/tree/block_indent)\n\n## 🏃 Other Tools Of Note\n\n* [DjHTML](https://github.com/rtts/djhtml) A pure-Python Django/Jinja template indenter without dependencies.\n* [HTMLHint](https://htmlhint.com) Static code analysis tool you need for your HTML\n* [curlylint](https://www.curlylint.org) Experimental HTML templates linting for Jinja, Nunjucks, Django templates, Twig, Liquid\n',
     'author': 'Christopher Pickering',
     'author_email': 'cpickering@rhc.net',
     'maintainer': 'Christopher Pickering',
     'maintainer_email': 'cpickering@rhc.net',
     'url': 'https://github.com/Riverside-Healthcare/djlint',
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 install_requires = \ ['PyYAML>=6.0,<7.0', 'click>=8.0.1,<9.0.0',
 'colorama>=0.4.4,<0.5.0', 'cssbeautifier>=1.14.4,<2.0.0', 'html-tag-
 names>=0.1.2,<0.2.0', 'html-void-elements>=0.1.0,<0.2.0', 'importlib-
 metadata>=4.11.0,<5.0.0', 'jsbeautifier>=1.14.4,<2.0.0',
 'pathspec>=0.9.0,<0.10.0', 'regex>=2022.1.18,<2023.0.0', 'tqdm>=4.62.2,<5.0.0']
 extras_require = \ {':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
 entry_points = \ {'console_scripts': ['djlint = djlint:main']} setup_kwargs =
-{ 'name': 'djlint', 'version': '1.9.4', 'description': 'HTML Template Linter
+{ 'name': 'djlint', 'version': '1.9.5', 'description': 'HTML Template Linter
 and Formatter', 'long_description': '\n
                                   ****** \n
                               \n [djLint_Logo]\n
                                    \n ******
 \n
              **** ð Passed 100k downloads! Thank you! ð ****
 \n
```

### Comparing `djlint-1.9.4/PKG-INFO` & `djlint-1.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djlint
-Version: 1.9.4
+Version: 1.9.5
 Summary: HTML Template Linter and Formatter
 Home-page: https://github.com/Riverside-Healthcare/djlint
 License: GPL-3.0-or-later
 Author: Christopher Pickering
 Author-email: cpickering@rhc.net
 Maintainer: Christopher Pickering
 Maintainer-email: cpickering@rhc.net
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: djlint Version: 1.9.4 Summary: HTML Template Linter
+Metadata-Version: 2.1 Name: djlint Version: 1.9.5 Summary: HTML Template Linter
 and Formatter Home-page: https://github.com/Riverside-Healthcare/djlint
 License: GPL-3.0-or-later Author: Christopher Pickering Author-email:
 cpickering@rhc.net Maintainer: Christopher Pickering Maintainer-email:
 cpickering@rhc.net Requires-Python: >=3.7.2,<4.0.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

