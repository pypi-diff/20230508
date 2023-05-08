# Comparing `tmp/dicompyler-core-0.5.5.tar.gz` & `tmp/dicompyler-core-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dicompyler-core-0.5.5.tar", last modified: Sat Jun  1 04:43:04 2019, max compression
+gzip compressed data, was "dicompyler-core-0.5.6.tar", last modified: Mon May  8 15:58:56 2023, max compression
```

## Comparing `dicompyler-core-0.5.5.tar` & `dicompyler-core-0.5.6.tar`

### file list

```diff
@@ -1,52 +1,57 @@
-drwxr-xr-x   0 apanchal   (501) staff       (20)        0 2019-06-01 04:43:04.000000 dicompyler-core-0.5.5/
--rw-r--r--   0 apanchal   (501) staff       (20)      309 2016-02-11 21:58:32.000000 dicompyler-core-0.5.5/.coveragerc
--rw-r--r--   0 apanchal   (501) staff       (20)      117 2016-02-18 00:01:05.000000 dicompyler-core-0.5.5/AUTHORS.rst
--rw-r--r--   0 apanchal   (501) staff       (20)     3374 2019-03-12 04:29:53.000000 dicompyler-core-0.5.5/CONTRIBUTING.rst
--rw-r--r--   0 apanchal   (501) staff       (20)     3402 2019-06-01 03:57:09.000000 dicompyler-core-0.5.5/HISTORY.rst
--rw-r--r--   0 apanchal   (501) staff       (20)     1537 2016-10-19 21:20:01.000000 dicompyler-core-0.5.5/LICENSE
--rw-r--r--   0 apanchal   (501) staff       (20)      357 2016-02-17 23:25:10.000000 dicompyler-core-0.5.5/MANIFEST.in
--rw-r--r--   0 apanchal   (501) staff       (20)     2403 2019-06-01 04:43:00.000000 dicompyler-core-0.5.5/Makefile
--rw-r--r--   0 apanchal   (501) staff       (20)     5827 2019-06-01 04:43:04.000000 dicompyler-core-0.5.5/PKG-INFO
--rw-r--r--   0 apanchal   (501) staff       (20)     3892 2019-03-12 04:29:53.000000 dicompyler-core-0.5.5/README.rst
-drwxr-xr-x   0 apanchal   (501) staff       (20)        0 2019-06-01 04:43:04.000000 dicompyler-core-0.5.5/dicompyler_core.egg-info/
--rw-r--r--   0 apanchal   (501) staff       (20)     5827 2019-06-01 04:43:03.000000 dicompyler-core-0.5.5/dicompyler_core.egg-info/PKG-INFO
--rw-r--r--   0 apanchal   (501) staff       (20)      967 2019-06-01 04:43:03.000000 dicompyler-core-0.5.5/dicompyler_core.egg-info/SOURCES.txt
--rw-r--r--   0 apanchal   (501) staff       (20)       66 2019-06-01 04:43:03.000000 dicompyler-core-0.5.5/dicompyler_core.egg-info/dependency_links.txt
--rw-r--r--   0 apanchal   (501) staff       (20)        1 2019-06-01 04:43:03.000000 dicompyler-core-0.5.5/dicompyler_core.egg-info/not-zip-safe
--rw-r--r--   0 apanchal   (501) staff       (20)      130 2019-06-01 04:43:03.000000 dicompyler-core-0.5.5/dicompyler_core.egg-info/requires.txt
--rw-r--r--   0 apanchal   (501) staff       (20)       15 2019-06-01 04:43:03.000000 dicompyler-core-0.5.5/dicompyler_core.egg-info/top_level.txt
-drwxr-xr-x   0 apanchal   (501) staff       (20)        0 2019-06-01 04:43:04.000000 dicompyler-core-0.5.5/dicompylercore/
--rw-r--r--   0 apanchal   (501) staff       (20)      483 2018-10-25 17:27:04.000000 dicompyler-core-0.5.5/dicompylercore/__init__.py
--rw-r--r--   0 apanchal   (501) staff       (20)      995 2018-04-04 17:17:52.000000 dicompyler-core-0.5.5/dicompylercore/config.py
--rwxr-xr-x   0 apanchal   (501) staff       (20)    33661 2019-04-26 19:25:53.000000 dicompyler-core-0.5.5/dicompylercore/dicomparser.py
--rw-r--r--   0 apanchal   (501) staff       (20)    21100 2019-03-12 04:29:53.000000 dicompyler-core-0.5.5/dicompylercore/dvh.py
--rwxr-xr-x   0 apanchal   (501) staff       (20)    18851 2019-05-20 15:20:07.000000 dicompyler-core-0.5.5/dicompylercore/dvhcalc.py
--rwxr-xr-x   0 apanchal   (501) staff       (20)     5294 2016-10-19 21:20:01.000000 dicompyler-core-0.5.5/dicompylercore/util.py
-drwxr-xr-x   0 apanchal   (501) staff       (20)        0 2019-06-01 04:43:04.000000 dicompyler-core-0.5.5/docs/
--rw-r--r--   0 apanchal   (501) staff       (20)     6975 2016-10-19 21:20:01.000000 dicompyler-core-0.5.5/docs/Makefile
--rw-r--r--   0 apanchal   (501) staff       (20)       28 2016-02-17 23:25:15.000000 dicompyler-core-0.5.5/docs/authors.rst
--rw-r--r--   0 apanchal   (501) staff       (20)     8662 2019-06-01 03:57:29.000000 dicompyler-core-0.5.5/docs/conf.py
--rw-r--r--   0 apanchal   (501) staff       (20)       33 2016-02-17 23:25:23.000000 dicompyler-core-0.5.5/docs/contributing.rst
--rw-r--r--   0 apanchal   (501) staff       (20)      428 2018-04-03 21:07:17.000000 dicompyler-core-0.5.5/docs/dicompylercore.rst
--rw-r--r--   0 apanchal   (501) staff       (20)       29 2016-10-19 21:20:01.000000 dicompyler-core-0.5.5/docs/history.rst
--rw-r--r--   0 apanchal   (501) staff       (20)      552 2018-04-04 02:49:27.000000 dicompyler-core-0.5.5/docs/index.rst
--rw-r--r--   0 apanchal   (501) staff       (20)      249 2019-03-12 04:29:53.000000 dicompyler-core-0.5.5/docs/installation.rst
--rw-r--r--   0 apanchal   (501) staff       (20)     6719 2016-10-19 21:20:01.000000 dicompyler-core-0.5.5/docs/make.bat
--rw-r--r--   0 apanchal   (501) staff       (20)       79 2019-06-01 03:57:51.000000 dicompyler-core-0.5.5/docs/modules.rst
--rw-r--r--   0 apanchal   (501) staff       (20)       28 2016-10-19 21:20:01.000000 dicompyler-core-0.5.5/docs/readme.rst
--rw-r--r--   0 apanchal   (501) staff       (20)     3163 2018-04-03 21:07:17.000000 dicompyler-core-0.5.5/docs/usage.rst
--rw-r--r--   0 apanchal   (501) staff       (20)      133 2019-05-20 15:20:07.000000 dicompyler-core-0.5.5/requirements_dev.txt
--rw-r--r--   0 apanchal   (501) staff       (20)      201 2019-06-01 04:43:04.000000 dicompyler-core-0.5.5/setup.cfg
--rw-r--r--   0 apanchal   (501) staff       (20)     2292 2019-06-01 04:08:35.000000 dicompyler-core-0.5.5/setup.py
-drwxr-xr-x   0 apanchal   (501) staff       (20)        0 2019-06-01 04:43:04.000000 dicompyler-core-0.5.5/tests/
--rw-r--r--   0 apanchal   (501) staff       (20)       25 2016-10-19 21:20:01.000000 dicompyler-core-0.5.5/tests/__init__.py
--rw-r--r--   0 apanchal   (501) staff       (20)    12466 2018-11-19 21:29:21.000000 dicompyler-core-0.5.5/tests/test_dicomparser.py
--rw-r--r--   0 apanchal   (501) staff       (20)     9219 2019-03-12 04:29:53.000000 dicompyler-core-0.5.5/tests/test_dvh.py
--rw-r--r--   0 apanchal   (501) staff       (20)     8004 2019-06-01 03:57:39.000000 dicompyler-core-0.5.5/tests/test_dvhcalc.py
-drwxr-xr-x   0 apanchal   (501) staff       (20)        0 2019-06-01 04:43:04.000000 dicompyler-core-0.5.5/tests/testdata/
-drwxr-xr-x   0 apanchal   (501) staff       (20)        0 2019-06-01 04:43:04.000000 dicompyler-core-0.5.5/tests/testdata/example_data/
--rw-r--r--   0 apanchal   (501) staff       (20)   525682 2016-02-10 21:48:18.000000 dicompyler-core-0.5.5/tests/testdata/example_data/ct.0.dcm
--rw-r--r--   0 apanchal   (501) staff       (20) 10014610 2010-07-10 03:31:42.000000 dicompyler-core-0.5.5/tests/testdata/example_data/rtdose.dcm
--rw-r--r--   0 apanchal   (501) staff       (20)   305836 2010-07-10 03:31:42.000000 dicompyler-core-0.5.5/tests/testdata/example_data/rtplan.dcm
--rw-r--r--   0 apanchal   (501) staff       (20)  1940626 2010-07-10 03:31:42.000000 dicompyler-core-0.5.5/tests/testdata/example_data/rtss.dcm
--rw-r--r--   0 apanchal   (501) staff       (20)      396 2019-06-01 04:08:30.000000 dicompyler-core-0.5.5/tox.ini
+drwxr-xr-x   0 apanchal   (501) staff       (20)        0 2023-05-08 15:58:56.226852 dicompyler-core-0.5.6/
+-rw-r--r--   0 apanchal   (501) staff       (20)      309 2016-02-11 21:58:32.000000 dicompyler-core-0.5.6/.coveragerc
+-rw-r--r--   0 apanchal   (501) staff       (20)      201 2023-05-08 04:58:12.000000 dicompyler-core-0.5.6/AUTHORS.rst
+-rw-r--r--   0 apanchal   (501) staff       (20)     3217 2022-10-22 04:48:06.000000 dicompyler-core-0.5.6/CONTRIBUTING.rst
+-rw-r--r--   0 apanchal   (501) staff       (20)     5338 2023-05-08 14:32:58.000000 dicompyler-core-0.5.6/HISTORY.rst
+-rw-r--r--   0 apanchal   (501) staff       (20)     1506 2023-05-08 05:06:30.000000 dicompyler-core-0.5.6/LICENSE
+-rw-r--r--   0 apanchal   (501) staff       (20)      357 2016-02-17 23:25:10.000000 dicompyler-core-0.5.6/MANIFEST.in
+-rw-r--r--   0 apanchal   (501) staff       (20)     2127 2022-04-22 15:40:05.000000 dicompyler-core-0.5.6/Makefile
+-rw-r--r--   0 apanchal   (501) staff       (20)     5747 2023-05-08 15:58:56.227019 dicompyler-core-0.5.6/PKG-INFO
+-rw-r--r--   0 apanchal   (501) staff       (20)     4592 2023-05-06 04:24:32.000000 dicompyler-core-0.5.6/README.rst
+drwxr-xr-x   0 apanchal   (501) staff       (20)        0 2023-05-08 15:58:56.197733 dicompyler-core-0.5.6/dicompyler_core.egg-info/
+-rw-r--r--   0 apanchal   (501) staff       (20)     5747 2023-05-08 15:58:56.000000 dicompyler-core-0.5.6/dicompyler_core.egg-info/PKG-INFO
+-rw-r--r--   0 apanchal   (501) staff       (20)     1081 2023-05-08 15:58:56.000000 dicompyler-core-0.5.6/dicompyler_core.egg-info/SOURCES.txt
+-rw-r--r--   0 apanchal   (501) staff       (20)        1 2023-05-08 15:58:56.000000 dicompyler-core-0.5.6/dicompyler_core.egg-info/dependency_links.txt
+-rw-r--r--   0 apanchal   (501) staff       (20)        1 2023-05-08 15:58:56.000000 dicompyler-core-0.5.6/dicompyler_core.egg-info/not-zip-safe
+-rw-r--r--   0 apanchal   (501) staff       (20)      157 2023-05-08 15:58:56.000000 dicompyler-core-0.5.6/dicompyler_core.egg-info/requires.txt
+-rw-r--r--   0 apanchal   (501) staff       (20)       15 2023-05-08 15:58:56.000000 dicompyler-core-0.5.6/dicompyler_core.egg-info/top_level.txt
+drwxr-xr-x   0 apanchal   (501) staff       (20)        0 2023-05-08 15:58:56.201588 dicompyler-core-0.5.6/dicompylercore/
+-rw-r--r--   0 apanchal   (501) staff       (20)      483 2023-05-08 15:58:52.000000 dicompyler-core-0.5.6/dicompylercore/__init__.py
+-rw-r--r--   0 apanchal   (501) staff       (20)     1695 2021-10-08 03:16:08.000000 dicompyler-core-0.5.6/dicompylercore/config.py
+-rwxr-xr-x   0 apanchal   (501) staff       (20)    41749 2023-05-02 04:32:42.000000 dicompyler-core-0.5.6/dicompylercore/dicomparser.py
+-rw-r--r--   0 apanchal   (501) staff       (20)    17181 2023-05-02 04:20:12.000000 dicompyler-core-0.5.6/dicompylercore/dose.py
+-rw-r--r--   0 apanchal   (501) staff       (20)    21111 2023-05-08 04:03:27.000000 dicompyler-core-0.5.6/dicompylercore/dvh.py
+-rw-r--r--   0 apanchal   (501) staff       (20)    22684 2023-05-02 04:32:42.000000 dicompyler-core-0.5.6/dicompylercore/dvhcalc.py
+-rw-r--r--   0 apanchal   (501) staff       (20)      757 2021-10-04 23:55:53.000000 dicompyler-core-0.5.6/dicompylercore/matplotlibshow2.py
+-rwxr--r--   0 apanchal   (501) staff       (20)     5294 2016-10-19 21:20:01.000000 dicompyler-core-0.5.6/dicompylercore/util.py
+drwxr-xr-x   0 apanchal   (501) staff       (20)        0 2023-05-08 15:58:56.206065 dicompyler-core-0.5.6/docs/
+-rw-r--r--   0 apanchal   (501) staff       (20)     6975 2016-10-19 21:20:01.000000 dicompyler-core-0.5.6/docs/Makefile
+-rw-r--r--   0 apanchal   (501) staff       (20)       28 2016-02-17 23:25:15.000000 dicompyler-core-0.5.6/docs/authors.rst
+-rw-r--r--   0 apanchal   (501) staff       (20)     8803 2023-05-08 05:02:29.000000 dicompyler-core-0.5.6/docs/conf.py
+-rw-r--r--   0 apanchal   (501) staff       (20)       33 2016-02-17 23:25:23.000000 dicompyler-core-0.5.6/docs/contributing.rst
+-rw-r--r--   0 apanchal   (501) staff       (20)      565 2021-10-08 03:16:08.000000 dicompyler-core-0.5.6/docs/dicompylercore.rst
+-rw-r--r--   0 apanchal   (501) staff       (20)       29 2016-10-19 21:20:01.000000 dicompyler-core-0.5.6/docs/history.rst
+-rw-r--r--   0 apanchal   (501) staff       (20)      552 2021-10-08 03:16:08.000000 dicompyler-core-0.5.6/docs/index.rst
+-rw-r--r--   0 apanchal   (501) staff       (20)      249 2021-10-08 03:16:08.000000 dicompyler-core-0.5.6/docs/installation.rst
+-rw-r--r--   0 apanchal   (501) staff       (20)     6719 2016-10-19 21:20:01.000000 dicompyler-core-0.5.6/docs/make.bat
+-rw-r--r--   0 apanchal   (501) staff       (20)       79 2023-05-08 14:32:59.000000 dicompyler-core-0.5.6/docs/modules.rst
+-rw-r--r--   0 apanchal   (501) staff       (20)       28 2016-10-19 21:20:01.000000 dicompyler-core-0.5.6/docs/readme.rst
+-rw-r--r--   0 apanchal   (501) staff       (20)     4138 2021-10-08 03:16:08.000000 dicompyler-core-0.5.6/docs/usage.rst
+-rw-r--r--   0 apanchal   (501) staff       (20)      133 2023-05-06 04:24:32.000000 dicompyler-core-0.5.6/requirements_dev.txt
+-rw-r--r--   0 apanchal   (501) staff       (20)      201 2023-05-08 15:58:56.227402 dicompyler-core-0.5.6/setup.cfg
+-rw-r--r--   0 apanchal   (501) staff       (20)     2180 2023-05-08 15:58:52.000000 dicompyler-core-0.5.6/setup.py
+drwxr-xr-x   0 apanchal   (501) staff       (20)        0 2023-05-08 15:58:56.207811 dicompyler-core-0.5.6/tests/
+-rw-r--r--   0 apanchal   (501) staff       (20)       25 2016-10-19 21:20:01.000000 dicompyler-core-0.5.6/tests/__init__.py
+-rw-r--r--   0 apanchal   (501) staff       (20)    24050 2022-04-18 15:32:03.000000 dicompyler-core-0.5.6/tests/decubitus_test.py
+-rw-r--r--   0 apanchal   (501) staff       (20)    13552 2022-05-15 19:22:10.000000 dicompyler-core-0.5.6/tests/test_dicomparser.py
+-rw-r--r--   0 apanchal   (501) staff       (20)    12219 2021-10-08 03:16:08.000000 dicompyler-core-0.5.6/tests/test_dose.py
+-rw-r--r--   0 apanchal   (501) staff       (20)     9780 2023-05-08 04:02:29.000000 dicompyler-core-0.5.6/tests/test_dvh.py
+-rw-r--r--   0 apanchal   (501) staff       (20)    25620 2022-05-15 19:22:10.000000 dicompyler-core-0.5.6/tests/test_dvhcalc.py
+drwxr-xr-x   0 apanchal   (501) staff       (20)        0 2023-05-08 15:58:56.192460 dicompyler-core-0.5.6/tests/testdata/
+drwxr-xr-x   0 apanchal   (501) staff       (20)        0 2023-05-08 15:58:56.222919 dicompyler-core-0.5.6/tests/testdata/example_data/
+-rw-r--r--   0 apanchal   (501) staff       (20)   525682 2016-02-10 21:48:18.000000 dicompyler-core-0.5.6/tests/testdata/example_data/ct.0.dcm
+-rw-r--r--   0 apanchal   (501) staff       (20) 10014610 2010-07-10 03:31:42.000000 dicompyler-core-0.5.6/tests/testdata/example_data/rtdose.dcm
+-rw-r--r--   0 apanchal   (501) staff       (20)   305836 2010-07-10 03:31:42.000000 dicompyler-core-0.5.6/tests/testdata/example_data/rtplan.dcm
+-rw-r--r--   0 apanchal   (501) staff       (20)  1940626 2010-07-10 03:31:42.000000 dicompyler-core-0.5.6/tests/testdata/example_data/rtss.dcm
+-rw-r--r--   0 apanchal   (501) staff       (20)     9179 2022-05-15 19:22:10.000000 dicompyler-core-0.5.6/tests/util.py
+-rw-r--r--   0 apanchal   (501) staff       (20)      406 2023-05-08 05:15:38.000000 dicompyler-core-0.5.6/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dicompyler-core-0.5.5/CONTRIBUTING.rst` & `dicompyler-core-0.5.6/CONTRIBUTING.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,113 +1,112 @@
-.. highlight:: shell
-
-============
-Contributing
-============
-
-Contributions are welcome, and they are greatly appreciated! Every
-little bit helps, and credit will always be given.
-
-You can contribute in many ways:
-
-Types of Contributions
-----------------------
-
-Report Bugs
-~~~~~~~~~~~
-
-Report bugs at https://github.com/dicompyler/dicompyler-core/issues.
-
-If you are reporting a bug, please include:
-
-* Your operating system name and version.
-* Any details about your local setup that might be helpful in troubleshooting.
-* Detailed steps to reproduce the bug.
-
-Fix Bugs
-~~~~~~~~
-
-Look through the GitHub issues for bugs. Anything tagged with "bug"
-is open to whoever wants to implement it.
-
-Implement Features
-~~~~~~~~~~~~~~~~~~
-
-Look through the GitHub issues for features. Anything tagged with "feature"
-is open to whoever wants to implement it.
-
-Write Documentation
-~~~~~~~~~~~~~~~~~~~
-
-dicompyler-core could always use more documentation, whether as part of the
-official dicompyler-core docs, in docstrings, or even on the web in blog posts,
-articles, and such.
-
-Submit Feedback
-~~~~~~~~~~~~~~~
-
-The best way to send feedback is to file an issue at https://github.com/dicompyler/dicompyler-core/issues.
-
-If you are proposing a feature:
-
-* Explain in detail how it would work.
-* Keep the scope as narrow as possible, to make it easier to implement.
-* Remember that this is a volunteer-driven project, and that contributions
-  are welcome :)
-
-Get Started!
-------------
-
-Ready to contribute? Here's how to set up `dicompyler-core` for local development.
-
-1. Fork the `dicompyler-core` repo on GitHub.
-2. Clone your fork locally::
-
-    $ git clone git@github.com:your_name_here/dicompyler-core.git
-
-3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
-
-    $ mkvirtualenv dicompyler-core
-    $ cd dicompyler-core/
-    $ python setup.py develop
-
-4. Create a branch for local development::
-
-    $ git checkout -b name-of-your-bugfix-or-feature
-
-   Now you can make your changes locally.
-
-5. When you're done making changes, check that your changes pass flake8 and the tests, including testing other Python versions with tox::
-
-    $ flake8 dicompyler-core tests
-    $ python setup.py test
-    $ tox
-
-   To get flake8 and tox, just pip install them into your virtualenv.
-
-6. Commit your changes and push your branch to GitHub::
-
-    $ git add .
-    $ git commit -m "Your detailed description of your changes."
-    $ git push origin name-of-your-bugfix-or-feature
-
-7. Submit a pull request through the GitHub website.
-
-Pull Request Guidelines
------------------------
-
-Before you submit a pull request, check that it meets these guidelines:
-
-1. The pull request should include tests.
-2. If the pull request adds functionality, the docs should be updated. Put
-   your new functionality into a function with a docstring, and add the
-   feature to the list in README.rst.
-3. The pull request should work for Python 2.7, 3.5, and 3.6. Check
-   https://travis-ci.org/dicompyler/dicompyler-core/pull_requests
-   and make sure that the tests pass for all supported Python versions.
-
-Tips
-----
-
-To run a subset of tests::
-
-    $ python -m unittest tests.test_dicompyler-core
+.. highlight:: shell
+
+============
+Contributing
+============
+
+Contributions are welcome, and they are greatly appreciated! Every
+little bit helps, and credit will always be given.
+
+You can contribute in many ways:
+
+Types of Contributions
+----------------------
+
+Report Bugs
+~~~~~~~~~~~
+
+Report bugs at https://github.com/dicompyler/dicompyler-core/issues.
+
+If you are reporting a bug, please include:
+
+* Your operating system name and version.
+* Any details about your local setup that might be helpful in troubleshooting.
+* Detailed steps to reproduce the bug.
+
+Fix Bugs
+~~~~~~~~
+
+Look through the GitHub issues for bugs. Anything tagged with "bug"
+is open to whoever wants to implement it.
+
+Implement Features
+~~~~~~~~~~~~~~~~~~
+
+Look through the GitHub issues for features. Anything tagged with "feature"
+is open to whoever wants to implement it.
+
+Write Documentation
+~~~~~~~~~~~~~~~~~~~
+
+dicompyler-core could always use more documentation, whether as part of the
+official dicompyler-core docs, in docstrings, or even on the web in blog posts,
+articles, and such.
+
+Submit Feedback
+~~~~~~~~~~~~~~~
+
+The best way to send feedback is to file an issue at https://github.com/dicompyler/dicompyler-core/issues.
+
+If you are proposing a feature:
+
+* Explain in detail how it would work.
+* Keep the scope as narrow as possible, to make it easier to implement.
+* Remember that this is a volunteer-driven project, and that contributions
+  are welcome :)
+
+Get Started!
+------------
+
+Ready to contribute? Here's how to set up `dicompyler-core` for local development.
+
+1. Fork the `dicompyler-core` repo on GitHub.
+2. Clone your fork locally::
+
+    $ git clone git@github.com:your_name_here/dicompyler-core.git
+
+3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
+
+    $ mkvirtualenv dicompyler-core
+    $ cd dicompyler-core/
+    $ python setup.py develop
+
+4. Create a branch for local development::
+
+    $ git checkout -b name-of-your-bugfix-or-feature
+
+   Now you can make your changes locally.
+
+5. When you're done making changes, check that your changes pass flake8 and the tests, including testing other Python versions with tox::
+
+    $ flake8 dicompyler-core tests
+    $ python -m unittest discover -v
+    $ tox
+
+   To get flake8 and tox, just pip install them into your virtualenv.
+
+6. Commit your changes and push your branch to GitHub::
+
+    $ git add .
+    $ git commit -m "Your detailed description of your changes."
+    $ git push origin name-of-your-bugfix-or-feature
+
+7. Submit a pull request through the GitHub website.
+
+Pull Request Guidelines
+-----------------------
+
+Before you submit a pull request, check that it meets these guidelines:
+
+1. The pull request should include tests.
+2. If the pull request adds functionality, the docs should be updated. Put
+   your new functionality into a function with a docstring, and add the
+   feature to the list in `README.rst`.
+3. The pull request should work for Python versions listed in `README.rst`. Check
+   that your pull request passes for all supported Python versions.
+
+Tips
+----
+
+To run a subset of tests::
+
+    $ python -m unittest tests.test_dicompyler-core
```

### Comparing `dicompyler-core-0.5.5/LICENSE` & `dicompyler-core-0.5.6/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Copyright (c) 2009-2016 Aditya Panchal and dicompyler-core contributors
-
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are
-met:
-
-    Redistributions of source code must retain the above copyright
-    notice, this list of conditions and the following disclaimer.
-
-    Redistributions in binary form must reproduce the above copyright
-    notice, this list of conditions and the following disclaimer in the
-    documentation and/or other materials provided with the
-    distribution.
-
-    The name of Aditya Panchal may not be used to endorse or promote
-    products derived from this software without specific prior written
-    permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
-PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER
-OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
-EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
-PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
-PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
-LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
-NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Copyright (c) 2009-2023 Aditya Panchal and dicompyler-core contributors
+
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are
+met:
+
+    Redistributions of source code must retain the above copyright
+    notice, this list of conditions and the following disclaimer.
+
+    Redistributions in binary form must reproduce the above copyright
+    notice, this list of conditions and the following disclaimer in the
+    documentation and/or other materials provided with the
+    distribution.
+
+    The name of Aditya Panchal may not be used to endorse or promote
+    products derived from this software without specific prior written
+    permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
+PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER
+OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
+EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
+PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
+PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
+LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
+NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `dicompyler-core-0.5.5/Makefile` & `dicompyler-core-0.5.6/Makefile`

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,84 @@
-.PHONY: clean-pyc clean-build docs clean
-define BROWSER_PYSCRIPT
-import os, webbrowser, sys
-try:
-	from urllib import pathname2url
-except:
-	from urllib.request import pathname2url
-
-webbrowser.open("file://" + pathname2url(os.path.abspath(sys.argv[1])))
-endef
-export BROWSER_PYSCRIPT
-BROWSER := python -c "$$BROWSER_PYSCRIPT"
-
-help:
-	@echo "clean - remove all build, test, coverage and Python artifacts"
-	@echo "clean-build - remove build artifacts"
-	@echo "clean-pyc - remove Python file artifacts"
-	@echo "clean-test - remove test and coverage artifacts"
-	@echo "lint - check style with flake8"
-	@echo "test - run tests quickly with the default Python"
-	@echo "test-all - run tests on every Python version with tox"
-	@echo "coverage - check code coverage quickly with the default Python"
-	@echo "docs - generate Sphinx HTML documentation, including API docs"
-	@echo "release - package and upload a release"
-	@echo "dist - package"
-	@echo "install - install the package to the active Python's site-packages"
-
-clean: clean-build clean-pyc clean-test
-
-clean-build:
-	rm -fr build/
-	rm -fr dist/
-	rm -fr .eggs/
-	find . -name '*.egg-info' -exec rm -fr {} +
-	find . -name '*.egg' -exec rm -f {} +
-
-clean-pyc:
-	find . -name '*.pyc' -exec rm -f {} +
-	find . -name '*.pyo' -exec rm -f {} +
-	find . -name '*~' -exec rm -f {} +
-	find . -name '__pycache__' -exec rm -fr {} +
-
-clean-test:
-	rm -fr .tox/
-	rm -f .coverage
-	rm -fr htmlcov/
-
-lint:
-	flake8 dicompylercore tests
-
-test:
-	python setup.py test
-
-test-all:
-	tox
-
-coverage:
-	coverage run --source dicompylercore setup.py test
-	coverage report -m
-	coverage html
-	$(BROWSER) htmlcov/index.html
-
-docs:
-	rm -f docs/dicompyler-core.rst
-	rm -f docs/modules.rst
-	sphinx-apidoc -o docs/ dicompylercore
-	$(MAKE) -C docs clean
-	$(MAKE) -C docs html
-	$(BROWSER) docs/_build/html/index.html
-
-servedocs: docs
-	watchmedo shell-command -p '*.rst' -c '$(MAKE) -C docs html' -R -D .
-
-uploadrelease: dist
-	twine upload --verbose dist/*
-
-uploadtestrelease: dist
-	twine upload --verbose --repository-url https://test.pypi.org/legacy/ dist/*
-
-installtestrelease:
-	pip uninstall dicompyler-core
-	pip install --index-url https://test.pypi.org/simple/ --no-deps dicompyler-core
-
-dist: clean
-	python setup.py sdist
-	python setup.py bdist_wheel
-	ls -l dist
-
-install: clean
-	python setup.py install
+.PHONY: clean-pyc clean-build docs clean
+define BROWSER_PYSCRIPT
+import os, webbrowser, sys
+try:
+	from urllib import pathname2url
+except:
+	from urllib.request import pathname2url
+
+webbrowser.open("file://" + pathname2url(os.path.abspath(sys.argv[1])))
+endef
+export BROWSER_PYSCRIPT
+BROWSER := python -c "$$BROWSER_PYSCRIPT"
+
+help:
+	@echo "clean - remove all build, test, coverage and Python artifacts"
+	@echo "clean-build - remove build artifacts"
+	@echo "clean-pyc - remove Python file artifacts"
+	@echo "clean-test - remove test and coverage artifacts"
+	@echo "lint - check style with flake8"
+	@echo "test - run tests quickly with the default Python"
+	@echo "test-all - run tests on every Python version with tox"
+	@echo "coverage - check code coverage quickly with the default Python"
+	@echo "docs - generate Sphinx HTML documentation, including API docs"
+	@echo "release - package and upload a release"
+	@echo "dist - package"
+	@echo "install - install the package to the active Python's site-packages"
+
+clean: clean-build clean-pyc clean-test
+
+clean-build:
+	rm -fr build/
+	rm -fr dist/
+	rm -fr .eggs/
+	find . -name '*.egg-info' -exec rm -fr {} +
+	find . -name '*.egg' -exec rm -f {} +
+
+clean-pyc:
+	find . -name '*.pyc' -exec rm -f {} +
+	find . -name '*.pyo' -exec rm -f {} +
+	find . -name '*~' -exec rm -f {} +
+	find . -name '__pycache__' -exec rm -fr {} +
+
+clean-test:
+	rm -fr .tox/
+	rm -f .coverage
+	rm -fr htmlcov/
+
+lint:
+	flake8 dicompylercore tests
+
+test:
+	python -m unittest discover -v
+
+test-all:
+	tox
+
+coverage:
+	coverage run --source dicompylercore -m unittest discover -v
+	coverage report -m
+	coverage html
+	$(BROWSER) htmlcov/index.html
+
+docs:
+	rm -f docs/dicompyler-core.rst
+	rm -f docs/modules.rst
+	sphinx-apidoc -o docs/ dicompylercore
+	$(MAKE) -C docs clean
+	$(MAKE) -C docs html
+	$(BROWSER) docs/_build/html/index.html
+
+servedocs: docs
+	watchmedo shell-command -p '*.rst' -c '$(MAKE) -C docs html' -R -D .
+
+release: clean
+	python setup.py sdist upload
+	python setup.py bdist_wheel upload
+
+dist: clean
+	python setup.py sdist
+	python setup.py bdist_wheel
+	ls -l dist
+
+install: clean
+	python setup.py install
```

### Comparing `dicompyler-core-0.5.5/PKG-INFO` & `dicompyler-core-0.5.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,126 +1,135 @@
 Metadata-Version: 2.1
 Name: dicompyler-core
-Version: 0.5.5
+Version: 0.5.6
 Summary: A library of core radiation therapy modules for DICOM / DICOM RT used by dicompyler
 Home-page: https://github.com/dicompyler/dicompyler-core
 Author: Aditya Panchal
 Author-email: apanchal@bastula.org
 License: BSD License
-Description: dicompyler-core
-        ===============
-        
-        |Binder| |pypi| |travis-ci| |coveralls| |Codacy| |Codecov| |Documentation Status| |Zenodo|
-        
-        A library of core radiation therapy modules for DICOM / DICOM RT used by `dicompyler <http://www.dicompyler.com>`__. This
-        package includes:
-        
-        -  ``dicomparser``: parse DICOM objects in an easy-to-use manner
-        -  ``dvh``: Pythonic access to dose volume histogram (DVH) data
-        -  ``dvhcalc``: Independent DVH calculation using DICOM RT Dose & RT Structure Set
-        
-        Other information
-        -----------------
-        
-        -  Free software: `BSD license <https://github.com/dicompyler/dicompyler-core/blob/master/LICENSE>`__
-        -  Documentation: `Read the docs <https://dicompyler-core.readthedocs.io>`__
-        -  Tested on Python 2.7, 3.5, 3.6
-        
-        Dependencies
-        ------------
-        
-        -  `numpy <http://www.numpy.org>`__ 1.2 or higher
-        -  `pydicom <https://pydicom.github.io>`__ 0.9.9 or higher (pydicom 1.0 compatible)
-        -  `matplotlib <http://matplotlib.org>`__ 1.3.0 or higher (for DVH calculation)
-        -  `six <https://pythonhosted.org/six/>`__ 1.5 or higher
-        -  Optional:
-        
-           -  `Pillow <https://pillow.readthedocs.io>`__ (for image display)
-           -  `Shapely <https://github.com/Toblerity/Shapely>`__ (for structure volume calculation)
-           -  `scikit-image <http://scikit-image.org/>`__ (for DVH interpolation)
-        
-        Basic Usage
-        ------------
-        
-        .. code-block:: python
-        
-            from dicompylercore import dicomparser, dvh, dvhcalc
-            dp = dicomparser.DicomParser("rtss.dcm")
-        
-            # i.e. Get a dict of structure information
-            structures = dp.GetStructures()
-        
-            >>> structures[5]
-            {'color': array([255, 128, 0]), 'type': 'ORGAN', 'id': 5, 'empty': False, 'name': 'Heart'}
-        
-            # Access DVH data
-            rtdose = dicomparser.DicomParser("rtdose.dcm")
-            heartdvh = dvh.DVH.from_dicom_dvh(rtdose.ds, 5)
-        
-            >>> heartdvh.describe()
-            Structure: Heart
-            DVH Type:  cumulative, abs dose: Gy, abs volume: cm3
-            Volume:    437.46 cm3
-            Max Dose:  3.10 Gy
-            Min Dose:  0.02 Gy
-            Mean Dose: 0.64 Gy
-            D100:      0.00 Gy
-            D98:       0.03 Gy
-            D95:       0.03 Gy
-            D2cc:      2.93 Gy
-        
-            # Calculate a DVH from DICOM RT data
-            calcdvh = dvhcalc.get_dvh("rtss.dcm", "rtdose.dcm", 5)
-        
-            >>> calcdvh.max, calcdvh.min, calcdvh.D2cc
-            (3.0899999999999999, 0.029999999999999999, dvh.DVHValue(2.96, 'Gy'))
-        
-        Advanced Usage and Examples can be found in Binder: |Binder|
-        
-        Citing dicompyler-core
-        ----------------------
-        A DOI for dicompyler-core with various citation styles can be found at Zenodo: |Zenodo|
-        
-        
-        Credits
-        -------
-        
-        This package was created with
-        `Cookiecutter <https://github.com/audreyr/cookiecutter>`__ and the
-        `audreyr/cookiecutter-pypackage <https://github.com/audreyr/cookiecutter-pypackage>`__ project template.
-        
-        .. |Binder| image:: http://mybinder.org/badge.svg
-           :target: http://mybinder.org/repo/bastula/dicom-notebooks
-        .. |pypi| image:: https://img.shields.io/pypi/v/dicompyler-core.svg
-           :target: https://pypi.python.org/pypi/dicompyler-core
-        .. |travis-ci| image:: https://img.shields.io/travis/dicompyler/dicompyler-core.svg
-           :target: https://travis-ci.org/dicompyler/dicompyler-core
-        .. |coveralls| image:: https://coveralls.io/repos/github/dicompyler/dicompyler-core/badge.svg?branch=master
-           :target: https://coveralls.io/github/dicompyler/dicompyler-core?branch=master
-        .. |Codacy| image:: https://api.codacy.com/project/badge/Grade/39060fc468844402a4030715fe01bb15
-           :target: https://www.codacy.com/app/bastula/dicompyler-core?utm_campaign=Badge_Coverage
-        .. |Codecov| image:: https://codecov.io/gh/dicompyler/dicompyler-core/branch/master/graph/badge.svg
-           :target: https://codecov.io/gh/dicompyler/dicompyler-core
-        .. |Documentation Status| image:: https://readthedocs.org/projects/dicompyler-core/badge/?version=latest
-           :target: https://dicompyler-core.readthedocs.io/en/latest/
-        .. |Zenodo| image:: https://zenodo.org/badge/51550203.svg
-           :target: https://zenodo.org/badge/latestdoi/51550203
-        
 Keywords: dicompyler-core,dicompylercore,dicompyler
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Physics
-Provides-Extra: dvhinterpolation
 Provides-Extra: image
+Provides-Extra: dvhinterpolation
 Provides-Extra: volume
+Provides-Extra: doseinterpolation
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+dicompyler-core
+===============
+
+|Binder| |pypi| |Python Version| |GH Actions| |Documentation Status| |coveralls| |Codacy| |Codecov| |Total Lines| |Code Size| |Zenodo|
+
+A library of core radiation therapy modules for DICOM / DICOM RT used by `dicompyler <http://www.dicompyler.com>`__. This
+package includes:
+
+-  ``dicomparser``: parse DICOM objects in an easy-to-use manner
+-  ``dvh``: Pythonic access to dose volume histogram (DVH) data
+-  ``dvhcalc``: Independent DVH calculation using DICOM RT Dose & RT Structure Set
+-  ``dose``: Pythonic access to RT Dose data including dose summation
+
+Other information
+-----------------
+
+-  Free software: `BSD license <https://github.com/dicompyler/dicompyler-core/blob/master/LICENSE>`__
+-  Documentation: `Read the docs <https://dicompyler-core.readthedocs.io>`__
+-  Tested on Python 3.7+
+
+Dependencies
+------------
+
+-  `numpy <http://www.numpy.org>`__ 1.2 or higher
+-  `pydicom <https://pydicom.github.io>`__ 0.9.9 or higher (pydicom 1.0 compatible)
+-  `matplotlib <http://matplotlib.org>`__ 1.3.0 or higher (for DVH calculation)
+-  `six <https://pythonhosted.org/six/>`__ 1.5 or higher
+-  Optional:
+
+   -  `Pillow <https://pillow.readthedocs.io>`__ (for image display)
+   -  `Shapely <https://github.com/Toblerity/Shapely>`__ (for structure volume calculation)
+   -  `scikit-image <http://scikit-image.org/>`__ (for DVH interpolation)
+   -  `scipy <https://scipy.org/>`__ (for dose grid summation using interpolation)
+
+Basic Usage
+------------
+
+.. code-block:: python
+
+    from dicompylercore import dicomparser, dvh, dvhcalc
+    dp = dicomparser.DicomParser("rtss.dcm")
+
+    # i.e. Get a dict of structure information
+    structures = dp.GetStructures()
+
+    >>> structures[5]
+    {'color': array([255, 128, 0]), 'type': 'ORGAN', 'id': 5, 'empty': False, 'name': 'Heart'}
+
+    # Access DVH data
+    rtdose = dicomparser.DicomParser("rtdose.dcm")
+    heartdvh = dvh.DVH.from_dicom_dvh(rtdose.ds, 5)
+
+    >>> heartdvh.describe()
+    Structure: Heart
+    DVH Type:  cumulative, abs dose: Gy, abs volume: cm3
+    Volume:    437.46 cm3
+    Max Dose:  3.10 Gy
+    Min Dose:  0.02 Gy
+    Mean Dose: 0.64 Gy
+    D100:      0.00 Gy
+    D98:       0.03 Gy
+    D95:       0.03 Gy
+    D2cc:      2.93 Gy
+
+    # Calculate a DVH from DICOM RT data
+    calcdvh = dvhcalc.get_dvh("rtss.dcm", "rtdose.dcm", 5)
+
+    >>> calcdvh.max, calcdvh.min, calcdvh.D2cc
+    (3.0899999999999999, 0.029999999999999999, dvh.DVHValue(2.96, 'Gy'))
+
+Advanced Usage and Examples can be found in Binder: |Binder|
+
+Citing dicompyler-core
+----------------------
+A DOI for dicompyler-core with various citation styles can be found at Zenodo: |Zenodo|
+
+
+Credits
+-------
+
+This package was created with
+`Cookiecutter <https://github.com/audreyr/cookiecutter>`__ and the
+`audreyr/cookiecutter-pypackage <https://github.com/audreyr/cookiecutter-pypackage>`__ project template.
+
+.. |Binder| image:: http://mybinder.org/badge.svg
+   :target: http://mybinder.org/repo/bastula/dicom-notebooks
+.. |pypi| image:: https://img.shields.io/pypi/v/dicompyler-core.svg
+   :target: https://pypi.python.org/pypi/dicompyler-core
+.. |Python Version| image:: https://img.shields.io/badge/python-3.7+-blue.svg
+   :target: https://pypi.python.org/pypi/dicompyler-core
+.. |GH Actions| image:: https://github.com/dicompyler/dicompyler-core/actions/workflows/build.yml/badge.svg
+   :target: https://github.com/dicompyler/dicompyler-core/actions
+.. |Documentation Status| image:: https://readthedocs.org/projects/dicompyler-core/badge/?version=latest
+   :target: https://dicompyler-core.readthedocs.io/en/latest/
+.. |coveralls| image:: https://coveralls.io/repos/github/dicompyler/dicompyler-core/badge.svg?branch=master
+   :target: https://coveralls.io/github/dicompyler/dicompyler-core?branch=master
+.. |Codacy| image:: https://api.codacy.com/project/badge/Grade/27ebb3802baf4d96b0783a2ae5904264
+   :target: https://app.codacy.com/gh/dicompyler/dicompyler-core/dashboard
+.. |Codecov| image:: https://codecov.io/gh/dicompyler/dicompyler-core/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/dicompyler/dicompyler-core
+.. |Total Lines| image:: https://img.shields.io/tokei/lines/github/dicompyler/dicompyler-core
+   :target: https://img.shields.io/tokei/lines/github/dicompyler/dicompyler-core
+.. |Code Size| image:: https://img.shields.io/github/languages/code-size/dicompyler/dicompyler-core
+   :target: https://img.shields.io/github/languages/code-size/dicompyler/dicompyler-core
+.. |Zenodo| image:: https://zenodo.org/badge/51550203.svg
+   :target: https://zenodo.org/badge/latestdoi/51550203
```

### Comparing `dicompyler-core-0.5.5/README.rst` & `dicompyler-core-0.5.6/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 dicompyler-core
 ===============
 
-|Binder| |pypi| |travis-ci| |coveralls| |Codacy| |Codecov| |Documentation Status| |Zenodo|
+|Binder| |pypi| |Python Version| |GH Actions| |Documentation Status| |coveralls| |Codacy| |Codecov| |Total Lines| |Code Size| |Zenodo|
 
 A library of core radiation therapy modules for DICOM / DICOM RT used by `dicompyler <http://www.dicompyler.com>`__. This
 package includes:
 
 -  ``dicomparser``: parse DICOM objects in an easy-to-use manner
 -  ``dvh``: Pythonic access to dose volume histogram (DVH) data
 -  ``dvhcalc``: Independent DVH calculation using DICOM RT Dose & RT Structure Set
+-  ``dose``: Pythonic access to RT Dose data including dose summation
 
 Other information
 -----------------
 
 -  Free software: `BSD license <https://github.com/dicompyler/dicompyler-core/blob/master/LICENSE>`__
 -  Documentation: `Read the docs <https://dicompyler-core.readthedocs.io>`__
--  Tested on Python 2.7, 3.5, 3.6
+-  Tested on Python 3.7+
 
 Dependencies
 ------------
 
 -  `numpy <http://www.numpy.org>`__ 1.2 or higher
 -  `pydicom <https://pydicom.github.io>`__ 0.9.9 or higher (pydicom 1.0 compatible)
 -  `matplotlib <http://matplotlib.org>`__ 1.3.0 or higher (for DVH calculation)
 -  `six <https://pythonhosted.org/six/>`__ 1.5 or higher
 -  Optional:
 
    -  `Pillow <https://pillow.readthedocs.io>`__ (for image display)
    -  `Shapely <https://github.com/Toblerity/Shapely>`__ (for structure volume calculation)
    -  `scikit-image <http://scikit-image.org/>`__ (for DVH interpolation)
+   -  `scipy <https://scipy.org/>`__ (for dose grid summation using interpolation)
 
 Basic Usage
 ------------
 
 .. code-block:: python
 
     from dicompylercore import dicomparser, dvh, dvhcalc
@@ -80,19 +82,25 @@
 `Cookiecutter <https://github.com/audreyr/cookiecutter>`__ and the
 `audreyr/cookiecutter-pypackage <https://github.com/audreyr/cookiecutter-pypackage>`__ project template.
 
 .. |Binder| image:: http://mybinder.org/badge.svg
    :target: http://mybinder.org/repo/bastula/dicom-notebooks
 .. |pypi| image:: https://img.shields.io/pypi/v/dicompyler-core.svg
    :target: https://pypi.python.org/pypi/dicompyler-core
-.. |travis-ci| image:: https://img.shields.io/travis/dicompyler/dicompyler-core.svg
-   :target: https://travis-ci.org/dicompyler/dicompyler-core
+.. |Python Version| image:: https://img.shields.io/badge/python-3.7+-blue.svg
+   :target: https://pypi.python.org/pypi/dicompyler-core
+.. |GH Actions| image:: https://github.com/dicompyler/dicompyler-core/actions/workflows/build.yml/badge.svg
+   :target: https://github.com/dicompyler/dicompyler-core/actions
+.. |Documentation Status| image:: https://readthedocs.org/projects/dicompyler-core/badge/?version=latest
+   :target: https://dicompyler-core.readthedocs.io/en/latest/
 .. |coveralls| image:: https://coveralls.io/repos/github/dicompyler/dicompyler-core/badge.svg?branch=master
    :target: https://coveralls.io/github/dicompyler/dicompyler-core?branch=master
-.. |Codacy| image:: https://api.codacy.com/project/badge/Grade/39060fc468844402a4030715fe01bb15
-   :target: https://www.codacy.com/app/bastula/dicompyler-core?utm_campaign=Badge_Coverage
+.. |Codacy| image:: https://api.codacy.com/project/badge/Grade/27ebb3802baf4d96b0783a2ae5904264
+   :target: https://app.codacy.com/gh/dicompyler/dicompyler-core/dashboard
 .. |Codecov| image:: https://codecov.io/gh/dicompyler/dicompyler-core/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/dicompyler/dicompyler-core
-.. |Documentation Status| image:: https://readthedocs.org/projects/dicompyler-core/badge/?version=latest
-   :target: https://dicompyler-core.readthedocs.io/en/latest/
+.. |Total Lines| image:: https://img.shields.io/tokei/lines/github/dicompyler/dicompyler-core
+   :target: https://img.shields.io/tokei/lines/github/dicompyler/dicompyler-core
+.. |Code Size| image:: https://img.shields.io/github/languages/code-size/dicompyler/dicompyler-core
+   :target: https://img.shields.io/github/languages/code-size/dicompyler/dicompyler-core
 .. |Zenodo| image:: https://zenodo.org/badge/51550203.svg
    :target: https://zenodo.org/badge/latestdoi/51550203
```

### Comparing `dicompyler-core-0.5.5/dicompyler_core.egg-info/PKG-INFO` & `dicompyler-core-0.5.6/dicompyler_core.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,126 +1,135 @@
 Metadata-Version: 2.1
 Name: dicompyler-core
-Version: 0.5.5
+Version: 0.5.6
 Summary: A library of core radiation therapy modules for DICOM / DICOM RT used by dicompyler
 Home-page: https://github.com/dicompyler/dicompyler-core
 Author: Aditya Panchal
 Author-email: apanchal@bastula.org
 License: BSD License
-Description: dicompyler-core
-        ===============
-        
-        |Binder| |pypi| |travis-ci| |coveralls| |Codacy| |Codecov| |Documentation Status| |Zenodo|
-        
-        A library of core radiation therapy modules for DICOM / DICOM RT used by `dicompyler <http://www.dicompyler.com>`__. This
-        package includes:
-        
-        -  ``dicomparser``: parse DICOM objects in an easy-to-use manner
-        -  ``dvh``: Pythonic access to dose volume histogram (DVH) data
-        -  ``dvhcalc``: Independent DVH calculation using DICOM RT Dose & RT Structure Set
-        
-        Other information
-        -----------------
-        
-        -  Free software: `BSD license <https://github.com/dicompyler/dicompyler-core/blob/master/LICENSE>`__
-        -  Documentation: `Read the docs <https://dicompyler-core.readthedocs.io>`__
-        -  Tested on Python 2.7, 3.5, 3.6
-        
-        Dependencies
-        ------------
-        
-        -  `numpy <http://www.numpy.org>`__ 1.2 or higher
-        -  `pydicom <https://pydicom.github.io>`__ 0.9.9 or higher (pydicom 1.0 compatible)
-        -  `matplotlib <http://matplotlib.org>`__ 1.3.0 or higher (for DVH calculation)
-        -  `six <https://pythonhosted.org/six/>`__ 1.5 or higher
-        -  Optional:
-        
-           -  `Pillow <https://pillow.readthedocs.io>`__ (for image display)
-           -  `Shapely <https://github.com/Toblerity/Shapely>`__ (for structure volume calculation)
-           -  `scikit-image <http://scikit-image.org/>`__ (for DVH interpolation)
-        
-        Basic Usage
-        ------------
-        
-        .. code-block:: python
-        
-            from dicompylercore import dicomparser, dvh, dvhcalc
-            dp = dicomparser.DicomParser("rtss.dcm")
-        
-            # i.e. Get a dict of structure information
-            structures = dp.GetStructures()
-        
-            >>> structures[5]
-            {'color': array([255, 128, 0]), 'type': 'ORGAN', 'id': 5, 'empty': False, 'name': 'Heart'}
-        
-            # Access DVH data
-            rtdose = dicomparser.DicomParser("rtdose.dcm")
-            heartdvh = dvh.DVH.from_dicom_dvh(rtdose.ds, 5)
-        
-            >>> heartdvh.describe()
-            Structure: Heart
-            DVH Type:  cumulative, abs dose: Gy, abs volume: cm3
-            Volume:    437.46 cm3
-            Max Dose:  3.10 Gy
-            Min Dose:  0.02 Gy
-            Mean Dose: 0.64 Gy
-            D100:      0.00 Gy
-            D98:       0.03 Gy
-            D95:       0.03 Gy
-            D2cc:      2.93 Gy
-        
-            # Calculate a DVH from DICOM RT data
-            calcdvh = dvhcalc.get_dvh("rtss.dcm", "rtdose.dcm", 5)
-        
-            >>> calcdvh.max, calcdvh.min, calcdvh.D2cc
-            (3.0899999999999999, 0.029999999999999999, dvh.DVHValue(2.96, 'Gy'))
-        
-        Advanced Usage and Examples can be found in Binder: |Binder|
-        
-        Citing dicompyler-core
-        ----------------------
-        A DOI for dicompyler-core with various citation styles can be found at Zenodo: |Zenodo|
-        
-        
-        Credits
-        -------
-        
-        This package was created with
-        `Cookiecutter <https://github.com/audreyr/cookiecutter>`__ and the
-        `audreyr/cookiecutter-pypackage <https://github.com/audreyr/cookiecutter-pypackage>`__ project template.
-        
-        .. |Binder| image:: http://mybinder.org/badge.svg
-           :target: http://mybinder.org/repo/bastula/dicom-notebooks
-        .. |pypi| image:: https://img.shields.io/pypi/v/dicompyler-core.svg
-           :target: https://pypi.python.org/pypi/dicompyler-core
-        .. |travis-ci| image:: https://img.shields.io/travis/dicompyler/dicompyler-core.svg
-           :target: https://travis-ci.org/dicompyler/dicompyler-core
-        .. |coveralls| image:: https://coveralls.io/repos/github/dicompyler/dicompyler-core/badge.svg?branch=master
-           :target: https://coveralls.io/github/dicompyler/dicompyler-core?branch=master
-        .. |Codacy| image:: https://api.codacy.com/project/badge/Grade/39060fc468844402a4030715fe01bb15
-           :target: https://www.codacy.com/app/bastula/dicompyler-core?utm_campaign=Badge_Coverage
-        .. |Codecov| image:: https://codecov.io/gh/dicompyler/dicompyler-core/branch/master/graph/badge.svg
-           :target: https://codecov.io/gh/dicompyler/dicompyler-core
-        .. |Documentation Status| image:: https://readthedocs.org/projects/dicompyler-core/badge/?version=latest
-           :target: https://dicompyler-core.readthedocs.io/en/latest/
-        .. |Zenodo| image:: https://zenodo.org/badge/51550203.svg
-           :target: https://zenodo.org/badge/latestdoi/51550203
-        
 Keywords: dicompyler-core,dicompylercore,dicompyler
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Physics
-Provides-Extra: dvhinterpolation
 Provides-Extra: image
+Provides-Extra: dvhinterpolation
 Provides-Extra: volume
+Provides-Extra: doseinterpolation
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+dicompyler-core
+===============
+
+|Binder| |pypi| |Python Version| |GH Actions| |Documentation Status| |coveralls| |Codacy| |Codecov| |Total Lines| |Code Size| |Zenodo|
+
+A library of core radiation therapy modules for DICOM / DICOM RT used by `dicompyler <http://www.dicompyler.com>`__. This
+package includes:
+
+-  ``dicomparser``: parse DICOM objects in an easy-to-use manner
+-  ``dvh``: Pythonic access to dose volume histogram (DVH) data
+-  ``dvhcalc``: Independent DVH calculation using DICOM RT Dose & RT Structure Set
+-  ``dose``: Pythonic access to RT Dose data including dose summation
+
+Other information
+-----------------
+
+-  Free software: `BSD license <https://github.com/dicompyler/dicompyler-core/blob/master/LICENSE>`__
+-  Documentation: `Read the docs <https://dicompyler-core.readthedocs.io>`__
+-  Tested on Python 3.7+
+
+Dependencies
+------------
+
+-  `numpy <http://www.numpy.org>`__ 1.2 or higher
+-  `pydicom <https://pydicom.github.io>`__ 0.9.9 or higher (pydicom 1.0 compatible)
+-  `matplotlib <http://matplotlib.org>`__ 1.3.0 or higher (for DVH calculation)
+-  `six <https://pythonhosted.org/six/>`__ 1.5 or higher
+-  Optional:
+
+   -  `Pillow <https://pillow.readthedocs.io>`__ (for image display)
+   -  `Shapely <https://github.com/Toblerity/Shapely>`__ (for structure volume calculation)
+   -  `scikit-image <http://scikit-image.org/>`__ (for DVH interpolation)
+   -  `scipy <https://scipy.org/>`__ (for dose grid summation using interpolation)
+
+Basic Usage
+------------
+
+.. code-block:: python
+
+    from dicompylercore import dicomparser, dvh, dvhcalc
+    dp = dicomparser.DicomParser("rtss.dcm")
+
+    # i.e. Get a dict of structure information
+    structures = dp.GetStructures()
+
+    >>> structures[5]
+    {'color': array([255, 128, 0]), 'type': 'ORGAN', 'id': 5, 'empty': False, 'name': 'Heart'}
+
+    # Access DVH data
+    rtdose = dicomparser.DicomParser("rtdose.dcm")
+    heartdvh = dvh.DVH.from_dicom_dvh(rtdose.ds, 5)
+
+    >>> heartdvh.describe()
+    Structure: Heart
+    DVH Type:  cumulative, abs dose: Gy, abs volume: cm3
+    Volume:    437.46 cm3
+    Max Dose:  3.10 Gy
+    Min Dose:  0.02 Gy
+    Mean Dose: 0.64 Gy
+    D100:      0.00 Gy
+    D98:       0.03 Gy
+    D95:       0.03 Gy
+    D2cc:      2.93 Gy
+
+    # Calculate a DVH from DICOM RT data
+    calcdvh = dvhcalc.get_dvh("rtss.dcm", "rtdose.dcm", 5)
+
+    >>> calcdvh.max, calcdvh.min, calcdvh.D2cc
+    (3.0899999999999999, 0.029999999999999999, dvh.DVHValue(2.96, 'Gy'))
+
+Advanced Usage and Examples can be found in Binder: |Binder|
+
+Citing dicompyler-core
+----------------------
+A DOI for dicompyler-core with various citation styles can be found at Zenodo: |Zenodo|
+
+
+Credits
+-------
+
+This package was created with
+`Cookiecutter <https://github.com/audreyr/cookiecutter>`__ and the
+`audreyr/cookiecutter-pypackage <https://github.com/audreyr/cookiecutter-pypackage>`__ project template.
+
+.. |Binder| image:: http://mybinder.org/badge.svg
+   :target: http://mybinder.org/repo/bastula/dicom-notebooks
+.. |pypi| image:: https://img.shields.io/pypi/v/dicompyler-core.svg
+   :target: https://pypi.python.org/pypi/dicompyler-core
+.. |Python Version| image:: https://img.shields.io/badge/python-3.7+-blue.svg
+   :target: https://pypi.python.org/pypi/dicompyler-core
+.. |GH Actions| image:: https://github.com/dicompyler/dicompyler-core/actions/workflows/build.yml/badge.svg
+   :target: https://github.com/dicompyler/dicompyler-core/actions
+.. |Documentation Status| image:: https://readthedocs.org/projects/dicompyler-core/badge/?version=latest
+   :target: https://dicompyler-core.readthedocs.io/en/latest/
+.. |coveralls| image:: https://coveralls.io/repos/github/dicompyler/dicompyler-core/badge.svg?branch=master
+   :target: https://coveralls.io/github/dicompyler/dicompyler-core?branch=master
+.. |Codacy| image:: https://api.codacy.com/project/badge/Grade/27ebb3802baf4d96b0783a2ae5904264
+   :target: https://app.codacy.com/gh/dicompyler/dicompyler-core/dashboard
+.. |Codecov| image:: https://codecov.io/gh/dicompyler/dicompyler-core/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/dicompyler/dicompyler-core
+.. |Total Lines| image:: https://img.shields.io/tokei/lines/github/dicompyler/dicompyler-core
+   :target: https://img.shields.io/tokei/lines/github/dicompyler/dicompyler-core
+.. |Code Size| image:: https://img.shields.io/github/languages/code-size/dicompyler/dicompyler-core
+   :target: https://img.shields.io/github/languages/code-size/dicompyler/dicompyler-core
+.. |Zenodo| image:: https://zenodo.org/badge/51550203.svg
+   :target: https://zenodo.org/badge/latestdoi/51550203
```

### Comparing `dicompyler-core-0.5.5/dicompyler_core.egg-info/SOURCES.txt` & `dicompyler-core-0.5.6/dicompyler_core.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -15,30 +15,35 @@
 dicompyler_core.egg-info/dependency_links.txt
 dicompyler_core.egg-info/not-zip-safe
 dicompyler_core.egg-info/requires.txt
 dicompyler_core.egg-info/top_level.txt
 dicompylercore/__init__.py
 dicompylercore/config.py
 dicompylercore/dicomparser.py
+dicompylercore/dose.py
 dicompylercore/dvh.py
 dicompylercore/dvhcalc.py
+dicompylercore/matplotlibshow2.py
 dicompylercore/util.py
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/dicompylercore.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/modules.rst
 docs/readme.rst
 docs/usage.rst
 tests/__init__.py
+tests/decubitus_test.py
 tests/test_dicomparser.py
+tests/test_dose.py
 tests/test_dvh.py
 tests/test_dvhcalc.py
+tests/util.py
 tests/testdata/example_data/ct.0.dcm
 tests/testdata/example_data/rtdose.dcm
 tests/testdata/example_data/rtplan.dcm
 tests/testdata/example_data/rtss.dcm
```

### Comparing `dicompyler-core-0.5.5/dicompylercore/dicomparser.py` & `dicompyler-core-0.5.6/dicompylercore/dicomparser.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 #    available at https://github.com/dicompyler/dicompyler-core/
 
 
 import logging
 import numpy as np
 try:
     from pydicom.dicomio import read_file
-    from pydicom.dataset import Dataset
+    from pydicom.dataset import Dataset, validate_file_meta
+    from pydicom.pixel_data_handlers.util import pixel_dtype
 except ImportError:
     from dicom import read_file
     from dicom.dataset import Dataset
 import random
 from numbers import Number
 from six import PY2, iterkeys, string_types, BytesIO
 from six.moves import range
@@ -27,178 +28,179 @@
 if pil_available:
     from PIL import Image
 if shapely_available:
     from shapely.geometry import Polygon
 
 logger = logging.getLogger('dicompylercore.dicomparser')
 
+
 class DicomParser:
-    """Parses DICOM / DICOM RT files."""
+    """Class to parse DICOM / DICOM RT files."""
 
-    def __init__(self, dataset):
+    def __init__(self, dataset, memmap_pixel_array=False):
+        """Initialize DicomParser from a pydicom Dataset or DICOM file.
 
+        Parameters
+        ----------
+        dataset : pydicom Dataset or filename
+            pydicom dataset object or DICOM file location
+        memmap_pixel_array : bool, optional
+            Enable pixel array access via memory mapping, by default False
+
+        Raises
+        ------
+        AttributeError
+            Raised if SOPClassUID is not present in the pydicom Dataset
+        AttributeError
+            Raised if the DICOM file or pydicom Dataset cannot be read
+        """
+        self.memmap_pixel_array = memmap_pixel_array
         if isinstance(dataset, Dataset):
             self.ds = dataset
         elif isinstance(dataset, (string_types, BytesIO)):
             try:
-                self.ds = \
-                    read_file(dataset, defer_size=100, force=True)
-            except:
+                with open(dataset, "rb") as fp:
+                    self.ds = read_file(fp, defer_size=100, force=True,
+                                        stop_before_pixels=memmap_pixel_array)
+                    if memmap_pixel_array:
+                        self.offset = fp.tell() + 8
+            except Exception:
                 # Raise the error for the calling method to handle
                 raise
             else:
                 # Sometimes DICOM files may not have headers,
                 # but they should always have a SOPClassUID
                 # to declare what type of file it is.
                 # If the file doesn't have a SOPClassUID,
                 # then it probably isn't DICOM.
-                if not "SOPClassUID" in self.ds:
+                if "SOPClassUID" not in self.ds:
                     raise AttributeError
         else:
             raise AttributeError
 
-######################## SOP Class and Instance Methods #######################
+        # Fix dataset file_meta if incorrect
+        try:
+            validate_file_meta(self.ds.file_meta)
+        except ValueError:
+            logger.debug('Fixing invalid File Meta for ' +
+                         str(self.ds.SOPInstanceUID))
+            self.ds.fix_meta_info()
+
+        # Remove the PixelData attribute if it is not set.
+        # i.e. RTStruct does not contain PixelData and its presence can confuse
+        # the parser
+        if "PixelData" in self.ds and self.ds.PixelData is None:
+            delattr(self.ds, 'PixelData')
+        if memmap_pixel_array:
+            self.filename = dataset
+            self.pixel_array = self.get_pixel_array
+        else:
+            if "PixelData" in self.ds:
+                self.pixel_array = self.ds.pixel_array
+
+# ====================== SOP Class and Instance Methods ======================
 
     def GetSOPClassUID(self):
         """Determine the SOP Class UID of the current file."""
+        uid = getattr(self.ds, 'SOPClassUID', None)
 
-        if (self.ds.SOPClassUID == '1.2.840.10008.5.1.4.1.1.481.2'):
+        if (uid == '1.2.840.10008.5.1.4.1.1.481.2'):
             return 'rtdose'
-        elif (self.ds.SOPClassUID == '1.2.840.10008.5.1.4.1.1.481.3'):
+        elif (uid == '1.2.840.10008.5.1.4.1.1.481.3'):
             return 'rtss'
-        elif (self.ds.SOPClassUID == '1.2.840.10008.5.1.4.1.1.481.5'):
+        elif (uid == '1.2.840.10008.5.1.4.1.1.481.5'):
             return 'rtplan'
-        elif (self.ds.SOPClassUID == '1.2.840.10008.5.1.4.1.1.2'):
+        elif (uid == '1.2.840.10008.5.1.4.1.1.2'):
             return 'ct'
         else:
             return None
 
     def GetSOPInstanceUID(self):
         """Determine the SOP Class UID of the current file."""
-
-        return self.ds.SOPInstanceUID
+        return getattr(self.ds, 'SOPInstanceUID', None)
 
     def GetStudyInfo(self):
         """Return the study information of the current file."""
-
-        study = {}
-        if 'StudyDescription' in self.ds:
-            desc = self.ds.StudyDescription
-        else:
-            desc = 'No description'
-        study['description'] = desc
-        if 'StudyDate' in self.ds:
-            date = self.ds.StudyDate
-        else:
-            date = None
-        study['date'] = date
-        if 'StudyTime' in self.ds:
-            time = self.ds.StudyTime
-        else:
-            time = None
-        study['time'] = time
-        # Don't assume that every dataset includes a study UID
-        if 'StudyInstanceUID' in self.ds:
-            study['id'] = self.ds.StudyInstanceUID
-        else:
-            study['id'] = str(random.randint(0, 65535))
-
-        return study
+        return {'description': getattr(self.ds, 'StudyDescription',
+                                       'No description'),
+                'date': getattr(self.ds, 'StudyDate', None),
+                'time': getattr(self.ds, 'StudyTime', None),
+                'id': getattr(self.ds, 'StudyInstanceUID',
+                              str(random.randint(0, 65535)))}
 
     def GetSeriesDateTime(self):
         """Return the series date/time information."""
-        dt = {}
-        if 'SeriesDate' in self.ds:
-            date = self.ds.SeriesDate
-        elif 'InstanceCreationDate' in self.ds:
-            date = self.ds.InstanceCreationDate
-        else:
-            date = None
-        dt['date'] = date
-        if 'SeriesTime' in self.ds:
-            time = self.ds.SeriesTime
-        elif 'InstanceCreationTime' in self.ds:
-            time = self.ds.InstanceCreationTime
-        else:
-            time = None
-        dt['time'] = time
+        dt = {'date': getattr(self.ds, 'SeriesDate', None),
+              'time': getattr(self.ds, 'SeriesTime', None)}
+
+        if dt['date'] is None:
+            dt['date'] = getattr(self.ds, 'InstanceCreationDate', None)
+        if dt['time'] is None:
+            dt['time'] = getattr(self.ds, 'InstanceCreationTime', None)
 
         return dt
 
     def GetSeriesInfo(self):
         """Return the series information of the current file."""
-
-        series = {}
-        if 'SeriesDescription' in self.ds:
-            desc = self.ds.SeriesDescription
-        else:
-            desc = 'No description'
-        series['description'] = desc
-        series['id'] = self.ds.SeriesInstanceUID
-        # Don't assume that every dataset includes a study UID
-        series['study'] = self.ds.SeriesInstanceUID
+        series = {'description': getattr(self.ds, 'SeriesDescription',
+                                         'No description'),
+                  'id': getattr(self.ds, 'SeriesInstanceUID', None),
+                  'study': getattr(self.ds, 'SeriesInstanceUID', None),
+                  'referenceframe': getattr(self.ds, 'FrameOfReferenceUID',
+                                            str(random.randint(0, 65535))),
+                  'modality': getattr(self.ds, 'Modality', 'OT')}
         series.update(self.GetSeriesDateTime())
-        if 'StudyInstanceUID' in self.ds:
-            series['study'] = self.ds.StudyInstanceUID
-        series['referenceframe'] = self.ds.FrameOfReferenceUID \
-            if 'FrameOfReferenceUID' in self.ds \
-            else str(random.randint(0, 65535))
-        if 'Modality' in self.ds:
-            series['modality'] = self.ds.Modality
-        else:
-            series['modality'] = 'OT'
+
+        series['study'] = getattr(self.ds, 'StudyInstanceUID', series['study'])
 
         return series
 
     def GetReferencedSeries(self):
         """Return the SOP Class UID of the referenced series."""
-
         if "ReferencedFrameOfReferenceSequence" in self.ds:
             frame = self.ds.ReferencedFrameOfReferenceSequence
             if "RTReferencedStudySequence" in frame[0]:
                 study = frame[0].RTReferencedStudySequence[0]
                 if "RTReferencedSeriesSequence" in study:
                     if "SeriesInstanceUID" in \
                             study.RTReferencedSeriesSequence[0]:
                         series = study.RTReferencedSeriesSequence[0]
                         return series.SeriesInstanceUID
         else:
             return ''
 
     def GetFrameOfReferenceUID(self):
         """Determine the Frame of Reference UID of the current file."""
-
         if 'FrameOfReferenceUID' in self.ds:
             # Some Files contain a Ref FoR but do not contain an FoR themselves
             if not self.ds.FrameOfReferenceUID == '':
                 return self.ds.FrameOfReferenceUID
         if 'ReferencedFrameOfReferenceSequence' in self.ds:
-            return self.ds.ReferencedFrameOfReferenceSequence[0].FrameOfReferenceUID
+            return self.ds.ReferencedFrameOfReferenceSequence[
+                0].FrameOfReferenceUID
         else:
             return ''
 
     def GetReferencedStructureSet(self):
         """Return the SOP Class UID of the referenced structure set."""
-
         if "ReferencedStructureSetSequence" in self.ds:
-            return self.ds.ReferencedStructureSetSequence[0].ReferencedSOPInstanceUID
+            return self.ds.ReferencedStructureSetSequence[
+                0].ReferencedSOPInstanceUID
         else:
             return ''
 
     def GetReferencedRTPlan(self):
         """Return the SOP Class UID of the referenced RT plan."""
-
         if "ReferencedRTPlanSequence" in self.ds:
             return self.ds.ReferencedRTPlanSequence[0].ReferencedSOPInstanceUID
         else:
             return ''
 
     def GetDemographics(self):
         """Return the patient demographics from a DICOM file."""
-
         # Set up some sensible defaults for demographics
         patient = {'name': 'None',
                    'id': 'None',
                    'birth_date': None,
                    'gender': 'Other'}
         if 'PatientName' in self.ds:
             if PY2:
@@ -219,20 +221,18 @@
                 patient['gender'] = 'O'
         if 'PatientBirthDate' in self.ds:
             if len(self.ds.PatientBirthDate):
                 patient['birth_date'] = str(self.ds.PatientBirthDate)
 
         return patient
 
-
-############################### Image Methods #################################
+# =============================== Image Methods ===============================
 
     def GetImageData(self):
         """Return the image data from a DICOM file."""
-
         data = {}
 
         if 'ImagePositionPatient' in self.ds:
             data['position'] = self.ds.ImagePositionPatient
         if 'ImageOrientationPatient' in self.ds:
             data['orientation'] = self.ds.ImageOrientationPatient
         if 'PixelSpacing' in self.ds:
@@ -247,17 +247,43 @@
             self.ds.file_meta.TransferSyntaxUID.is_little_endian
         if 'PatientPosition' in self.ds:
             data['patientposition'] = self.ds.PatientPosition
         data['frames'] = self.GetNumberOfFrames()
 
         return data
 
+    def GetPixelArray(self):
+        """Generate a memory mapped numpy accessor to the pixel array."""
+        if self.memmap_pixel_array is False:
+            return self.pixel_array
+        data = self.GetImageData()
+        filename = self.filename
+        dtype = pixel_dtype(self.ds)
+        offset = self.offset
+        frames = int(data['frames'])
+        shape = (int(self.GetNumberOfFrames()),
+                 data['rows'], data['columns']) if frames > 1 \
+            else (data['rows'], data['columns'])
+
+        def get_pixel_array(filename, dtype, offset, shape):
+            array = np.memmap(
+                filename,
+                dtype=dtype,
+                mode="r",
+                offset=offset,
+                shape=shape
+            )
+            yield array
+            del array
+        return list(get_pixel_array(filename, dtype, offset, shape))[0]
+
+    get_pixel_array = property(GetPixelArray)
+
     def GetImageLocation(self):
         """Calculate the location of the current image slice."""
-
         ipp = self.ds.ImagePositionPatient
         iop = self.ds.ImageOrientationPatient
 
         normal = []
         normal.append(iop[1] * iop[5] - iop[2] * iop[4])
         normal.append(iop[2] * iop[3] - iop[0] * iop[5])
         normal.append(iop[0] * iop[4] - iop[1] * iop[3])
@@ -271,124 +297,137 @@
             if ('ff' in self.ds.PatientPosition.lower()):
                 loc = loc * -1
 
         return loc
 
     def GetImageOrientationType(self):
         """Get the orientation of the current image slice."""
-
         if 'ImageOrientationPatient' in self.ds:
             iop = np.array(self.ds.ImageOrientationPatient)
 
             orientations = [
                 ["SA", np.array([1, 0, 0, 0, 1, 0])],      # supine axial
                 ["PA", np.array([-1, 0, 0, 0, -1, 0])],    # prone axial
                 ["SS", np.array([0, 1, 0, 0, 0, -1])],     # supine sagittal
                 ["PS", np.array([0, -1, 0, 0, 0, -1])],    # prone sagittal
                 ["SC", np.array([1, 0, 0, 0, 0, -1])],     # supine coronal
                 ["PC", np.array([-1, 0, 0, 0, 0, -1])]     # prone coronal
             ]
 
             for o in orientations:
-                if (not np.any(np.array(np.round(iop - o[1]), dtype=np.int32))):
+                if (not np.any(np.array(np.round(iop - o[1]),
+                                        dtype=np.int32))):
                     return o[0]
-        # Return N/A if the orientation was not found or could not be determined
+        # Return N/A if orientation was not found or could not be determined
         return "NA"
 
     def GetNumberOfFrames(self):
         """Return the number of frames in a DICOM image file."""
-
         frames = 1
         if 'NumberOfFrames' in self.ds:
             frames = self.ds.NumberOfFrames.real
         else:
-            try:
-                self.ds.pixel_array
-            except:
+            if "PixelData" not in self.ds:
                 return 0
             else:
-                if (self.ds.pixel_array.ndim > 2):
+                if (self.pixel_array.ndim > 2):
                     if (self.ds.SamplesPerPixel == 1) and not \
                        (self.ds.PhotometricInterpretation == 'RGB'):
-                        frames = self.ds.pixel_array.shape[0]
+                        frames = self.pixel_array.shape[0]
         return frames
 
     def GetRescaleInterceptSlope(self):
         """Return the rescale intercept and slope if present."""
-
         intercept, slope = 0, 1
         if ('RescaleIntercept' in self.ds and 'RescaleSlope' in self.ds):
             intercept = self.ds.RescaleIntercept if \
                 isinstance(self.ds.RescaleIntercept, Number) else 0
             slope = self.ds.RescaleSlope if \
                 isinstance(self.ds.RescaleSlope, Number) else 1
 
         return intercept, slope
 
     def GetImage(self, window=0, level=0, size=None, background=False,
                  frames=0):
-        """Return the image from a DICOM image storage file."""
+        """Return the image from a DICOM image storage file.
 
+        Parameters
+        ----------
+        window : int, optional
+            Image window, by default 0
+        level : int, optional
+            Image level or width, by default 0
+        size : tuple, optional
+            Image size tuple in pixels, by default None
+        background : bool, optional
+            Enable a black image background, by default False
+        frames : int, optional
+            If multi-frame, use requested frame to generate image, by default 0
+
+        Returns
+        -------
+        Pillow Image
+            A Pillow Image object
+        """
         if not pil_available:
-            print("Python imaging library not available." + \
-                " Cannot generate images.")
+            print("Python imaging library not available." +
+                  " Cannot generate images.")
             return
 
-        # Return None if the Numpy pixel array cannot be accessed
+        # Return a black image if the Numpy pixel array cannot be accessed
         try:
-            self.ds.pixel_array
-        except:
-            return Image.new('RGB', size, (0, 0, 0))
+            self.pixel_array
+        except BaseException:
+            return Image.new('L', size)
 
         # Samples per pixel are > 1 & RGB format
         if (self.ds.SamplesPerPixel > 1) and \
            (self.ds.PhotometricInterpretation == 'RGB'):
 
             # Little Endian
             if self.ds.file_meta.TransferSyntaxUID.is_little_endian:
                 im = Image.frombuffer('RGB', (self.ds.Columns, self.ds.Rows),
                                       self.ds.PixelData, 'raw', 'RGB', 0, 1)
             # Big Endian
             else:
                 im = Image.fromarray(np.rollaxis(
-                    self.ds.pixel_array.transpose(), 0, 2))
+                    self.pixel_array.transpose(), 0, 2))
 
         # Otherwise the image is monochrome
         else:
             if ((window == 0) and (level == 0)):
                 window, level = self.GetDefaultImageWindowLevel()
             # Rescale the slope and intercept of the image if present
             intercept, slope = self.GetRescaleInterceptSlope()
             # Get the requested frame if multi-frame
             if (frames > 0):
-                pixel_array = self.ds.pixel_array[frames]
+                pixel_array = self.pixel_array[frames]
             else:
-                pixel_array = self.ds.pixel_array
+                pixel_array = self.pixel_array
 
             rescaled_image = pixel_array * slope + intercept
 
             image = self.GetLUTValue(rescaled_image, window, level)
             im = Image.fromarray(image).convert('L')
 
         # Resize the image if a size is provided
         if size:
             im.thumbnail(size, Image.ANTIALIAS)
 
         # Add a black background if requested
         if background:
             bg = Image.new('RGBA', size, (0, 0, 0, 255))
             bg.paste(im, ((size[0] - im.size[0]) // 2,
-                     (size[1] - im.size[1]) // 2))
+                          (size[1] - im.size[1]) // 2))
             return bg
 
         return im
 
     def GetDefaultImageWindowLevel(self):
         """Determine the default window/level for the DICOM image."""
-
         window, level = 0, 0
         if ('WindowWidth' in self.ds) and ('WindowCenter' in self.ds):
             if isinstance(self.ds.WindowWidth, float):
                 window = self.ds.WindowWidth
             elif isinstance(self.ds.WindowWidth, list):
                 if (len(self.ds.WindowWidth) > 1):
                     window = self.ds.WindowWidth[1]
@@ -399,81 +438,105 @@
                     level = self.ds.WindowCenter[1]
 
         if ((window, level) == (0, 0)):
             wmax = 0
             wmin = 0
             # Rescale the slope and intercept of the image if present
             intercept, slope = self.GetRescaleInterceptSlope()
-            pixel_array = self.ds.pixel_array * slope + intercept
+            pixel_array = self.pixel_array * slope + intercept
 
             if (pixel_array.max() > wmax):
                 wmax = pixel_array.max()
             if (pixel_array.min() < wmin):
                 wmin = pixel_array.min()
             # Default window is the range of the data array
             window = int(wmax - wmin)
             # Default level is the range midpoint minus the window minimum
             level = int(window / 2 - abs(wmin))
         return window, level
 
     def GetLUTValue(self, data, window, level):
-        """Apply the RGB Look-Up Table for the data and window/level value."""
+        """Apply the RGB Look-Up Table for the data and window/level value.
 
-        lutvalue = util.piecewise(data,
-                                [data <= (level - 0.5 - (window - 1) / 2),
-                                 data > (level - 0.5 + (window - 1) / 2)],
-                                [0, 255, lambda data:
-                                 ((data - (level - 0.5)) / (window-1) + 0.5) *
-                                 (255 - 0)])
+        Parameters
+        ----------
+        data : numpy array
+            Pixel data array from pydicom dataset
+        window : float
+            Image window value
+        level : float
+            Image window level or width
+
+        Returns
+        -------
+        numpy array
+            Modified numpy array with RGB LUT applied
+        """
+        lutvalue = util.piecewise(
+            data,
+            [data <= (level - 0.5 - (window - 1) / 2),
+             data > (level - 0.5 + (window - 1) / 2)],
+            [0, 255, lambda data:
+             ((data - (level - 0.5)) / (window-1) + 0.5) *
+             (255 - 0)])
         # Convert the resultant array to an unsigned 8-bit array to create
         # an 8-bit grayscale LUT since the range is only from 0 to 255
         return np.array(lutvalue, dtype=np.uint8)
 
     def GetPatientToPixelLUT(self):
-        """Get the image transformation matrix from the DICOM standard Part 3
-            Section C.7.6.2.1.1"""
+        """Get image transformation matrix from the DICOM standard.
 
-        di = self.ds.PixelSpacing[0]
-        dj = self.ds.PixelSpacing[1]
-        orientation = self.ds.ImageOrientationPatient
-        position = self.ds.ImagePositionPatient
+        Referenced matrix can be found in Part 3 Section C.7.6.2.1.1
+        """
+        drow, dcol = self.ds.PixelSpacing
 
-        m = np.matrix(
-            [[orientation[0]*di, orientation[3]*dj, 0, position[0]],
-            [orientation[1]*di, orientation[4]*dj, 0, position[1]],
-            [orientation[2]*di, orientation[5]*dj, 0, position[2]],
-            [0, 0, 0, 1]])
-
-        x = []
-        y = []
-        for i in range(0, self.ds.Columns):
-            imat = m * np.matrix([[i], [0], [0], [1]])
-            x.append(float(imat[0]))
-        for j in range(0, self.ds.Rows):
-            jmat = m * np.matrix([[0], [j], [0], [1]])
-            y.append(float(jmat[1]))
+        orientation = self.ds.ImageOrientationPatient
+        first_x, first_y, first_z = self.ds.ImagePositionPatient
+        num_cols = self.ds.Columns
+        num_rows = self.ds.Rows
+
+        # Determine which way X and Y real-world coords run
+        # X runs across columns if x_lut_index is 0
+        # limits to head-first/feet-first and prone/supine/decubitus
+        x_index = self.x_lut_index()
+
+        m = np.array(
+            [[orientation[0]*dcol, orientation[3]*drow, 0, first_x],
+             [orientation[1]*dcol, orientation[4]*drow, 0, first_y],
+             [orientation[2]*dcol, orientation[5]*drow, 0, first_z],
+             [0, 0, 0, 1]])
+
+        last_xy = np.matmul(
+            m, np.array([[num_cols-1], [num_rows-1], [0], [1]])
+        )
+        last_x, last_y = last_xy[0][0], last_xy[1][0]
+
+        if x_index == 0:
+            col_lut = np.linspace(first_x, last_x, num_cols)
+            row_lut = np.linspace(first_y, last_y, num_rows)
+        else:
+            col_lut = np.linspace(first_y, last_y, num_cols)
+            row_lut = np.linspace(first_x, last_x, num_rows)
 
-        return (np.array(x), np.array(y))
+        return col_lut, row_lut
 
-########################## RT Structure Set Methods ###########################
+# ========================= RT Structure Set Methods =========================
 
     def GetStructureInfo(self):
         """Return the patient demographics from a DICOM file."""
-
         structure = {}
-        structure['label'] = self.ds.StructureSetLabel
-        structure['date'] = self.ds.StructureSetDate
-        structure['time'] = self.ds.StructureSetTime
+        structure['label'] = getattr(self.ds, 'StructureSetLabel', '')
+        structure['date'] = getattr(self.ds, 'StructureSetDate', '')
+        structure['time'] = getattr(self.ds, 'StructureSetTime', '')
         structure['numcontours'] = len(self.ds.ROIContourSequence)
 
         return structure
 
     def GetStructures(self):
-        """Returns a dictionary of structures (ROIs)."""
-
+        """Return a dictionary of structures (ROIs)."""
         structures = {}
 
         # Determine whether this is RT Structure Set file
         if not (self.GetSOPClassUID() == 'rtss'):
             return structures
 
         # Locate the name and number of each ROI
@@ -513,65 +576,99 @@
                         value = roi[0x3006, 0x002a].repval
                         color = value.strip("'").split("/")
                     # Try to convert the detected value to a color triplet
                     try:
                         structures[number]['color'] = \
                             np.array(color, dtype=int)
                     # Otherwise fail and fallback on the random color
-                    except:
+                    except Exception:
                         logger.debug(
                             "Unable to decode display color for ROI #%s",
                             str(number))
 
                 # Determine whether the ROI has any contours present
                 if 'ContourSequence' in roi:
                     structures[number]['empty'] = False
                 else:
                     structures[number]['empty'] = True
 
         return structures
 
     def GetStructureCoordinates(self, roi_number):
-        """Get the list of coordinates for each plane of the structure."""
+        """Get the list of coordinates for each plane of the structure.
+
+        Parameters
+        ----------
+        roi_number : integer
+            ROI number used to index structure from RT Struct
 
+        Returns
+        -------
+        dict
+            Dict of structure coordinates sorted by slice position (z)
+        """
         planes = {}
         # The coordinate data of each ROI is stored within ROIContourSequence
         if 'ROIContourSequence' in self.ds:
             for roi in self.ds.ROIContourSequence:
                 if (roi.ReferencedROINumber == int(roi_number)):
                     if 'ContourSequence' in roi:
                         # Locate the contour sequence for each referenced ROI
                         for c in roi.ContourSequence:
                             # For each plane, initialize a new plane dict
                             plane = dict()
 
                             # Determine all the plane properties
                             plane['type'] = c.ContourGeometricType
                             plane['num_points'] = int(c.NumberOfContourPoints)
+                            # Since DICOM RT Structure Set (C.8.8.6) specifies
+                            # that a ContourData is stored as an flattened list
+                            # of xyz triples, convert it to a unflattened list
+                            # for easier parsing
                             plane['data'] = \
                                 self.GetContourPoints(c.ContourData)
 
                             # Add each plane to the planes dict
                             # of the current ROI
                             z = str(round(plane['data'][0][2], 2)) + '0'
                             if z not in planes:
                                 planes[z] = []
                             planes[z].append(plane)
 
         return planes
 
     def GetContourPoints(self, array):
-        """Parses an array of xyz points & returns a array of point dicts."""
+        """Unflatten a flattened list of xyz point triples.
+
+        Parameters
+        ----------
+        array : list
+            Flattened list of xyz point triples
 
+        Returns
+        -------
+        list
+            Unflattened list of xyz point triples
+        """
         n = 3
         return [array[i:i+n] for i in range(0, len(array), n)]
 
     def CalculatePlaneThickness(self, planesDict):
-        """Calculates the plane thickness for each structure."""
+        """Calculate the plane thickness for each structure.
 
+        Parameters
+        ----------
+        planesDict : dict
+            Output from GetStructureCoordinates
+
+        Returns
+        -------
+        float
+            Thickness of the structure in mm
+        """
         planes = []
 
         # Iterate over each plane in the structure
         for z in iterkeys(planesDict):
             planes.append(float(z))
         planes.sort()
 
@@ -586,30 +683,34 @@
         # If the thickness was not detected, set it to 0
         if (thickness == 10000):
             thickness = 0
 
         return thickness
 
     def CalculateStructureVolume(self, coords, thickness):
-        """Calculates the volume of the given structure.
+        """Calculate the volume of the given structure.
 
         Parameters
         ----------
         coords : dict
             Coordinates of each plane of the structure
         thickness : float
-            Thickness of the structure
-        """
+            Thickness of the structure in mm
 
+        Returns
+        -------
+        float
+            Volume of structure in cm3
+        """
         if not shapely_available:
             print("Shapely library not available." +
                   " Please install to calculate.")
             return 0
 
-        class Within(Polygon):
+        class Within:
             def __init__(self, o):
                 self.o = o
 
             def __lt__(self, other):
                 return self.o.within(other.o)
 
         s = 0
@@ -641,69 +742,76 @@
                         (p != ordered_polygons[0]):
                     s -= pa
                 else:
                     s += pa
         vol = s * thickness / 1000
         return vol
 
-############################## RT Dose Methods ###############################
+# ============================== RT Dose Methods ==============================
 
     def HasDVHs(self):
-        """Returns whether dose-volume histograms (DVHs) exist."""
-
-        if not "DVHSequence" in self.ds:
+        """Return whether dose-volume histograms (DVHs) exist."""
+        if "DVHSequence" not in self.ds:
             return False
         else:
             return True
 
     def GetDVHs(self):
-        """Returns cumulative dose-volume histograms (DVHs)."""
-
+        """Return cumulative dose-volume histograms (DVHs)."""
         self.dvhs = {}
 
         if self.HasDVHs():
             for item in self.ds.DVHSequence:
                 # Make sure that the DVH has a referenced structure / ROI
-                if not 'DVHReferencedROISequence' in item:
+                if 'DVHReferencedROISequence' not in item:
                     continue
                 number = item.DVHReferencedROISequence[0].ReferencedROINumber
                 logger.debug("Found DVH for ROI #%s", str(number))
                 self.dvhs[number] = dvh.DVH.from_dicom_dvh(self.ds, number)
 
         return self.dvhs
 
     def GetDoseGrid(self, z=0, threshold=0.5):
-        """
-        Return the 2d dose grid for the given slice position (mm).
+        """Return the 2d dose grid for the given slice position (mm).
 
-        :param z:           Slice position in mm.
-        :param threshold:   Threshold in mm to determine the max difference
-                            from z to the closest dose slice without
-                            using interpolation.
-        :return:            An numpy 2d array of dose points.
+        Parameters
+        ----------
+        z : int, optional
+            Slice position in mm, by default 0
+        threshold : float, optional
+            Threshold in mm to determine the max difference from z
+            to the closest dose slice without using interpolation,
+            by default 0.5
+
+        Returns
+        -------
+        np.array
+            An numpy 2d array of dose points
         """
-
         # If this is a multi-frame dose pixel array,
         # determine the offset for each frame
         if 'GridFrameOffsetVector' in self.ds:
+            pixel_array = self.GetPixelArray()
             z = float(z)
             # Get the initial dose grid position (z) in patient coordinates
-            imagepatpos = self.ds.ImagePositionPatient[2]
-            orientation = self.ds.ImageOrientationPatient[0]
+            ipp = self.ds.ImagePositionPatient
+            gfov = self.ds.GridFrameOffsetVector
             # Add the position to the offset vector to determine the
             # z coordinate of each dose plane
-            planes = orientation * np.array(self.ds.GridFrameOffsetVector) + \
-                imagepatpos
+
+            z_sign = 1 if self.is_head_first_orientation() else -1
+
+            planes = (z_sign * np.array(gfov)) + ipp[2]
             frame = -1
             # Check to see if the requested plane exists in the array
             if (np.amin(np.fabs(planes - z)) < threshold):
                 frame = np.argmin(np.fabs(planes - z))
             # Return the requested dose plane, since it was found
             if not (frame == -1):
-                return self.ds.pixel_array[frame]
+                return pixel_array[frame]
             # Check if the requested plane is within the dose grid boundaries
             elif ((z < np.amin(planes)) or (z > np.amax(planes))):
                 return np.array([])
             # The requested plane was not found, so interpolate between planes
             else:
                 # Determine the upper and lower bounds
                 umin = np.fabs(planes - z)
@@ -711,100 +819,202 @@
                 lmin = umin.copy()
                 # Change the min value to the max so we can find the 2nd min
                 lmin[ub] = np.amax(umin)
                 lb = np.argmin(lmin)
                 # Fractional distance of dose plane between upper & lower bound
                 fz = (z - planes[lb]) / (planes[ub] - planes[lb])
                 plane = self.InterpolateDosePlanes(
-                    self.ds.pixel_array[ub], self.ds.pixel_array[lb], fz)
+                    pixel_array[ub], pixel_array[lb], fz)
                 return plane
         else:
             return np.array([])
 
     def InterpolateDosePlanes(self, uplane, lplane, fz):
-        """Interpolates a dose plane between two bounding planes at the given
-           relative location.
+        """Interpolate a dose plane between two bounding planes.
 
-        :param uplane:      Upper dose plane boundary.
-        :param uplane:      Lower dose plane boundary.
-        :param fz:          Fractional distance from the bottom to the top,
-                            where the new plane is located.
-                            E.g. if fz = 1, the plane is at the upper plane,
-                            fz = 0, it is at the lower plane.
-        :return:            An numpy 2d array of the interpolated dose plane.
+        Parameters
+        ----------
+        uplane : float
+            Upper dose plane boundary in mm
+        lplane : float
+            Lower dose plane boundary in mm
+        fz : float
+            Fractional distance from the bottom to the top,
+            where the new plane is located.
+            E.g. if fz = 1, the plane is at the upper plane,
+            fz = 0, it is at the lower plane.
+
+        Returns
+        -------
+        numpy array
+            An numpy 2d array of the interpolated dose plane
         """
-
         # A simple linear interpolation
         doseplane = fz*uplane + (1.0 - fz)*lplane
 
         return doseplane
 
-    def GetIsodosePoints(self, z=0, level=100, threshold=0.5):
-        """Return points for the given isodose level and slice position
-           from the dose grid.
+    def is_head_first_orientation(self):
+        """Return True if self.orientation is head-first.
+
+        Raises
+        ------
+        NotImplementedError
+            Raised if orientation is not one of head/feet-first
+            and supine/prone/decubitus
+
+        Returns
+        -------
+        bool
+            True if orientation is head-first, else False
+
 
-        :param z:           Slice position in mm.
-        :param threshold:   Threshold in mm to determine the max difference
-                            from z to the closest dose slice without
-                            using interpolation.
-        :param level:       Isodose level in scaled form
-                            (multiplied by self.ds.DoseGridScaling)
-        :return:            An array of tuples representing isodose points.
         """
+        orientation = self.ds.ImageOrientationPatient
+        if any(
+            all(np.isclose(orientation, hf_orientation))
+            for hf_orientation in (  # noqa
+                [1,  0,  0,  0,  1,  0],  # Head First Supine
+                [-1,  0,  0,  0, -1,  0],  # Head First Prone
+                [0, -1,  0,  1,  0,  0],  # Head First Decubitus Left
+                [0,  1,  0, -1,  0,  0]   # Head First Decubitus Right
+            )
+        ):
+            return True
+        elif any(
+            all(np.isclose(orientation, ff_orientation))
+            for ff_orientation in (
+                [0,  1,  0,  1,  0,  0],  # Feet First Decubitus Left
+                [0, -1,  0, -1,  0,  0],  # Feet First Decubitus Right
+                [1,  0,  0,  0, -1,  0],  # Feet First Prone
+                [-1,  0,  0,  0,  1,  0]   # Feet First Supine
+            )
+        ):
+            return False
+        else:
+            raise NotImplementedError(
+                "Cannot calculate dose plane sign for non-standard orientation"
+            )
+
+    def x_lut_index(self):
+        """Return LUT index for real-world X direction.
+
+        Raises
+        ------
+        NotImplementedError
+            Raised if orientation is not one of head/feet-first
+            and supine/prone/decubitus
+
+        Returns
+        -------
+        X direction LUT index, matching 'lut' from GetDoseData
+            0 if real-world X across columns
+            1 if real-world X along rows
+        """
+        orientation = self.ds.ImageOrientationPatient
+        if any(
+            all(np.isclose(orientation, non_decub))
+            for non_decub in (
+                [1,  0,  0,  0,  1,  0],  # Head First Supine
+                [-1,  0,  0,  0, -1,  0],  # Head First Prone
+                [-1,  0,  0,  0,  1,  0],  # Feet First Supine
+                [1,  0,  0,  0, -1,  0]   # Feet First Prone
+            )
+        ):
+            return 0
+        elif any(
+            all(np.isclose(orientation, decub))
+            for decub in (
+                [0, -1,  0,  1,  0,  0],  # Head First Decubitus Left
+                [0,  1,  0, -1,  0,  0],  # Head First Decubitus Right
+                [0,  1,  0,  1,  0,  0],  # Feet First Decubitus Left
+                [0, -1,  0, -1,  0,  0]   # Feet First Decubitus Right
+            )
+        ):
+            return 1
+        else:
+            raise NotImplementedError(
+                "Cannot calculate X direction for non-standard orientation"
+            )
 
+    def GetIsodosePoints(self, z=0, level=100, threshold=0.5):
+        """Return dose grid points from an isodose level & slice position.
+
+        Parameters
+        ----------
+        z : int, optional
+            Slice position in mm., by default 0
+        level : int, optional
+            Isodose level in scaled form
+            (multiplied by self.ds.DoseGridScaling), by default 100
+        threshold : float, optional
+            Threshold in mm to determine the max difference
+            from z to the closest dose slice without
+            using interpolation, by default 0.5
+
+        Returns
+        -------
+        list
+            An list of tuples representing isodose points
+        """
         plane = self.GetDoseGrid(z, threshold)
         isodose = (plane >= level).nonzero()
         return list(zip(isodose[1].tolist(), isodose[0].tolist()))
 
     def GetDoseData(self):
         """Return the dose data from a DICOM RT Dose file."""
-
         data = self.GetImageData()
-        data['doseunits'] = self.ds.DoseUnits
-        data['dosetype'] = self.ds.DoseType
-        data['dosecomment'] = self.ds.DoseComment \
-            if 'DoseComment' in self.ds else ''
-        data['dosesummationtype'] = self.ds.DoseSummationType
-        data['dosegridscaling'] = self.ds.DoseGridScaling
-        data['dosemax'] = float(self.ds.pixel_array.max())
+        data['doseunits'] = getattr(self.ds, 'DoseUnits', '')
+        data['dosetype'] = getattr(self.ds, 'DoseType', '')
+        data['dosecomment'] = getattr(self.ds, 'DoseComment', '')
+        data['dosesummationtype'] = getattr(self.ds, 'DoseSummationType', '')
+        data['dosegridscaling'] = getattr(self.ds, 'DoseGridScaling', '')
+        dosemax = 0
+        for x in range(data["frames"]):
+            pixel_array = self.GetPixelArray()
+            newmax = pixel_array[x].max()
+            dosemax = newmax if newmax > dosemax else dosemax
+            if self.memmap_pixel_array:
+                del pixel_array
+        data['dosemax'] = float(dosemax)
         data['lut'] = self.GetPatientToPixelLUT()
+        data['x_lut_index'] = self.x_lut_index()
         data['fraction'] = ''
         if "ReferencedRTPlanSequence" in self.ds:
             plan = self.ds.ReferencedRTPlanSequence[0]
             if "ReferencedFractionGroupSequence" in plan:
                 data['fraction'] = \
-                plan.ReferencedFractionGroupSequence[0].ReferencedFractionGroupNumber
+                    plan.ReferencedFractionGroupSequence[
+                        0].ReferencedFractionGroupNumber
 
         return data
 
     def GetReferencedBeamNumber(self):
         """Return the referenced beam number (if it exists) from RT Dose."""
-
         beam = None
         if "ReferencedRTPlanSequence" in self.ds:
             rp = self.ds.ReferencedRTPlanSequence[0]
             if "ReferencedFractionGroupSequence" in rp:
                 rf = rp.ReferencedFractionGroupSequence[0]
                 if "ReferencedBeamSequence" in rf:
                     if "ReferencedBeamNumber" in rf.ReferencedBeamSequence[0]:
                         beam = \
                             rf.ReferencedBeamSequence[0].ReferencedBeamNumber
 
         return beam
 
-############################## RT Plan Methods ###############################
+# ============================== RT Plan Methods ==============================
 
     def GetPlan(self):
-        """Returns the plan information."""
-
+        """Return the plan information."""
         self.plan = {}
 
-        self.plan['label'] = self.ds.RTPlanLabel
-        self.plan['date'] = self.ds.RTPlanDate
-        self.plan['time'] = self.ds.RTPlanTime
+        self.plan['label'] = getattr(self.ds, 'RTPlanLabel', '')
+        self.plan['date'] = getattr(self.ds, 'RTPlanDate', '')
+        self.plan['time'] = getattr(self.ds, 'RTPlanTime', '')
         self.plan['name'] = ''
         self.plan['rxdose'] = 0
         if "DoseReferenceSequence" in self.ds:
             for item in self.ds.DoseReferenceSequence:
                 if item.DoseReferenceStructureType == 'SITE':
                     self.plan['name'] = "N/A"
                     if "DoseReferenceDescription" in item:
@@ -812,15 +1022,16 @@
                     if 'TargetPrescriptionDose' in item:
                         rxdose = item.TargetPrescriptionDose * 100
                         if (rxdose > self.plan['rxdose']):
                             self.plan['rxdose'] = rxdose
                 elif item.DoseReferenceStructureType == 'VOLUME':
                     if 'TargetPrescriptionDose' in item:
                         self.plan['rxdose'] = item.TargetPrescriptionDose * 100
-        if (("FractionGroupSequence" in self.ds) and (self.plan['rxdose'] == 0)):
+        if (("FractionGroupSequence" in self.ds) and
+                (self.plan['rxdose'] == 0)):
             fg = self.ds.FractionGroupSequence[0]
             if ("ReferencedBeamSequence" in fg) and \
                ("NumberOfFractionsPlanned" in fg):
                 beams = fg.ReferencedBeamSequence
                 fx = fg.NumberOfFractionsPlanned
                 for beam in beams:
                     if "BeamDose" in beam:
@@ -829,16 +1040,26 @@
         self.plan['brachy'] = False
         if ("BrachyTreatmentTechnique" in self.ds) or \
                 ("BrachyTreatmentType" in self.ds):
             self.plan['brachy'] = True
         return self.plan
 
     def GetReferencedBeamsInFraction(self, fx=0):
-        """Return the referenced beams from the specified fraction."""
+        """Return the referenced beams from the specified fraction.
 
+        Parameters
+        ----------
+        fx : int, optional
+            FractionGroupSequence number, by default 0
+
+        Returns
+        -------
+        dict
+            Dictionary of referenced beam data
+        """
         beams = {}
         if ("BeamSequence" in self.ds):
             bdict = self.ds.BeamSequence
         elif ("IonBeamSequence" in self.ds):
             bdict = self.ds.IonBeamSequence
         else:
             return beams
```

### Comparing `dicompyler-core-0.5.5/dicompylercore/dvh.py` & `dicompyler-core-0.5.6/dicompylercore/dvh.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # This file is part of dicompyler-core, released under a BSD license.
 #    See the file license.txt included with this distribution, also
 #    available at https://github.com/dicompyler/dicompyler-core/
 
 import numpy as np
 import re
 import logging
-logger = logging.getLogger('dicompyler.dvh')
+logger = logging.getLogger('dicompylercore.dvh')
 
 # Set default absolute dose and volume  units
 abs_dose_units = 'Gy'
 abs_volume_units = 'cm3'
 relative_units = '%'
 
 
@@ -57,31 +57,31 @@
         self.rx_dose = rx_dose
         self.name = name
         self.color = color
         self.notes = notes
 
     @classmethod
     def from_dicom_dvh(cls, dataset, roi_num, rx_dose=None, name=None,
-            color=None):
+                       color=None):
         """Initialization for a DVH from a pydicom RT Dose DVH sequence."""
         sequence_num = -1
         for i, d in enumerate(dataset.DVHSequence):
             if 'DVHReferencedROISequence' in d:
                 if 'ReferencedROINumber' in d.DVHReferencedROISequence[0]:
                     if roi_num == \
                             d.DVHReferencedROISequence[0].ReferencedROINumber:
                         sequence_num = i
                         break
         if sequence_num == -1:
             raise AttributeError(
                 "'DVHSequence' has no DVH with ROI Number '%d'." % roi_num)
         dvh = dataset.DVHSequence[sequence_num]
         data = np.array(dvh.DVHData)
-        return cls(counts=data[1::2] * dvh.DVHDoseScaling,
-                   bins=data[0::2].cumsum(),
+        return cls(counts=data[1::2],
+                   bins=data[0::2].cumsum() * dvh.DVHDoseScaling,
                    dvh_type=dvh.DVHType.lower(),
                    dose_units=dvh.DoseUnits.capitalize(),
                    volume_units=dvh.DVHVolumeUnits.lower(),
                    rx_dose=rx_dose,
                    name=name,
                    color=color)
 
@@ -465,15 +465,15 @@
         if volume_counts.size == 0 or volume > volume_counts.max():
             return DVHValue(0.0, self.dose_units)
 
         # D100 case
         if volume == 100 and not volume_units:
             # Flipping the difference volume array
             reversed_difference_of_volume = np.flip(
-                    np.fabs(volume_counts - volume), 0)
+                np.fabs(volume_counts - volume), 0)
 
             # Index of the first minimum value in reversed array
             index_min_value = np.argmin(reversed_difference_of_volume)
             index_range = len(reversed_difference_of_volume) - 1
 
             return DVHValue(
                 self.bins[index_range - index_min_value], self.dose_units)
```

### Comparing `dicompyler-core-0.5.5/dicompylercore/dvhcalc.py` & `dicompyler-core-0.5.6/dicompylercore/dvhcalc.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 from __future__ import division
 import numpy as np
 import numpy.ma as ma
 import matplotlib.path
 from dicompylercore import dvh
 from dicompylercore.config import skimage_available
 import collections
+try:
+    from collections.abc import Sequence
+except ImportError:
+    from collections import Sequence
 from six import iteritems
 import logging
 logger = logging.getLogger('dicompylercore.dvhcalc')
 
 if skimage_available:
     from skimage.transform import rescale
 
@@ -28,102 +32,126 @@
             roi,
             limit=None,
             calculate_full_volume=True,
             use_structure_extents=False,
             interpolation_resolution=None,
             interpolation_segments_between_planes=0,
             thickness=None,
+            memmap_rtdose=False,
             callback=None):
     """Calculate a cumulative DVH in Gy from a DICOM RT Structure Set & Dose.
 
     Parameters
     ----------
-    structure : pydicom Dataset
+    structure : pydicom Dataset or filename
         DICOM RT Structure Set used to determine the structure data.
-    dose : pydicom Dataset
+    dose : pydicom Dataset or filename
         DICOM RT Dose used to determine the dose grid.
     roi : int
         The ROI number used to uniquely identify the structure in the structure
         set.
     limit : int, optional
         Dose limit in cGy as a maximum bin for the histogram.
     calculate_full_volume : bool, optional
         Calculate the full structure volume including contours outside of the
         dose grid.
     use_structure_extents : bool, optional
         Limit the DVH calculation to the in-plane structure boundaries.
-    interpolation_resolution : float, optional
-        Resolution in mm to interpolate the structure and dose data to.
+    interpolation_resolution : tuple or float, optional
+        Resolution in mm (row, col) to interpolate structure and dose data to.
+        If float is provided, original dose grid pixel spacing must be square.
     interpolation_segments_between_planes : integer, optional
         Number of segments to interpolate between structure slices.
     thickness : float, optional
         Structure thickness used to calculate volume of a voxel.
+    memmap_rtdose : bool, optional
+        Use memory mapping to access the pixel array of the DICOM RT Dose.
+        This reduces memory usage at the expense of increased calculation time.
     callback : function, optional
         A function that will be called at every iteration of the calculation.
+
+    Returns
+    -------
+    dvh.DVH
+        An instance of dvh.DVH in cumulative dose. This can be converted to
+        different formats using the attributes and properties of the DVH class.
     """
     from dicompylercore import dicomparser
+
     rtss = dicomparser.DicomParser(structure)
-    rtdose = dicomparser.DicomParser(dose)
+    rtdose = dicomparser.DicomParser(dose, memmap_pixel_array=memmap_rtdose)
     structures = rtss.GetStructures()
     s = structures[roi]
     s['planes'] = rtss.GetStructureCoordinates(roi)
     s['thickness'] = thickness if thickness else rtss.CalculatePlaneThickness(
         s['planes'])
 
-    calcdvh = calculate_dvh(s, rtdose, limit, calculate_full_volume,
-                            use_structure_extents, interpolation_resolution,
-                            interpolation_segments_between_planes,
-                            callback)
+    calcdvh = _calculate_dvh(s, rtdose, limit, calculate_full_volume,
+                             use_structure_extents, interpolation_resolution,
+                             interpolation_segments_between_planes,
+                             callback)
     return dvh.DVH(counts=calcdvh.histogram,
                    bins=(np.arange(0, 2) if (calcdvh.histogram.size == 1) else
                          np.arange(0, calcdvh.histogram.size + 1) / 100),
                    dvh_type='differential',
                    dose_units='Gy',
                    notes=calcdvh.notes,
                    name=s['name']).cumulative
 
 
-def calculate_dvh(structure,
-                  dose,
-                  limit=None,
-                  calculate_full_volume=True,
-                  use_structure_extents=False,
-                  interpolation_resolution=None,
-                  interpolation_segments_between_planes=0,
-                  callback=None):
-    """Calculate the differential DVH for the given structure and dose grid.
+def _calculate_dvh(structure,
+                   dose,
+                   limit=None,
+                   calculate_full_volume=True,
+                   use_structure_extents=False,
+                   interpolation_resolution=None,
+                   interpolation_segments_between_planes=0,
+                   callback=None):
+    """Calculate a differential DVH for the given structure and dose grid.
 
     Parameters
     ----------
     structure : dict
-        A structure (ROI) from an RT Structure Set parsed using DicomParser
+        A structure (ROI) from an RT Structure Set parsed using DicomParser.
+        The dictionary must include a `thickness` key with a thickness `float`.
     dose : DicomParser
         A DicomParser instance of an RT Dose
     limit : int, optional
         Dose limit in cGy as a maximum bin for the histogram.
     calculate_full_volume : bool, optional
         Calculate the full structure volume including contours outside of the
         dose grid.
     use_structure_extents : bool, optional
         Limit the DVH calculation to the in-plane structure boundaries.
-    interpolation_resolution : float, optional
-        Resolution in mm to interpolate the structure and dose data to.
+    interpolation_resolution : tuple or float, optional
+        Resolution in mm (row, col) to interpolate structure and dose data to.
+        If float is provided, original dose grid pixel spacing must be square.
     interpolation_segments_between_planes : integer, optional
         Number of segments to interpolate between structure slices.
     callback : function, optional
         A function that will be called at every iteration of the calculation.
+
+    Returns
+    -------
+    calcdvh: collections.namedtuple
+        A named tuple of notes and and histogram data.
+
+    Notes
+    -----
+    This is an internal function called by `get_dvh` and
+    should not be called directly.
     """
     planes = collections.OrderedDict(sorted(iteritems(structure['planes'])))
     calcdvh = collections.namedtuple('DVH', ['notes', 'histogram'])
     logger.debug("Calculating DVH of %s %s", structure['id'],
                  structure['name'])
 
     # Create an empty array of bins to store the histogram in cGy
     # only if the structure has contour data or the dose grid exists
-    if ((len(planes)) and ("PixelData" in dose.ds)):
+    if ((len(planes)) and (hasattr(dose, 'pixel_array'))):
 
         # Get the dose and image data information
         dd = dose.GetDoseData()
         id = dose.GetImageData()
 
         # Determine structure and respectively dose grid extents
         if interpolation_resolution or use_structure_extents:
@@ -139,23 +167,26 @@
                      dd['lut'][1][dgindexextents[1]:dgindexextents[3]])
             # If interpolation is enabled, generate new LUT from extents
             if interpolation_resolution:
                 dd['lut'] = get_resampled_lut(
                     dgindexextents,
                     dgextents,
                     new_pixel_spacing=interpolation_resolution,
-                    min_pixel_spacing=id['pixelspacing'][0])
+                    min_pixel_spacing=id['pixelspacing'])
             dd['rows'] = dd['lut'][1].shape[0]
             dd['columns'] = dd['lut'][0].shape[0]
 
         # Generate a 2d mesh grid to create a polygon mask in dose coordinates
         # Code taken from Stack Overflow Answer from Joe Kington:
         # https://stackoverflow.com/q/3654289/74123
         # Create vertex coordinates for each grid cell
-        x, y = np.meshgrid(np.array(dd['lut'][0]), np.array(dd['lut'][1]))
+        x_index = dd['x_lut_index']
+        x, y = np.meshgrid(
+            np.array(dd['lut'][x_index]), np.array(dd['lut'][1-x_index])
+        )
         x, y = x.flatten(), y.flatten()
         dosegridpoints = np.vstack((x, y)).T
 
         maxdose = int(dd['dosemax'] * dd['dosegridscaling'] * 100) + 1
         # Remove values above the limit (cGy) if specified
         if isinstance(limit, int):
             if (limit < maxdose):
@@ -197,16 +228,26 @@
                 notes = 'Dose grid does not encompass every contour.' + \
                     ' Volume calculated within dose grid.'
             else:
                 origin_z = id['position'][2]
                 logger.warning('Dose plane not found for %s.' +
                                ' Using %s to calculate contour volume.',
                                z, origin_z)
+                # Create a dummy dose grid with the correct size.
+                # calculate_plane_histogram() and its methods provide the
+                # volume calc needed, but do so as part of DVH calc,
+                # which requires a dose grid
+                dummy_dose = dose.GetDoseGrid(origin_z)
+                if use_structure_extents:
+                    extents = dgindexextents
+                    dummy_dose = dummy_dose[
+                        extents[1]:extents[3], extents[0]:extents[2]
+                    ]
                 _, vol = calculate_plane_histogram(
-                    plane, dose.GetDoseGrid(origin_z), dosegridpoints, maxdose,
+                    plane, dummy_dose, dosegridpoints, maxdose,
                     dd, id, structure, hist)
                 planedata[z] = (np.array([0]), vol)
                 notes = 'Dose grid does not encompass every contour.' + \
                     ' Volume calculated for all contours.'
         n += 1
         if callback:
             callback(n, len(planes))
@@ -233,15 +274,15 @@
     # Create a zero valued bool grid
     grid = np.zeros((dd['rows'], dd['columns']), dtype=np.uint8)
 
     # Calculate the dose plane mask for each contour in the plane
     # and boolean xor to remove holes
     for i, contour in enumerate(contours):
         m = get_contour_mask(dd, id, dosegridpoints, contour)
-        grid = np.logical_xor(m.astype(np.uint8), grid).astype(np.bool)
+        grid = np.logical_xor(m.astype(np.uint8), grid).astype(np.bool_)
 
     hist, vol = calculate_contour_dvh(grid, doseplane, maxdose, dd, id,
                                       structure)
     return (hist, vol)
 
 
 def get_contour_mask(dd, id, dosegridpoints, contour):
@@ -257,31 +298,34 @@
 
     # p = Polygon(contour)
     # x, y = np.meshgrid(np.array(dd['lut'][0]), np.array(dd['lut'][1]))
     # mask = inpolygon(p, x.ravel(), y.ravel())
     # return mask.reshape((len(doselut[1]), len(doselut[0])))
 
     grid = c.contains_points(dosegridpoints)
-    grid = grid.reshape((len(doselut[1]), len(doselut[0])))
+    if dd['x_lut_index'] == 0:  # X values across columns
+        grid = grid.reshape((len(doselut[1]), len(doselut[0])))
+    else:  # decubitus
+        grid = grid.reshape((len(doselut[0]), len(doselut[1]))).T
 
     return grid
 
 
 def calculate_contour_dvh(mask, doseplane, maxdose, dd, id, structure):
     """Calculate the differential DVH for the given contour and dose plane."""
     # Multiply the structure mask by the dose plane to get the dose mask
     mask = ma.array(doseplane * dd['dosegridscaling'] * 100, mask=~mask)
     # Calculate the differential dvh
     hist, edges = np.histogram(mask.compressed(),
                                bins=maxdose,
                                range=(0, maxdose))
 
     # Calculate the volume for the contour for the given dose plane
-    vol = sum(hist) * ((np.mean(np.diff(dd['lut'][0]))) *
-                       (np.mean(np.diff(dd['lut'][1]))) *
+    vol = sum(hist) * (abs(np.mean(np.diff(dd['lut'][0]))) *
+                       abs(np.mean(np.diff(dd['lut'][1]))) *
                        (structure['thickness']))
     return hist, vol
 
 
 def structure_extents(coords):
     """Determine structure extents in patient coordinates.
 
@@ -310,51 +354,69 @@
 
 def dosegrid_extents_indices(extents, dd, padding=1):
     """Determine dose grid extents from structure extents as array indices.
 
     Parameters
     ----------
     extents : list
-        Structure extents in patient coordintes: [xmin, ymin, xmax, ymax].
+        Structure extents in patient coordinates: [xmin, ymin, xmax, ymax].
         If an empty list, no structure extents will be used in the calculation.
     dd : dict
         Dose data from dicomparser.GetDoseData.
     padding : int, optional
         Pixel padding around the structure extents.
 
     Returns
     -------
     list
-        Dose grid extents in pixel coordintes as array indices:
-        [xmin, ymin, xmax, ymax].
+        Dose grid extents in pixel coordinates as array indices:
+        [col_min, row_min, col_max, row_max].
     """
+    col_lut, row_lut = dd['lut']
+    num_cols = len(col_lut)
+    num_rows = len(row_lut)
     if not len(extents):
-        return [0, 0, dd['lut'][0].shape[0] - 1, dd['lut'][1].shape[0] - 1]
-    dgxmin = np.argmin(np.fabs(dd['lut'][0] - extents[0])) - padding
-    if dd['lut'][0][dgxmin] > extents[0]:
-        dgxmin -= 1
-    dgxmax = np.argmin(np.fabs(dd['lut'][0] - extents[2])) + padding
-    dgymin = np.argmin(np.fabs(dd['lut'][1] - extents[1])) - padding
-    dgymax = np.argmin(np.fabs(dd['lut'][1] - extents[3])) + padding
-    dgxmin = 0 if dgxmin < 0 else dgxmin
-    dgymin = 0 if dgymin < 0 else dgymin
-    if dgxmax == dd['lut'][0].shape[0]:
-        dgxmax = dd['lut'][0].shape[0] - 1
-    if dgymax == dd['lut'][1].shape[0]:
-        dgymax = dd['lut'][1].shape[0] - 1
-    return [dgxmin, dgymin, dgxmax, dgymax]
+        return [0, 0, num_cols - 1, num_rows - 1]
+
+    if dd['x_lut_index'] == 0:  # X is across rows
+        strx_col_min, strx_col_max = extents[0], extents[2]
+        strx_row_min, strx_row_max = extents[1], extents[3]
+    else:  # decubitus case, X down rows
+        strx_col_min, strx_col_max = extents[1], extents[3]
+        strx_row_min, strx_row_max = extents[0], extents[2]
+
+    dg_col_min = np.argmin(np.fabs(col_lut - strx_col_min))
+    dg_col_max = np.argmin(np.fabs(col_lut - strx_col_max))
+    if dg_col_min > dg_col_max:
+        dg_col_min, dg_col_max = dg_col_max, dg_col_min
+    if col_lut[dg_col_min] > strx_col_min:
+        dg_col_min -= 1
+
+    dg_row_min = np.argmin(np.fabs(row_lut - strx_row_min))
+    dg_row_max = np.argmin(np.fabs(row_lut - strx_row_max))
+    if dg_row_min > dg_row_max:
+        dg_row_min, dg_row_max = dg_row_max, dg_row_min
+
+    # Ensure indices within array limits regardless of padding
+    dg_col_min = max(0, dg_col_min-padding)
+    dg_row_min = max(0, dg_row_min-padding)
+    dg_col_max = min(num_cols - 1, dg_col_max+padding)
+    dg_row_max = min(num_rows - 1, dg_row_max+padding)
+
+    return [dg_col_min, dg_row_min, dg_col_max, dg_row_max]
 
 
 def dosegrid_extents_positions(extents, dd):
     """Determine dose grid extents in patient coordinate indices.
 
     Parameters
     ----------
     extents : list
-        Dose grid extents in pixel coordintes: [xmin, ymin, xmax, ymax].
+        Dose grid extents in pixel coordintes:
+        [col_pos_min, row_pos_min, col_pos_max, row_pos_max].
     dd : dict
         Dose data from dicomparser.GetDoseData.
 
     Returns
     -------
     list
         Dose grid extents in patient coordintes: [xmin, ymin, xmax, ymax].
@@ -372,94 +434,125 @@
     """Determine the patient to pixel LUT based on new pixel spacing.
 
     Parameters
     ----------
     index_extents : list
         Dose grid extents as array indices.
     extents : list
-        Dose grid extents in patient coordinates.
-    new_pixel_spacing : float
-        New pixel spacing in mm
-    min_pixel_spacing : float
-        Minimum pixel spacing used to determine the new pixel spacing
+        Dose grid extents in patient coordinates:
+        [col_pos_min, row_pos_min, col_pos_max, row_pos_max].
+    new_pixel_spacing : tuple or float
+        New pixel spacing in mm (row, column).
+        If float is provided, original dose grid pixel spacing must be square.
+    min_pixel_spacing : tuple
+        Min pixel spacing used to determine new pixel spacing (row, column).
 
     Returns
     -------
     tuple
-        A tuple of lists (x, y) of patient to pixel coordinate mappings.
+        A tuple of lut lists (col lut, row lut) with the coordinates of the
+        dose grid in patient coordinates
 
     Raises
     ------
     AttributeError
         Raised if the new pixel_spacing is not a factor of the minimum pixel
         spacing.
 
     Notes
     -----
     The new pixel spacing must be a factor of the original (minimum) pixel
     spacing. For example if the original pixel spacing was ``3`` mm, the new
     pixel spacing should be: ``3 / (2^n)`` mm, where ``n`` is an integer.
+    This applies independently to both the row and column pixel spacing.
+
+    If a single float value is provided it will be applied to both row and
+    column. Additionally, the original dose grid pixel spacing must be square.
 
     Examples
     --------
     Original pixel spacing: ``3`` mm, new pixel spacing: ``0.375`` mm
     Derived via: ``(3 / 2^16) == 0.375``
 
     """
-    if (min_pixel_spacing % new_pixel_spacing != 0.0):
+    if not isinstance(new_pixel_spacing, Sequence):
+        if not (min_pixel_spacing[0] == min_pixel_spacing[1]):
+            raise AttributeError(
+                "New pixel spacing must be provided as a (row, column) tuple.")
+        else:
+            new_pixel_spacing = (new_pixel_spacing, new_pixel_spacing)
+    if (min_pixel_spacing[0] % new_pixel_spacing[0] != 0.0):
+        raise AttributeError(
+            "New row pixel spacing must be a factor of %s/(2^n),"
+            % min_pixel_spacing[0] +
+            " where n is an integer. Value provided was %s."
+            % new_pixel_spacing[0])
+    if (min_pixel_spacing[1] % new_pixel_spacing[1] != 0.0):
         raise AttributeError(
-            "New pixel spacing must be a factor of %g/(2^n),"
-            % min_pixel_spacing +
-            " where n is an integer. Value provided was %g."
-            % new_pixel_spacing)
-    sampling_rate = np.array([
-        abs(index_extents[0] - index_extents[2]),
-        abs(index_extents[1] - index_extents[3])
-    ])
-    xsamples, ysamples = sampling_rate * min_pixel_spacing / new_pixel_spacing
-    x = np.linspace(extents[0], extents[2], int(xsamples), dtype=np.float)
-    y = np.linspace(extents[1], extents[3], int(ysamples), dtype=np.float)
-    return x, y
+            "New column pixel spacing must be a factor of %s/(2^n),"
+            % min_pixel_spacing[1] +
+            " where n is an integer. Value provided was %s."
+            % new_pixel_spacing[1])
+
+    # Existing number of cols, rows
+    num_cols = abs(index_extents[0] - index_extents[2])
+    num_rows = abs(index_extents[1] - index_extents[3])
+
+    col_samples = round(num_cols * min_pixel_spacing[1] / new_pixel_spacing[1])
+    row_samples = round(num_rows * min_pixel_spacing[0] / new_pixel_spacing[0])
+
+    col_lut = np.linspace(
+        extents[0], extents[2], int(col_samples), dtype=np.float64
+    )
+    row_lut = np.linspace(
+        extents[1], extents[3], int(row_samples), dtype=np.float64
+    )
+    return col_lut, row_lut
 
 
 def get_interpolated_dose(dose, z, resolution, extents):
     """Get interpolated dose for the given z, resolution & array extents.
 
     Parameters
     ----------
     dose : DicomParser
         A DicomParser instance of an RT Dose.
     z : float
         Index in mm of z plane of dose grid.dose
-    resolution : float
+    resolution : tuple
         Interpolation resolution less than or equal to dose grid pixel spacing.
+        Provided in (row, col) format.
     extents : list
         Dose grid index extents.
 
     Returns
     -------
     ndarray
         Interpolated dose grid with a shape larger than the input dose grid.
     """
     # Return the dose bounded by extents if interpolation is not required
     d = dose.GetDoseGrid(z)
+    if not d.size:
+        return d  # cannot take 2d index below if empty
     extent_dose = d[extents[1]:extents[3],
                     extents[0]:extents[2]] if len(extents) else d
     if not resolution:
         return extent_dose
     if not skimage_available:
         raise ImportError(
             "scikit-image must be installed to perform DVH interpolation.")
     scale = (np.array(dose.ds.PixelSpacing) / resolution).tolist()
     interp_dose = rescale(
         extent_dose,
         scale=scale,
-        mode='symmetric',
         order=1,
-        preserve_range=True)
+        mode='symmetric',
+        preserve_range=True,
+        channel_axis=None
+    )
     return interp_dose
 
 
 def interpolate_between_planes(planes, n=2):
     """Interpolate n additional structure planes (segments) in between planes.
 
     Parameters
```

### Comparing `dicompyler-core-0.5.5/dicompylercore/util.py` & `dicompyler-core-0.5.6/dicompylercore/util.py`

 * *Files identical despite different names*

### Comparing `dicompyler-core-0.5.5/docs/Makefile` & `dicompyler-core-0.5.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dicompyler-core-0.5.5/docs/conf.py` & `dicompyler-core-0.5.6/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
+import dicompylercore
 import sys
 import os
 
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
@@ -27,29 +28,29 @@
 project_root = os.path.dirname(cwd)
 
 # Insert the project root dir as the first element in the PYTHONPATH.
 # This lets us ensure that the source package is imported, and that its
 # version is used.
 sys.path.insert(0, project_root)
 
-import dicompylercore
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode',
               'sphinx.ext.napoleon']
 
 autodoc_mock_imports = [
     'numpy', 'dicom', 'pydicom', 'pydicom', 'dicom',
-    'PIL', 'numpy', 'matplotlib', 'skimage']
+    'PIL', 'numpy.core', 'matplotlib', 'skimage', 'scipy']
+autodoc_member_order = 'bysource'
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
 
@@ -57,15 +58,15 @@
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'dicompyler-core'
-copyright = u'2016-2019, Aditya Panchal'
+copyright = u'2016-2023, Aditya Panchal'
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
 version = dicompylercore.__version__
@@ -196,21 +197,21 @@
 htmlhelp_basename = 'dicompyler-coredoc'
 
 
 # -- Options for LaTeX output ------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
-    #'papersize': 'letterpaper',
+    # 'papersize': 'letterpaper',
 
     # The font size ('10pt', '11pt' or '12pt').
-    #'pointsize': '10pt',
+    # 'pointsize': '10pt',
 
     # Additional stuff for the LaTeX preamble.
-    #'preamble': '',
+    # 'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto/manual]).
 latex_documents = [
     ('index', 'dicompyler-core.tex',
@@ -274,7 +275,10 @@
 #texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
 #texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 #texinfo_no_detailmenu = False
+
+# Set autoclass_content to show both class and init docstring
+autoclass_content = "both"
```

### Comparing `dicompyler-core-0.5.5/docs/index.rst` & `dicompyler-core-0.5.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dicompyler-core-0.5.5/docs/make.bat` & `dicompyler-core-0.5.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dicompyler-core-0.5.5/setup.py` & `dicompyler-core-0.5.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 test_requirements = [
     # TODO: put package test requirements here
 ]
 
 setup(
     name='dicompyler-core',
-    version='0.5.5',
+    version='0.5.6',
     description="A library of core radiation therapy modules for DICOM / " +
                 "DICOM RT used by dicompyler",
     long_description=readme,
     author="Aditya Panchal",
     author_email='apanchal@bastula.org',
     url='https://github.com/dicompyler/dicompyler-core',
     packages=[
@@ -36,38 +36,35 @@
         "six>=1.5",
         "pydicom>=0.9.9",
         "matplotlib>=1.3.0"
     ],
     extras_require={
         'image': ["pillow>=1.0"],
         'dvhinterpolation': ["scikit-image"],
-        'volume': ["shapely>=1.6"]
+        'volume': ["shapely>=1.6"],
+        'doseinterpolation': ["scipy"]
     },
-    dependency_links=[
-        "git+https://github.com/darcymason/pydicom.git#egg=pydicom-1.0.0a1"
-    ],
     license="BSD License",
     zip_safe=False,
     keywords=[
         'dicompyler-core',
         'dicompylercore',
         'dicompyler'
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Healthcare Industry',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
         'Natural Language :: English',
-        "Programming Language :: Python :: 2",
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering :: Medical Science Apps.',
         'Topic :: Scientific/Engineering :: Physics'
     ],
     test_suite='tests',
     tests_require=test_requirements
 )
```

### Comparing `dicompyler-core-0.5.5/tests/test_dicomparser.py` & `dicompyler-core-0.5.6/tests/test_dicomparser.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,22 @@
         ct_0_dcm = os.path.join(example_data, "ct.0.dcm")
         self.dp = dicomparser.DicomParser(ct_0_dcm)
 
     def test_file_import(self):
         """Test if a standard DICOM file can be parsed."""
         self.assertEqual(self.dp.GetSOPClassUID(), 'ct')
 
+    def test_missing_file_meta(self):
+        """Test if a standard DICOM file can be parsed."""
+        file_meta_original = self.dp.ds.file_meta.copy()
+        self.dp.ds.file_meta.clear()
+        dp = dicomparser.DicomParser(self.dp.ds)
+        file_meta_fixed = dp.ds.file_meta
+        self.assertEqual(file_meta_original, file_meta_fixed)
+
     def test_dataset_import(self):
         """Test if a pydicom dataset file can be parsed."""
         dp1 = dicomparser.DicomParser(self.dp.ds)
         self.assertEqual(self.dp.ds, dp1.ds)
 
     def test_study_info(self):
         """Test if the study info can be parsed."""
@@ -131,16 +139,16 @@
         """Test if the image can be generated."""
         image = 90
         self.assertEqual(self.dp.GetImage().getpixel((255, 254)), image)
 
     def test_patient_to_pixel_lut(self):
         """Test if the image transformation matrix (LUT) can be generated."""
         lutvalue = 273.925909
-        self.assertAlmostEqual(
-            self.dp.GetPatientToPixelLUT()[0][-1], lutvalue)
+        doselut = self.dp.GetPatientToPixelLUT()
+        self.assertAlmostEqual(doselut[0][-1], lutvalue)
 
 
 class TestRTStructureSet(unittest.TestCase):
     """Unit tests for RT Structure Set Modality."""
 
     def setUp(self):
         """Setup the files for RT Structure Set modality testing."""
@@ -300,14 +308,22 @@
         assert_array_equal(self.dp.GetDoseGrid(-10000), array([]))
 
     def test_isodose_points(self):
         """Test if isodose points can be generated from the dose grid."""
         points = [(106, 20), (108, 20), (110, 20)]
         self.assertEqual(self.dp.GetIsodosePoints()[0:3], points)
 
+    def test_isodose_points_memmap(self):
+        """Test if isodose points can be generated via a memmapped dose grid."""
+        points = [(106, 20), (108, 20), (110, 20)]
+        dp = dicomparser.DicomParser(
+            os.path.join(example_data, "rtdose.dcm"),
+            memmap_pixel_array=True)
+        self.assertEqual(dp.GetIsodosePoints()[0:3], points)
+
     def test_dose_data(self):
         """Test if the dose data can be parsed."""
         data = {
             'position': mv(
                 DSfloat, ['-228.6541915', '-419.2444776', '-122.4407']),
             'orientation':
                 mv(DSfloat, ['1', '0.0', '0.0', '0.0', '1', '0.0']),
@@ -321,19 +337,28 @@
             'doseunits': 'GY',
             'dosetype': 'PHYSICAL',
             'dosecomment': '',
             'dosesummationtype': 'PLAN',
             'dosegridscaling': 1.4e-05,
             'dosemax': 1048626.0,
             'lut': 253.8458085,
-            'fraction': ''
+            'fraction': '',
+            'x_lut_index': 0,
         }
         dosedata = self.dp.GetDoseData()
         # Pop the LUT numpy array
         assert_array_almost_equal(
             dosedata.pop('lut')[0][-1], data.pop('lut'))
         self.assertEqual(dosedata, data)
+        dp = dicomparser.DicomParser(
+            os.path.join(example_data, "rtdose.dcm"),
+            memmap_pixel_array=True)
+        dosedata = dp.GetDoseData()
+        data['lut'] = 253.8458085
+        assert_array_almost_equal(
+            dosedata.pop('lut')[0][-1], data.pop('lut'))
+        self.assertEqual(dosedata, data)
 
 
 if __name__ == '__main__':
     import sys
     sys.exit(unittest.main())
```

### Comparing `dicompyler-core-0.5.5/tests/test_dvh.py` & `dicompyler-core-0.5.6/tests/test_dvh.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,25 @@
         # Test if rx_dose is not included in initial constructor
         # but is accessed as if it is provided
         with self.assertRaises(AttributeError):
             self.dvh.relative_dose()
         with self.assertRaises(AttributeError):
             self.dvh.relative_dose(14).absolute_dose()
 
+    def test_dvh_dosescaling(self):
+        """Test if the DVH Dose Scaling is applied properly."""
+        rtdose_dcm = os.path.join(example_data, "rtdose.dcm")
+        rtdose = dicomparser.DicomParser(rtdose_dcm)
+        rtdose.ds.DVHSequence[7].DVHDoseScaling = 2
+        scaleddvh = dvh.DVH.from_dicom_dvh(rtdose.ds, 9)
+        self.assertEqual(self.dvh.max * 2, scaleddvh.max)
+        self.assertEqual(self.dvh.min * 2, scaleddvh.min)
+        self.assertEqual(self.dvh.mean * 2, scaleddvh.mean)
+        self.assertEqual(self.dvh.volume, scaleddvh.volume)
+
     def test_dvh_properties(self):
         """Test if the DVH properties can be derived."""
         self.assertEqual(self.dvh.max, 14.579999999999734)
         self.assertEqual(self.dvh.min, 14.069999999999744)
         self.assertEqual(self.dvh.mean, 14.285830178442307)
         self.assertEqual(self.dvh.volume, 12.809180549338803)
```

### Comparing `dicompyler-core-0.5.5/tests/testdata/example_data/ct.0.dcm` & `dicompyler-core-0.5.6/tests/testdata/example_data/ct.0.dcm`

 * *Files identical despite different names*

### Comparing `dicompyler-core-0.5.5/tests/testdata/example_data/rtdose.dcm` & `dicompyler-core-0.5.6/tests/testdata/example_data/rtdose.dcm`

 * *Files identical despite different names*

### Comparing `dicompyler-core-0.5.5/tests/testdata/example_data/rtplan.dcm` & `dicompyler-core-0.5.6/tests/testdata/example_data/rtplan.dcm`

 * *Files identical despite different names*

### Comparing `dicompyler-core-0.5.5/tests/testdata/example_data/rtss.dcm` & `dicompyler-core-0.5.6/tests/testdata/example_data/rtss.dcm`

 * *Files identical despite different names*

