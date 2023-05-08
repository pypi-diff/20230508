# Comparing `tmp/jdDiff-1.3.tar.gz` & `tmp/jdDiff-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdDiff-1.3.tar", last modified: Mon Dec  5 21:33:33 2022, max compression
+gzip compressed data, was "jdDiff-1.4.tar", last modified: Mon May  8 08:37:41 2023, max compression
```

## Comparing `jdDiff-1.3.tar` & `jdDiff-1.4.tar`

### file list

```diff
@@ -1,31 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 21:33:33.943069 jdDiff-1.3/
--rw-rw-rw-   0 root         (0) root         (0)    35064 2022-12-05 21:33:14.000000 jdDiff-1.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2022-12-05 21:33:14.000000 jdDiff-1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1599 2022-12-05 21:33:33.942152 jdDiff-1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       49 2022-12-05 21:33:14.000000 jdDiff-1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 21:33:33.940319 jdDiff-1.3/jdDiff/
--rw-rw-rw-   0 root         (0) root         (0)      580 2022-12-05 21:33:14.000000 jdDiff-1.3/jdDiff/AboutDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2022-12-05 21:33:14.000000 jdDiff-1.3/jdDiff/AboutDialog.ui
--rw-rw-rw-   0 root         (0) root         (0)     5578 2022-12-05 21:33:14.000000 jdDiff-1.3/jdDiff/BrowseDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     2913 2022-12-05 21:33:14.000000 jdDiff-1.3/jdDiff/BrowseDialog.ui
--rw-rw-rw-   0 root         (0) root         (0)     5186 2022-12-05 21:33:14.000000 jdDiff-1.3/jdDiff/CompareThread.py
--rw-rw-rw-   0 root         (0) root         (0)     1209 2022-12-05 21:33:14.000000 jdDiff-1.3/jdDiff/Enviroment.py
--rw-rw-rw-   0 root         (0) root         (0)     2518 2022-12-05 21:33:14.000000 jdDiff-1.3/jdDiff/Functions.py
--rw-rw-rw-   0 root         (0) root         (0)     2978 2022-12-05 21:33:14.000000 jdDiff-1.3/jdDiff/Icon.svg
--rw-rw-rw-   0 root         (0) root         (0)     4087 2022-12-05 21:33:14.000000 jdDiff-1.3/jdDiff/MainWindow.py
--rw-rw-rw-   0 root         (0) root         (0)     4799 2022-12-05 21:33:14.000000 jdDiff-1.3/jdDiff/MainWindow.ui
--rw-rw-rw-   0 root         (0) root         (0)     1447 2022-12-05 21:33:14.000000 jdDiff-1.3/jdDiff/Settings.py
--rw-rw-rw-   0 root         (0) root         (0)     3311 2022-12-05 21:33:14.000000 jdDiff-1.3/jdDiff/SettingsDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3477 2022-12-05 21:33:14.000000 jdDiff-1.3/jdDiff/SettingsDialog.ui
--rw-rw-rw-   0 root         (0) root         (0)      974 2022-12-05 21:33:14.000000 jdDiff-1.3/jdDiff/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        4 2022-12-05 21:33:14.000000 jdDiff-1.3/jdDiff/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 21:33:33.942152 jdDiff-1.3/jdDiff.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1599 2022-12-05 21:33:33.000000 jdDiff-1.3/jdDiff.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      555 2022-12-05 21:33:33.000000 jdDiff-1.3/jdDiff.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-05 21:33:33.000000 jdDiff-1.3/jdDiff.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2022-12-05 21:33:33.000000 jdDiff-1.3/jdDiff.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-12-05 21:33:33.000000 jdDiff-1.3/jdDiff.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-12-05 21:33:33.000000 jdDiff-1.3/jdDiff.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1637 2022-12-05 21:33:14.000000 jdDiff-1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-05 21:33:33.943069 jdDiff-1.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3084 2022-12-05 21:33:14.000000 jdDiff-1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:37:41.307906 jdDiff-1.4/
+-rw-r--r--   0 root         (0) root         (0)     2846 2023-05-08 08:36:09.000000 jdDiff-1.4/BuildBackend.py
+-rw-r--r--   0 root         (0) root         (0)    35064 2023-05-08 08:36:09.000000 jdDiff-1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-08 08:36:09.000000 jdDiff-1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4871 2023-05-08 08:37:41.307906 jdDiff-1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3372 2023-05-08 08:36:09.000000 jdDiff-1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:37:41.307906 jdDiff-1.4/jdDiff/
+-rw-r--r--   0 root         (0) root         (0)      562 2023-05-08 08:36:09.000000 jdDiff-1.4/jdDiff/AboutDialog.py
+-rw-r--r--   0 root         (0) root         (0)     5570 2023-05-08 08:36:09.000000 jdDiff-1.4/jdDiff/BrowseDialog.py
+-rw-r--r--   0 root         (0) root         (0)     5186 2023-05-08 08:36:09.000000 jdDiff-1.4/jdDiff/CompareThread.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2023-05-08 08:36:09.000000 jdDiff-1.4/jdDiff/Enviroment.py
+-rw-r--r--   0 root         (0) root         (0)     2518 2023-05-08 08:36:09.000000 jdDiff-1.4/jdDiff/Functions.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2023-05-08 08:36:09.000000 jdDiff-1.4/jdDiff/Icon.svg
+-rw-r--r--   0 root         (0) root         (0)     4065 2023-05-08 08:36:09.000000 jdDiff-1.4/jdDiff/MainWindow.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2023-05-08 08:36:09.000000 jdDiff-1.4/jdDiff/Settings.py
+-rw-r--r--   0 root         (0) root         (0)     3307 2023-05-08 08:36:09.000000 jdDiff-1.4/jdDiff/SettingsDialog.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-05-08 08:36:09.000000 jdDiff-1.4/jdDiff/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:37:41.307906 jdDiff-1.4/jdDiff/translations/
+-rw-r--r--   0 root         (0) root         (0)    12989 2023-05-08 08:36:09.000000 jdDiff-1.4/jdDiff/translations/jdDiff_de.ts
+-rw-r--r--   0 root         (0) root         (0)    12493 2023-05-08 08:36:09.000000 jdDiff-1.4/jdDiff/translations/jdDiff_nl.ts
+-rw-r--r--   0 root         (0) root         (0)    12707 2023-05-08 08:36:09.000000 jdDiff-1.4/jdDiff/translations/jdDiff_sv.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:37:41.307906 jdDiff-1.4/jdDiff/ui/
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-05-08 08:36:09.000000 jdDiff-1.4/jdDiff/ui/AboutDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     2913 2023-05-08 08:36:09.000000 jdDiff-1.4/jdDiff/ui/BrowseDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     4799 2023-05-08 08:36:09.000000 jdDiff-1.4/jdDiff/ui/MainWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     3477 2023-05-08 08:36:09.000000 jdDiff-1.4/jdDiff/ui/SettingsDialog.ui
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-08 08:36:09.000000 jdDiff-1.4/jdDiff/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:37:41.307906 jdDiff-1.4/jdDiff.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4871 2023-05-08 08:37:41.000000 jdDiff-1.4/jdDiff.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      673 2023-05-08 08:37:41.000000 jdDiff-1.4/jdDiff.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 08:37:41.000000 jdDiff-1.4/jdDiff.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-08 08:37:41.000000 jdDiff-1.4/jdDiff.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-08 08:37:41.000000 jdDiff-1.4/jdDiff.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-08 08:37:41.000000 jdDiff-1.4/jdDiff.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-05-08 08:36:09.000000 jdDiff-1.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 08:37:41.307906 jdDiff-1.4/setup.cfg
```

### Comparing `jdDiff-1.3/LICENSE` & `jdDiff-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jdDiff-1.3/jdDiff/AboutDialog.ui` & `jdDiff-1.4/jdDiff/ui/AboutDialog.ui`

 * *Files 0% similar despite different names*

#### Comparing `jdDiff-1.3/jdDiff/AboutDialog.ui` & `jdDiff-1.4/jdDiff/ui/AboutDialog.ui`

```diff
@@ -65,15 +65,15 @@
             <set>Qt::AlignCenter</set>
           </property>
         </widget>
       </item>
       <item>
         <widget class="QLabel" name="label_3">
           <property name="text">
-            <string notr="true">Copyright © 2022 JakobDev</string>
+            <string notr="true">Copyright © 2022-2023 JakobDev</string>
           </property>
           <property name="alignment">
             <set>Qt::AlignCenter</set>
           </property>
         </widget>
       </item>
       <item>
```

### Comparing `jdDiff-1.3/jdDiff/BrowseDialog.py` & `jdDiff-1.4/jdDiff/BrowseDialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from PyQt6.QtWidgets import QDialog, QFileDialog, QMessageBox
 from .Functions import read_json_file, remove_list_duplicates
+from .ui_compiled.BrowseDialog import Ui_BrowseDialog
 from PyQt6.QtCore import QCoreApplication
 from typing import Optional
-from PyQt6 import uic
 import json
 import os
 
 
-class BrowseDialog(QDialog):
+class BrowseDialog(QDialog, Ui_BrowseDialog):
     def __init__(self, env):
         super().__init__()
-        uic.loadUi(os.path.join(os.path.dirname(__file__), "BrowseDialog.ui"), self)
+
+        self.setupUi(self)
 
         self._env = env
 
         self.button_browse_original.clicked.connect(self._browse_original_clicked)
         self.button_browse_copy.clicked.connect(self._browse_copy_clicked)
 
         self.button_ok.clicked.connect(self._ok_clicked)
```

### Comparing `jdDiff-1.3/jdDiff/BrowseDialog.ui` & `jdDiff-1.4/jdDiff/ui/BrowseDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDiff-1.3/jdDiff/CompareThread.py` & `jdDiff-1.4/jdDiff/CompareThread.py`

 * *Files identical despite different names*

### Comparing `jdDiff-1.3/jdDiff/Enviroment.py` & `jdDiff-1.4/jdDiff/Enviroment.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,17 +16,17 @@
         self.icon = QIcon(os.path.join(self.program_dir, "Icon.svg"))
 
         self.settings = Settings()
         self.settings.load(os.path.join(self.data_dir, "settings.json"))
 
     def _get_data_path(self) -> str:
         if platform.system() == "Windows":
-            return os.path.join(os.getenv("appdata"), "jdDiff")
+            return os.path.join(os.getenv("appdata"), "JakobDev", "jdDiff")
         elif platform.system() == "Darwin":
-            return os.path.join(str(Path.home()), "Library", "Application Support", "jdDiff")
+            return os.path.join(str(Path.home()), "Library", "Application Support", "JakobDev", "jdDiff")
         elif platform.system() == "Haiku":
-            return os.path.join(str(Path.home()), "config", "settings", "jdDiff")
+            return os.path.join(str(Path.home()), "config", "settings", "JakobDev", "jdDiff")
         else:
             if os.getenv("XDG_DATA_HOME"):
-                return os.path.join(os.getenv("XDG_DATA_HOME"), "jdDiff")
+                return os.path.join(os.getenv("XDG_DATA_HOME"), "JakobDev", "jdDiff")
             else:
-                return os.path.join(str(Path.home()), ".local", "share", "jdDiff")
+                return os.path.join(str(Path.home()), ".local", "share", "JakobDev", "jdDiff")
```

### Comparing `jdDiff-1.3/jdDiff/Functions.py` & `jdDiff-1.4/jdDiff/Functions.py`

 * *Files identical despite different names*

### Comparing `jdDiff-1.3/jdDiff/Icon.svg` & `jdDiff-1.4/jdDiff/Icon.svg`

 * *Files identical despite different names*

### Comparing `jdDiff-1.3/jdDiff/MainWindow.py` & `jdDiff-1.4/jdDiff/MainWindow.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from PyQt6.QtWidgets import QMainWindow, QApplication, QMessageBox, QFileDialog
+from .ui_compiled.MainWindow import Ui_MainWindow
+from .SettingsDialog import SettingsDialog
 from PyQt6.QtCore import QCoreApplication
 from .CompareThread import CompareThread
 from .BrowseDialog import BrowseDialog
-from .SettingsDialog import SettingsDialog
 from .AboutDialog import AboutDialog
-from PyQt6 import uic
 import subprocess
 import shutil
 import sys
-import os
 
 
-class MainWindow(QMainWindow):
+class MainWindow(QMainWindow, Ui_MainWindow):
     def __init__(self, env):
         super().__init__()
-        uic.loadUi(os.path.join(os.path.dirname(__file__), "MainWindow.ui"), self)
+
+        self.setupUi(self)
 
         self._browse_dialog = BrowseDialog(env)
         self._settings_dialog = SettingsDialog(env)
         self._about_dialog = AboutDialog(env)
 
         self._compare_thread = CompareThread(env)
         self._compare_thread.finished.connect(self._compare_finished)
```

### Comparing `jdDiff-1.3/jdDiff/MainWindow.ui` & `jdDiff-1.4/jdDiff/ui/MainWindow.ui`

 * *Files identical despite different names*

### Comparing `jdDiff-1.3/jdDiff/Settings.py` & `jdDiff-1.4/jdDiff/Settings.py`

 * *Files identical despite different names*

### Comparing `jdDiff-1.3/jdDiff/SettingsDialog.py` & `jdDiff-1.4/jdDiff/SettingsDialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+from .ui_compiled.SettingsDialog import Ui_SettingsDialog
 from PyQt6.QtCore import QCoreApplication, QLocale
 from PyQt6.QtWidgets import QDialog, QColorDialog
 from .Functions import select_combo_box_data
 from .Settings import Settings
-from PyQt6 import uic
 import os
 
 
-class SettingsDialog(QDialog):
+class SettingsDialog(QDialog, Ui_SettingsDialog):
     def __init__(self, env):
         super().__init__()
-        uic.loadUi(os.path.join(os.path.dirname(__file__), "SettingsDialog.ui"), self)
+
+        self.setupUi(self)
 
         self._env = env
 
         self.box_language.addItem(QCoreApplication.translate("SettingsDialog", "System language"), "default")
         self.box_language.addItem("English", "en")
         for i in os.listdir(os.path.join(env.program_dir, "translations")):
             if i.endswith(".qm"):
```

### Comparing `jdDiff-1.3/jdDiff/SettingsDialog.ui` & `jdDiff-1.4/jdDiff/ui/SettingsDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDiff-1.3/jdDiff/__init__.py` & `jdDiff-1.4/jdDiff/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,18 +3,22 @@
 from .MainWindow import MainWindow
 from .Enviroment import Enviroment
 import sys
 import os
 
 
 def main():
+    if not os.path.isdir(os.path.join(os.path.dirname(__file__), "ui_compiled")):
+        print("Could not find compiled ui files. Please run tools/CompileUI.py first.", file=sys.stderr)
+        sys.exit(1)
+
     app = QApplication(sys.argv)
     env = Enviroment()
 
-    app.setDesktopFileName("com.gitlab.JakobDev.jdDiff")
+    app.setDesktopFileName("page.codeberg.JakobDev.jdDiff")
     app.setApplicationName("jdDiff")
     app.setWindowIcon(env.icon)
 
     translator = QTranslator()
     language = env.settings.get("language")
     if language == "default":
         system_language = QLocale.system().name()
```

### Comparing `jdDiff-1.3/pyproject.toml` & `jdDiff-1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools", "PyQt6"]
 build-backend = "BuildBackend"
 backend-path = ["."]
 
 [project]
 name = "jdDiff"
 description = "A graphical cross platform diff viewer"
 readme = "README.md"
@@ -40,16 +40,17 @@
 ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = { file = "jdDiff/version.txt" }
 
 [project.urls]
+Translate = "https://translate.codeberg.org/projects/jdDiff"
 Issues = "https://gitlab.com/JakobDev/jdDiff/-/issues"
 Source = "https://gitlab.com/JakobDev/jdDiff"
 Donation = "https://ko-fi.com/jakobdev"
 
-[tool.setuptools.packages.find]
-include = ["jdDiff*"]
+[tool.setuptools.package-dir]
+jdDiff = "jdDiff"
 
-[project.scripts]
+[project.gui-scripts]
 jddiff = "jdDiff:main"
```

