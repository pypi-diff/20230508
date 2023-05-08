# Comparing `tmp/gcp-releasetool-1.9.0.tar.gz` & `tmp/gcp-releasetool-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gcp-releasetool-1.9.0.tar", last modified: Wed Oct 26 07:09:01 2022, max compression
+gzip compressed data, was "dist/gcp-releasetool-1.9.1.tar", last modified: Wed Nov  2 21:18:05 2022, max compression
```

## Comparing `gcp-releasetool-1.9.0.tar` & `gcp-releasetool-1.9.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-26 07:09:01.000000 gcp-releasetool-1.9.0/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-26 07:09:01.000000 gcp-releasetool-1.9.0/gcp_releasetool.egg-info/
--rw-r--r--   0 root         (0)     1003        1 2022-10-26 07:09:00.000000 gcp-releasetool-1.9.0/gcp_releasetool.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003      141 2022-10-26 07:09:00.000000 gcp-releasetool-1.9.0/gcp_releasetool.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003       37 2022-10-26 07:09:00.000000 gcp-releasetool-1.9.0/gcp_releasetool.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003     1565 2022-10-26 07:09:00.000000 gcp-releasetool-1.9.0/gcp_releasetool.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003       59 2022-10-26 07:09:00.000000 gcp-releasetool-1.9.0/gcp_releasetool.egg-info/entry_points.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-26 07:09:00.000000 gcp-releasetool-1.9.0/gcp_releasetool.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      570 2022-10-26 07:09:00.000000 gcp-releasetool-1.9.0/gcp_releasetool.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/LICENSE
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-26 07:09:01.000000 gcp-releasetool-1.9.0/releasetool/
--rw-rw-r--   0 root         (0)     1003     1137 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/secrets.py
--rw-rw-r--   0 root         (0)     1003     1901 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/update_check.py
--rw-rw-r--   0 root         (0)     1003     9724 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/github.py
--rw-rw-r--   0 root         (0)     1003     6772 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/__main__.py
--rw-rw-r--   0 root         (0)     1003      638 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/__init__.py
--rw-rw-r--   0 root         (0)     1003     4056 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/git.py
--rw-rw-r--   0 root         (0)     1003     4296 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/circleci.py
--rw-rw-r--   0 root         (0)     1003     2367 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/filehelpers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-26 07:09:01.000000 gcp-releasetool-1.9.0/releasetool/commands/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-26 07:09:01.000000 gcp-releasetool-1.9.0/releasetool/commands/start/
--rw-rw-r--   0 root         (0)     1003     2268 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/commands/start/python_tool.py
--rw-rw-r--   0 root         (0)     1003     7501 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/commands/start/nodejs.py
--rw-rw-r--   0 root         (0)     1003     8303 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/commands/start/python.py
--rw-rw-r--   0 root         (0)     1003        0 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/commands/start/__init__.py
--rw-rw-r--   0 root         (0)     1003     8090 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/commands/start/go.py
--rw-rw-r--   0 root         (0)     1003    13934 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/commands/start/java.py
--rw-rw-r--   0 root         (0)     1003     8739 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/commands/start/ruby.py
--rw-rw-r--   0 root         (0)     1003     1958 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/commands/publish_reporter.sh
--rw-rw-r--   0 root         (0)     1003        0 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/commands/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-26 07:09:01.000000 gcp-releasetool-1.9.0/releasetool/commands/tag/
--rw-rw-r--   0 root         (0)     1003     3475 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/commands/tag/python_tool.py
--rw-rw-r--   0 root         (0)     1003     7683 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/commands/tag/nodejs.py
--rw-rw-r--   0 root         (0)     1003     5849 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/commands/tag/python.py
--rw-rw-r--   0 root         (0)     1003        0 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/commands/tag/__init__.py
--rw-rw-r--   0 root         (0)     1003     3683 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/commands/tag/java.py
--rw-rw-r--   0 root         (0)     1003     4833 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/commands/tag/dotnet.py
--rw-rw-r--   0 root         (0)     1003     1633 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/commands/tag/php.py
--rw-rw-r--   0 root         (0)     1003     8146 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/commands/tag/ruby.py
--rw-rw-r--   0 root         (0)     1003     6077 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/commands/publish_reporter.py
--rw-rw-r--   0 root         (0)     1003     6214 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/releasetool/commands/common.py
--rw-r--r--   0 root         (0)     1003       38 2022-10-26 07:09:01.000000 gcp-releasetool-1.9.0/setup.cfg
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-26 07:09:01.000000 gcp-releasetool-1.9.0/protos/
--rw-rw-r--   0 root         (0)     1003        0 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/protos/__init__.py
--rw-rw-r--   0 root         (0)     1003    13221 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/protos/kokoro_api_pb2.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-26 07:09:01.000000 gcp-releasetool-1.9.0/autorelease/
--rw-rw-r--   0 root         (0)     1003     3181 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/autorelease/kokoro.py
--rw-rw-r--   0 root         (0)     1003     9001 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/autorelease/github.py
--rw-rw-r--   0 root         (0)     1003     2799 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/autorelease/__main__.py
--rw-rw-r--   0 root         (0)     1003        0 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/autorelease/__init__.py
--rw-rw-r--   0 root         (0)     1003     1787 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/autorelease/reporter.py
--rw-rw-r--   0 root         (0)     1003     7420 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/autorelease/trigger.py
--rw-rw-r--   0 root         (0)     1003     3170 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/autorelease/common.py
--rw-rw-r--   0 root         (0)     1003     5258 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/autorelease/tag.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-26 07:09:01.000000 gcp-releasetool-1.9.0/tests/
--rw-rw-r--   0 root         (0)     1003     1715 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/tests/test_publish_reporter.py
--rw-rw-r--   0 root         (0)     1003     6835 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/tests/test_autorelease_tag.py
--rw-rw-r--   0 root         (0)     1003    11735 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/tests/test_autorelease_trigger.py
--rw-rw-r--   0 root         (0)     1003        0 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/tests/__init__.py
--rw-rw-r--   0 root         (0)     1003    65497 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/tests/common_test.py
--rw-rw-r--   0 root         (0)     1003       34 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/tests/test_dummy.py
--rw-rw-r--   0 root         (0)     1003     2013 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/README.md
--rw-rw-r--   0 root         (0)     1003       60 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/MANIFEST.in
--rw-rw-r--   0 root         (0)     1003     1861 2022-10-26 07:06:21.000000 gcp-releasetool-1.9.0/setup.py
--rw-r--r--   0 root         (0)     1003      570 2022-10-26 07:09:01.000000 gcp-releasetool-1.9.0/PKG-INFO
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-02 21:18:05.000000 gcp-releasetool-1.9.1/
+-rw-rw-r--   0 root         (0)     1003     2013 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/README.md
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-02 21:18:05.000000 gcp-releasetool-1.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003     6835 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/tests/test_autorelease_tag.py
+-rw-rw-r--   0 root         (0)     1003    65497 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/tests/common_test.py
+-rw-rw-r--   0 root         (0)     1003    11735 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/tests/test_autorelease_trigger.py
+-rw-rw-r--   0 root         (0)     1003        0 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/tests/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1715 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/tests/test_publish_reporter.py
+-rw-rw-r--   0 root         (0)     1003       34 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/tests/test_dummy.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-02 21:18:05.000000 gcp-releasetool-1.9.1/releasetool/
+-rw-rw-r--   0 root         (0)     1003     2367 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/filehelpers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-02 21:18:05.000000 gcp-releasetool-1.9.1/releasetool/commands/
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-02 21:18:05.000000 gcp-releasetool-1.9.1/releasetool/commands/start/
+-rw-rw-r--   0 root         (0)     1003    13934 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/commands/start/java.py
+-rw-rw-r--   0 root         (0)     1003     8090 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/commands/start/go.py
+-rw-rw-r--   0 root         (0)     1003     7501 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/commands/start/nodejs.py
+-rw-rw-r--   0 root         (0)     1003        0 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/commands/start/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2268 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/commands/start/python_tool.py
+-rw-rw-r--   0 root         (0)     1003     8739 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/commands/start/ruby.py
+-rw-rw-r--   0 root         (0)     1003     8303 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/commands/start/python.py
+-rw-rw-r--   0 root         (0)     1003     1958 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/commands/publish_reporter.sh
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-02 21:18:05.000000 gcp-releasetool-1.9.1/releasetool/commands/tag/
+-rw-rw-r--   0 root         (0)     1003     3683 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/commands/tag/java.py
+-rw-rw-r--   0 root         (0)     1003     4833 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/commands/tag/dotnet.py
+-rw-rw-r--   0 root         (0)     1003     7683 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/commands/tag/nodejs.py
+-rw-rw-r--   0 root         (0)     1003        0 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/commands/tag/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1633 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/commands/tag/php.py
+-rw-rw-r--   0 root         (0)     1003     3475 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/commands/tag/python_tool.py
+-rw-rw-r--   0 root         (0)     1003     8146 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/commands/tag/ruby.py
+-rw-rw-r--   0 root         (0)     1003     5849 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/commands/tag/python.py
+-rw-rw-r--   0 root         (0)     1003        0 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/commands/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6077 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/commands/publish_reporter.py
+-rw-rw-r--   0 root         (0)     1003     6214 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/commands/common.py
+-rw-rw-r--   0 root         (0)     1003      638 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4056 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/git.py
+-rw-rw-r--   0 root         (0)     1003     4296 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/circleci.py
+-rw-rw-r--   0 root         (0)     1003     9724 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/github.py
+-rw-rw-r--   0 root         (0)     1003     6772 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/__main__.py
+-rw-rw-r--   0 root         (0)     1003     1901 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/update_check.py
+-rw-rw-r--   0 root         (0)     1003     1137 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/releasetool/secrets.py
+-rw-rw-r--   0 root         (0)     1003     1861 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/setup.py
+-rw-r--r--   0 root         (0)     1003       38 2022-11-02 21:18:05.000000 gcp-releasetool-1.9.1/setup.cfg
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-02 21:18:05.000000 gcp-releasetool-1.9.1/autorelease/
+-rw-rw-r--   0 root         (0)     1003     5258 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/autorelease/tag.py
+-rw-rw-r--   0 root         (0)     1003     1787 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/autorelease/reporter.py
+-rw-rw-r--   0 root         (0)     1003        0 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/autorelease/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3181 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/autorelease/kokoro.py
+-rw-rw-r--   0 root         (0)     1003     9001 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/autorelease/github.py
+-rw-rw-r--   0 root         (0)     1003     3170 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/autorelease/common.py
+-rw-rw-r--   0 root         (0)     1003     7420 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/autorelease/trigger.py
+-rw-rw-r--   0 root         (0)     1003     2799 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/autorelease/__main__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-02 21:18:05.000000 gcp-releasetool-1.9.1/gcp_releasetool.egg-info/
+-rw-r--r--   0 root         (0)     1003       59 2022-11-02 21:18:05.000000 gcp-releasetool-1.9.1/gcp_releasetool.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0)     1003       37 2022-11-02 21:18:05.000000 gcp-releasetool-1.9.1/gcp_releasetool.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-11-02 21:18:05.000000 gcp-releasetool-1.9.1/gcp_releasetool.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003     1565 2022-11-02 21:18:05.000000 gcp-releasetool-1.9.1/gcp_releasetool.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-11-02 21:18:05.000000 gcp-releasetool-1.9.1/gcp_releasetool.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003      570 2022-11-02 21:18:05.000000 gcp-releasetool-1.9.1/gcp_releasetool.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      141 2022-11-02 21:18:05.000000 gcp-releasetool-1.9.1/gcp_releasetool.egg-info/requires.txt
+-rw-rw-r--   0 root         (0)     1003       60 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/MANIFEST.in
+-rw-rw-r--   0 root         (0)     1003    11358 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/LICENSE
+-rw-r--r--   0 root         (0)     1003      570 2022-11-02 21:18:05.000000 gcp-releasetool-1.9.1/PKG-INFO
+drwxr-sr-x   0 root         (0)     1003        0 2022-11-02 21:18:05.000000 gcp-releasetool-1.9.1/protos/
+-rw-rw-r--   0 root         (0)     1003        0 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/protos/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13221 2022-11-02 21:15:26.000000 gcp-releasetool-1.9.1/protos/kokoro_api_pb2.py
```

### Comparing `gcp-releasetool-1.9.0/gcp_releasetool.egg-info/SOURCES.txt` & `gcp-releasetool-1.9.1/gcp_releasetool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/gcp_releasetool.egg-info/PKG-INFO` & `gcp-releasetool-1.9.1/gcp_releasetool.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: gcp-releasetool
-Version: 1.9.0
+Version: 1.9.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Google LLC
 Author-email: theaflowers@google.com
 License: Apache 2.0
 Description: UNKNOWN
 Platform: Posix; MacOS X; Windows
```

### Comparing `gcp-releasetool-1.9.0/LICENSE` & `gcp-releasetool-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/secrets.py` & `gcp-releasetool-1.9.1/releasetool/secrets.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/update_check.py` & `gcp-releasetool-1.9.1/releasetool/update_check.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/github.py` & `gcp-releasetool-1.9.1/releasetool/github.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/__main__.py` & `gcp-releasetool-1.9.1/releasetool/__main__.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/__init__.py` & `gcp-releasetool-1.9.1/releasetool/__init__.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/git.py` & `gcp-releasetool-1.9.1/releasetool/git.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/circleci.py` & `gcp-releasetool-1.9.1/releasetool/circleci.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/filehelpers.py` & `gcp-releasetool-1.9.1/releasetool/filehelpers.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/commands/start/python_tool.py` & `gcp-releasetool-1.9.1/releasetool/commands/start/python_tool.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/commands/start/nodejs.py` & `gcp-releasetool-1.9.1/releasetool/commands/start/nodejs.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/commands/start/python.py` & `gcp-releasetool-1.9.1/releasetool/commands/start/python.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/commands/start/go.py` & `gcp-releasetool-1.9.1/releasetool/commands/start/go.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/commands/start/java.py` & `gcp-releasetool-1.9.1/releasetool/commands/start/java.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/commands/start/ruby.py` & `gcp-releasetool-1.9.1/releasetool/commands/start/ruby.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/commands/publish_reporter.sh` & `gcp-releasetool-1.9.1/releasetool/commands/publish_reporter.sh`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/commands/tag/python_tool.py` & `gcp-releasetool-1.9.1/releasetool/commands/tag/python_tool.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/commands/tag/nodejs.py` & `gcp-releasetool-1.9.1/releasetool/commands/tag/nodejs.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/commands/tag/python.py` & `gcp-releasetool-1.9.1/releasetool/commands/tag/python.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/commands/tag/java.py` & `gcp-releasetool-1.9.1/releasetool/commands/tag/java.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/commands/tag/dotnet.py` & `gcp-releasetool-1.9.1/releasetool/commands/tag/dotnet.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/commands/tag/php.py` & `gcp-releasetool-1.9.1/releasetool/commands/tag/php.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/commands/tag/ruby.py` & `gcp-releasetool-1.9.1/releasetool/commands/tag/ruby.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/commands/publish_reporter.py` & `gcp-releasetool-1.9.1/releasetool/commands/publish_reporter.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/releasetool/commands/common.py` & `gcp-releasetool-1.9.1/releasetool/commands/common.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/protos/kokoro_api_pb2.py` & `gcp-releasetool-1.9.1/protos/kokoro_api_pb2.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/autorelease/kokoro.py` & `gcp-releasetool-1.9.1/autorelease/kokoro.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/autorelease/github.py` & `gcp-releasetool-1.9.1/autorelease/github.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/autorelease/__main__.py` & `gcp-releasetool-1.9.1/autorelease/__main__.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/autorelease/reporter.py` & `gcp-releasetool-1.9.1/autorelease/reporter.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/autorelease/trigger.py` & `gcp-releasetool-1.9.1/autorelease/trigger.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/autorelease/common.py` & `gcp-releasetool-1.9.1/autorelease/common.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/autorelease/tag.py` & `gcp-releasetool-1.9.1/autorelease/tag.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/tests/test_publish_reporter.py` & `gcp-releasetool-1.9.1/tests/test_publish_reporter.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/tests/test_autorelease_tag.py` & `gcp-releasetool-1.9.1/tests/test_autorelease_tag.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/tests/test_autorelease_trigger.py` & `gcp-releasetool-1.9.1/tests/test_autorelease_trigger.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/tests/common_test.py` & `gcp-releasetool-1.9.1/tests/common_test.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/README.md` & `gcp-releasetool-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-1.9.0/setup.py` & `gcp-releasetool-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import setuptools
 
 name = 'gcp-releasetool'
 description = ''
-version = "1.9.0"
+version = "1.9.1"
 release_status = 'Development Status :: 3 - Alpha'
 dependencies = [
     "requests",
     "attrs",
     "click>=8.0.4, <8.1.0",
     "cryptography",
     "google-auth",
```

### Comparing `gcp-releasetool-1.9.0/PKG-INFO` & `gcp-releasetool-1.9.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: gcp-releasetool
-Version: 1.9.0
+Version: 1.9.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Google LLC
 Author-email: theaflowers@google.com
 License: Apache 2.0
 Description: UNKNOWN
 Platform: Posix; MacOS X; Windows
```

