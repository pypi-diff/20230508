# Comparing `tmp/pyshortcuts-1.8.3.tar.gz` & `tmp/pyshortcuts-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyshortcuts-1.8.3.tar", last modified: Wed Nov 23 20:42:28 2022, max compression
+gzip compressed data, was "pyshortcuts-1.9.0.tar", last modified: Mon May  8 17:05:17 2023, max compression
```

## Comparing `pyshortcuts-1.8.3.tar` & `pyshortcuts-1.9.0.tar`

### file list

```diff
@@ -1,60 +1,64 @@
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-23 20:42:28.824183 pyshortcuts-1.8.3/
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-23 20:42:28.808492 pyshortcuts-1.8.3/.github/
--rw-r--r--   0 Newville   (501) staff       (20)      502 2022-03-03 01:54:53.000000 pyshortcuts-1.8.3/.github/dependabot.yml
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-23 20:42:28.809236 pyshortcuts-1.8.3/.github/workflows/
--rw-r--r--   0 Newville   (501) staff       (20)      730 2022-03-03 01:54:20.000000 pyshortcuts-1.8.3/.github/workflows/test-macos.yml
--rw-r--r--   0 Newville   (501) staff       (20)      732 2022-03-03 01:54:20.000000 pyshortcuts-1.8.3/.github/workflows/test-ubuntu.yml
--rw-r--r--   0 Newville   (501) staff       (20)      742 2022-03-03 01:54:20.000000 pyshortcuts-1.8.3/.github/workflows/test-windows.yml
--rw-r--r--   0 Newville   (501) staff       (20)      115 2022-03-03 01:54:20.000000 pyshortcuts-1.8.3/.gitignore
--rw-r--r--   0 Newville   (501) staff       (20)     1107 2018-10-13 13:02:16.000000 pyshortcuts-1.8.3/LICENSE
--rw-r--r--   0 Newville   (501) staff       (20)      355 2022-01-28 18:15:23.000000 pyshortcuts-1.8.3/MANIFEST.in
--rw-r--r--   0 Newville   (501) staff       (20)     2425 2022-11-23 20:42:28.824313 pyshortcuts-1.8.3/PKG-INFO
--rw-r--r--   0 Newville   (501) staff       (20)     7484 2022-11-03 23:23:34.000000 pyshortcuts-1.8.3/README.md
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-23 20:42:28.810093 pyshortcuts-1.8.3/doc/
--rw-r--r--   0 Newville   (501) staff       (20)   264749 2019-09-25 20:19:15.000000 pyshortcuts-1.8.3/doc/pyshortcutgui_screenshot.png
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-23 20:42:28.811753 pyshortcuts-1.8.3/examples/
--rw-r--r--   0 Newville   (501) staff       (20)     6148 2019-09-22 01:41:23.000000 pyshortcuts-1.8.3/examples/.DS_Store
--rw-r--r--   0 Newville   (501) staff       (20)       96 2018-10-11 23:54:21.000000 pyshortcuts-1.8.3/examples/README.md
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-23 20:42:28.811974 pyshortcuts-1.8.3/examples/console_scripts/
--rw-r--r--   0 Newville   (501) staff       (20)      890 2018-10-11 23:54:21.000000 pyshortcuts-1.8.3/examples/console_scripts/timer.py
--rw-r--r--   0 Newville   (501) staff       (20)      334 2019-02-10 16:27:05.000000 pyshortcuts-1.8.3/examples/gui_bootstrap.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-23 20:42:28.815575 pyshortcuts-1.8.3/examples/icons/
--rw-r--r--   0 Newville   (501) staff       (20)    59139 2018-10-07 20:14:46.000000 pyshortcuts-1.8.3/examples/icons/coffeecup.icns
--rw-r--r--   0 Newville   (501) staff       (20)   161862 2018-10-07 20:14:46.000000 pyshortcuts-1.8.3/examples/icons/coffeecup.ico
--rw-r--r--   0 Newville   (501) staff       (20)   151792 2018-10-07 20:14:33.000000 pyshortcuts-1.8.3/examples/icons/microscope.icns
--rw-r--r--   0 Newville   (501) staff       (20)   184915 2018-10-07 20:14:33.000000 pyshortcuts-1.8.3/examples/icons/microscope.ico
--rw-r--r--   0 Newville   (501) staff       (20)    95882 2018-10-07 18:01:19.000000 pyshortcuts-1.8.3/examples/icons/python.icns
--rw-r--r--   0 Newville   (501) staff       (20)   167233 2018-10-07 18:01:22.000000 pyshortcuts-1.8.3/examples/icons/python.ico
--rw-r--r--   0 Newville   (501) staff       (20)    37653 2018-10-08 21:25:33.000000 pyshortcuts-1.8.3/examples/icons/stopwatch.icns
--rw-r--r--   0 Newville   (501) staff       (20)    67646 2018-10-08 21:26:18.000000 pyshortcuts-1.8.3/examples/icons/stopwatch.ico
--rw-r--r--   0 Newville   (501) staff       (20)   110445 2018-10-07 20:14:57.000000 pyshortcuts-1.8.3/examples/icons/wheelbarrow.icns
--rw-r--r--   0 Newville   (501) staff       (20)   370070 2018-10-07 20:14:57.000000 pyshortcuts-1.8.3/examples/icons/wheelbarrow.ico
--rw-r--r--   0 Newville   (501) staff       (20)      335 2019-09-22 02:29:32.000000 pyshortcuts-1.8.3/examples/mmmm.py
--rw-r--r--   0 Newville   (501) staff       (20)      208 2022-01-28 18:21:22.000000 pyshortcuts-1.8.3/pyproject.toml
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-23 20:42:28.820657 pyshortcuts-1.8.3/pyshortcuts/
--rw-r--r--   0 Newville   (501) staff       (20)     4867 2022-03-05 22:01:02.000000 pyshortcuts-1.8.3/pyshortcuts/__init__.py
--rw-r--r--   0 Newville   (501) staff       (20)     5650 2022-11-04 00:33:24.000000 pyshortcuts-1.8.3/pyshortcuts/darwin.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-23 20:42:28.823361 pyshortcuts-1.8.3/pyshortcuts/icons/
--rw-r--r--   0 Newville   (501) staff       (20)    65247 2020-12-09 20:20:47.000000 pyshortcuts-1.8.3/pyshortcuts/icons/ladder.icns
--rw-r--r--   0 Newville   (501) staff       (20)   370070 2020-12-09 20:20:47.000000 pyshortcuts-1.8.3/pyshortcuts/icons/ladder.ico
--rw-r--r--   0 Newville   (501) staff       (20)     5780 2020-12-09 20:20:47.000000 pyshortcuts-1.8.3/pyshortcuts/icons/ladder.png
--rw-r--r--   0 Newville   (501) staff       (20)    95882 2018-10-11 02:26:47.000000 pyshortcuts-1.8.3/pyshortcuts/icons/py.icns
--rw-r--r--   0 Newville   (501) staff       (20)   167233 2018-10-11 02:26:47.000000 pyshortcuts-1.8.3/pyshortcuts/icons/py.ico
--rw-r--r--   0 Newville   (501) staff       (20)     4735 2022-11-04 02:31:08.000000 pyshortcuts-1.8.3/pyshortcuts/linux.py
--rw-r--r--   0 Newville   (501) staff       (20)     4181 2022-11-03 23:24:12.000000 pyshortcuts-1.8.3/pyshortcuts/shortcut.py
--rw-r--r--   0 Newville   (501) staff       (20)       91 2019-09-25 20:19:15.000000 pyshortcuts-1.8.3/pyshortcuts/utils.py
--rw-r--r--   0 Newville   (501) staff       (20)      176 2022-11-23 20:42:28.000000 pyshortcuts-1.8.3/pyshortcuts/version.py
--rw-r--r--   0 Newville   (501) staff       (20)     5476 2022-11-03 23:25:51.000000 pyshortcuts-1.8.3/pyshortcuts/windows.py
--rw-r--r--   0 Newville   (501) staff       (20)    12359 2022-11-23 01:41:16.000000 pyshortcuts-1.8.3/pyshortcuts/wxgui.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-23 20:42:28.821476 pyshortcuts-1.8.3/pyshortcuts.egg-info/
--rw-r--r--   0 Newville   (501) staff       (20)     2425 2022-11-23 20:42:28.000000 pyshortcuts-1.8.3/pyshortcuts.egg-info/PKG-INFO
--rw-r--r--   0 Newville   (501) staff       (20)     1223 2022-11-23 20:42:28.000000 pyshortcuts-1.8.3/pyshortcuts.egg-info/SOURCES.txt
--rw-r--r--   0 Newville   (501) staff       (20)        1 2022-11-23 20:42:28.000000 pyshortcuts-1.8.3/pyshortcuts.egg-info/dependency_links.txt
--rw-r--r--   0 Newville   (501) staff       (20)       56 2022-11-23 20:42:28.000000 pyshortcuts-1.8.3/pyshortcuts.egg-info/entry_points.txt
--rw-r--r--   0 Newville   (501) staff       (20)       41 2022-11-23 20:42:28.000000 pyshortcuts-1.8.3/pyshortcuts.egg-info/requires.txt
--rw-r--r--   0 Newville   (501) staff       (20)       12 2022-11-23 20:42:28.000000 pyshortcuts-1.8.3/pyshortcuts.egg-info/top_level.txt
--rw-r--r--   0 Newville   (501) staff       (20)     2632 2022-11-23 20:42:28.824910 pyshortcuts-1.8.3/setup.cfg
--rw-r--r--   0 Newville   (501) staff       (20)       92 2022-01-28 18:08:54.000000 pyshortcuts-1.8.3/setup.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-23 20:42:28.823947 pyshortcuts-1.8.3/tests/
--rw-r--r--   0 Newville   (501) staff       (20)      501 2019-09-25 20:19:15.000000 pyshortcuts-1.8.3/tests/make_timer_bat.bat
--rw-r--r--   0 Newville   (501) staff       (20)     1599 2020-01-09 15:19:25.000000 pyshortcuts-1.8.3/tests/test_pyshortcuts.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-08 17:05:17.265981 pyshortcuts-1.9.0/
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-08 17:05:17.248187 pyshortcuts-1.9.0/.github/
+-rw-r--r--   0 Newville   (501) staff       (20)      502 2022-03-03 01:54:53.000000 pyshortcuts-1.9.0/.github/dependabot.yml
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-08 17:05:17.248951 pyshortcuts-1.9.0/.github/workflows/
+-rw-r--r--   0 Newville   (501) staff       (20)      731 2023-05-07 17:54:02.000000 pyshortcuts-1.9.0/.github/workflows/test-macos.yml
+-rw-r--r--   0 Newville   (501) staff       (20)      735 2023-05-07 17:54:02.000000 pyshortcuts-1.9.0/.github/workflows/test-ubuntu.yml
+-rw-r--r--   0 Newville   (501) staff       (20)      745 2023-05-07 17:54:02.000000 pyshortcuts-1.9.0/.github/workflows/test-windows.yml
+-rw-r--r--   0 Newville   (501) staff       (20)      115 2022-03-03 01:54:20.000000 pyshortcuts-1.9.0/.gitignore
+-rw-r--r--   0 Newville   (501) staff       (20)     1107 2018-10-13 13:02:16.000000 pyshortcuts-1.9.0/LICENSE
+-rw-r--r--   0 Newville   (501) staff       (20)      355 2022-01-28 18:15:23.000000 pyshortcuts-1.9.0/MANIFEST.in
+-rw-r--r--   0 Newville   (501) staff       (20)     2426 2023-05-08 17:05:17.266115 pyshortcuts-1.9.0/PKG-INFO
+-rw-r--r--   0 Newville   (501) staff       (20)     8844 2023-05-07 20:59:01.000000 pyshortcuts-1.9.0/README.md
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-08 17:05:17.249106 pyshortcuts-1.9.0/doc/
+-rw-r--r--   0 Newville   (501) staff       (20)   264749 2019-09-25 20:19:15.000000 pyshortcuts-1.9.0/doc/pyshortcutgui_screenshot.png
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-08 17:05:17.251445 pyshortcuts-1.9.0/examples/
+-rw-r--r--   0 Newville   (501) staff       (20)     6148 2023-05-08 14:52:34.000000 pyshortcuts-1.9.0/examples/.DS_Store
+-rw-r--r--   0 Newville   (501) staff       (20)       96 2018-10-11 23:54:21.000000 pyshortcuts-1.9.0/examples/README.md
+-rw-r--r--   0 Newville   (501) staff       (20)    50587 2023-05-07 18:10:07.000000 pyshortcuts-1.9.0/examples/S.zip
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-08 17:05:17.251690 pyshortcuts-1.9.0/examples/console_scripts/
+-rw-r--r--   0 Newville   (501) staff       (20)      890 2018-10-11 23:54:21.000000 pyshortcuts-1.9.0/examples/console_scripts/timer.py
+-rw-r--r--   0 Newville   (501) staff       (20)      334 2019-02-10 16:27:05.000000 pyshortcuts-1.9.0/examples/gui_bootstrap.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-08 17:05:17.260606 pyshortcuts-1.9.0/examples/icons/
+-rw-r--r--   0 Newville   (501) staff       (20)    59139 2018-10-07 20:14:46.000000 pyshortcuts-1.9.0/examples/icons/coffeecup.icns
+-rw-r--r--   0 Newville   (501) staff       (20)   161862 2018-10-07 20:14:46.000000 pyshortcuts-1.9.0/examples/icons/coffeecup.ico
+-rw-r--r--   0 Newville   (501) staff       (20)   151792 2018-10-07 20:14:33.000000 pyshortcuts-1.9.0/examples/icons/microscope.icns
+-rw-r--r--   0 Newville   (501) staff       (20)   184915 2018-10-07 20:14:33.000000 pyshortcuts-1.9.0/examples/icons/microscope.ico
+-rw-r--r--   0 Newville   (501) staff       (20)    95882 2018-10-07 18:01:19.000000 pyshortcuts-1.9.0/examples/icons/python.icns
+-rw-r--r--   0 Newville   (501) staff       (20)   167233 2018-10-07 18:01:22.000000 pyshortcuts-1.9.0/examples/icons/python.ico
+-rw-r--r--   0 Newville   (501) staff       (20)    67141 2023-05-07 18:41:16.000000 pyshortcuts-1.9.0/examples/icons/shovel.icns
+-rw-r--r--   0 Newville   (501) staff       (20)     2300 2023-05-07 18:41:16.000000 pyshortcuts-1.9.0/examples/icons/shovel.ico
+-rw-r--r--   0 Newville   (501) staff       (20)     4919 2023-05-07 18:41:16.000000 pyshortcuts-1.9.0/examples/icons/shovel.png
+-rw-r--r--   0 Newville   (501) staff       (20)    37653 2018-10-08 21:25:33.000000 pyshortcuts-1.9.0/examples/icons/stopwatch.icns
+-rw-r--r--   0 Newville   (501) staff       (20)    67646 2018-10-08 21:26:18.000000 pyshortcuts-1.9.0/examples/icons/stopwatch.ico
+-rw-r--r--   0 Newville   (501) staff       (20)   110445 2018-10-07 20:14:57.000000 pyshortcuts-1.9.0/examples/icons/wheelbarrow.icns
+-rw-r--r--   0 Newville   (501) staff       (20)   370070 2018-10-07 20:14:57.000000 pyshortcuts-1.9.0/examples/icons/wheelbarrow.ico
+-rw-r--r--   0 Newville   (501) staff       (20)      683 2023-05-07 20:59:01.000000 pyshortcuts-1.9.0/examples/make_pip_updater.py
+-rw-r--r--   0 Newville   (501) staff       (20)      199 2023-05-07 17:54:02.000000 pyshortcuts-1.9.0/pyproject.toml
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-08 17:05:17.262465 pyshortcuts-1.9.0/pyshortcuts/
+-rw-r--r--   0 Newville   (501) staff       (20)     4806 2023-05-07 20:59:01.000000 pyshortcuts-1.9.0/pyshortcuts/__init__.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4671 2023-05-07 20:59:01.000000 pyshortcuts-1.9.0/pyshortcuts/darwin.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-08 17:05:17.265224 pyshortcuts-1.9.0/pyshortcuts/icons/
+-rw-r--r--   0 Newville   (501) staff       (20)    65247 2020-12-09 20:20:47.000000 pyshortcuts-1.9.0/pyshortcuts/icons/ladder.icns
+-rw-r--r--   0 Newville   (501) staff       (20)   370070 2020-12-09 20:20:47.000000 pyshortcuts-1.9.0/pyshortcuts/icons/ladder.ico
+-rw-r--r--   0 Newville   (501) staff       (20)     5780 2020-12-09 20:20:47.000000 pyshortcuts-1.9.0/pyshortcuts/icons/ladder.png
+-rw-r--r--   0 Newville   (501) staff       (20)    95882 2018-10-11 02:26:47.000000 pyshortcuts-1.9.0/pyshortcuts/icons/py.icns
+-rw-r--r--   0 Newville   (501) staff       (20)   167233 2018-10-11 02:26:47.000000 pyshortcuts-1.9.0/pyshortcuts/icons/py.ico
+-rw-r--r--   0 Newville   (501) staff       (20)     4870 2023-05-07 20:59:01.000000 pyshortcuts-1.9.0/pyshortcuts/linux.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4408 2023-05-07 20:59:01.000000 pyshortcuts-1.9.0/pyshortcuts/shortcut.py
+-rw-r--r--   0 Newville   (501) staff       (20)       91 2019-09-25 20:19:15.000000 pyshortcuts-1.9.0/pyshortcuts/utils.py
+-rw-r--r--   0 Newville   (501) staff       (20)      160 2023-05-08 17:05:17.000000 pyshortcuts-1.9.0/pyshortcuts/version.py
+-rw-r--r--   0 Newville   (501) staff       (20)     5351 2023-05-07 20:59:01.000000 pyshortcuts-1.9.0/pyshortcuts/windows.py
+-rw-r--r--   0 Newville   (501) staff       (20)    12442 2023-05-07 17:54:02.000000 pyshortcuts-1.9.0/pyshortcuts/wxgui.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-08 17:05:17.263367 pyshortcuts-1.9.0/pyshortcuts.egg-info/
+-rw-r--r--   0 Newville   (501) staff       (20)     2426 2023-05-08 17:05:17.000000 pyshortcuts-1.9.0/pyshortcuts.egg-info/PKG-INFO
+-rw-r--r--   0 Newville   (501) staff       (20)     1329 2023-05-08 17:05:17.000000 pyshortcuts-1.9.0/pyshortcuts.egg-info/SOURCES.txt
+-rw-r--r--   0 Newville   (501) staff       (20)        1 2023-05-08 17:05:17.000000 pyshortcuts-1.9.0/pyshortcuts.egg-info/dependency_links.txt
+-rw-r--r--   0 Newville   (501) staff       (20)       56 2023-05-08 17:05:17.000000 pyshortcuts-1.9.0/pyshortcuts.egg-info/entry_points.txt
+-rw-r--r--   0 Newville   (501) staff       (20)       41 2023-05-08 17:05:17.000000 pyshortcuts-1.9.0/pyshortcuts.egg-info/requires.txt
+-rw-r--r--   0 Newville   (501) staff       (20)       12 2023-05-08 17:05:17.000000 pyshortcuts-1.9.0/pyshortcuts.egg-info/top_level.txt
+-rw-r--r--   0 Newville   (501) staff       (20)     2633 2023-05-08 17:05:17.266613 pyshortcuts-1.9.0/setup.cfg
+-rw-r--r--   0 Newville   (501) staff       (20)       92 2022-01-28 18:08:54.000000 pyshortcuts-1.9.0/setup.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-08 17:05:17.265799 pyshortcuts-1.9.0/tests/
+-rw-r--r--   0 Newville   (501) staff       (20)      501 2019-09-25 20:19:15.000000 pyshortcuts-1.9.0/tests/make_timer_bat.bat
+-rw-r--r--   0 Newville   (501) staff       (20)     1599 2020-01-09 15:19:25.000000 pyshortcuts-1.9.0/tests/test_pyshortcuts.py
```

### Comparing `pyshortcuts-1.8.3/.github/workflows/test-macos.yml` & `pyshortcuts-1.9.0/.github/workflows/test-macos.yml`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 jobs:
   build:
     runs-on: macos-latest
     strategy:
       max-parallel: 5
       fail-fast: false
       matrix:
-        python-version: [3.7, 3.8, 3.9, "3.10"]
+        python-version: [3.8, 3.9, "3.10", 3.11]
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python from Miniconda
       uses: actions/setup-python@v2
       with:
           python-version: ${{ matrix.python-version }}
     - name: Install dependencies
```

### Comparing `pyshortcuts-1.8.3/.github/workflows/test-ubuntu.yml` & `pyshortcuts-1.9.0/.github/workflows/test-ubuntu.yml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       max-parallel: 5
       fail-fast: false
       matrix:
-        python-version: [3.7, 3.8, 3.9, "3.10"]
+        python-version: [3.8, 3.9, "3.10", "3.11"]
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python from Miniconda
       uses: actions/setup-python@v2
       with:
           python-version: ${{ matrix.python-version }}
     - name: Install dependencies
```

### Comparing `pyshortcuts-1.8.3/.github/workflows/test-windows.yml` & `pyshortcuts-1.9.0/.github/workflows/test-windows.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 jobs:
   build:
     runs-on: windows-latest
     strategy:
       max-parallel: 5
       fail-fast: false
       matrix:
-        python-version: [3.7, 3.8, 3.9, "3.10"]
+        python-version: [3.8, 3.9, "3.10", "3.11"]
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python from Miniconda
       uses: actions/setup-python@v2
       with:
           python-version: ${{ matrix.python-version }}
     - name: Install dependencies
```

### Comparing `pyshortcuts-1.8.3/LICENSE` & `pyshortcuts-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyshortcuts-1.8.3/PKG-INFO` & `pyshortcuts-1.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshortcuts
-Version: 1.8.3
+Version: 1.9.0
 Summary: Create desktop and Start Menu shortcuts for python scripts
 Home-page: https://github.com/newville/pyshortcuts
 Author: Matthew Newville
 Author-email: matt.newville@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/newville/pyshortcuts
 Project-URL: Documentation, https://github.com/newville/pyshortcuts/README.md
@@ -16,20 +16,20 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 
 
 Pyshortcuts helps developers and Python users to create shortcuts on a
 Users Desktop or Start Menu that will run python scripts and applications.
 Pyshortcuts is cross-platform, supporting Windows, MacOS, and Linux each in
 the way most natural for the OS.  On Windows, a Shortcut or Link is
```

### Comparing `pyshortcuts-1.8.3/README.md` & `pyshortcuts-1.9.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,59 +4,58 @@
 
 [![Version](https://img.shields.io/pypi/v/pyshortcuts.svg)](https://pypi.org/project/pyshortcuts)
 [![Downloads](https://pepy.tech/badge/pyshortcuts/month)](https://pepy.tech/project/pyshortcuts)
 
 # pyshortcuts
 
 
-Pyshortcuts helps Python developers and users create shortcuts that will
-run python scripts and other applications.  The shortcuts created can go
-onto the users desktop or into the Start Menu (for systems with Start
-Menus) or both.
-
-Pyshortcuts works on Windows, MacOS, and Linux in the way that is most
-natural for each OS.  On Windows, a Shortcut Link is created and
-placed on the users Desktop and in the Start Menu. On MacOS, a minimal but
-complete Application is created and placed on the users Desktop.  On Linux
-a ".desktop" file is created and placed on the users Desktop (if that
-exists) and in $HOME/.local/share/applications (if that exists), which will
-often get presented in a Start Menu for windowing desktop themes that use a
-one.  On all platforms, the shortcuts created on the Deskop or Start
-Menu can be put either directly onto the Desktop / Start Menu or in a sub-folder
-of the Desktop / Start Menu.
-
-Special attention is given to Anaconda Python.  On Windows, this means the
-program linked to by the shortcut will be run in an Anaconda environment,
-explicitly selecting the "base" environment even if that has not been
-explicitly set.  On MacOS, the shortcut will make sure to use the
-`python.app` application so that GUI programs will be able to draw to
-properly draw to the screen.
-
-By writing only to the users Desktop or application folder that gets read
-by the Start Menu, there is no need for elevated permission and no writing
-to system-level files (registry entries, /Applications, /usr/bin, etc).
-After the shortcut has been created, the user has complete control to
-rename, move, or delete it.  Shortcuts can have a custom icon (`.ico` files
-on Windows or Linux, or `.icns` files on MacOS) specified, defaulting to a
-Python icon included with pyshortcuts.
-
-Pyshortcuts is pure python, small, easy to install, and easy to use from a
-python script.   This means that Pyshortcuts can be made part of an
-installation (or post-installation process) process for larger packages.
+Pyshortcuts helps Python developers and users create shortcuts that will run
+python scripts and other applications.  The shortcuts created can go onto the
+users desktop or into the Start Menu (for systems with Start Menus) or both.
+Pyshortcuts gives a consistent interface for building shortcuts that run on
+Windows, macOS, and Linux in the way that is most natural for each OS.
+
+On Windows, a Shortcut Link is created and placed on the users Desktop and in
+the Start Menu. On macOS, a minimal but complete Application is created and
+placed on the users Desktop.  On Linux a ".desktop" file is created and placed
+on the users Desktop (if that exists) and in $HOME/.local/share/applications
+(if that exists), which will often get presented in a Start Menu for windowing
+desktop themes that use a one.  On all platforms, the shortcuts created on the
+Deskop or Start Menu can be put either directly onto the Desktop / Start Menu
+or in a sub-folder of the Desktop / Start Menu.  Shortcuts can have a custom
+icon (`.ico` files on Windows or Linux, or `.icns` files on macOS) specified,
+defaulting to a Python icon included with pyshortcuts.
+
+
+By writing only to the users Desktop or application folder that gets read by
+the Start Menu, there is no need for elevated permission and no writing to
+system-level files (registry entries, /Applications, /usr/bin, etc).  After the
+shortcut has been created, the end user has complete control to rename, move,
+or delete it.
+
+Pyshortcuts is pure python, small, readily installed, and easy to use from a
+the command-line or from Python scripts.  This means that Pyshortcuts can be
+made part of an installation (or post-installation process) process for larger
+packages.
+
+Special attention is given to Anaconda Python on Windows.  For that
+environment, the shortcut created will be sure to run in an Anaconda
+environment, explicitly selecting the "base" environment even if that has not
+been explicitly set by the user.
 
 ## installation
 
 To install `pyshortcuts`, use
 
 ```
 pip install pyshortcuts
 ```
 
 On Windows, pyshortcuts requires the pywin32 package and will be installed
-automatically if needed.
+if needed. There are no depenendencies on macOS or Linux.
 
 In order to use the pyshortcut GUI, the wxPython package is required.
 
 ## usage from Python
 
 Shortcuts can be created from a Python script with
 
@@ -75,22 +74,22 @@
   * `icon`        (str or None) path to icon file [defaults to python icon]
   * `folder`      (str or None) folder on Desktop to put shortcut [defaults to Desktop]
   * `terminal`    (bool) whether to run in a Terminal [True]
   * `desktop`  ((bool) whether to add shortcut to Desktop [True]
   * `startmenu`   (bool) whether to add shortcut to Start Menu [True]
   * `executable`  (str or None) name of executable to use [this Python]
 
-Note that the Start Menu does not exist for MacOSX.
+Note that the Start Menu does not exist for macOSX.
 
 The `executable` defaults to the version of Python executable used to make shortcut.
 
 
 ##  `pyshortcut` command-line program
 
-pyshortcuts also installs a `pyshortcut` command-line program for creating a shortcut.
+Pyshortcuts installs a `pyshortcut` command-line program for creating a shortcut.
 From a shell or Command window with PATH set to include python programs and scripts,
 a command to create a shortcut might look like:
 
 ```
 ~> pyshortcut -n MyApp -i /home/user/icons/myicon.icns  /home/user/bin/myapp.py
 ```
 
@@ -130,14 +129,64 @@
 
 Note that running in the Terminal is True by default, which means that each
 time the shortcut is used to launch the application, a new Terminal or Command
 window will be created for it.  For many command-line applications, this is
 appropriate.  The extra Terminal or Command window may be unwanted for some GUI
 applications, and can be disabled with the `-g` or `--gui` option.
 
+## Making a shortcut for single python command
+
+A common request and simple use-case for `pyshortcuts` is to wrap a single
+python command.  An example of this might look like this:
+
+```
+import sys
+from pyshortcuts import make_shortcut
+
+pycmd = "_ -m pip install --upgrade pyshortcuts"
+
+make_shortcut(pycmd, name='Update Pyshortcuts')
+```
+
+Note that using `_` or `{}` as the command name will indicate that the
+current Python executable should be be used. An example that includes
+an icon is given in the examples folder.
+
+The above could be done from the command line with
+
+```
+~> pyshortcut -n "Update Pyshortcuts" "_ -m pip install pyshortcuts"
+```
+
+## Note for running wxPython GUIs on macOS with Anaconda Python
+
+If your application uses wxPython and you are running with Anaconda Python on
+macOS, you may experience problems that your application does not start.  If
+you try to run your script from the command line, you may see the following
+error message:
+
+
+```
+~> python my_wxpython_app.py
+This program needs access to the screen. Please run with a
+Framework build of python, and only when you are logged in
+on the main display of your Mac.
+```
+
+
+If you do see that, it can be fixed and your script run properly by adding
+
+```
+import wx
+wx.PyApp.IsDisplayAvailable = lambda _: True
+```
+
+in your script before runnig your starting the `wxPython` `mainloop` event handler.
+
+
 
 ## `pyshortcut` GUI
 
 In addition to the `pyshortcut` command-line program, there is a small GUI
 application that provides a simple form to help the user browse for script
 and icons, and set options before creating a shortcut or generating an
 example Python script to create the shortcut.
```

### Comparing `pyshortcuts-1.8.3/doc/pyshortcutgui_screenshot.png` & `pyshortcuts-1.9.0/doc/pyshortcutgui_screenshot.png`

 * *Files identical despite different names*

### Comparing `pyshortcuts-1.8.3/examples/.DS_Store` & `pyshortcuts-1.9.0/examples/.DS_Store`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
-00000010: 0000 1000 0000 0087 0000 0000 0000 0000  ................
+00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0002  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0004  ................
 00000050: 0000 0001 0000 1000 006f 006c 0065 005f  .........o.l.e._
 00000060: 0073 0063 0000 0000 0000 0000 0000 0000  .s.c............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000080: 0000 0000 0000 0000 0000 0002 0000 000f  ................
-00000090: 0063 006f 006e 0073 006f 006c 0065 005f  .c.o.n.s.o.l.e._
-000000a0: 0073 0063 0072 0069 0070 0074 0073 6664  .s.c.r.i.p.t.sfd
-000000b0: 7363 626f 6f6c 0100 0000 0500 6900 6300  scbool......i.c.
-000000c0: 6f00 6e00 7366 6473 6362 6f6f 6c01 0000  o.n.sfdscbool...
+00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,34 +26,34 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000200: 0000 0000 0000 0000 0000 0004 0000 000f  ................
+00000210: 0063 006f 006e 0073 006f 006c 0065 005f  .c.o.n.s.o.l.e._
+00000220: 0073 0063 0072 0069 0070 0074 0073 6664  .s.c.r.i.p.t.sfd
+00000230: 7363 626f 6f6c 0100 0000 0500 6900 6300  scbool......i.c.
+00000240: 6f00 6e00 7362 7773 7062 6c6f 6200 0000  o.n.sbwspblob...
+00000250: b862 706c 6973 7430 30d6 0102 0304 0506  .bplist00.......
+00000260: 0708 0708 0b08 5d53 686f 7753 7461 7475  ......]ShowStatu
+00000270: 7342 6172 5b53 686f 7754 6f6f 6c62 6172  sBar[ShowToolbar
+00000280: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
+00000290: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
+000002a0: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
+000002b0: 5b53 686f 7753 6964 6562 6172 0809 0809  [ShowSidebar....
+000002c0: 5f10 187b 7b31 3130 2c20 3435 307d 2c20  _..{{110, 450}, 
+000002d0: 7b39 3230 2c20 3433 367d 7d09 0815 232f  {920, 436}}...#/
+000002e0: 3b52 5f6b 6c6d 6e6f 8a00 0000 0000 0001  ;R_klmno........
+000002f0: 0100 0000 0000 0000 0d00 0000 0000 0000  ................
+00000300: 0000 0000 0000 0000 8b00 0000 0500 6900  ..............i.
+00000310: 6300 6f00 6e00 7366 6473 6362 6f6f 6c01  c.o.n.sfdscbool.
+00000320: 0000 0005 0069 0063 006f 006e 0073 7653  .....i.c.o.n.svS
+00000330: 726e 6c6f 6e67 0000 0001 0000 0000 0000  rnlong..........
 00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,15 +251,15 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0003 0000 0000 0000 100b  ................
-00001010: 0000 0045 0000 0087 0000 0000 0000 0000  ...E............
+00001010: 0000 0045 0000 0209 0000 0000 0000 0000  ...E............
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -318,15 +318,15 @@
 000013d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00001440: 0000 0000 0100 0001 0000 0000 0100 0002  ................
+00001440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
 00001450: 0000 0000 0100 0004 0000 0000 0200 0008  ................
 00001460: 0000 0018 0000 0000 0000 0000 0100 0020  ............... 
 00001470: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
 00001480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 000014a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 000014b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
```

### Comparing `pyshortcuts-1.8.3/examples/console_scripts/timer.py` & `pyshortcuts-1.9.0/examples/console_scripts/timer.py`

 * *Files identical despite different names*

### Comparing `pyshortcuts-1.8.3/examples/icons/coffeecup.icns` & `pyshortcuts-1.9.0/examples/icons/coffeecup.icns`

 * *Files identical despite different names*

### Comparing `pyshortcuts-1.8.3/examples/icons/coffeecup.ico` & `pyshortcuts-1.9.0/examples/icons/coffeecup.ico`

 * *Files identical despite different names*

### Comparing `pyshortcuts-1.8.3/examples/icons/microscope.icns` & `pyshortcuts-1.9.0/examples/icons/microscope.icns`

 * *Files identical despite different names*

### Comparing `pyshortcuts-1.8.3/examples/icons/microscope.ico` & `pyshortcuts-1.9.0/examples/icons/microscope.ico`

 * *Files identical despite different names*

### Comparing `pyshortcuts-1.8.3/examples/icons/python.icns` & `pyshortcuts-1.9.0/examples/icons/python.icns`

 * *Files identical despite different names*

### Comparing `pyshortcuts-1.8.3/examples/icons/python.ico` & `pyshortcuts-1.9.0/examples/icons/python.ico`

 * *Files identical despite different names*

### Comparing `pyshortcuts-1.8.3/examples/icons/stopwatch.icns` & `pyshortcuts-1.9.0/examples/icons/stopwatch.icns`

 * *Files identical despite different names*

### Comparing `pyshortcuts-1.8.3/examples/icons/stopwatch.ico` & `pyshortcuts-1.9.0/examples/icons/stopwatch.ico`

 * *Files identical despite different names*

### Comparing `pyshortcuts-1.8.3/examples/icons/wheelbarrow.icns` & `pyshortcuts-1.9.0/examples/icons/wheelbarrow.icns`

 * *Files identical despite different names*

### Comparing `pyshortcuts-1.8.3/examples/icons/wheelbarrow.ico` & `pyshortcuts-1.9.0/examples/icons/wheelbarrow.ico`

 * *Files identical despite different names*

### Comparing `pyshortcuts-1.8.3/pyshortcuts/__init__.py` & `pyshortcuts-1.9.0/pyshortcuts/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,13 +131,11 @@
     else:
         if args.gui:
             args.terminal = False
 
         if args.scriptname is None:
             print("pyshortcut: must provide one script.  try 'pyshortcuts -h'")
         else:
-
-            desc = scriptname = args.scriptname
-            make_shortcut(scriptname, name=args.name, description=desc,
+            make_shortcut(args.scriptname, name=args.name, 
                           terminal=args.terminal, folder=args.folder,
                           icon=args.icon, desktop=args.desktop,
                           startmenu=args.startmenu, executable=args.exe)
```

### Comparing `pyshortcuts-1.8.3/pyshortcuts/darwin.py` & `pyshortcuts-1.9.0/pyshortcuts/darwin.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 Create desktop shortcuts for Darwin / MacOS
 """
 import os
 import sys
 import shutil
 
-from .shortcut import shortcut
+from .shortcut import shortcut, get_pyexe
 from .linux import get_homedir, get_desktop
 from . import UserFolders
 
 scut_ext = 'app'
 ico_ext = ('icns',)
 
 
@@ -32,33 +32,14 @@
     >>> folders = get_folders()
     >>> print("Home, Desktop, StartMenu ",
     ...       folders.home, folders.desktop, folders.startmenu)
     """
     return UserFolders(get_homedir(), get_desktop(), get_startmenu())
 
 
-def fix_anacondapy_pythonw(fname):
-    """fix shebang line for scripts using anaconda python
-    to use 'pythonw' instead of 'python'
-    """
-    # print(" fix anaconda py (%s) for %s" % (sys.prefix, script))
-    with open(fname, 'r') as fh:
-        try:
-            lines = fh.readlines()
-        except IOError:
-            lines = ['-']
-    firstline = lines[0][:-1].strip()
-    if firstline.startswith('#!') and 'python' in firstline:
-        firstline = '#!/usr/bin/env pythonw'
-        fh = open(fname, 'w')
-        fh.write('%s\n' % firstline)
-        fh.write("".join(lines[1:]))
-        fh.close()
-
-
 def make_shortcut(script, name=None, description=None, icon=None, working_dir=None,
                   folder=None, terminal=True, desktop=True,
                   startmenu=True, executable=None):
     """create shortcut
 
     Arguments:
     ---------
@@ -89,22 +70,19 @@
     scut = shortcut(script, userfolders, name=name, description=description,
                     working_dir=working_dir, folder=folder, icon=icon)
 
     osascript = '%s %s' % (scut.full_script, scut.arguments)
     osascript = osascript.replace(' ', '\\ ')
     prefix = os.path.normpath(sys.prefix)
     if executable is None:
-        executable = sys.executable
-        # check for Anaconda on MacOSX
-        has_conda = os.path.exists(os.path.join(prefix, 'conda-meta'))
-        pyapp_exe = "{:s}/python.app/Contents/MacOS/python".format(prefix)
-        if has_conda and os.path.exists(pyapp_exe):
-            executable = pyapp_exe
-            fix_anacondapy_pythonw(scut.full_script)
+        executable = get_pyexe()
+
     executable = os.path.normpath(executable)
+    if os.path.realpath(scut.full_script) == os.path.realpath(executable):
+        executable = ''
 
     if not os.path.exists(scut.desktop_dir):
         os.makedirs(scut.desktop_dir)
 
     dest = os.path.join(scut.desktop_dir, scut.target)
 
     if os.path.exists(dest):
@@ -135,19 +113,17 @@
   <key>CFBundleIconFile</key> <string>{name:s}</string>
   <key>CFBundlePackageType</key> <string>APPL</string>
   </dict>
 </plist>
 """
 
     text = ['#!/bin/bash',
-            "## Make sure to set PYTHONEXECUTABLE to Python that created this script",
-            "export PYTHONEXECUTABLE={prefix:s}/bin/python",
             "export EXE={exe:s}",
             "export SCRIPT={script:s}",
-            "export ARGS='{args:s}'", " "]
+            "export ARGS='{args:s}'"]
 
     if scut.working_dir not in (None, ''):
         text.append("cd {workdir:s}")
 
     if terminal:
         text.append("""osascript -e 'tell application "Terminal"
    do script "'${{EXE}}\ {osascript:s}'"
```

### Comparing `pyshortcuts-1.8.3/pyshortcuts/icons/ladder.icns` & `pyshortcuts-1.9.0/pyshortcuts/icons/ladder.icns`

 * *Files identical despite different names*

### Comparing `pyshortcuts-1.8.3/pyshortcuts/icons/ladder.ico` & `pyshortcuts-1.9.0/pyshortcuts/icons/ladder.ico`

 * *Files identical despite different names*

### Comparing `pyshortcuts-1.8.3/pyshortcuts/icons/ladder.png` & `pyshortcuts-1.9.0/pyshortcuts/icons/ladder.png`

 * *Files identical despite different names*

### Comparing `pyshortcuts-1.8.3/pyshortcuts/icons/py.icns` & `pyshortcuts-1.9.0/pyshortcuts/icons/py.icns`

 * *Files identical despite different names*

### Comparing `pyshortcuts-1.8.3/pyshortcuts/icons/py.ico` & `pyshortcuts-1.9.0/pyshortcuts/icons/py.ico`

 * *Files identical despite different names*

### Comparing `pyshortcuts-1.8.3/pyshortcuts/linux.py` & `pyshortcuts-1.9.0/pyshortcuts/linux.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 HAS_PWD = False
 try:
     import pwd
     HAS_PWD = True
 except ImportError:
     pass
 
-from .shortcut import shortcut
+from .shortcut import shortcut, get_pyexe
 from . import UserFolders
 
 scut_ext = 'desktop'
 ico_ext = ('ico', 'svg', 'png')
 
 DESKTOP_FORM = """[Desktop Entry]
 Name={name:s}
 Type=Application
 Path={workdir:s}
 Comment={desc:s}
 Terminal={term:s}
 Icon={icon:s}
-Exec={exe:s} {script:s} {args:s}
+Exec={execstring:s}
 """
 
 _HOME = None
 def get_homedir():
     "determine home directory of current user"
     global _HOME
     if _HOME is None:
@@ -122,21 +122,26 @@
     userfolders = get_folders()
     if working_dir is None:
         working_dir = userfolders.home
     scut = shortcut(script, userfolders, name=name, description=description,
                     working_dir=working_dir, folder=folder, icon=icon)
 
     if executable is None:
-        executable = sys.executable
+        executable = get_pyexe()
+
+    executable = os.path.normpath(executable)
+    if os.path.realpath(scut.full_script) == os.path.realpath(executable):
+        executable = ''
+
+    execstring=f"{executable:s} {scut.full_script:s} {scut.arguments:s}".strip()
 
     text = DESKTOP_FORM.format(name=scut.name, desc=scut.description,
                                workdir=scut.working_dir,
-                               exe=os.path.normpath(executable),
-                               icon=scut.icon, script=scut.full_script,
-                               args=scut.arguments,
+                               execstring=execstring,
+                               icon=scut.icon,
                                term='true' if terminal else 'false')
 
     for (create, folder) in ((desktop, scut.desktop_dir),
                              (startmenu, scut.startmenu_dir)):
         if create:
             if not os.path.exists(folder):
                 os.makedirs(folder)
```

### Comparing `pyshortcuts-1.8.3/pyshortcuts/shortcut.py` & `pyshortcuts-1.9.0/pyshortcuts/shortcut.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 #!/usr/bin/env python
-import os
 import sys
+import os
+from os.path import abspath, normpath, realpath
+from os.path import (split as path_split, join as path_join,
+                     exists as path_exists)
 from collections import namedtuple
 
 BAD_FILECHARS = ';~,`!%$@$&^?*#:"/|\'\\\t\r\n(){}[]<>'
 GOOD_FILECHARS = '_'*len(BAD_FILECHARS)
 
 
 def fix_filename(s, allow_multiple_dots=True):
@@ -18,14 +21,16 @@
     if not allow_multiple_dots:
         if t.count('.') > 1:
             for i in range(t.count('.') - 1):
                 idot = t.find('.')
                 t = "%s_%s" % (t[:idot], t[idot+1:])
     return t
 
+def get_pyexe():
+    return realpath(normpath(sys.executable))
 
 Shortcut = namedtuple("Shortcut", ('name', 'description', 'icon', 'target', 'working_dir',
                                    'script', 'full_script', 'arguments',
                                    'desktop_dir', 'startmenu_dir'))
 
 
 def shortcut(script, userfolders, name=None, description=None, folder=None, working_dir=None,
@@ -59,56 +64,59 @@
 
     """
     from . import platform, scut_ext, ico_ext
 
     if not isinstance(script, str) or len(script) < 1:
         raise ValueError("`script` for shortcut must be a non-zero length string")
 
-    words = script.split(' ', 1)
+    words = script.strip().split(' ', 1)
     if len(words) < 2:
         words.append('')
 
     script, arguments = words[0], words[1]
-
-    full_script = os.path.normpath(os.path.abspath(script))
+    if script in ('_', '{}'):
+        script = words[0] = get_pyexe()
+        
+    full_script = normpath(abspath(script))
 
     if name is None:
         name = script
-
-    _path, name = os.path.split(name)
+    
+    _path, name = path_split(name)
     name = fix_filename(name)
     if name.endswith('.py'):
         name = name[:-3]
 
     if description is None:
         description = name
 
     target = '%s.%s' % (name, scut_ext)
 
     if icon is not None and len(str(icon)) > 0:
-        icon = os.path.normpath(os.path.abspath(icon))
-        if not os.path.exists(icon):
+        icon = normpath(abspath(icon))
+        if not path_exists(icon):
             for ext in ico_ext:
                 ticon = "{:s}.{:s}".format(icon, ext)
-                if os.path.exists(ticon):
+                if path_exists(ticon):
                     icon = ticon
                     break
 
-    if icon is None or not os.path.exists(icon):
-        _path, _fname = os.path.split(__file__)
-        icon = os.path.normpath(os.path.join(os.path.abspath(_path), 'icons',
-                                             'py.{:s}'.format(ico_ext[0])))
+    if icon is None or not path_exists(icon):
+        _path, _fname = path_split(__file__)
+        icon = normpath(path_join(abspath(_path), 'icons',
+                                  'py.{:s}'.format(ico_ext[0])))
 
     desktop_dir = userfolders.desktop
     if folder is not None:
         if folder.startswith(desktop_dir):
             folder = folder[len(desktop_dir)+1:]
-        desktop_dir = os.path.normpath(os.path.join(desktop_dir, folder))
+        desktop_dir = normpath(path_join(desktop_dir, folder))
 
     startmenu_dir = userfolders.startmenu
     if folder is not None and len(startmenu_dir) > 1:
         if folder.startswith(startmenu_dir):
             folder = folder[len(startmenu_dir)+1:]
-        startmenu_dir = os.path.normpath(os.path.join(startmenu_dir, folder))
+        startmenu_dir = normpath(path_join(startmenu_dir, folder))
 
-    return Shortcut(name, description, icon, target, working_dir, script, full_script,
-                    arguments, desktop_dir, startmenu_dir)
+    return Shortcut(name, description, icon, target, working_dir,
+                    script, full_script, arguments, desktop_dir,
+                    startmenu_dir)
```

### Comparing `pyshortcuts-1.8.3/pyshortcuts/windows.py` & `pyshortcuts-1.9.0/pyshortcuts/windows.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 """
 Create desktop shortcuts for Windows
 """
 import os
 import sys
 import time
-from .shortcut import shortcut
+from .shortcut import shortcut, get_pyexe
 from . import UserFolders
 
 import win32com.client
 from win32com.shell import shell, shellcon
 
 scut_ext = 'lnk'
 ico_ext = ('ico',)
@@ -103,18 +103,17 @@
     3. executable defaults to the Python executable used to make shortcut.
     """
     userfolders = get_folders()
 
     scut = shortcut(script, userfolders, name=name, description=description, working_dir=working_dir,
                     folder=folder, icon=icon)
     full_script = scut.full_script
+    
     if executable is None:
-        pyexe = 'python.exe' if terminal else 'pythonw.exe'
-        pydir = os.path.dirname(sys.executable)
-        executable = os.path.normpath(os.path.join(pydir, pyexe))
+        executable = get_pyexe()
 
     # Check for other valid ways to run the script
     # try appending .exe if script itself not found
     if not os.path.exists(scut.full_script):
         tname = scut.full_script + '.exe'
         if os.path.exists(tname):
             executable = tname
```

### Comparing `pyshortcuts-1.8.3/pyshortcuts/wxgui.py` & `pyshortcuts-1.9.0/pyshortcuts/wxgui.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 ALL_LEFT =  wx.ALL|LEFT
 ALL_RIGHT =  wx.ALL|RIGHT
 
 FONTSIZE = 11
 if platform == 'linux':
     FONTSIZE = 10
 
+if platform.startswith('darwin'):
+    wx.PyApp.IsDisplayAvailable = lambda _: True
 
 class ShortcutFrame(wx.Frame):
     def __init__(self):
 
         wx.Frame.__init__(self, None, -1, 'Pyshortcuts Creator',
                           style=wx.DEFAULT_FRAME_STYLE|wx.RESIZE_BORDER|wx.TAB_TRAVERSAL)
         self.SetTitle('Pyshortcuts Creator')
```

### Comparing `pyshortcuts-1.8.3/pyshortcuts.egg-info/PKG-INFO` & `pyshortcuts-1.9.0/pyshortcuts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshortcuts
-Version: 1.8.3
+Version: 1.9.0
 Summary: Create desktop and Start Menu shortcuts for python scripts
 Home-page: https://github.com/newville/pyshortcuts
 Author: Matthew Newville
 Author-email: matt.newville@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/newville/pyshortcuts
 Project-URL: Documentation, https://github.com/newville/pyshortcuts/README.md
@@ -16,20 +16,20 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 
 
 Pyshortcuts helps developers and Python users to create shortcuts on a
 Users Desktop or Start Menu that will run python scripts and applications.
 Pyshortcuts is cross-platform, supporting Windows, MacOS, and Linux each in
 the way most natural for the OS.  On Windows, a Shortcut or Link is
```

### Comparing `pyshortcuts-1.8.3/pyshortcuts.egg-info/SOURCES.txt` & `pyshortcuts-1.9.0/pyshortcuts.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,23 +8,27 @@
 .github/dependabot.yml
 .github/workflows/test-macos.yml
 .github/workflows/test-ubuntu.yml
 .github/workflows/test-windows.yml
 doc/pyshortcutgui_screenshot.png
 examples/.DS_Store
 examples/README.md
+examples/S.zip
 examples/gui_bootstrap.py
-examples/mmmm.py
+examples/make_pip_updater.py
 examples/console_scripts/timer.py
 examples/icons/coffeecup.icns
 examples/icons/coffeecup.ico
 examples/icons/microscope.icns
 examples/icons/microscope.ico
 examples/icons/python.icns
 examples/icons/python.ico
+examples/icons/shovel.icns
+examples/icons/shovel.ico
+examples/icons/shovel.png
 examples/icons/stopwatch.icns
 examples/icons/stopwatch.ico
 examples/icons/wheelbarrow.icns
 examples/icons/wheelbarrow.ico
 pyshortcuts/__init__.py
 pyshortcuts/darwin.py
 pyshortcuts/linux.py
```

### Comparing `pyshortcuts-1.8.3/setup.cfg` & `pyshortcuts-1.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -20,40 +20,40 @@
 	easily be part of a installation (or post-installation process) process for
 	larger packages.
 author = Matthew Newville
 author_email = matt.newville@gmail.com
 url = https://github.com/newville/pyshortcuts
 license = MIT License
 platforms = any
-version = 1.8.1
+version = 1.9.0
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: End Users/Desktop
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: PyPy
 keywords = desktop shortcuts
 project_urls = 
 	Source =  https://github.com/newville/pyshortcuts
 	Documentation = https://github.com/newville/pyshortcuts/README.md
 	Tracker = https://github.com/newville/pyshortcuts/issues
 
 [options]
 packages = find:
 include_package_data = True
-python_requires = >=3.6
+python_requires = >=3.8
 setup_requires = setuptools_scm
 install_requires = 
 	pywin32 ; platform_system== "Windows"
 
 [options.package_data]
 * = icons/*
```

### Comparing `pyshortcuts-1.8.3/tests/test_pyshortcuts.py` & `pyshortcuts-1.9.0/tests/test_pyshortcuts.py`

 * *Files identical despite different names*

