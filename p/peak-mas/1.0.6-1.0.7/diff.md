# Comparing `tmp/peak-mas-1.0.6.tar.gz` & `tmp/peak-mas-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peak-mas-1.0.6.tar", last modified: Tue May  2 13:06:26 2023, max compression
+gzip compressed data, was "peak-mas-1.0.7.tar", last modified: Mon May  8 16:11:29 2023, max compression
```

## Comparing `peak-mas-1.0.6.tar` & `peak-mas-1.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-02 13:06:26.483331 peak-mas-1.0.6/
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)    35148 2022-11-16 18:35:26.000000 peak-mas-1.0.6/LICENSE
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     6792 2023-05-02 13:06:26.483331 peak-mas-1.0.6/PKG-INFO
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     5843 2022-11-16 18:35:26.000000 peak-mas-1.0.6/README.md
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     1664 2023-05-02 13:06:10.000000 peak-mas-1.0.6/pyproject.toml
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)       38 2023-05-02 13:06:26.483331 peak-mas-1.0.6/setup.cfg
-drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-02 13:06:26.480331 peak-mas-1.0.6/src/
-drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-02 13:06:26.482331 peak-mas-1.0.6/src/peak/
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      603 2023-05-02 13:06:10.000000 peak-mas-1.0.6/src/peak/__init__.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3299 2023-04-20 14:45:48.000000 peak-mas-1.0.6/src/peak/__main__.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)    17777 2023-05-02 11:06:09.000000 peak-mas-1.0.6/src/peak/agents.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3519 2023-04-20 14:36:05.000000 peak-mas-1.0.6/src/peak/behaviours.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3608 2023-04-20 14:39:46.000000 peak-mas-1.0.6/src/peak/bootloader.py
-drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-02 13:06:26.482331 peak-mas-1.0.6/src/peak/cli/
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2022-11-16 18:35:26.000000 peak-mas-1.0.6/src/peak/cli/__init__.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      845 2023-04-20 14:39:59.000000 peak-mas-1.0.6/src/peak/cli/df.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     2837 2023-04-20 14:45:48.000000 peak-mas-1.0.6/src/peak/cli/mas.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     6727 2023-04-20 14:39:52.000000 peak-mas-1.0.6/src/peak/core.py
-drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-02 13:06:26.483331 peak-mas-1.0.6/src/peak_mas.egg-info/
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     6792 2023-05-02 13:06:26.000000 peak-mas-1.0.6/src/peak_mas.egg-info/PKG-INFO
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      438 2023-05-02 13:06:26.000000 peak-mas-1.0.6/src/peak_mas.egg-info/SOURCES.txt
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        1 2023-05-02 13:06:26.000000 peak-mas-1.0.6/src/peak_mas.egg-info/dependency_links.txt
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)       44 2023-05-02 13:06:26.000000 peak-mas-1.0.6/src/peak_mas.egg-info/entry_points.txt
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      119 2023-05-02 13:06:26.000000 peak-mas-1.0.6/src/peak_mas.egg-info/requires.txt
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        5 2023-05-02 13:06:26.000000 peak-mas-1.0.6/src/peak_mas.egg-info/top_level.txt
+drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-08 16:11:29.820867 peak-mas-1.0.7/
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)    35148 2022-11-16 18:35:26.000000 peak-mas-1.0.7/LICENSE
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     6943 2023-05-08 16:11:29.819867 peak-mas-1.0.7/PKG-INFO
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     5994 2023-05-02 14:41:35.000000 peak-mas-1.0.7/README.md
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     1664 2023-05-08 16:11:16.000000 peak-mas-1.0.7/pyproject.toml
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)       38 2023-05-08 16:11:29.820867 peak-mas-1.0.7/setup.cfg
+drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-08 16:11:29.816867 peak-mas-1.0.7/src/
+drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-08 16:11:29.818867 peak-mas-1.0.7/src/peak/
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      603 2023-05-08 16:11:16.000000 peak-mas-1.0.7/src/peak/__init__.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3342 2023-05-08 16:10:15.000000 peak-mas-1.0.7/src/peak/__main__.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)    17777 2023-05-02 14:40:53.000000 peak-mas-1.0.7/src/peak/agents.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3519 2023-05-02 14:40:53.000000 peak-mas-1.0.7/src/peak/behaviours.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3608 2023-05-02 14:40:53.000000 peak-mas-1.0.7/src/peak/bootloader.py
+drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-08 16:11:29.819867 peak-mas-1.0.7/src/peak/cli/
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2022-11-16 18:35:26.000000 peak-mas-1.0.7/src/peak/cli/__init__.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      845 2023-05-02 14:40:53.000000 peak-mas-1.0.7/src/peak/cli/df.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     2837 2023-05-02 14:40:53.000000 peak-mas-1.0.7/src/peak/cli/mas.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     6727 2023-05-02 14:40:53.000000 peak-mas-1.0.7/src/peak/core.py
+drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-08 16:11:29.819867 peak-mas-1.0.7/src/peak_mas.egg-info/
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     6943 2023-05-08 16:11:29.000000 peak-mas-1.0.7/src/peak_mas.egg-info/PKG-INFO
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      438 2023-05-08 16:11:29.000000 peak-mas-1.0.7/src/peak_mas.egg-info/SOURCES.txt
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        1 2023-05-08 16:11:29.000000 peak-mas-1.0.7/src/peak_mas.egg-info/dependency_links.txt
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)       44 2023-05-08 16:11:29.000000 peak-mas-1.0.7/src/peak_mas.egg-info/entry_points.txt
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      119 2023-05-08 16:11:29.000000 peak-mas-1.0.7/src/peak_mas.egg-info/requires.txt
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        5 2023-05-08 16:11:29.000000 peak-mas-1.0.7/src/peak_mas.egg-info/top_level.txt
```

### Comparing `peak-mas-1.0.6/LICENSE` & `peak-mas-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `peak-mas-1.0.6/PKG-INFO` & `peak-mas-1.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peak-mas
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python-based framework for heterogeneous agent communities
 Author-email: Bruno Ribeiro <brgri@isep.ipp.pt>
 Project-URL: Homepage, https://www.gecad.isep.ipp.pt/peak
 Project-URL: Github, https://github.com/gecad-group/peak-mas
 Keywords: framework,multiagent,agent-based,ecosystem,spade,xmpp
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
@@ -19,15 +19,21 @@
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
 
 # PEAK: Python-based framework for heterogenous agent communities
 
-![DOI](https://img.shields.io/static/v1?link=https://doi.org/10.1007/978-3-031-18050-7_7&link=https://doi.org/10.1007/978-3-031-18050-7_7&label=DOI&message=978-3-031-18050-7&color=blue) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/peak-mas) ![PyPI](https://img.shields.io/pypi/v/peak-mas) ![GitHub](https://img.shields.io/github/license/gecad-group/peak-mas) ![powered by](https://img.shields.io/static/v1?label=powered%20by&message=GECAD&color=177985&labelColor=de5d4a&?link=http://gecad.isep.ipp.pt&link=http://gecad.isep.ipp.pt/) ![code style](https://img.shields.io/badge/code%20style-black-black) ![imports isort](https://img.shields.io/static/v1?label=imports&message=isort&color=blue&labelColor=orange)
+[![DOI](https://img.shields.io/badge/DOI-10.1007%2F978--3--031--18050--7__7-blue)](https://link.springer.com/chapter/10.1007/978-3-031-18050-7_7)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/peak-mas)](https://pypi.org/project/peak-mas/)
+[![PyPI](https://img.shields.io/pypi/v/peak-mas)](https://pypi.org/project/peak-mas/)
+[![GitHub](https://img.shields.io/github/license/gecad-group/peak-mas)](https://github.com/gecad-group/peak-mas)
+[![powered by](https://img.shields.io/static/v1?label=powered%20by&message=GECAD&color=177985&labelColor=de5d4a)](https://www.gecad.isep.ipp.pt/GECAD/Pages/Presentation/Home.aspx)
+[![code style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
+[![imports isort](https://img.shields.io/static/v1?label=imports&message=isort&color=blue&labelColor=orange)](https://pycqa.github.io/isort/)
 
 PEAK is a multi-agent system framework which helps the users develop, monitor, analyze and maintain ecosystem of heterogeneous agent communities. This ecosystem is  where various multi-agent systems can coexist, interact and share resources between them. 
 This framework is based on <a href="https://spade-mas.readthedocs.io/en/latest/" target="_blank">SPADE</a>.
 
 
 ## Prerequisites
```

### Comparing `peak-mas-1.0.6/README.md` & `peak-mas-1.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # PEAK: Python-based framework for heterogenous agent communities
 
-![DOI](https://img.shields.io/static/v1?link=https://doi.org/10.1007/978-3-031-18050-7_7&link=https://doi.org/10.1007/978-3-031-18050-7_7&label=DOI&message=978-3-031-18050-7&color=blue) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/peak-mas) ![PyPI](https://img.shields.io/pypi/v/peak-mas) ![GitHub](https://img.shields.io/github/license/gecad-group/peak-mas) ![powered by](https://img.shields.io/static/v1?label=powered%20by&message=GECAD&color=177985&labelColor=de5d4a&?link=http://gecad.isep.ipp.pt&link=http://gecad.isep.ipp.pt/) ![code style](https://img.shields.io/badge/code%20style-black-black) ![imports isort](https://img.shields.io/static/v1?label=imports&message=isort&color=blue&labelColor=orange)
+[![DOI](https://img.shields.io/badge/DOI-10.1007%2F978--3--031--18050--7__7-blue)](https://link.springer.com/chapter/10.1007/978-3-031-18050-7_7)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/peak-mas)](https://pypi.org/project/peak-mas/)
+[![PyPI](https://img.shields.io/pypi/v/peak-mas)](https://pypi.org/project/peak-mas/)
+[![GitHub](https://img.shields.io/github/license/gecad-group/peak-mas)](https://github.com/gecad-group/peak-mas)
+[![powered by](https://img.shields.io/static/v1?label=powered%20by&message=GECAD&color=177985&labelColor=de5d4a)](https://www.gecad.isep.ipp.pt/GECAD/Pages/Presentation/Home.aspx)
+[![code style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
+[![imports isort](https://img.shields.io/static/v1?label=imports&message=isort&color=blue&labelColor=orange)](https://pycqa.github.io/isort/)
 
 PEAK is a multi-agent system framework which helps the users develop, monitor, analyze and maintain ecosystem of heterogeneous agent communities. This ecosystem is  where various multi-agent systems can coexist, interact and share resources between them. 
 This framework is based on <a href="https://spade-mas.readthedocs.io/en/latest/" target="_blank">SPADE</a>.
 
 
 ## Prerequisites
```

### Comparing `peak-mas-1.0.6/pyproject.toml` & `peak-mas-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "peak-mas"
-version = "1.0.6"
+version = "1.0.7"
 description = "Python-based framework for heterogeneous agent communities"
 readme = "README.md"
 authors = [{ name = "Bruno Ribeiro", email = "brgri@isep.ipp.pt" }]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -38,15 +38,15 @@
 Homepage = "https://www.gecad.isep.ipp.pt/peak"
 Github = "https://github.com/gecad-group/peak-mas"
 
 [project.scripts]
 peak = "peak.__main__:main"
 
 [tool.bumpver]
-current_version = "1.0.6"
+current_version = "1.0.7"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "chore: bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `peak-mas-1.0.6/src/peak/__init__.py` & `peak-mas-1.0.7/src/peak/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 from peak.agents import *
 from peak.behaviours import *
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 __author__ = "Bruno Ribeiro"
 __email__ = "brgri@isep.ipp.pt"
-__version__ = "1.0.6"
+__version__ = "1.0.7"
```

### Comparing `peak-mas-1.0.6/src/peak/__main__.py` & `peak-mas-1.0.7/src/peak/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import logging
+import os
 import sys
 from argparse import ArgumentParser
 from pathlib import Path
 
 from peak import JID
 from peak import __name__ as peak_name
 from peak import __version__ as version
 from peak.cli import df, mas
 
+sys.path.append(os.getcwd())
 _logger = logging.getLogger(peak_name)
 
 
 def main(args=None):
     _logger.setLevel(logging.INFO)
     handler = logging.StreamHandler(sys.stdout)
     handler.setFormatter(
         logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
     )
     _logger.addHandler(handler)
     try:
-        _main()
+        _main(args)
     except Exception as e:
         _logger.critical(e, exc_info=1)
     except KeyboardInterrupt:
         _logger.info("Stoping PEAK: (reason: KeyboardInterrupt)")
 
 
 def _main(args=None):
```

### Comparing `peak-mas-1.0.6/src/peak/agents.py` & `peak-mas-1.0.7/src/peak/agents.py`

 * *Files identical despite different names*

### Comparing `peak-mas-1.0.6/src/peak/behaviours.py` & `peak-mas-1.0.7/src/peak/behaviours.py`

 * *Files identical despite different names*

### Comparing `peak-mas-1.0.6/src/peak/bootloader.py` & `peak-mas-1.0.7/src/peak/bootloader.py`

 * *Files identical despite different names*

### Comparing `peak-mas-1.0.6/src/peak/cli/df.py` & `peak-mas-1.0.7/src/peak/cli/df.py`

 * *Files identical despite different names*

### Comparing `peak-mas-1.0.6/src/peak/cli/mas.py` & `peak-mas-1.0.7/src/peak/cli/mas.py`

 * *Files identical despite different names*

### Comparing `peak-mas-1.0.6/src/peak/core.py` & `peak-mas-1.0.7/src/peak/core.py`

 * *Files identical despite different names*

### Comparing `peak-mas-1.0.6/src/peak_mas.egg-info/PKG-INFO` & `peak-mas-1.0.7/src/peak_mas.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peak-mas
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python-based framework for heterogeneous agent communities
 Author-email: Bruno Ribeiro <brgri@isep.ipp.pt>
 Project-URL: Homepage, https://www.gecad.isep.ipp.pt/peak
 Project-URL: Github, https://github.com/gecad-group/peak-mas
 Keywords: framework,multiagent,agent-based,ecosystem,spade,xmpp
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
@@ -19,15 +19,21 @@
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
 
 # PEAK: Python-based framework for heterogenous agent communities
 
-![DOI](https://img.shields.io/static/v1?link=https://doi.org/10.1007/978-3-031-18050-7_7&link=https://doi.org/10.1007/978-3-031-18050-7_7&label=DOI&message=978-3-031-18050-7&color=blue) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/peak-mas) ![PyPI](https://img.shields.io/pypi/v/peak-mas) ![GitHub](https://img.shields.io/github/license/gecad-group/peak-mas) ![powered by](https://img.shields.io/static/v1?label=powered%20by&message=GECAD&color=177985&labelColor=de5d4a&?link=http://gecad.isep.ipp.pt&link=http://gecad.isep.ipp.pt/) ![code style](https://img.shields.io/badge/code%20style-black-black) ![imports isort](https://img.shields.io/static/v1?label=imports&message=isort&color=blue&labelColor=orange)
+[![DOI](https://img.shields.io/badge/DOI-10.1007%2F978--3--031--18050--7__7-blue)](https://link.springer.com/chapter/10.1007/978-3-031-18050-7_7)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/peak-mas)](https://pypi.org/project/peak-mas/)
+[![PyPI](https://img.shields.io/pypi/v/peak-mas)](https://pypi.org/project/peak-mas/)
+[![GitHub](https://img.shields.io/github/license/gecad-group/peak-mas)](https://github.com/gecad-group/peak-mas)
+[![powered by](https://img.shields.io/static/v1?label=powered%20by&message=GECAD&color=177985&labelColor=de5d4a)](https://www.gecad.isep.ipp.pt/GECAD/Pages/Presentation/Home.aspx)
+[![code style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
+[![imports isort](https://img.shields.io/static/v1?label=imports&message=isort&color=blue&labelColor=orange)](https://pycqa.github.io/isort/)
 
 PEAK is a multi-agent system framework which helps the users develop, monitor, analyze and maintain ecosystem of heterogeneous agent communities. This ecosystem is  where various multi-agent systems can coexist, interact and share resources between them. 
 This framework is based on <a href="https://spade-mas.readthedocs.io/en/latest/" target="_blank">SPADE</a>.
 
 
 ## Prerequisites
```

