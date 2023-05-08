# Comparing `tmp/xiaopy-0.0.19.tar.gz` & `tmp/xiaopy-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaopy-0.0.19.tar", last modified: Tue Mar 21 13:30:40 2023, max compression
+gzip compressed data, was "xiaopy-0.0.20.tar", last modified: Mon May  8 07:17:42 2023, max compression
```

## Comparing `xiaopy-0.0.19.tar` & `xiaopy-0.0.20.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 13:30:40.433556 xiaopy-0.0.19/
--rw-rw-rw-   0        0        0      262 2023-03-21 13:30:40.433556 xiaopy-0.0.19/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-21 13:30:40.422586 xiaopy-0.0.19/PyGameAutoAndroid/
--rw-rw-rw-   0        0        0     9678 2023-03-21 13:27:50.000000 xiaopy-0.0.19/PyGameAutoAndroid/PyGameAutoAndroid.py
--rw-rw-rw-   0        0        0      261 2023-02-15 16:25:44.000000 xiaopy-0.0.19/PyGameAutoAndroid/__init__.py
--rw-rw-rw-   0        0        0       42 2023-03-21 13:30:40.433556 xiaopy-0.0.19/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-21 13:30:40.425578 xiaopy-0.0.19/xiaopy/
--rw-rw-rw-   0        0        0      250 2023-02-15 16:25:49.000000 xiaopy-0.0.19/xiaopy/__init__.py
--rw-rw-rw-   0        0        0     9678 2023-03-21 13:27:44.000000 xiaopy-0.0.19/xiaopy/xiaopy.py
-drwxrwxrwx   0        0        0        0 2023-03-21 13:30:40.431561 xiaopy-0.0.19/xiaopy.egg-info/
--rw-rw-rw-   0        0        0      262 2023-03-21 13:30:40.000000 xiaopy-0.0.19/xiaopy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-03-21 13:30:40.000000 xiaopy-0.0.19/xiaopy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 13:30:40.000000 xiaopy-0.0.19/xiaopy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-03-21 13:30:40.000000 xiaopy-0.0.19/xiaopy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      631 2023-03-21 13:18:22.000000 xiaopy-0.0.19/xiaopy_setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:17:42.253083 xiaopy-0.0.20/
+-rw-rw-rw-   0        0        0      262 2023-05-08 07:17:42.253083 xiaopy-0.0.20/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-08 07:17:42.236128 xiaopy-0.0.20/PyGameAutoAndroid/
+-rw-rw-rw-   0        0        0    10028 2023-04-25 10:19:41.000000 xiaopy-0.0.20/PyGameAutoAndroid/PyGameAutoAndroid.py
+-rw-rw-rw-   0        0        0      261 2023-02-15 16:25:44.000000 xiaopy-0.0.20/PyGameAutoAndroid/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-08 07:17:42.254080 xiaopy-0.0.20/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 07:17:42.240117 xiaopy-0.0.20/xiaopy/
+-rw-rw-rw-   0        0        0      250 2023-02-15 16:25:49.000000 xiaopy-0.0.20/xiaopy/__init__.py
+-rw-rw-rw-   0        0        0    10028 2023-04-25 10:20:08.000000 xiaopy-0.0.20/xiaopy/xiaopy.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:17:42.250093 xiaopy-0.0.20/xiaopy.egg-info/
+-rw-rw-rw-   0        0        0      262 2023-05-08 07:17:42.000000 xiaopy-0.0.20/xiaopy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-05-08 07:17:42.000000 xiaopy-0.0.20/xiaopy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 07:17:42.000000 xiaopy-0.0.20/xiaopy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-08 07:17:42.000000 xiaopy-0.0.20/xiaopy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      631 2023-05-08 07:09:14.000000 xiaopy-0.0.20/xiaopy_setup.py
```

### Comparing `xiaopy-0.0.19/PyGameAutoAndroid/PyGameAutoAndroid.py` & `xiaopy-0.0.20/PyGameAutoAndroid/PyGameAutoAndroid.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,22 +18,24 @@
 
 class Rect:
     x = None
     y = None
     width = None
     height = None
 
+
 class TextRect:
     x = None
     y = None
     width = None
     height = None
     text = None
     confidence = None
 
+
 class Text:
     text = None
     confidence = None
 
 
 class Node:
     index = None
@@ -93,38 +95,40 @@
         pass
 
 
 class Size:
     width = None
     height = None
 
+
 class Selector:
     def join(self, selector):
         pass
 
 
 class IdSelector(Selector):
     def __init__(self, id: str):
         pass
 
 
-
 class TextSelector(Selector):
     def __init__(self, text: str):
         pass
 
 
 class DescSelector(Selector):
     def __init__(self, desc: str):
         pass
 
+
 class ClassSelector(Selector):
     def __init__(self, cls: str):
         pass
 
+
 class xp:
     @classmethod
     def tap(cls, x1: float, y1: float, duration: float = 0.05):
         """
         点击
         :param x1: x坐标
         :param y1: y坐标
@@ -160,14 +164,15 @@
         """
         pass
 
     @classmethod
     def matchColor(cls, colorDesc: str, x: int, y: int, sim: float):
         """
         匹配颜色
+        :param sim: 相似度
         :param colorDesc: 颜色描述
         :param x: x 坐标
         :param y: y 坐标
         :return:
         """
         return
 
@@ -179,15 +184,15 @@
         :param colorDesc2: 颜色描述
         :param sim: 相似度
         :return:
         """
         return
 
     @classmethod
-    def matchColorStrGroups(cls, *args):
+    def matchColorGroups(cls, *args):
         """
         多点比色
         :return:
         """
         return
 
     @classmethod
@@ -201,57 +206,57 @@
         :param x2: 终点 x 坐标
         :param y2: 终点 y 坐标
         :return:
         """
         return Point
 
     @classmethod
-    def findImage(cls, imgName: str, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0, sim: float = 0.9):
+    def findImage(cls, imgName: str, x1: object = 0, y1: object = 0, x2: object = 0, y2: object = 0, sim: float = 0.9):
         """
         找图
         :param imgName: 图片名称, 包含后缀
         :param x1: 起点 x 坐标
         :param y1: 起点 y 坐标
         :param x2: 终点 x 坐标
         :param y2: 终点 y 坐标
         :param sim: 相似度
         :return:
         """
         return Rect
 
     @classmethod
-    def findImageAll(cls, imgName: str, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0, sim: float = 0.9):
+    def findImageAll(cls, imgName: str, x1: object = 0, y1: object = 0, x2: object = 0, y2: object = 0, sim: float = 0.9):
         """
         找图
         :param imgName: 图片名称, 包含后缀
         :param x1: 起点 x 坐标
         :param y1: 起点 y 坐标
         :param x2: 终点 x 坐标
         :param y2: 终点 y 坐标
         :param sim: 相似度
         :return:
         """
         return [Rect]
 
     @classmethod
-    def findText(cls, text: str, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0, sim: float = 0.9):
+    def findText(cls, text: str, x1: object = 0, y1: object = 0, x2: object = 0, y2: object = 0, sim: float = 0.9):
         """
         文字查找
         :param text: 文本内容
         :param x1: 起点 x 坐标
         :param y1: 起点 y 坐标
         :param x2: 终点 x 坐标
         :param y2: 终点 y 坐标
         :param sim: 相似度
         :return:
         """
         return TextRect
 
     @classmethod
-    def findTextAll(cls, text: str, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0, sim: float = 0.9):
+    def findTextAll(cls, text: str, x1: object = 0, y1: object = 0, x2: object = 0, y2: object = 0, sim: float = 0.9):
         """
         查找范围内所有文字
         :param text:
         :param x1:
         :param y1:
         :param x2:
         :param y2:
@@ -281,22 +286,30 @@
         :param x2:
         :param y2:
         :return:
         """
         return [TextRect]
 
     @classmethod
-    def getTextAll(cls, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0, padding: int = 0, boxScoreThresh: float = 0.2, boxThresh: float = 0.3, unClipRatio: float = 2.0,
+    def getTextAll(cls, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0, padding: int = 0,
+                   boxScoreThresh: float = 0.2, boxThresh: float = 0.3, unClipRatio: float = 2.0,
                    doAngle: bool = False, mostAngle: bool = False, isShotscreen: bool = False):
         """
         识别获取范围内所有文字
         :param x1:
         :param y1:
         :param x2:
         :param y2:
+        :param padding:
+        :param boxScoreThresh:
+        :param boxThresh:
+        :param unClipRatio:
+        :param doAngle:
+        :param mostAngle:
+        :param isShotscreen:
         :return:
         """
         return [TextRect]
 
     @classmethod
     def findNode(cls, selector):
         """
@@ -373,17 +386,18 @@
         """
         手机返回键
         :return:
         """
         pass
 
     @classmethod
-    def launchApp(cls, packageName: str):
+    def launchApp(cls, packageName: str, activityName: str):
         """
         包名运行APP
+        :param activityName:
         :param packageName:
         :return:
         """
         pass
 
     @classmethod
     def closeApp(cls, packageName: str):
@@ -407,15 +421,15 @@
         """
         获取屏幕分辨率
         :return:
         """
         return Size
 
     @classmethod
-    def screenshot(cls, fileName: str=None, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0):
+    def screenshot(cls, fileName: str = None, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0):
         """
         截图
         :param fileName: 文件名
         :return:
         """
         pass
```

### Comparing `xiaopy-0.0.19/xiaopy/xiaopy.py` & `xiaopy-0.0.20/xiaopy/xiaopy.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,22 +18,24 @@
 
 class Rect:
     x = None
     y = None
     width = None
     height = None
 
+
 class TextRect:
     x = None
     y = None
     width = None
     height = None
     text = None
     confidence = None
 
+
 class Text:
     text = None
     confidence = None
 
 
 class Node:
     index = None
@@ -93,38 +95,40 @@
         pass
 
 
 class Size:
     width = None
     height = None
 
+
 class Selector:
     def join(self, selector):
         pass
 
 
 class IdSelector(Selector):
     def __init__(self, id: str):
         pass
 
 
-
 class TextSelector(Selector):
     def __init__(self, text: str):
         pass
 
 
 class DescSelector(Selector):
     def __init__(self, desc: str):
         pass
 
+
 class ClassSelector(Selector):
     def __init__(self, cls: str):
         pass
 
+
 class xp:
     @classmethod
     def tap(cls, x1: float, y1: float, duration: float = 0.05):
         """
         点击
         :param x1: x坐标
         :param y1: y坐标
@@ -160,14 +164,15 @@
         """
         pass
 
     @classmethod
     def matchColor(cls, colorDesc: str, x: int, y: int, sim: float):
         """
         匹配颜色
+        :param sim: 相似度
         :param colorDesc: 颜色描述
         :param x: x 坐标
         :param y: y 坐标
         :return:
         """
         return
 
@@ -179,15 +184,15 @@
         :param colorDesc2: 颜色描述
         :param sim: 相似度
         :return:
         """
         return
 
     @classmethod
-    def matchColorStrGroups(cls, *args):
+    def matchColorGroups(cls, *args):
         """
         多点比色
         :return:
         """
         return
 
     @classmethod
@@ -201,57 +206,57 @@
         :param x2: 终点 x 坐标
         :param y2: 终点 y 坐标
         :return:
         """
         return Point
 
     @classmethod
-    def findImage(cls, imgName: str, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0, sim: float = 0.9):
+    def findImage(cls, imgName: str, x1: object = 0, y1: object = 0, x2: object = 0, y2: object = 0, sim: float = 0.9):
         """
         找图
         :param imgName: 图片名称, 包含后缀
         :param x1: 起点 x 坐标
         :param y1: 起点 y 坐标
         :param x2: 终点 x 坐标
         :param y2: 终点 y 坐标
         :param sim: 相似度
         :return:
         """
         return Rect
 
     @classmethod
-    def findImageAll(cls, imgName: str, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0, sim: float = 0.9):
+    def findImageAll(cls, imgName: str, x1: object = 0, y1: object = 0, x2: object = 0, y2: object = 0, sim: float = 0.9):
         """
         找图
         :param imgName: 图片名称, 包含后缀
         :param x1: 起点 x 坐标
         :param y1: 起点 y 坐标
         :param x2: 终点 x 坐标
         :param y2: 终点 y 坐标
         :param sim: 相似度
         :return:
         """
         return [Rect]
 
     @classmethod
-    def findText(cls, text: str, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0, sim: float = 0.9):
+    def findText(cls, text: str, x1: object = 0, y1: object = 0, x2: object = 0, y2: object = 0, sim: float = 0.9):
         """
         文字查找
         :param text: 文本内容
         :param x1: 起点 x 坐标
         :param y1: 起点 y 坐标
         :param x2: 终点 x 坐标
         :param y2: 终点 y 坐标
         :param sim: 相似度
         :return:
         """
         return TextRect
 
     @classmethod
-    def findTextAll(cls, text: str, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0, sim: float = 0.9):
+    def findTextAll(cls, text: str, x1: object = 0, y1: object = 0, x2: object = 0, y2: object = 0, sim: float = 0.9):
         """
         查找范围内所有文字
         :param text:
         :param x1:
         :param y1:
         :param x2:
         :param y2:
@@ -281,22 +286,30 @@
         :param x2:
         :param y2:
         :return:
         """
         return [TextRect]
 
     @classmethod
-    def getTextAll(cls, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0, padding: int = 0, boxScoreThresh: float = 0.2, boxThresh: float = 0.3, unClipRatio: float = 2.0,
+    def getTextAll(cls, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0, padding: int = 0,
+                   boxScoreThresh: float = 0.2, boxThresh: float = 0.3, unClipRatio: float = 2.0,
                    doAngle: bool = False, mostAngle: bool = False, isShotscreen: bool = False):
         """
         识别获取范围内所有文字
         :param x1:
         :param y1:
         :param x2:
         :param y2:
+        :param padding:
+        :param boxScoreThresh:
+        :param boxThresh:
+        :param unClipRatio:
+        :param doAngle:
+        :param mostAngle:
+        :param isShotscreen:
         :return:
         """
         return [TextRect]
 
     @classmethod
     def findNode(cls, selector):
         """
@@ -373,17 +386,18 @@
         """
         手机返回键
         :return:
         """
         pass
 
     @classmethod
-    def launchApp(cls, packageName: str):
+    def launchApp(cls, packageName: str, activityName: str):
         """
         包名运行APP
+        :param activityName:
         :param packageName:
         :return:
         """
         pass
 
     @classmethod
     def closeApp(cls, packageName: str):
@@ -407,15 +421,15 @@
         """
         获取屏幕分辨率
         :return:
         """
         return Size
 
     @classmethod
-    def screenshot(cls, fileName: str=None, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0):
+    def screenshot(cls, fileName: str = None, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0):
         """
         截图
         :param fileName: 文件名
         :return:
         """
         pass
```

### Comparing `xiaopy-0.0.19/xiaopy_setup.py` & `xiaopy-0.0.20/xiaopy_setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Description：
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name='xiaopy',
-    version='0.0.19',
+    version='0.0.20',
     packages=find_packages(),
     license='MIT',
     author='小派精灵',
     author_email='3383716176@qq.com',
     description='小派精灵手机自动化',
     classifiers=[
         "Programming Language :: Python :: 3",
```

