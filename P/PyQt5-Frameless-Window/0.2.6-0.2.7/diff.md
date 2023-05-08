# Comparing `tmp/PyQt5-Frameless-Window-0.2.6.tar.gz` & `tmp/PyQt5-Frameless-Window-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt5-Frameless-Window-0.2.6.tar", last modified: Sat Apr 29 15:58:52 2023, max compression
+gzip compressed data, was "dist\PyQt5-Frameless-Window-0.2.7.tar", last modified: Mon May  8 13:19:02 2023, max compression
```

## Comparing `PyQt5-Frameless-Window-0.2.6.tar` & `PyQt5-Frameless-Window-0.2.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 15:58:52.260164 PyQt5-Frameless-Window-0.2.6/
--rw-rw-rw-   0        0        0    35823 2023-04-27 01:27:43.000000 PyQt5-Frameless-Window-0.2.6/LICENSE
--rw-rw-rw-   0        0        0     5051 2023-04-29 15:58:52.259155 PyQt5-Frameless-Window-0.2.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-29 15:58:52.222398 PyQt5-Frameless-Window-0.2.6/PyQt5_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5051 2023-04-29 15:58:51.000000 PyQt5-Frameless-Window-0.2.6/PyQt5_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      848 2023-04-29 15:58:52.000000 PyQt5-Frameless-Window-0.2.6/PyQt5_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 15:58:51.000000 PyQt5-Frameless-Window-0.2.6/PyQt5_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      126 2023-04-29 15:58:51.000000 PyQt5-Frameless-Window-0.2.6/PyQt5_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-29 15:58:51.000000 PyQt5-Frameless-Window-0.2.6/PyQt5_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4481 2023-04-27 01:27:43.000000 PyQt5-Frameless-Window-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 15:58:52.224504 PyQt5-Frameless-Window-0.2.6/qframelesswindow/
--rw-rw-rw-   0        0        0     1616 2023-04-29 15:58:33.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:58:52.228510 PyQt5-Frameless-Window-0.2.6/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:58:52.232684 PyQt5-Frameless-Window-0.2.6/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     2891 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     2683 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:58:52.237120 PyQt5-Frameless-Window-0.2.6/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     2994 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     3898 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:58:52.241467 PyQt5-Frameless-Window-0.2.6/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     4984 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9057 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:58:52.250211 PyQt5-Frameless-Window-0.2.6/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0     5299 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1850 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     8190 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:58:52.256726 PyQt5-Frameless-Window-0.2.6/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     6975 2023-04-29 15:57:34.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4013 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     8344 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-04-29 15:58:52.261214 PyQt5-Frameless-Window-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1023 2023-04-29 15:58:28.000000 PyQt5-Frameless-Window-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:19:01.995115 PyQt5-Frameless-Window-0.2.7/
+-rw-rw-rw-   0        0        0    35823 2023-04-29 16:05:01.000000 PyQt5-Frameless-Window-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0     5051 2023-05-08 13:19:01.995115 PyQt5-Frameless-Window-0.2.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-08 13:19:01.967979 PyQt5-Frameless-Window-0.2.7/PyQt5_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5051 2023-05-08 13:19:01.000000 PyQt5-Frameless-Window-0.2.7/PyQt5_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2023-05-08 13:19:01.000000 PyQt5-Frameless-Window-0.2.7/PyQt5_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 13:19:01.000000 PyQt5-Frameless-Window-0.2.7/PyQt5_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      126 2023-05-08 13:19:01.000000 PyQt5-Frameless-Window-0.2.7/PyQt5_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-08 13:19:01.000000 PyQt5-Frameless-Window-0.2.7/PyQt5_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4481 2023-04-29 16:05:01.000000 PyQt5-Frameless-Window-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 13:19:01.969498 PyQt5-Frameless-Window-0.2.7/qframelesswindow/
+-rw-rw-rw-   0        0        0     1616 2023-05-08 13:15:17.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:19:01.972501 PyQt5-Frameless-Window-0.2.7/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-04-29 16:05:01.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:19:01.976015 PyQt5-Frameless-Window-0.2.7/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     2891 2023-04-29 16:05:01.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     2904 2023-05-08 13:12:25.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:19:01.978256 PyQt5-Frameless-Window-0.2.7/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     2994 2023-04-29 16:05:01.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     4119 2023-05-08 13:12:11.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:19:01.982278 PyQt5-Frameless-Window-0.2.7/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     4984 2023-04-29 16:05:01.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9057 2023-04-29 16:05:01.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:19:01.988191 PyQt5-Frameless-Window-0.2.7/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0     5299 2023-04-29 16:05:01.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1850 2023-04-29 16:05:01.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     8352 2023-05-08 13:03:27.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:19:01.993600 PyQt5-Frameless-Window-0.2.7/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     6942 2023-05-08 13:08:28.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4263 2023-05-08 13:07:12.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     8523 2023-05-08 13:12:49.000000 PyQt5-Frameless-Window-0.2.7/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-05-08 13:19:01.996213 PyQt5-Frameless-Window-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-05-08 13:15:11.000000 PyQt5-Frameless-Window-0.2.7/setup.py
```

### Comparing `PyQt5-Frameless-Window-0.2.6/LICENSE` & `PyQt5-Frameless-Window-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.6/PKG-INFO` & `PyQt5-Frameless-Window-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt5-Frameless-Window
-Version: 0.2.6
+Version: 0.2.7
 Summary: A cross-platform frameless window based on pyqt5, support Win32, X11, Wayland and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt frameless
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyQt5-Frameless-Window-0.2.6/PyQt5_Frameless_Window.egg-info/PKG-INFO` & `PyQt5-Frameless-Window-0.2.7/PyQt5_Frameless_Window.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt5-Frameless-Window
-Version: 0.2.6
+Version: 0.2.7
 Summary: A cross-platform frameless window based on pyqt5, support Win32, X11, Wayland and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt frameless
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyQt5-Frameless-Window-0.2.6/PyQt5_Frameless_Window.egg-info/SOURCES.txt` & `PyQt5-Frameless-Window-0.2.7/PyQt5_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.6/README.md` & `PyQt5-Frameless-Window-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.6/qframelesswindow/__init__.py` & `PyQt5-Frameless-Window-0.2.7/qframelesswindow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/master/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: GPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 
 import sys
 
 from PyQt5.QtWidgets import QDialog, QMainWindow
 
 from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar
```

### Comparing `PyQt5-Frameless-Window-0.2.6/qframelesswindow/_rc/resource.py` & `PyQt5-Frameless-Window-0.2.7/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.6/qframelesswindow/linux/__init__.py` & `PyQt5-Frameless-Window-0.2.7/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.6/qframelesswindow/linux/window_effect.py` & `PyQt5-Frameless-Window-0.2.7/qframelesswindow/linux/window_effect.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,7 +112,15 @@
 
         Parameters
         ----------
         hWnd : int or `sip.voidptr`
             Window handle
         """
         pass
+
+    def enableBlurBehindWindow(self, hWnd):
+        """ enable the blur effect behind the whole client
+        Parameters
+        ----------
+        hWnd: int or `sip.voidptr`
+            Window handle
+        """
```

### Comparing `PyQt5-Frameless-Window-0.2.6/qframelesswindow/mac/__init__.py` & `PyQt5-Frameless-Window-0.2.7/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.6/qframelesswindow/mac/window_effect.py` & `PyQt5-Frameless-Window-0.2.7/qframelesswindow/mac/window_effect.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,7 +133,15 @@
 
         Parameters
         ----------
         hWnd : int or `sip.voidptr`
             Window handle
         """
         pass
+
+    def enableBlurBehindWindow(self, hWnd):
+        """ enable the blur effect behind the whole client
+        Parameters
+        ----------
+        hWnd: int or `sip.voidptr`
+            Window handle
+        """
```

### Comparing `PyQt5-Frameless-Window-0.2.6/qframelesswindow/titlebar/__init__.py` & `PyQt5-Frameless-Window-0.2.7/qframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.6/qframelesswindow/titlebar/title_bar_buttons.py` & `PyQt5-Frameless-Window-0.2.7/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.6/qframelesswindow/utils/__init__.py` & `PyQt5-Frameless-Window-0.2.7/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.6/qframelesswindow/utils/linux_utils.py` & `PyQt5-Frameless-Window-0.2.7/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.6/qframelesswindow/utils/mac_utils.py` & `PyQt5-Frameless-Window-0.2.7/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.6/qframelesswindow/utils/win32_utils.py` & `PyQt5-Frameless-Window-0.2.7/qframelesswindow/utils/win32_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # coding:utf-8
-from ctypes import Structure, byref, sizeof, windll
+from ctypes import Structure, byref, sizeof, windll, c_int
 from ctypes.wintypes import DWORD, HWND, LPARAM, RECT, UINT
 from platform import platform
 import sys
 
 import win32api
 import win32con
 import win32gui
 import win32print
 from PyQt5.QtCore import QOperatingSystemVersion
 from PyQt5.QtGui import QGuiApplication
-from PyQt5.QtWinExtras import QtWin
 from win32comext.shell import shellcon
 
 
 def isMaximized(hWnd):
     """ Determine whether the window is maximized
 
     Parameters
@@ -49,14 +48,21 @@
     if not monitorInfo:
         return False
 
     monitorRect = monitorInfo["Monitor"]
     return all(i == j for i, j in zip(winRect, monitorRect))
 
 
+def isCompositionEnabled():
+    """ detect if dwm composition is enabled """
+    bResult = c_int(0)
+    windll.dwmapi.DwmIsCompositionEnabled(byref(bResult))
+    return bool(bResult.value)
+
+
 def getMonitorInfo(hWnd, dwFlags):
     """ get monitor info, return `None` if failed
 
     Parameters
     ----------
     hWnd: int or `sip.voidptr`
         window handle
@@ -88,15 +94,15 @@
 
     frame = win32con.SM_CXSIZEFRAME if horizontal else win32con.SM_CYSIZEFRAME
     result = getSystemMetrics(hWnd, frame, horizontal) + getSystemMetrics(hWnd, 92, horizontal)
 
     if result > 0:
         return result
 
-    thickness = 8 if QtWin.isCompositionEnabled() else 4
+    thickness = 8 if isCompositionEnabled() else 4
     return round(thickness*window.devicePixelRatio())
 
 
 def getSystemMetrics(hWnd, index, horizontal):
     """ get system metrics """
     if not hasattr(windll.user32, 'GetSystemMetricsForDpi'):
         return win32api.GetSystemMetrics(index)
```

### Comparing `PyQt5-Frameless-Window-0.2.6/qframelesswindow/windows/__init__.py` & `PyQt5-Frameless-Window-0.2.7/qframelesswindow/windows/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 import win32api
 import win32con
 import win32gui
 from PyQt5.QtCore import Qt
 from PyQt5.QtGui import QCloseEvent, QCursor
 from PyQt5.QtWidgets import QApplication, QWidget
-from PyQt5.QtWinExtras import QtWin
 
 from ..titlebar import TitleBar
 from ..utils import win32_utils as win_utils
 from ..utils.win32_utils import Taskbar
 from .c_structures import LPNCCALCSIZE_PARAMS
 from .window_effect import WindowsWindowEffect
 
@@ -145,21 +144,21 @@
 class AcrylicWindow(WindowsFramelessWindow):
     """ A frameless window with acrylic effect """
 
     def __init__(self, parent=None):
         super().__init__(parent=parent)
         self.__closedByKey = False
 
-        QtWin.enableBlurBehindWindow(self)
-        
+        self.windowEffect.enableBlurBehindWindow(self.winId())
+
         if win_utils.isWin7() and parent:
             self.setWindowFlags(parent.windowFlags() | Qt.FramelessWindowHint | Qt.WindowMinMaxButtonsHint)
         else:
             self.setWindowFlags(Qt.FramelessWindowHint | Qt.WindowMinMaxButtonsHint)
-        
+
         self.windowEffect.addWindowAnimation(self.winId())
 
         if win_utils.isWin7():
             self.windowEffect.addShadowEffect(self.winId())
             self.windowEffect.setAeroEffect(self.winId())
         else:
             self.windowEffect.setAcrylicEffect(self.winId())
```

### Comparing `PyQt5-Frameless-Window-0.2.6/qframelesswindow/windows/c_structures.py` & `PyQt5-Frameless-Window-0.2.7/qframelesswindow/windows/c_structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding:utf-8
 from ctypes import POINTER, Structure, c_int
-from ctypes.wintypes import DWORD, HWND, ULONG, POINT, RECT, UINT
+from ctypes.wintypes import DWORD, HWND, ULONG, POINT, RECT, UINT, BOOL, HRGN
 from enum import Enum
 
 
 class WINDOWCOMPOSITIONATTRIB(Enum):
     WCA_UNDEFINED = 0
     WCA_NCRENDERING_ENABLED = 1
     WCA_NCRENDERING_POLICY = 2
@@ -137,8 +137,17 @@
 class NCCALCSIZE_PARAMS(Structure):
     _fields_ = [
         ('rgrc', RECT*3),
         ('lppos', POINTER(PWINDOWPOS))
     ]
 
 
-LPNCCALCSIZE_PARAMS = POINTER(NCCALCSIZE_PARAMS)
+LPNCCALCSIZE_PARAMS = POINTER(NCCALCSIZE_PARAMS)
+
+
+class DWM_BLURBEHIND(Structure):
+    _fields_ = [
+        ('dwFlags',                DWORD),
+        ('fEnable',                BOOL),
+        ('hRgnBlur',               HRGN),
+        ('fTransitionOnMaximized', BOOL),
+    ]
```

### Comparing `PyQt5-Frameless-Window-0.2.6/qframelesswindow/windows/window_effect.py` & `PyQt5-Frameless-Window-0.2.7/qframelesswindow/windows/window_effect.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,44 +3,48 @@
 import warnings
 from ctypes import POINTER, byref, c_bool, c_int, pointer, sizeof, WinDLL
 from ctypes.wintypes import DWORD, LONG, LPCVOID
 
 import win32api
 import win32con
 import win32gui
-from PyQt5.QtWinExtras import QtWin
 
 from .c_structures import (ACCENT_POLICY, ACCENT_STATE, DWMNCRENDERINGPOLICY,
                            DWMWINDOWATTRIBUTE, MARGINS,
                            WINDOWCOMPOSITIONATTRIB,
-                           WINDOWCOMPOSITIONATTRIBDATA)
-from ..utils.win32_utils import isGreaterEqualWin10, isGreaterEqualWin11
+                           WINDOWCOMPOSITIONATTRIBDATA, DWM_BLURBEHIND)
+from ..utils.win32_utils import isGreaterEqualWin10, isGreaterEqualWin11, isCompositionEnabled
 
 
 class WindowsWindowEffect:
     """ Windows window effect """
 
     def __init__(self, window):
         self.window = window
 
         # Declare the function signature of the API
         self.user32 = WinDLL("user32")
         self.dwmapi = WinDLL("dwmapi")
         self.SetWindowCompositionAttribute = self.user32.SetWindowCompositionAttribute
         self.DwmExtendFrameIntoClientArea = self.dwmapi.DwmExtendFrameIntoClientArea
+        self.DwmEnableBlurBehindWindow = self.dwmapi.DwmEnableBlurBehindWindow
         self.DwmSetWindowAttribute = self.dwmapi.DwmSetWindowAttribute
+
         self.SetWindowCompositionAttribute.restype = c_bool
         self.DwmExtendFrameIntoClientArea.restype = LONG
+        self.DwmEnableBlurBehindWindow.restype = LONG
         self.DwmSetWindowAttribute.restype = LONG
+
         self.SetWindowCompositionAttribute.argtypes = [
             c_int,
             POINTER(WINDOWCOMPOSITIONATTRIBDATA),
         ]
         self.DwmSetWindowAttribute.argtypes = [c_int, DWORD, LPCVOID, DWORD]
         self.DwmExtendFrameIntoClientArea.argtypes = [c_int, POINTER(MARGINS)]
+        self.DwmEnableBlurBehindWindow.argtypes = [c_int, POINTER(DWM_BLURBEHIND)]
 
         # Initialize structure
         self.accentPolicy = ACCENT_POLICY()
         self.winCompAttrData = WINDOWCOMPOSITIONATTRIBDATA()
         self.winCompAttrData.Attribute = WINDOWCOMPOSITIONATTRIB.WCA_ACCENT_POLICY.value
         self.winCompAttrData.SizeOfData = sizeof(self.accentPolicy)
         self.winCompAttrData.Data = pointer(self.accentPolicy)
@@ -131,53 +135,38 @@
         hWnd: int or `sip.voidptr`
             Window handle
         """
         hWnd = int(hWnd)
         self.accentPolicy.AccentState = ACCENT_STATE.ACCENT_DISABLED.value
         self.SetWindowCompositionAttribute(hWnd, pointer(self.winCompAttrData))
 
-    @staticmethod
-    def moveWindow(hWnd):
-        """ Move the window
-
-        Parameters
-        ----------
-        hWnd: int or `sip.voidptr`
-            Window handle
-        """
-        hWnd = int(hWnd)
-        win32gui.ReleaseCapture()
-        win32api.SendMessage(
-            hWnd, win32con.WM_SYSCOMMAND, win32con.SC_MOVE + win32con.HTCAPTION, 0
-        )
-
     def addShadowEffect(self, hWnd):
         """ Add DWM shadow to window
 
         Parameters
         ----------
         hWnd: int or `sip.voidptr`
             Window handle
         """
-        if not QtWin.isCompositionEnabled():
+        if not isCompositionEnabled():
             return
 
         hWnd = int(hWnd)
         margins = MARGINS(-1, -1, -1, -1)
         self.DwmExtendFrameIntoClientArea(hWnd, byref(margins))
 
     def addMenuShadowEffect(self, hWnd):
         """ Add DWM shadow to menu
 
         Parameters
         ----------
         hWnd: int or `sip.voidptr`
             Window handle
         """
-        if not QtWin.isCompositionEnabled():
+        if not isCompositionEnabled():
             return
 
         hWnd = int(hWnd)
         self.DwmSetWindowAttribute(
             hWnd,
             DWMWINDOWATTRIBUTE.DWMWA_NCRENDERING_POLICY.value,
             byref(c_int(DWMNCRENDERINGPOLICY.DWMNCRP_ENABLED.value)),
@@ -233,7 +222,17 @@
             style
             | win32con.WS_MINIMIZEBOX
             | win32con.WS_MAXIMIZEBOX
             | win32con.WS_CAPTION
             | win32con.CS_DBLCLKS
             | win32con.WS_THICKFRAME,
         )
+
+    def enableBlurBehindWindow(self, hWnd):
+        """ enable the blur effect behind the whole client
+        Parameters
+        ----------
+        hWnd: int or `sip.voidptr`
+            Window handle
+        """
+        blurBehind = DWM_BLURBEHIND(1, True, 0, False)
+        self.DwmEnableBlurBehindWindow(int(hWnd), byref(blurBehind))
```

### Comparing `PyQt5-Frameless-Window-0.2.6/setup.py` & `PyQt5-Frameless-Window-0.2.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt5-Frameless-Window",
-    version="0.2.6",
+    version="0.2.7",
     keywords="pyqt frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyqt5, support Win32, X11, Wayland and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

