# Comparing `tmp/ipykernel-6.9.1.tar.gz` & `tmp/ipykernel-6.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipykernel-6.9.1.tar", last modified: Tue Feb 15 15:52:53 2022, max compression
+gzip compressed data, was "ipykernel-6.9.2.tar", last modified: Mon Mar 14 11:21:48 2022, max compression
```

## Comparing `ipykernel-6.9.1.tar` & `ipykernel-6.9.2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:52:53.615234 ipykernel-6.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)    54001 2022-02-15 15:52:14.000000 ipykernel-6.9.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2022-02-15 15:52:14.000000 ipykernel-6.9.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     2835 2022-02-15 15:52:14.000000 ipykernel-6.9.1/COPYING.md
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-02-15 15:52:14.000000 ipykernel-6.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1509 2022-02-15 15:52:53.615234 ipykernel-6.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-02-15 15:52:14.000000 ipykernel-6.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-02-15 15:52:14.000000 ipykernel-6.9.1/RELEASE.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:52:53.607234 ipykernel-6.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7437 2022-02-15 15:52:14.000000 ipykernel-6.9.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    10092 2022-02-15 15:52:14.000000 ipykernel-6.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-02-15 15:52:14.000000 ipykernel-6.9.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7258 2022-02-15 15:52:14.000000 ipykernel-6.9.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-02-15 15:52:14.000000 ipykernel-6.9.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:52:53.607234 ipykernel-6.9.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:52:53.607234 ipykernel-6.9.1/examples/embedding/
--rw-r--r--   0 runner    (1001) docker     (121)     2427 2022-02-15 15:52:14.000000 ipykernel-6.9.1/examples/embedding/inprocess_qtconsole.py
--rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-02-15 15:52:14.000000 ipykernel-6.9.1/examples/embedding/inprocess_terminal.py
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-02-15 15:52:14.000000 ipykernel-6.9.1/examples/embedding/internal_ipkernel.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2822 2022-02-15 15:52:14.000000 ipykernel-6.9.1/examples/embedding/ipkernel_qtapp.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4308 2022-02-15 15:52:14.000000 ipykernel-6.9.1/examples/embedding/ipkernel_wxapp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:52:53.611234 ipykernel-6.9.1/ipykernel/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4047 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/_eventloop_macos.py
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-02-15 15:52:35.000000 ipykernel-6.9.1/ipykernel/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:52:53.611234 ipykernel-6.9.1/ipykernel/comm/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/comm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5485 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/comm/comm.py
--rw-r--r--   0 runner    (1001) docker     (121)     4012 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/comm/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     2554 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     3744 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/connect.py
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/control.py
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/datapub.py
--rw-r--r--   0 runner    (1001) docker     (121)    24376 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/debugger.py
--rw-r--r--   0 runner    (1001) docker     (121)     2632 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/displayhook.py
--rw-r--r--   0 runner    (1001) docker     (121)     2057 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/embed.py
--rw-r--r--   0 runner    (1001) docker     (121)    13442 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/eventloops.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:52:53.611234 ipykernel-6.9.1/ipykernel/gui/
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/gui/gtk3embed.py
--rw-r--r--   0 runner    (1001) docker     (121)     3123 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/gui/gtkembed.py
--rw-r--r--   0 runner    (1001) docker     (121)     4358 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/heartbeat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:52:53.611234 ipykernel-6.9.1/ipykernel/inprocess/
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/inprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3388 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/inprocess/blocking.py
--rw-r--r--   0 runner    (1001) docker     (121)     2534 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/inprocess/channels.py
--rw-r--r--   0 runner    (1001) docker     (121)     7268 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/inprocess/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/inprocess/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     6878 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/inprocess/ipkernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2736 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/inprocess/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/inprocess/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:52:53.611234 ipykernel-6.9.1/ipykernel/inprocess/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/inprocess/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4196 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/inprocess/tests/test_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     3353 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/inprocess/tests/test_kernelmanager.py
--rw-r--r--   0 runner    (1001) docker     (121)    19633 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/iostream.py
--rw-r--r--   0 runner    (1001) docker     (121)    21623 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/ipkernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4936 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/jsonutil.py
--rw-r--r--   0 runner    (1001) docker     (121)    27407 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/kernelapp.py
--rw-r--r--   0 runner    (1001) docker     (121)    41176 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/kernelbase.py
--rw-r--r--   0 runner    (1001) docker     (121)     7299 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/kernelspec.py
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     4064 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/parentpoller.py
--rw-r--r--   0 runner    (1001) docker     (121)    12404 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/pickleutil.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:52:53.611234 ipykernel-6.9.1/ipykernel/pylab/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/pylab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/pylab/backend_inline.py
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/pylab/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:52:53.611234 ipykernel-6.9.1/ipykernel/resources/
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/resources/logo-32x32.png
--rw-r--r--   0 runner    (1001) docker     (121)     2180 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/resources/logo-64x64.png
--rw-r--r--   0 runner    (1001) docker     (121)     6171 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:52:53.615234 ipykernel-6.9.1/ipykernel/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      930 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/tests/_asyncio_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1892 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (121)     4197 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/tests/test_connect.py
--rw-r--r--   0 runner    (1001) docker     (121)     7746 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/tests/test_debugger.py
--rw-r--r--   0 runner    (1001) docker     (121)     5003 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/tests/test_embed_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/tests/test_eventloop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/tests/test_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     3487 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/tests/test_jsonutil.py
--rw-r--r--   0 runner    (1001) docker     (121)    16698 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/tests/test_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4220 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/tests/test_kernelspec.py
--rw-r--r--   0 runner    (1001) docker     (121)    16096 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/tests/test_message_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/tests/test_pickleutil.py
--rw-r--r--   0 runner    (1001) docker     (121)     1873 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/tests/test_start_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     5737 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/tests/test_zmq_shell.py
--rw-r--r--   0 runner    (1001) docker     (121)     5679 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/trio_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)    23065 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel/zmqshell.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 15:52:53.611234 ipykernel-6.9.1/ipykernel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1509 2022-02-15 15:52:53.000000 ipykernel-6.9.1/ipykernel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2383 2022-02-15 15:52:53.000000 ipykernel-6.9.1/ipykernel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-15 15:52:53.000000 ipykernel-6.9.1/ipykernel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-02-15 15:52:53.000000 ipykernel-6.9.1/ipykernel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-02-15 15:52:53.000000 ipykernel-6.9.1/ipykernel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-02-15 15:52:14.000000 ipykernel-6.9.1/ipykernel_launcher.py
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-02-15 15:52:35.000000 ipykernel-6.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-02-15 15:52:53.615234 ipykernel-6.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3551 2022-02-15 15:52:14.000000 ipykernel-6.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 11:21:48.905651 ipykernel-6.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)    55851 2022-03-14 11:21:01.000000 ipykernel-6.9.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1858 2022-03-14 11:21:01.000000 ipykernel-6.9.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2835 2022-03-14 11:21:01.000000 ipykernel-6.9.2/COPYING.md
+-rw-r--r--   0 runner    (1001) docker     (121)      435 2022-03-14 11:21:01.000000 ipykernel-6.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1509 2022-03-14 11:21:48.905651 ipykernel-6.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      657 2022-03-14 11:21:01.000000 ipykernel-6.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2022-03-14 11:21:01.000000 ipykernel-6.9.2/RELEASE.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 11:21:48.893651 ipykernel-6.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     7437 2022-03-14 11:21:01.000000 ipykernel-6.9.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)    10092 2022-03-14 11:21:01.000000 ipykernel-6.9.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2022-03-14 11:21:01.000000 ipykernel-6.9.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7258 2022-03-14 11:21:01.000000 ipykernel-6.9.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-03-14 11:21:01.000000 ipykernel-6.9.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 11:21:48.889651 ipykernel-6.9.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 11:21:48.893651 ipykernel-6.9.2/examples/embedding/
+-rw-r--r--   0 runner    (1001) docker     (121)     2427 2022-03-14 11:21:01.000000 ipykernel-6.9.2/examples/embedding/inprocess_qtconsole.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-03-14 11:21:01.000000 ipykernel-6.9.2/examples/embedding/inprocess_terminal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-03-14 11:21:01.000000 ipykernel-6.9.2/examples/embedding/internal_ipkernel.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2822 2022-03-14 11:21:01.000000 ipykernel-6.9.2/examples/embedding/ipkernel_qtapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4308 2022-03-14 11:21:01.000000 ipykernel-6.9.2/examples/embedding/ipkernel_wxapp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 11:21:48.897651 ipykernel-6.9.2/ipykernel/
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4047 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/_eventloop_macos.py
+-rw-r--r--   0 runner    (1001) docker     (121)      561 2022-03-14 11:21:26.000000 ipykernel-6.9.2/ipykernel/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 11:21:48.901651 ipykernel-6.9.2/ipykernel/comm/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/comm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5485 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/comm/comm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4012 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/comm/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2554 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3744 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/connect.py
+-rw-r--r--   0 runner    (1001) docker     (121)      786 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/control.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/datapub.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24484 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2632 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/displayhook.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2057 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/embed.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13493 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/eventloops.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 11:21:48.901651 ipykernel-6.9.2/ipykernel/gui/
+-rw-r--r--   0 runner    (1001) docker     (121)      580 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/gui/gtk3embed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3123 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/gui/gtkembed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4358 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/heartbeat.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 11:21:48.901651 ipykernel-6.9.2/ipykernel/inprocess/
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/inprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3388 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/inprocess/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2534 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/inprocess/channels.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7268 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/inprocess/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/inprocess/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6878 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/inprocess/ipkernel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2736 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/inprocess/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/inprocess/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 11:21:48.901651 ipykernel-6.9.2/ipykernel/inprocess/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/inprocess/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4196 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/inprocess/tests/test_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3353 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/inprocess/tests/test_kernelmanager.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19633 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/iostream.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21531 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/ipkernel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4936 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/jsonutil.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27407 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/kernelapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43891 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/kernelbase.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7299 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/kernelspec.py
+-rw-r--r--   0 runner    (1001) docker     (121)      736 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4064 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/parentpoller.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12404 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/pickleutil.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 11:21:48.901651 ipykernel-6.9.2/ipykernel/pylab/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/pylab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      418 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/pylab/backend_inline.py
+-rw-r--r--   0 runner    (1001) docker     (121)      343 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/pylab/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 11:21:48.905651 ipykernel-6.9.2/ipykernel/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/resources/logo-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2180 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/resources/logo-64x64.png
+-rw-r--r--   0 runner    (1001) docker     (121)     6171 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 11:21:48.905651 ipykernel-6.9.2/ipykernel/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      930 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/tests/_asyncio_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1892 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4197 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/tests/test_connect.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7746 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/tests/test_debugger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5003 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/tests/test_embed_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (121)      970 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/tests/test_eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/tests/test_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3487 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/tests/test_jsonutil.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18974 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/tests/test_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4220 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/tests/test_kernelspec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16096 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/tests/test_message_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/tests/test_pickleutil.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1873 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/tests/test_start_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5737 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/tests/test_zmq_shell.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5679 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/trio_runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23065 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel/zmqshell.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 11:21:48.897651 ipykernel-6.9.2/ipykernel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1509 2022-03-14 11:21:48.000000 ipykernel-6.9.2/ipykernel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2383 2022-03-14 11:21:48.000000 ipykernel-6.9.2/ipykernel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-14 11:21:48.000000 ipykernel-6.9.2/ipykernel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2022-03-14 11:21:48.000000 ipykernel-6.9.2/ipykernel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-03-14 11:21:48.000000 ipykernel-6.9.2/ipykernel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      451 2022-03-14 11:21:01.000000 ipykernel-6.9.2/ipykernel_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2022-03-14 11:21:26.000000 ipykernel-6.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-03-14 11:21:48.905651 ipykernel-6.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3569 2022-03-14 11:21:01.000000 ipykernel-6.9.2/setup.py
```

### Comparing `ipykernel-6.9.1/CHANGELOG.md` & `ipykernel-6.9.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,33 @@
 # Changes in IPython kernel
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 6.9.2
+
+([Full Changelog](https://github.com/ipython/ipykernel/compare/v6.9.1...d6744f9e423dacc6b317b1d31805304e89cbec5d))
+
+### Bugs fixed
+
+- Catch error when shutting down kernel from the control channel [#877](https://github.com/ipython/ipykernel/pull/877) ([@ccordoba12](https://github.com/ccordoba12))
+- Only kill children in process group at shutdown [#874](https://github.com/ipython/ipykernel/pull/874) ([@minrk](https://github.com/minrk))
+- BUG: Kill subprocesses on shutdown. [#869](https://github.com/ipython/ipykernel/pull/869) ([@Carreau](https://github.com/Carreau))
+
+### Maintenance and upkeep improvements
+
+- Clean up CI [#871](https://github.com/ipython/ipykernel/pull/871) ([@blink1073](https://github.com/blink1073))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/ipython/ipykernel/graphs/contributors?from=2022-02-15&to=2022-03-14&type=c))
+
+[@blink1073](https://github.com/search?q=repo%3Aipython%2Fipykernel+involves%3Ablink1073+updated%3A2022-02-15..2022-03-14&type=Issues) | [@Carreau](https://github.com/search?q=repo%3Aipython%2Fipykernel+involves%3ACarreau+updated%3A2022-02-15..2022-03-14&type=Issues) | [@ccordoba12](https://github.com/search?q=repo%3Aipython%2Fipykernel+involves%3Accordoba12+updated%3A2022-02-15..2022-03-14&type=Issues) | [@echarles](https://github.com/search?q=repo%3Aipython%2Fipykernel+involves%3Aecharles+updated%3A2022-02-15..2022-03-14&type=Issues) | [@fabioz](https://github.com/search?q=repo%3Aipython%2Fipykernel+involves%3Afabioz+updated%3A2022-02-15..2022-03-14&type=Issues) | [@minrk](https://github.com/search?q=repo%3Aipython%2Fipykernel+involves%3Aminrk+updated%3A2022-02-15..2022-03-14&type=Issues) | [@vidartf](https://github.com/search?q=repo%3Aipython%2Fipykernel+involves%3Avidartf+updated%3A2022-02-15..2022-03-14&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 6.9.1
 
 ([Full Changelog](https://github.com/ipython/ipykernel/compare/v6.9.0...c27e5b95c3d104d9fb6cae3375aec0e98974dcff))
 
 ### Bugs fixed
 
 - Add hostname to the usage reply [#865](https://github.com/ipython/ipykernel/pull/865) ([@echarles](https://github.com/echarles))
@@ -14,16 +36,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/ipython/ipykernel/graphs/contributors?from=2022-02-07&to=2022-02-15&type=c))
 
 [@blink1073](https://github.com/search?q=repo%3Aipython%2Fipykernel+involves%3Ablink1073+updated%3A2022-02-07..2022-02-15&type=Issues) | [@echarles](https://github.com/search?q=repo%3Aipython%2Fipykernel+involves%3Aecharles+updated%3A2022-02-07..2022-02-15&type=Issues) | [@minrk](https://github.com/search?q=repo%3Aipython%2Fipykernel+involves%3Aminrk+updated%3A2022-02-07..2022-02-15&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 6.9.0
 
 ([Full Changelog](https://github.com/ipython/ipykernel/compare/v6.8.0...7a229c6c83d44d315f637ef63159a43c64ec73d6))
 
 ### Bugs fixed
 
 - Fixed event forwarding [#855](https://github.com/ipython/ipykernel/pull/855) ([@JohanMabille](https://github.com/JohanMabille))
```

### Comparing `ipykernel-6.9.1/CONTRIBUTING.md` & `ipykernel-6.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/COPYING.md` & `ipykernel-6.9.2/COPYING.md`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/PKG-INFO` & `ipykernel-6.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipykernel
-Version: 6.9.1
+Version: 6.9.2
 Summary: IPython Kernel for Jupyter
 Home-page: https://ipython.org
 Author: IPython Development Team
 Author-email: ipython-dev@scipy.org
 License: BSD
 Keywords: Interactive,Interpreter,Shell,Web
 Platform: Linux
```

### Comparing `ipykernel-6.9.1/README.md` & `ipykernel-6.9.2/README.md`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/RELEASE.md` & `ipykernel-6.9.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/docs/Makefile` & `ipykernel-6.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/docs/conf.py` & `ipykernel-6.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/docs/make.bat` & `ipykernel-6.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/examples/embedding/inprocess_qtconsole.py` & `ipykernel-6.9.2/examples/embedding/inprocess_qtconsole.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/examples/embedding/inprocess_terminal.py` & `ipykernel-6.9.2/examples/embedding/inprocess_terminal.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/examples/embedding/internal_ipkernel.py` & `ipykernel-6.9.2/examples/embedding/internal_ipkernel.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/examples/embedding/ipkernel_qtapp.py` & `ipykernel-6.9.2/examples/embedding/ipkernel_qtapp.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/examples/embedding/ipkernel_wxapp.py` & `ipykernel-6.9.2/examples/embedding/ipkernel_wxapp.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/_eventloop_macos.py` & `ipykernel-6.9.2/ipykernel/_eventloop_macos.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/_version.py` & `ipykernel-6.9.2/ipykernel/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 store the current version info of the server.
 """
 import re
 
 # Version string must appear intact for tbump versioning
-__version__ = '6.9.1'
+__version__ = '6.9.2'
 
 # Build up version_info tuple for backwards compatibility
 pattern = r'(?P<major>\d+).(?P<minor>\d+).(?P<patch>\d+)(?P<rest>.*)'
 match = re.match(pattern, __version__)
 parts = [int(match[part]) for part in ['major', 'minor', 'patch']]
 if match['rest']:
     parts.append(match['rest'])
```

### Comparing `ipykernel-6.9.1/ipykernel/comm/comm.py` & `ipykernel-6.9.2/ipykernel/comm/comm.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/comm/manager.py` & `ipykernel-6.9.2/ipykernel/comm/manager.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/compiler.py` & `ipykernel-6.9.2/ipykernel/compiler.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/connect.py` & `ipykernel-6.9.2/ipykernel/connect.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/control.py` & `ipykernel-6.9.2/ipykernel/control.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/datapub.py` & `ipykernel-6.9.2/ipykernel/datapub.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/debugger.py` & `ipykernel-6.9.2/ipykernel/debugger.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,22 @@
 try:
     from jupyter_client.jsonutil import json_default
 except ImportError:
     from jupyter_client.jsonutil import date_default as json_default
 
 from .compiler import (get_file_name, get_tmp_directory, get_tmp_hash_seed)
 
-# This import is required to have the next ones working...
-from debugpy.server import api  # noqa
-from _pydevd_bundle import pydevd_frame_utils
-from _pydevd_bundle.pydevd_suspended_frames import SuspendedFramesManager, _FramesTracker
+try:
+    # This import is required to have the next ones working...
+    from debugpy.server import api  # noqa
+    from _pydevd_bundle import pydevd_frame_utils
+    from _pydevd_bundle.pydevd_suspended_frames import SuspendedFramesManager, _FramesTracker
+    _is_debugpy_available = True
+except ImportError:
+    _is_debugpy_available = False
 
 # Required for backwards compatiblity
 ROUTING_ID = getattr(zmq, 'ROUTING_ID', None) or zmq.IDENTITY
 
 
 class _FakeCode:
     def __init__(self, co_filename, co_name):
```

### Comparing `ipykernel-6.9.1/ipykernel/displayhook.py` & `ipykernel-6.9.2/ipykernel/displayhook.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/embed.py` & `ipykernel-6.9.2/ipykernel/embed.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/eventloops.py` & `ipykernel-6.9.2/ipykernel/eventloops.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,15 +281,18 @@
 
         kernel.app_wrapper = TimedAppWrapper(app, doi)
         kernel.app_wrapper.start()
 
 
 @loop_tk.exit
 def loop_tk_exit(kernel):
-    kernel.app_wrapper.app.destroy()
+    try:
+        kernel.app_wrapper.app.destroy()
+    except RuntimeError:
+        pass
 
 
 @register_integration('gtk')
 def loop_gtk(kernel):
     """Start the kernel, coordinating with the GTK event loop"""
     from .gui.gtkembed import GTKEmbed
```

### Comparing `ipykernel-6.9.1/ipykernel/gui/__init__.py` & `ipykernel-6.9.2/ipykernel/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/gui/gtk3embed.py` & `ipykernel-6.9.2/ipykernel/gui/gtk3embed.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/gui/gtkembed.py` & `ipykernel-6.9.2/ipykernel/gui/gtkembed.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/heartbeat.py` & `ipykernel-6.9.2/ipykernel/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/inprocess/blocking.py` & `ipykernel-6.9.2/ipykernel/inprocess/blocking.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/inprocess/channels.py` & `ipykernel-6.9.2/ipykernel/inprocess/channels.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/inprocess/client.py` & `ipykernel-6.9.2/ipykernel/inprocess/client.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/inprocess/ipkernel.py` & `ipykernel-6.9.2/ipykernel/inprocess/ipkernel.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/inprocess/manager.py` & `ipykernel-6.9.2/ipykernel/inprocess/manager.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/inprocess/socket.py` & `ipykernel-6.9.2/ipykernel/inprocess/socket.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/inprocess/tests/test_kernel.py` & `ipykernel-6.9.2/ipykernel/inprocess/tests/test_kernel.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/inprocess/tests/test_kernelmanager.py` & `ipykernel-6.9.2/ipykernel/inprocess/tests/test_kernelmanager.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/iostream.py` & `ipykernel-6.9.2/ipykernel/iostream.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/ipkernel.py` & `ipykernel-6.9.2/ipykernel/ipkernel.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from zmq.eventloop.zmqstream import ZMQStream
 
 from .comm import CommManager
 from .kernelbase import Kernel as KernelBase
 from .zmqshell import ZMQInteractiveShell
 from .eventloops import _use_appnope
 from .compiler import XCachingCompiler
+from .debugger import Debugger, _is_debugpy_available
 
 try:
     from IPython.core.interactiveshell import _asyncio_runner
 except ImportError:
     _asyncio_runner = None
 
 try:
@@ -29,20 +30,14 @@
         rectify_completions as _rectify_completions,
         provisionalcompleter as _provisionalcompleter,
     )
     _use_experimental_60_completion = True
 except ImportError:
     _use_experimental_60_completion = False
 
-try:
-    import debugpy
-    from .debugger import Debugger
-    _is_debugpy_available = True
-except ImportError:
-    _is_debugpy_available = False
 
 _EXPERIMENTAL_KEY_NAME = '_jupyter_types_experimental'
 
 
 class IPythonKernel(KernelBase):
     shell = Instance('IPython.core.interactiveshell.InteractiveShellABC',
                      allow_none=True)
```

### Comparing `ipykernel-6.9.1/ipykernel/jsonutil.py` & `ipykernel-6.9.2/ipykernel/jsonutil.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/kernelapp.py` & `ipykernel-6.9.2/ipykernel/kernelapp.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/kernelbase.py` & `ipykernel-6.9.2/ipykernel/kernelbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 """Base class for a kernel that talks to frontends over 0MQ."""
 
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 
 import asyncio
 import concurrent.futures
-from datetime import datetime
-from functools import partial
+import inspect
 import itertools
 import logging
-import inspect
 import os
-from signal import signal, default_int_handler, SIGINT
-import sys
 import socket
+import sys
 import time
 import uuid
 import warnings
-try:
-    import psutil
-except ImportError:
-    psutil = None
+from datetime import datetime
+from functools import partial
+from signal import SIGINT, SIGTERM, Signals, default_int_handler, signal
+
+if sys.platform != "win32":
+    from signal import SIGKILL
+else:
+    SIGKILL = "windown-SIGKILL-sentinel"
+
+
+
 
 try:
     # jupyter_client >= 5, use tz-aware now
     from jupyter_client.session import utcnow as now
 except ImportError:
     # jupyter_client < 5, use local now()
     now = datetime.now
 
+import psutil
+import zmq
+from IPython.core.error import StdinNotImplementedError
+from jupyter_client.session import Session
 from tornado import ioloop
 from tornado.queues import Queue, QueueEmpty
-import zmq
+from traitlets import (Any, Bool, Dict, Float, Instance, Integer, List, Set,
+                       Unicode, default, observe)
+from traitlets.config.configurable import SingletonConfigurable
 from zmq.eventloop.zmqstream import ZMQStream
 
-from traitlets.config.configurable import SingletonConfigurable
-from IPython.core.error import StdinNotImplementedError
 from ipykernel.jsonutil import json_clean
-from traitlets import (
-    Any, Instance, Float, Dict, List, Set, Integer, Unicode, Bool,
-    observe, default
-)
-
-from jupyter_client.session import Session
 
 from ._version import kernel_protocol_version
 
 
 class Kernel(SingletonConfigurable):
 
     #---------------------------------------------------------------------------
@@ -792,49 +794,50 @@
         else:
             comms = {}
         reply_content = dict(comms=comms, status='ok')
         msg = self.session.send(stream, 'comm_info_reply',
                                 reply_content, parent, ident)
         self.log.debug("%s", msg)
 
-    async def interrupt_request(self, stream, ident, parent):
-        pid = os.getpid()
-        pgid = os.getpgid(pid)
-
+    def _send_interupt_children(self):
         if os.name == "nt":
             self.log.error("Interrupt message not supported on Windows")
-
         else:
+            pid = os.getpid()
+            pgid = os.getpgid(pid)
             # Prefer process-group over process
-            if pgid and hasattr(os, "killpg"):
+            # but only if the kernel is the leader of the process group
+            if pgid and pgid == pid and hasattr(os, "killpg"):
                 try:
                     os.killpg(pgid, SIGINT)
                     return
                 except OSError:
                     pass
             try:
                 os.kill(pid, SIGINT)
             except OSError:
                 pass
 
+    async def interrupt_request(self, stream, ident, parent):
+        self._send_interupt_children()
         content = parent['content']
         self.session.send(stream, 'interrupt_reply', content, parent, ident=ident)
         return
 
     async def shutdown_request(self, stream, ident, parent):
         content = self.do_shutdown(parent['content']['restart'])
         if inspect.isawaitable(content):
             content = await content
         self.session.send(stream, 'shutdown_reply', content, parent, ident=ident)
         # same content, but different msg_id for broadcasting on IOPub
         self._shutdown_message = self.session.msg('shutdown_reply',
                                                   content, parent
         )
 
-        self._at_shutdown()
+        await self._at_shutdown()
 
         self.log.debug('Stopping control ioloop')
         control_io_loop = self.control_stream.io_loop
         control_io_loop.add_callback(control_io_loop.stop)
 
         self.log.debug('Stopping shell ioloop')
         shell_io_loop = self.shell_stream.io_loop
@@ -888,16 +891,14 @@
         except BaseException:
             return None
 
     async def usage_request(self, stream, ident, parent):
         reply_content = {
             'hostname': socket.gethostname()
         }
-        if psutil is None:
-            return reply_content
         current_process = psutil.Process()
         all_processes = [current_process] + current_process.children(recursive=True)
         process_metric_value = self.get_process_metric_value
         reply_content['kernel_cpu'] = sum([process_metric_value(process, 'cpu_percent', None) for process in all_processes])
         reply_content['kernel_memory'] = sum([process_metric_value(process, 'memory_info', 'rss') for process in all_processes])
         cpu_percent = psutil.cpu_percent()
         # https://psutil.readthedocs.io/en/latest/index.html?highlight=cpu#psutil.cpu_percent
@@ -1127,14 +1128,85 @@
             self.log.error("Bad input_reply: %s", parent)
             value = ''
         if value == '\x04':
             # EOF
             raise EOFError
         return value
 
-    def _at_shutdown(self):
+    def _signal_children(self, signum):
+        """
+        Send a signal to all our children
+
+        Like `killpg`, but does not include the current process
+        (or possible parents).
+        """
+        for p in self._process_children():
+            self.log.debug(f"Sending {Signals(signum)!r} to subprocess {p}")
+            try:
+                if signum == SIGTERM:
+                    p.terminate()
+                elif signum == SIGKILL:
+                    p.kill()
+                else:
+                    p.send_signal(signum)
+            except psutil.NoSuchProcess:
+                pass
+
+    def _process_children(self):
+        """Retrieve child processes in the kernel's process group
+
+        Avoids:
+        - including parents and self with killpg
+        - including all children that may have forked-off a new group
+        """
+        kernel_process = psutil.Process()
+        all_children = kernel_process.children(recursive=True)
+        if os.name == "nt":
+            return all_children
+        kernel_pgid = os.getpgrp()
+        process_group_children = []
+        for child in all_children:
+            try:
+                child_pgid = os.getpgid(child.pid)
+            except OSError:
+                pass
+            else:
+                if child_pgid == kernel_pgid:
+                    process_group_children.append(child)
+        return process_group_children
+
+    async def _progressively_terminate_all_children(self):
+        sleeps = (0.01, 0.03, 0.1, 0.3, 1, 3, 10)
+        if not self._process_children():
+            self.log.debug("Kernel has no children.")
+            return
+
+        for signum in (SIGTERM, SIGKILL):
+            for delay in sleeps:
+                children = self._process_children()
+                if not children:
+                    self.log.debug("No more children, continuing shutdown routine.")
+                    return
+                # signals only children, not current process
+                self._signal_children(signum)
+                self.log.debug(
+                    f"Will sleep {delay}s before checking for children and retrying. {children}"
+                )
+                await asyncio.sleep(delay)
+
+    async def _at_shutdown(self):
         """Actions taken at shutdown by the kernel, called by python's atexit.
         """
-        if self._shutdown_message is not None:
-            self.session.send(self.iopub_socket, self._shutdown_message, ident=self._topic('shutdown'))
-            self.log.debug("%s", self._shutdown_message)
-        self.control_stream.flush(zmq.POLLOUT)
+        try:
+            await self._progressively_terminate_all_children()
+        except Exception as e:
+            self.log.exception("Exception during subprocesses termination %s", e)
+
+        finally:
+            if self._shutdown_message is not None:
+                self.session.send(
+                    self.iopub_socket,
+                    self._shutdown_message,
+                    ident=self._topic("shutdown"),
+                )
+                self.log.debug("%s", self._shutdown_message)
+            self.control_stream.flush(zmq.POLLOUT)
```

### Comparing `ipykernel-6.9.1/ipykernel/kernelspec.py` & `ipykernel-6.9.2/ipykernel/kernelspec.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import shutil
 import stat
 import sys
 import tempfile
 
 from jupyter_client.kernelspec import KernelSpecManager
 
-from .ipkernel import _is_debugpy_available
+from .debugger import _is_debugpy_available
 
 pjoin = os.path.join
 
 KERNEL_NAME = 'python%i' % sys.version_info[0]
 
 # path to kernelspec resources
 RESOURCES = pjoin(os.path.dirname(__file__), 'resources')
```

### Comparing `ipykernel-6.9.1/ipykernel/log.py` & `ipykernel-6.9.2/ipykernel/log.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/parentpoller.py` & `ipykernel-6.9.2/ipykernel/parentpoller.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/pickleutil.py` & `ipykernel-6.9.2/ipykernel/pickleutil.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/resources/logo-32x32.png` & `ipykernel-6.9.2/ipykernel/resources/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/resources/logo-64x64.png` & `ipykernel-6.9.2/ipykernel/resources/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/serialize.py` & `ipykernel-6.9.2/ipykernel/serialize.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/tests/__init__.py` & `ipykernel-6.9.2/ipykernel/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/tests/test_async.py` & `ipykernel-6.9.2/ipykernel/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/tests/test_connect.py` & `ipykernel-6.9.2/ipykernel/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/tests/test_debugger.py` & `ipykernel-6.9.2/ipykernel/tests/test_debugger.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/tests/test_embed_kernel.py` & `ipykernel-6.9.2/ipykernel/tests/test_embed_kernel.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/tests/test_eventloop.py` & `ipykernel-6.9.2/ipykernel/tests/test_eventloop.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/tests/test_heartbeat.py` & `ipykernel-6.9.2/ipykernel/tests/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/tests/test_io.py` & `ipykernel-6.9.2/ipykernel/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/tests/test_jsonutil.py` & `ipykernel-6.9.2/ipykernel/tests/test_jsonutil.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/tests/test_kernel.py` & `ipykernel-6.9.2/ipykernel/tests/test_kernel.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 
 import ast
 import os.path
 import platform
+import signal
 import subprocess
 import sys
 import time
+from subprocess import Popen
 from tempfile import TemporaryDirectory
 
 from flaky import flaky
+import psutil
 import pytest
-from packaging import version
 
 import IPython
 from IPython.paths import locate_profile
 
 from .utils import (
     new_kernel, kernel, TIMEOUT, assemble_output, execute,
     flush_channels, wait_for_idle, get_reply,
@@ -492,7 +494,79 @@
 
     # verify that all control messages were handled before all shell messages
     shell_dates = [msg["header"]["date"] for msg in shell_replies]
     control_dates = [msg["header"]["date"] for msg in control_replies]
     # comparing first to last ought to be enough, since queues preserve order
     # use <= in case of very-fast handling and/or low resolution timers
     assert control_dates[-1] <= shell_dates[0]
+
+
+def _child():
+    print("in child", os.getpid())
+
+    def _print_and_exit(sig, frame):
+        print(f"Received signal {sig}")
+        # take some time so retries are triggered
+        time.sleep(0.5)
+        sys.exit(-sig)
+
+    signal.signal(signal.SIGTERM, _print_and_exit)
+    time.sleep(30)
+
+
+def _start_children():
+    ip = IPython.get_ipython()
+    ns = ip.user_ns
+
+    cmd = [sys.executable, "-c", f"from {__name__} import _child; _child()"]
+    child_pg = Popen(cmd, start_new_session=False)
+    child_newpg = Popen(cmd, start_new_session=True)
+    ns["pid"] = os.getpid()
+    ns["child_pg"] = child_pg.pid
+    ns["child_newpg"] = child_newpg.pid
+    # give them time to start up and register signal handlers
+    time.sleep(1)
+
+
+@pytest.mark.skipif(
+    platform.python_implementation() == "PyPy",
+    reason="does not work on PyPy",
+)
+def test_shutdown_subprocesses():
+    """Kernel exits after polite shutdown_request"""
+    with new_kernel() as kc:
+        km = kc.parent
+        msg_id, reply = execute(
+            f"from {__name__} import _start_children\n_start_children()",
+            kc=kc,
+            user_expressions={
+                "pid": "pid",
+                "child_pg": "child_pg",
+                "child_newpg": "child_newpg",
+            },
+        )
+        print(reply)
+        expressions = reply["user_expressions"]
+        kernel_process = psutil.Process(int(expressions["pid"]["data"]["text/plain"]))
+        child_pg = psutil.Process(int(expressions["child_pg"]["data"]["text/plain"]))
+        child_newpg = psutil.Process(
+            int(expressions["child_newpg"]["data"]["text/plain"])
+        )
+        wait_for_idle(kc)
+
+        kc.shutdown()
+        for i in range(300):  # 30s timeout
+            if km.is_alive():
+                time.sleep(0.1)
+            else:
+                break
+        assert not km.is_alive()
+        assert not kernel_process.is_running()
+        # child in the process group shut down
+        assert not child_pg.is_running()
+        # child outside the process group was not shut down (unix only)
+        if os.name != 'nt':
+            assert child_newpg.is_running()
+        try:
+            child_newpg.terminate()
+        except psutil.NoSuchProcess:
+            pass
```

### Comparing `ipykernel-6.9.1/ipykernel/tests/test_kernelspec.py` & `ipykernel-6.9.2/ipykernel/tests/test_kernelspec.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/tests/test_message_spec.py` & `ipykernel-6.9.2/ipykernel/tests/test_message_spec.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/tests/test_pickleutil.py` & `ipykernel-6.9.2/ipykernel/tests/test_pickleutil.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/tests/test_start_kernel.py` & `ipykernel-6.9.2/ipykernel/tests/test_start_kernel.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/tests/test_zmq_shell.py` & `ipykernel-6.9.2/ipykernel/tests/test_zmq_shell.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/tests/utils.py` & `ipykernel-6.9.2/ipykernel/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/trio_runner.py` & `ipykernel-6.9.2/ipykernel/trio_runner.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel/zmqshell.py` & `ipykernel-6.9.2/ipykernel/zmqshell.py`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/ipykernel.egg-info/PKG-INFO` & `ipykernel-6.9.2/ipykernel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipykernel
-Version: 6.9.1
+Version: 6.9.2
 Summary: IPython Kernel for Jupyter
 Home-page: https://ipython.org
 Author: IPython Development Team
 Author-email: ipython-dev@scipy.org
 License: BSD
 Keywords: Interactive,Interpreter,Shell,Web
 Platform: Linux
```

### Comparing `ipykernel-6.9.1/ipykernel.egg-info/SOURCES.txt` & `ipykernel-6.9.2/ipykernel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/pyproject.toml` & `ipykernel-6.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [tool.check-manifest]
 ignore = []
 
 [tool.jupyter-releaser]
 skip = ["check-links"]
 
 [tool.tbump.version]
-current = "6.9.1"
+current = "6.9.2"
 regex = '''
   (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)
   ((?P<channel>a|b|rc|.dev)(?P<release>\d+))?
 '''
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
```

### Comparing `ipykernel-6.9.1/setup.cfg` & `ipykernel-6.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ipykernel-6.9.1/setup.py` & `ipykernel-6.9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         'debugpy>=1.0.0,<2.0',
         'ipython>=7.23.1',
         'traitlets>=5.1.0,<6.0',
         'jupyter_client<8.0',
         'tornado>=4.2,<7.0',
         'matplotlib-inline>=0.1.0,<0.2.0',
         'appnope;platform_system=="Darwin"',
+        'psutil',
         'nest_asyncio',
     ],
     extras_require={
         "test": [
             "pytest !=5.3.4",
             "pytest-cov",
             "flaky",
```

