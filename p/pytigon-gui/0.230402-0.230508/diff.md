# Comparing `tmp/pytigon-gui-0.230402.tar.gz` & `tmp/pytigon-gui-0.230508.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytigon-gui-0.230402.tar", last modified: Sun Apr  2 17:40:21 2023, max compression
+gzip compressed data, was "pytigon-gui-0.230508.tar", last modified: Mon May  8 20:09:46 2023, max compression
```

## Comparing `pytigon-gui-0.230402.tar` & `pytigon-gui-0.230508.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:40:21.631042 pytigon-gui-0.230402/
--rw-rw-r--   0 sch       (1000) sch       (1000)     7633 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/LICENSE
--rw-rw-r--   0 sch       (1000) sch       (1000)     1017 2023-04-02 17:40:21.631042 pytigon-gui-0.230402/PKG-INFO
--rw-rw-r--   0 sch       (1000) sch       (1000)       13 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/README.md
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:40:21.623042 pytigon-gui-0.230402/pytigon_gui/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/__init__.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:40:21.627042 pytigon-gui-0.230402/pytigon_gui/guictrl/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guictrl/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     8763 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guictrl/basectrl.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:40:21.627042 pytigon-gui-0.230402/pytigon_gui/guictrl/button/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guictrl/button/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3421 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guictrl/button/toolbarbutton.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    70515 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guictrl/ctrl.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:40:21.627042 pytigon-gui-0.230402/pytigon_gui/guictrl/grid/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guictrl/grid/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    28216 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guictrl/grid/grid.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     8655 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guictrl/grid/gridpanel.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    10822 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guictrl/grid/gridtable_base.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    12128 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guictrl/grid/gridtable_from_html_table.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    16003 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guictrl/grid/gridtable_from_proxy.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     6772 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guictrl/grid/popupcelleditors.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     8379 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guictrl/grid/renderers.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     6564 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guictrl/grid/tabproxy.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:40:21.627042 pytigon-gui-0.230402/pytigon_gui/guictrl/popup/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guictrl/popup/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     9819 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guictrl/popup/popuphtml.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    11535 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guictrl/popup/select2.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    25501 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guictrl/tag.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:40:21.627042 pytigon-gui-0.230402/pytigon_gui/guiframe/
--rw-rw-r--   0 sch       (1000) sch       (1000)     1104 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guiframe/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    44713 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guiframe/appframe.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     4204 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guiframe/baseframe.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3529 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guiframe/browserframe.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    43509 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guiframe/form.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2137 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guiframe/manager.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     8187 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guiframe/notebook.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    18048 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guiframe/notebookpage.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    19083 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guiframe/page.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:40:21.627042 pytigon-gui-0.230402/pytigon_gui/guilib/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guilib/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2441 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guilib/events.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3320 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guilib/httperror.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     9834 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guilib/image.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2490 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guilib/logindialog.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3934 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guilib/pytigon_install.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2074 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guilib/signal.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     4967 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guilib/threadwindow.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     4321 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guilib/tools.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1653 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/guilib/websocket.py
--rwxrwxr-x   0 sch       (1000) sch       (1000)    46779 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/pytigon.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:40:21.631042 pytigon-gui-0.230402/pytigon_gui/toolbar/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/toolbar/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    14182 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/toolbar/basetoolbar.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     5910 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/toolbar/generictoolbar.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2498 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/toolbar/menubar.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     8759 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/toolbar/moderntoolbar.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     4498 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/toolbar/standardtoolbar.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    25006 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/toolbar/standardtoolbarbuttons.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    10675 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/pytigon_gui/toolbar/treetoolbar.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:40:21.623042 pytigon-gui-0.230402/pytigon_gui.egg-info/
--rw-rw-r--   0 sch       (1000) sch       (1000)     1017 2023-04-02 17:40:21.000000 pytigon-gui-0.230402/pytigon_gui.egg-info/PKG-INFO
--rw-rw-r--   0 sch       (1000) sch       (1000)     1913 2023-04-02 17:40:21.000000 pytigon-gui-0.230402/pytigon_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)        1 2023-04-02 17:40:21.000000 pytigon-gui-0.230402/pytigon_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)       47 2023-04-02 17:40:21.000000 pytigon-gui-0.230402/pytigon_gui.egg-info/entry_points.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)       74 2023-04-02 17:40:21.000000 pytigon-gui-0.230402/pytigon_gui.egg-info/requires.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)       12 2023-04-02 17:40:21.000000 pytigon-gui-0.230402/pytigon_gui.egg-info/top_level.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)       75 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/requirements.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)       38 2023-04-02 17:40:21.631042 pytigon-gui-0.230402/setup.cfg
--rw-rw-r--   0 sch       (1000) sch       (1000)     1819 2023-04-02 17:20:55.000000 pytigon-gui-0.230402/setup.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:09:46.846265 pytigon-gui-0.230508/
+-rw-rw-r--   0 sch       (1000) sch       (1000)     7633 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/LICENSE
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1068 2023-05-08 20:09:46.846265 pytigon-gui-0.230508/PKG-INFO
+-rw-rw-r--   0 sch       (1000) sch       (1000)       13 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/README.md
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:09:46.834265 pytigon-gui-0.230508/pytigon_gui/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/__init__.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:09:46.838265 pytigon-gui-0.230508/pytigon_gui/guictrl/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guictrl/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     8763 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guictrl/basectrl.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:09:46.838265 pytigon-gui-0.230508/pytigon_gui/guictrl/button/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guictrl/button/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3421 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guictrl/button/toolbarbutton.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    70515 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guictrl/ctrl.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:09:46.838265 pytigon-gui-0.230508/pytigon_gui/guictrl/grid/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guictrl/grid/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    28216 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guictrl/grid/grid.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     8655 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guictrl/grid/gridpanel.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    10822 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guictrl/grid/gridtable_base.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    12128 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guictrl/grid/gridtable_from_html_table.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    16003 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guictrl/grid/gridtable_from_proxy.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     6772 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guictrl/grid/popupcelleditors.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     8379 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guictrl/grid/renderers.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     6564 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guictrl/grid/tabproxy.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:09:46.842265 pytigon-gui-0.230508/pytigon_gui/guictrl/popup/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guictrl/popup/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     9819 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guictrl/popup/popuphtml.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    11535 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guictrl/popup/select2.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    25501 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guictrl/tag.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:09:46.842265 pytigon-gui-0.230508/pytigon_gui/guiframe/
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1104 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guiframe/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    44728 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guiframe/appframe.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     4204 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guiframe/baseframe.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3529 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guiframe/browserframe.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    43509 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guiframe/form.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2137 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guiframe/manager.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     8187 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guiframe/notebook.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    18048 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guiframe/notebookpage.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    19310 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guiframe/page.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:09:46.842265 pytigon-gui-0.230508/pytigon_gui/guilib/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guilib/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2441 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guilib/events.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3320 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guilib/httperror.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     9834 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guilib/image.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2490 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guilib/logindialog.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3934 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guilib/pytigon_install.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2074 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guilib/signal.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     4967 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guilib/threadwindow.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     4321 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guilib/tools.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1653 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/guilib/websocket.py
+-rwxrwxr-x   0 sch       (1000) sch       (1000)    46779 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/pytigon.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:09:46.846265 pytigon-gui-0.230508/pytigon_gui/toolbar/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/toolbar/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    14182 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/toolbar/basetoolbar.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     5910 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/toolbar/generictoolbar.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2498 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/toolbar/menubar.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     8759 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/toolbar/moderntoolbar.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     4498 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/toolbar/standardtoolbar.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    25006 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/toolbar/standardtoolbarbuttons.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    10675 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/pytigon_gui/toolbar/treetoolbar.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:09:46.838265 pytigon-gui-0.230508/pytigon_gui.egg-info/
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1068 2023-05-08 20:09:46.000000 pytigon-gui-0.230508/pytigon_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1913 2023-05-08 20:09:46.000000 pytigon-gui-0.230508/pytigon_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)        1 2023-05-08 20:09:46.000000 pytigon-gui-0.230508/pytigon_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)       47 2023-05-08 20:09:46.000000 pytigon-gui-0.230508/pytigon_gui.egg-info/entry_points.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)       74 2023-05-08 20:09:46.000000 pytigon-gui-0.230508/pytigon_gui.egg-info/requires.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)       12 2023-05-08 20:09:46.000000 pytigon-gui-0.230508/pytigon_gui.egg-info/top_level.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)       75 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/requirements.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)       38 2023-05-08 20:09:46.846265 pytigon-gui-0.230508/setup.cfg
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1869 2023-05-08 20:06:51.000000 pytigon-gui-0.230508/setup.py
```

### Comparing `pytigon-gui-0.230402/LICENSE` & `pytigon-gui-0.230508/LICENSE`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/PKG-INFO` & `pytigon-gui-0.230508/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytigon-gui
-Version: 0.230402
+Version: 0.230508
 Summary: Pytigon GUI
 Home-page: UNKNOWN
 Author: Sławomir Chołaj
 Author-email: slawomir.cholaj@gmail.com
 License: LGPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `pytigon-gui-0.230402/pytigon_gui/__init__.py` & `pytigon-gui-0.230508/pytigon_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guictrl/__init__.py` & `pytigon-gui-0.230508/pytigon_gui/guictrl/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guictrl/basectrl.py` & `pytigon-gui-0.230508/pytigon_gui/guictrl/basectrl.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guictrl/button/__init__.py` & `pytigon-gui-0.230508/pytigon_gui/guictrl/button/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guictrl/button/toolbarbutton.py` & `pytigon-gui-0.230508/pytigon_gui/guictrl/button/toolbarbutton.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guictrl/ctrl.py` & `pytigon-gui-0.230508/pytigon_gui/guictrl/ctrl.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guictrl/grid/__init__.py` & `pytigon-gui-0.230508/pytigon_gui/guictrl/grid/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guictrl/grid/grid.py` & `pytigon-gui-0.230508/pytigon_gui/guictrl/grid/grid.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guictrl/grid/gridpanel.py` & `pytigon-gui-0.230508/pytigon_gui/guictrl/grid/gridpanel.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guictrl/grid/gridtable_base.py` & `pytigon-gui-0.230508/pytigon_gui/guictrl/grid/gridtable_base.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guictrl/grid/gridtable_from_html_table.py` & `pytigon-gui-0.230508/pytigon_gui/guictrl/grid/gridtable_from_html_table.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guictrl/grid/gridtable_from_proxy.py` & `pytigon-gui-0.230508/pytigon_gui/guictrl/grid/gridtable_from_proxy.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guictrl/grid/popupcelleditors.py` & `pytigon-gui-0.230508/pytigon_gui/guictrl/grid/popupcelleditors.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guictrl/grid/renderers.py` & `pytigon-gui-0.230508/pytigon_gui/guictrl/grid/renderers.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guictrl/grid/tabproxy.py` & `pytigon-gui-0.230508/pytigon_gui/guictrl/grid/tabproxy.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guictrl/popup/__init__.py` & `pytigon-gui-0.230508/pytigon_gui/guictrl/popup/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guictrl/popup/popuphtml.py` & `pytigon-gui-0.230508/pytigon_gui/guictrl/popup/popuphtml.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guictrl/popup/select2.py` & `pytigon-gui-0.230508/pytigon_gui/guictrl/popup/select2.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guictrl/tag.py` & `pytigon-gui-0.230508/pytigon_gui/guictrl/tag.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guiframe/__init__.py` & `pytigon-gui-0.230508/pytigon_gui/guiframe/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guiframe/appframe.py` & `pytigon-gui-0.230508/pytigon_gui/guiframe/appframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1015,15 +1015,15 @@
                     panel = page.append(row[1].data)
                 if pos == 3:
                     try:
                         bitmap = (wx.GetApp().images)[int(row[4].data)]
                     except:
                         if row[4].data and row[4].data != "" and row[4].data != "None":
                             try:
-                                bitmap = bitmap_from_href(row[4].data)
+                                bitmap = bitmap_from_href(row[4].data.split("<=")[0])
                             except:
                                 bitmap = (wx.GetApp().images)[0]
                         else:
                             bitmap = (wx.GetApp().images)[0]
                     if not bitmap:
                         bitmap = (wx.GetApp().images)[0]
                     idn = self._append_command(row[5].data, row[6].data)
```

### Comparing `pytigon-gui-0.230402/pytigon_gui/guiframe/baseframe.py` & `pytigon-gui-0.230508/pytigon_gui/guiframe/baseframe.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guiframe/browserframe.py` & `pytigon-gui-0.230508/pytigon_gui/guiframe/browserframe.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guiframe/form.py` & `pytigon-gui-0.230508/pytigon_gui/guiframe/form.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guiframe/manager.py` & `pytigon-gui-0.230508/pytigon_gui/guiframe/manager.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guiframe/notebook.py` & `pytigon-gui-0.230508/pytigon_gui/guiframe/notebook.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guiframe/notebookpage.py` & `pytigon-gui-0.230508/pytigon_gui/guiframe/notebookpage.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guiframe/page.py` & `pytigon-gui-0.230508/pytigon_gui/guiframe/page.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,20 @@
     from wx.adv import LayoutAlgorithm
 except:
     from wx import LayoutAlgorithm
 from pytigon_gui.guilib import events
 from pytigon_gui.guilib.signal import Signal
 from pytigon_lib.schtools import createparm
 from pytigon_lib.schparser.html_parsers import ShtmlParser
+from pytigon_lib.schhttptools.httpclient import HttpResponse
 from pytigon_gui.guiframe.form import SchForm
 from pytigon_gui.guilib.events import *
 
 
+
 class SchPage(wx.Window, Signal):
     """SchPage class"""
 
     def __init__(
         self, parent, address_or_parser, parameters, pos=(0, 0), size=wx.DefaultSize
     ):
         """Contructor
@@ -316,15 +318,18 @@
     def _refresh(self):
         if self.address_or_parser.__class__.__name__ == "ShtmlParser":
             if self.address_or_parser.address:
                 mp = self._read_html(self.address_or_parser.address, self.parameters)
             else:
                 mp = self._read_html(self.address_or_parser, self.parameters)
         else:
-            mp = self._read_html(self.address_or_parser, self.parameters)
+            if type(self.address_or_parser) == HttpResponse:
+                mp = self._read_html(self.address_or_parser.url, self.parameters)
+            else:
+                mp = self._read_html(self.address_or_parser, self.parameters)
         if not mp:
             return
         address = mp.address
         header = mp.get_header()
         body = mp.get_body()
         footer = mp.get_footer()
         panel = mp.get_panel()
```

### Comparing `pytigon-gui-0.230402/pytigon_gui/guilib/__init__.py` & `pytigon-gui-0.230508/pytigon_gui/guilib/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guilib/events.py` & `pytigon-gui-0.230508/pytigon_gui/guilib/events.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guilib/httperror.py` & `pytigon-gui-0.230508/pytigon_gui/guilib/httperror.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guilib/image.py` & `pytigon-gui-0.230508/pytigon_gui/guilib/image.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guilib/logindialog.py` & `pytigon-gui-0.230508/pytigon_gui/guilib/logindialog.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guilib/pytigon_install.py` & `pytigon-gui-0.230508/pytigon_gui/guilib/pytigon_install.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guilib/signal.py` & `pytigon-gui-0.230508/pytigon_gui/guilib/signal.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guilib/threadwindow.py` & `pytigon-gui-0.230508/pytigon_gui/guilib/threadwindow.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guilib/tools.py` & `pytigon-gui-0.230508/pytigon_gui/guilib/tools.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/guilib/websocket.py` & `pytigon-gui-0.230508/pytigon_gui/guilib/websocket.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/pytigon.py` & `pytigon-gui-0.230508/pytigon_gui/pytigon.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/toolbar/__init__.py` & `pytigon-gui-0.230508/pytigon_gui/toolbar/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/toolbar/basetoolbar.py` & `pytigon-gui-0.230508/pytigon_gui/toolbar/basetoolbar.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/toolbar/generictoolbar.py` & `pytigon-gui-0.230508/pytigon_gui/toolbar/generictoolbar.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/toolbar/menubar.py` & `pytigon-gui-0.230508/pytigon_gui/toolbar/menubar.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/toolbar/moderntoolbar.py` & `pytigon-gui-0.230508/pytigon_gui/toolbar/moderntoolbar.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/toolbar/standardtoolbar.py` & `pytigon-gui-0.230508/pytigon_gui/toolbar/standardtoolbar.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/toolbar/standardtoolbarbuttons.py` & `pytigon-gui-0.230508/pytigon_gui/toolbar/standardtoolbarbuttons.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui/toolbar/treetoolbar.py` & `pytigon-gui-0.230508/pytigon_gui/toolbar/treetoolbar.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/pytigon_gui.egg-info/PKG-INFO` & `pytigon-gui-0.230508/pytigon_gui.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytigon-gui
-Version: 0.230402
+Version: 0.230508
 Summary: Pytigon GUI
 Home-page: UNKNOWN
 Author: Sławomir Chołaj
 Author-email: slawomir.cholaj@gmail.com
 License: LGPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `pytigon-gui-0.230402/pytigon_gui.egg-info/SOURCES.txt` & `pytigon-gui-0.230508/pytigon_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.230402/setup.py` & `pytigon-gui-0.230508/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     tmp = f.read().strip().split("\n")
     install_requires = [pos for pos in tmp if "://" not in pos]
     dependency_links = [pos for pos in tmp if "://" in pos]
 
 
 setup(
     name="pytigon-gui",
-    version="0.230402",
+    version="0.230508",
     description="Pytigon GUI",
     author="Sławomir Chołaj",
     author_email="slawomir.cholaj@gmail.com",
     license="LGPLv3",
     packages=find_packages(),
     package_data={"": extra_files},
     install_requires=install_requires,
@@ -37,14 +37,15 @@
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     entry_points={
         "gui_scripts": [
```

