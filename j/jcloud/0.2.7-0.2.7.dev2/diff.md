# Comparing `tmp/jcloud-0.2.7.tar.gz` & `tmp/jcloud-0.2.7.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jcloud-0.2.7.tar", last modified: Mon May  8 13:24:34 2023, max compression
+gzip compressed data, was "jcloud-0.2.7.dev2.tar", last modified: Thu May  4 08:46:59 2023, max compression
```

## Comparing `jcloud-0.2.7.tar` & `jcloud-0.2.7.dev2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:24:34.000000 jcloud-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 13:24:18.000000 jcloud-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-08 13:24:18.000000 jcloud-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-08 13:24:34.000000 jcloud-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-08 13:24:18.000000 jcloud-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:24:34.000000 jcloud-0.2.7/jcloud/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12562 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/env_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21449 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:24:34.000000 jcloud-0.2.7/jcloud/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/parsers/custom_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/parsers/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/parsers/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/parsers/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/parsers/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/parsers/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/parsers/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/parsers/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:24:34.000000 jcloud-0.2.7/jcloud/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:24:34.000000 jcloud-0.2.7/jcloud/resources/project-template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/resources/project-template/.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:24:34.000000 jcloud-0.2.7/jcloud/resources/project-template/executor1/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/resources/project-template/executor1/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/resources/project-template/executor1/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/resources/project-template/executor1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/resources/project-template/flow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-08 13:24:18.000000 jcloud-0.2.7/jcloud/survey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:24:34.000000 jcloud-0.2.7/jcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-08 13:24:34.000000 jcloud-0.2.7/jcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-08 13:24:34.000000 jcloud-0.2.7/jcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:24:34.000000 jcloud-0.2.7/jcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-08 13:24:34.000000 jcloud-0.2.7/jcloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:24:34.000000 jcloud-0.2.7/jcloud.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-08 13:24:34.000000 jcloud-0.2.7/jcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-08 13:24:34.000000 jcloud-0.2.7/jcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-08 13:24:18.000000 jcloud-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:24:34.000000 jcloud-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-08 13:24:18.000000 jcloud-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:46:59.207906 jcloud-0.2.7.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-04 08:46:59.207906 jcloud-0.2.7.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:46:59.199905 jcloud-0.2.7.dev2/jcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 08:46:58.000000 jcloud-0.2.7.dev2/jcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12562 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/env_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21449 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:46:59.203905 jcloud-0.2.7.dev2/jcloud/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/parsers/custom_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/parsers/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/parsers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/parsers/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/parsers/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/parsers/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/parsers/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/parsers/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:46:59.195905 jcloud-0.2.7.dev2/jcloud/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:46:59.203905 jcloud-0.2.7.dev2/jcloud/resources/project-template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/resources/project-template/.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:46:59.207906 jcloud-0.2.7.dev2/jcloud/resources/project-template/executor1/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/resources/project-template/executor1/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/resources/project-template/executor1/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/resources/project-template/executor1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/resources/project-template/flow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/survey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:46:59.203905 jcloud-0.2.7.dev2/jcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-04 08:46:59.000000 jcloud-0.2.7.dev2/jcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-04 08:46:59.000000 jcloud-0.2.7.dev2/jcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:46:59.000000 jcloud-0.2.7.dev2/jcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-04 08:46:59.000000 jcloud-0.2.7.dev2/jcloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:46:59.000000 jcloud-0.2.7.dev2/jcloud.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-04 08:46:59.000000 jcloud-0.2.7.dev2/jcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 08:46:59.000000 jcloud-0.2.7.dev2/jcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 08:46:59.207906 jcloud-0.2.7.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jcloud-0.2.7/LICENSE` & `jcloud-0.2.7.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.7/PKG-INFO` & `jcloud-0.2.7.dev2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,66 +1,19 @@
 Metadata-Version: 2.1
 Name: jcloud
-Version: 0.2.7
+Version: 0.2.7.dev2
 Summary: Simplify deploying and managing Jina projects on Jina Cloud
 Home-page: https://github.com/jina-ai/jcloud
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/jcloud/tags
 Project-URL: Documentation, https://jcloud.jina.ai
 Project-URL: Source, https://github.com/jina-ai/jcloud/
 Project-URL: Tracker, https://github.com/jina-ai/jcloud/issues
-Description: <p align="center">
-        <br>
-        <br>
-        <br>
-        <img src="https://github.com/jina-ai/jcloud/blob/main/.github/README-img/logo.svg?raw=true" alt="JCloud logo: the command line interface that simplifies deploying and managing Jina projects on Jina Cloud" width="80px">
-        <br>
-        <br>
-        <br>
-        <b>Simplify deploying and hosting Jina projects on Jina Cloud</b>
-        </p>
-        
-        <p align=center>
-        <a href="https://pypi.org/project/jcloud/"><img alt="PyPI" src="https://img.shields.io/pypi/v/jcloud?label=PyPI&logo=pypi&logoColor=white&style=flat-square"></a>
-        <a href="https://slack.jina.ai"><img src="https://img.shields.io/badge/Slack-2.8k-blueviolet?logo=slack&amp;logoColor=white&style=flat-square"></a>
-        </p>
-        
-        ☁️ **To the cloud!** - Smoothly deploy a local project as a cloud service. Radically easy, no nasty surprises.
-        
-        🎯 **Cut to the chase** - One CLI with five commands to manage the lifecycle of your Jina projects.
-        
-        🎟️ **Early free access** - Sneak peek at our stealthy cloud hosting platform. Built on latest cloud-native tech stack, we now host your Jina project and offer computational and storage resources, for free!
-        
-        ## Install
-        
-        ```bash
-        pip install jcloud
-        jc -h
-        ```
-        
-        In case `jc` is already occupied by another tool, please use `jcloud` instead. If your pip install doesn't register bash commands for you, you can run `python -m jcloud -h`.
-        
-        ## [Documentation](https://docs.jina.ai/concepts/jcloud/)
-        
-        ## Support
-        
-        - Join our [Slack community](https://slack.jina.ai) and chat with other community members about ideas.
-        - Join our [Engineering All Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to discuss your use case and learn Jina's new features.
-          - **When?** The second Tuesday of every month
-          - **Where?**
-            Zoom ([see our public events calendar](https://calendar.google.com/calendar/embed?src=c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com&ctz=Europe%2FBerlin)/[.ical](https://calendar.google.com/calendar/ical/c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics))
-            and [live stream on YouTube](https://youtube.com/c/jina-ai)
-        - Subscribe to the latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
-        
-        ## Join Us
-        
-        JCloud is backed by [Jina AI](https://jina.ai) and licensed under [Apache-2.0](./LICENSE). [We are actively hiring](https://jobs.jina.ai) AI engineers, solution engineers to build the next neural search ecosystem in open-source.
-        
 Keywords: jcloud neural-search serverless deployment devops mlops
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
@@ -79,7 +32,57 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+<p align="center">
+<br>
+<br>
+<br>
+<img src="https://github.com/jina-ai/jcloud/blob/main/.github/README-img/logo.svg?raw=true" alt="JCloud logo: the command line interface that simplifies deploying and managing Jina projects on Jina Cloud" width="80px">
+<br>
+<br>
+<br>
+<b>Simplify deploying and hosting Jina projects on Jina Cloud</b>
+</p>
+
+<p align=center>
+<a href="https://pypi.org/project/jcloud/"><img alt="PyPI" src="https://img.shields.io/pypi/v/jcloud?label=PyPI&logo=pypi&logoColor=white&style=flat-square"></a>
+<a href="https://slack.jina.ai"><img src="https://img.shields.io/badge/Slack-2.8k-blueviolet?logo=slack&amp;logoColor=white&style=flat-square"></a>
+</p>
+
+☁️ **To the cloud!** - Smoothly deploy a local project as a cloud service. Radically easy, no nasty surprises.
+
+🎯 **Cut to the chase** - One CLI with five commands to manage the lifecycle of your Jina projects.
+
+🎟️ **Early free access** - Sneak peek at our stealthy cloud hosting platform. Built on latest cloud-native tech stack, we now host your Jina project and offer computational and storage resources, for free!
+
+## Install
+
+```bash
+pip install jcloud
+jc -h
+```
+
+In case `jc` is already occupied by another tool, please use `jcloud` instead. If your pip install doesn't register bash commands for you, you can run `python -m jcloud -h`.
+
+## [Documentation](https://docs.jina.ai/concepts/jcloud/)
+
+## Support
+
+- Join our [Slack community](https://slack.jina.ai) and chat with other community members about ideas.
+- Join our [Engineering All Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to discuss your use case and learn Jina's new features.
+  - **When?** The second Tuesday of every month
+  - **Where?**
+    Zoom ([see our public events calendar](https://calendar.google.com/calendar/embed?src=c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com&ctz=Europe%2FBerlin)/[.ical](https://calendar.google.com/calendar/ical/c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics))
+    and [live stream on YouTube](https://youtube.com/c/jina-ai)
+- Subscribe to the latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
+
+## Join Us
+
+JCloud is backed by [Jina AI](https://jina.ai) and licensed under [Apache-2.0](./LICENSE). [We are actively hiring](https://jobs.jina.ai) AI engineers, solution engineers to build the next neural search ecosystem in open-source.
+
+
```

#### html2text {}

```diff
@@ -1,14 +1,31 @@
-Metadata-Version: 2.1 Name: jcloud Version: 0.2.7 Summary: Simplify deploying
-and managing Jina projects on Jina Cloud Home-page: https://github.com/jina-ai/
-jcloud Author: Jina AI Author-email: hello@jina.ai License: Apache 2.0
-Download-URL: https://github.com/jina-ai/jcloud/tags Project-URL:
+Metadata-Version: 2.1 Name: jcloud Version: 0.2.7.dev2 Summary: Simplify
+deploying and managing Jina projects on Jina Cloud Home-page: https://
+github.com/jina-ai/jcloud Author: Jina AI Author-email: hello@jina.ai License:
+Apache 2.0 Download-URL: https://github.com/jina-ai/jcloud/tags Project-URL:
 Documentation, https://jcloud.jina.ai Project-URL: Source, https://github.com/
 jina-ai/jcloud/ Project-URL: Tracker, https://github.com/jina-ai/jcloud/issues
-Description:
+Keywords: jcloud neural-search serverless deployment devops mlops Platform:
+UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Unix Shell
+Classifier: Environment :: Console Classifier: License :: OSI Approved ::
+Apache Software License Classifier: Operating System :: OS Independent
+Classifier: Topic :: Database :: Database Engines/Servers Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Internet
+:: WWW/HTTP :: Indexing/Search Classifier: Topic :: Scientific/Engineering ::
+Image Recognition Classifier: Topic :: Multimedia :: Video Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Mathematics Classifier: Topic :: Software Development Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Description-Content-Type: text/markdown Provides-
+Extra: test License-File: LICENSE
 
 
 
 [JCloud logo: the command line interface that simplifies deploying and managing
                          Jina projects on Jina Cloud]
 
 
@@ -35,25 +52,8 @@
 [.ical](https://calendar.google.com/calendar/ical/
 c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics)) and
 [live stream on YouTube](https://youtube.com/c/jina-ai) - Subscribe to the
 latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
 ## Join Us JCloud is backed by [Jina AI](https://jina.ai) and licensed under
 [Apache-2.0](./LICENSE). [We are actively hiring](https://jobs.jina.ai) AI
 engineers, solution engineers to build the next neural search ecosystem in
-open-source. Keywords: jcloud neural-search serverless deployment devops mlops
-Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Education Classifier: Intended Audience :: Science/Research Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language :: Unix
-Shell Classifier: Environment :: Console Classifier: License :: OSI Approved ::
-Apache Software License Classifier: Operating System :: OS Independent
-Classifier: Topic :: Database :: Database Engines/Servers Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Internet
-:: WWW/HTTP :: Indexing/Search Classifier: Topic :: Scientific/Engineering ::
-Image Recognition Classifier: Topic :: Multimedia :: Video Classifier: Topic ::
-Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
-Mathematics Classifier: Topic :: Software Development Classifier: Topic ::
-Software Development :: Libraries Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Description-Content-Type: text/markdown Provides-
-Extra: test
+open-source.
```

### Comparing `jcloud-0.2.7/README.md` & `jcloud-0.2.7.dev2/README.md`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.7/jcloud/__main__.py` & `jcloud-0.2.7.dev2/jcloud/__main__.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.7/jcloud/api.py` & `jcloud-0.2.7.dev2/jcloud/api.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.7/jcloud/constants.py` & `jcloud-0.2.7.dev2/jcloud/constants.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.7/jcloud/env_helper.py` & `jcloud-0.2.7.dev2/jcloud/env_helper.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.7/jcloud/flow.py` & `jcloud-0.2.7.dev2/jcloud/flow.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.7/jcloud/helper.py` & `jcloud-0.2.7.dev2/jcloud/helper.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.7/jcloud/normalize.py` & `jcloud-0.2.7.dev2/jcloud/normalize.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.7/jcloud/parsers/__init__.py` & `jcloud-0.2.7.dev2/jcloud/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.7/jcloud/parsers/base.py` & `jcloud-0.2.7.dev2/jcloud/parsers/base.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.7/jcloud/parsers/custom_actions.py` & `jcloud-0.2.7.dev2/jcloud/parsers/custom_actions.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.7/jcloud/parsers/helper.py` & `jcloud-0.2.7.dev2/jcloud/parsers/helper.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.7/jcloud/parsers/list.py` & `jcloud-0.2.7.dev2/jcloud/parsers/list.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.7/jcloud/parsers/normalize.py` & `jcloud-0.2.7.dev2/jcloud/parsers/normalize.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.7/jcloud/parsers/remove.py` & `jcloud-0.2.7.dev2/jcloud/parsers/remove.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.7/jcloud/survey.py` & `jcloud-0.2.7.dev2/jcloud/survey.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.7/jcloud.egg-info/PKG-INFO` & `jcloud-0.2.7.dev2/jcloud.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,66 +1,19 @@
 Metadata-Version: 2.1
 Name: jcloud
-Version: 0.2.7
+Version: 0.2.7.dev2
 Summary: Simplify deploying and managing Jina projects on Jina Cloud
 Home-page: https://github.com/jina-ai/jcloud
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/jcloud/tags
 Project-URL: Documentation, https://jcloud.jina.ai
 Project-URL: Source, https://github.com/jina-ai/jcloud/
 Project-URL: Tracker, https://github.com/jina-ai/jcloud/issues
-Description: <p align="center">
-        <br>
-        <br>
-        <br>
-        <img src="https://github.com/jina-ai/jcloud/blob/main/.github/README-img/logo.svg?raw=true" alt="JCloud logo: the command line interface that simplifies deploying and managing Jina projects on Jina Cloud" width="80px">
-        <br>
-        <br>
-        <br>
-        <b>Simplify deploying and hosting Jina projects on Jina Cloud</b>
-        </p>
-        
-        <p align=center>
-        <a href="https://pypi.org/project/jcloud/"><img alt="PyPI" src="https://img.shields.io/pypi/v/jcloud?label=PyPI&logo=pypi&logoColor=white&style=flat-square"></a>
-        <a href="https://slack.jina.ai"><img src="https://img.shields.io/badge/Slack-2.8k-blueviolet?logo=slack&amp;logoColor=white&style=flat-square"></a>
-        </p>
-        
-        ☁️ **To the cloud!** - Smoothly deploy a local project as a cloud service. Radically easy, no nasty surprises.
-        
-        🎯 **Cut to the chase** - One CLI with five commands to manage the lifecycle of your Jina projects.
-        
-        🎟️ **Early free access** - Sneak peek at our stealthy cloud hosting platform. Built on latest cloud-native tech stack, we now host your Jina project and offer computational and storage resources, for free!
-        
-        ## Install
-        
-        ```bash
-        pip install jcloud
-        jc -h
-        ```
-        
-        In case `jc` is already occupied by another tool, please use `jcloud` instead. If your pip install doesn't register bash commands for you, you can run `python -m jcloud -h`.
-        
-        ## [Documentation](https://docs.jina.ai/concepts/jcloud/)
-        
-        ## Support
-        
-        - Join our [Slack community](https://slack.jina.ai) and chat with other community members about ideas.
-        - Join our [Engineering All Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to discuss your use case and learn Jina's new features.
-          - **When?** The second Tuesday of every month
-          - **Where?**
-            Zoom ([see our public events calendar](https://calendar.google.com/calendar/embed?src=c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com&ctz=Europe%2FBerlin)/[.ical](https://calendar.google.com/calendar/ical/c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics))
-            and [live stream on YouTube](https://youtube.com/c/jina-ai)
-        - Subscribe to the latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
-        
-        ## Join Us
-        
-        JCloud is backed by [Jina AI](https://jina.ai) and licensed under [Apache-2.0](./LICENSE). [We are actively hiring](https://jobs.jina.ai) AI engineers, solution engineers to build the next neural search ecosystem in open-source.
-        
 Keywords: jcloud neural-search serverless deployment devops mlops
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
@@ -79,7 +32,57 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+<p align="center">
+<br>
+<br>
+<br>
+<img src="https://github.com/jina-ai/jcloud/blob/main/.github/README-img/logo.svg?raw=true" alt="JCloud logo: the command line interface that simplifies deploying and managing Jina projects on Jina Cloud" width="80px">
+<br>
+<br>
+<br>
+<b>Simplify deploying and hosting Jina projects on Jina Cloud</b>
+</p>
+
+<p align=center>
+<a href="https://pypi.org/project/jcloud/"><img alt="PyPI" src="https://img.shields.io/pypi/v/jcloud?label=PyPI&logo=pypi&logoColor=white&style=flat-square"></a>
+<a href="https://slack.jina.ai"><img src="https://img.shields.io/badge/Slack-2.8k-blueviolet?logo=slack&amp;logoColor=white&style=flat-square"></a>
+</p>
+
+☁️ **To the cloud!** - Smoothly deploy a local project as a cloud service. Radically easy, no nasty surprises.
+
+🎯 **Cut to the chase** - One CLI with five commands to manage the lifecycle of your Jina projects.
+
+🎟️ **Early free access** - Sneak peek at our stealthy cloud hosting platform. Built on latest cloud-native tech stack, we now host your Jina project and offer computational and storage resources, for free!
+
+## Install
+
+```bash
+pip install jcloud
+jc -h
+```
+
+In case `jc` is already occupied by another tool, please use `jcloud` instead. If your pip install doesn't register bash commands for you, you can run `python -m jcloud -h`.
+
+## [Documentation](https://docs.jina.ai/concepts/jcloud/)
+
+## Support
+
+- Join our [Slack community](https://slack.jina.ai) and chat with other community members about ideas.
+- Join our [Engineering All Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to discuss your use case and learn Jina's new features.
+  - **When?** The second Tuesday of every month
+  - **Where?**
+    Zoom ([see our public events calendar](https://calendar.google.com/calendar/embed?src=c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com&ctz=Europe%2FBerlin)/[.ical](https://calendar.google.com/calendar/ical/c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics))
+    and [live stream on YouTube](https://youtube.com/c/jina-ai)
+- Subscribe to the latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
+
+## Join Us
+
+JCloud is backed by [Jina AI](https://jina.ai) and licensed under [Apache-2.0](./LICENSE). [We are actively hiring](https://jobs.jina.ai) AI engineers, solution engineers to build the next neural search ecosystem in open-source.
+
+
```

#### html2text {}

```diff
@@ -1,14 +1,31 @@
-Metadata-Version: 2.1 Name: jcloud Version: 0.2.7 Summary: Simplify deploying
-and managing Jina projects on Jina Cloud Home-page: https://github.com/jina-ai/
-jcloud Author: Jina AI Author-email: hello@jina.ai License: Apache 2.0
-Download-URL: https://github.com/jina-ai/jcloud/tags Project-URL:
+Metadata-Version: 2.1 Name: jcloud Version: 0.2.7.dev2 Summary: Simplify
+deploying and managing Jina projects on Jina Cloud Home-page: https://
+github.com/jina-ai/jcloud Author: Jina AI Author-email: hello@jina.ai License:
+Apache 2.0 Download-URL: https://github.com/jina-ai/jcloud/tags Project-URL:
 Documentation, https://jcloud.jina.ai Project-URL: Source, https://github.com/
 jina-ai/jcloud/ Project-URL: Tracker, https://github.com/jina-ai/jcloud/issues
-Description:
+Keywords: jcloud neural-search serverless deployment devops mlops Platform:
+UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Unix Shell
+Classifier: Environment :: Console Classifier: License :: OSI Approved ::
+Apache Software License Classifier: Operating System :: OS Independent
+Classifier: Topic :: Database :: Database Engines/Servers Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Internet
+:: WWW/HTTP :: Indexing/Search Classifier: Topic :: Scientific/Engineering ::
+Image Recognition Classifier: Topic :: Multimedia :: Video Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Mathematics Classifier: Topic :: Software Development Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Description-Content-Type: text/markdown Provides-
+Extra: test License-File: LICENSE
 
 
 
 [JCloud logo: the command line interface that simplifies deploying and managing
                          Jina projects on Jina Cloud]
 
 
@@ -35,25 +52,8 @@
 [.ical](https://calendar.google.com/calendar/ical/
 c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics)) and
 [live stream on YouTube](https://youtube.com/c/jina-ai) - Subscribe to the
 latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
 ## Join Us JCloud is backed by [Jina AI](https://jina.ai) and licensed under
 [Apache-2.0](./LICENSE). [We are actively hiring](https://jobs.jina.ai) AI
 engineers, solution engineers to build the next neural search ecosystem in
-open-source. Keywords: jcloud neural-search serverless deployment devops mlops
-Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Education Classifier: Intended Audience :: Science/Research Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language :: Unix
-Shell Classifier: Environment :: Console Classifier: License :: OSI Approved ::
-Apache Software License Classifier: Operating System :: OS Independent
-Classifier: Topic :: Database :: Database Engines/Servers Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Internet
-:: WWW/HTTP :: Indexing/Search Classifier: Topic :: Scientific/Engineering ::
-Image Recognition Classifier: Topic :: Multimedia :: Video Classifier: Topic ::
-Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
-Mathematics Classifier: Topic :: Software Development Classifier: Topic ::
-Software Development :: Libraries Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Description-Content-Type: text/markdown Provides-
-Extra: test
+open-source.
```

### Comparing `jcloud-0.2.7/jcloud.egg-info/SOURCES.txt` & `jcloud-0.2.7.dev2/jcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.7/setup.py` & `jcloud-0.2.7.dev2/setup.py`

 * *Files identical despite different names*

