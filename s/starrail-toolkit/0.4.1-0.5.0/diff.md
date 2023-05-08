# Comparing `tmp/starrail-toolkit-0.4.1.tar.gz` & `tmp/starrail-toolkit-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrail-toolkit-0.4.1.tar", last modified: Thu May  4 18:30:41 2023, max compression
+gzip compressed data, was "starrail-toolkit-0.5.0.tar", last modified: Mon May  8 13:30:27 2023, max compression
```

## Comparing `starrail-toolkit-0.4.1.tar` & `starrail-toolkit-0.5.0.tar`

### file list

```diff
@@ -1,45 +1,58 @@
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 18:30:41.691133 starrail-toolkit-0.4.1/
--rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/LICENSE
--rw-r--r--   0 littlenyima   (501) staff       (20)     4593 2023-05-04 18:30:41.690971 starrail-toolkit-0.4.1/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     4086 2023-05-04 18:22:59.000000 starrail-toolkit-0.4.1/README.md
--rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-04 18:30:41.691312 starrail-toolkit-0.4.1/setup.cfg
--rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 18:30:41.686674 starrail-toolkit-0.4.1/starrail/
--rw-r--r--   0 littlenyima   (501) staff       (20)      724 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      996 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/config.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 18:30:41.687245 starrail-toolkit-0.4.1/starrail/entry/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/entry/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1581 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/entry/cli.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      285 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/entry/gui.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1301 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/entry/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 18:30:41.688566 starrail-toolkit-0.4.1/starrail/gacha/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/gacha/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3636 2023-05-04 18:29:24.000000 starrail-toolkit-0.4.1/starrail/gacha/autodet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/gacha/database.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      806 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/gacha/fetch.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5178 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/gacha/fileio.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5088 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/gacha/parse.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3400 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/gacha/service.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/gacha/type.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3448 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/gacha/url.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 18:30:41.688840 starrail-toolkit-0.4.1/starrail/gui/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/gui/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      183 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/gui/application.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 18:30:41.689234 starrail-toolkit-0.4.1/starrail/utils/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/utils/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)        6 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/utils/auto_update.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 18:30:41.689885 starrail-toolkit-0.4.1/starrail/utils/babelfish/
--rw-r--r--   0 littlenyima   (501) staff       (20)      408 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/utils/babelfish/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1387 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/utils/babelfish/dictionary.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      373 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/utils/babelfish/locale.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      586 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/utils/babelfish/multilingual.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/utils/babelfish/translate.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/utils/loggings.py
--rw-r--r--   0 littlenyima   (501) staff       (20)       22 2023-05-04 18:28:29.000000 starrail-toolkit-0.4.1/starrail/version.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 18:30:41.690749 starrail-toolkit-0.4.1/starrail_toolkit.egg-info/
--rw-r--r--   0 littlenyima   (501) staff       (20)     4593 2023-05-04 18:30:41.000000 starrail-toolkit-0.4.1/starrail_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)      974 2023-05-04 18:30:41.000000 starrail-toolkit-0.4.1/starrail_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-04 18:30:41.000000 starrail-toolkit-0.4.1/starrail_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-04 18:30:41.000000 starrail-toolkit-0.4.1/starrail_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       46 2023-05-04 18:30:41.000000 starrail-toolkit-0.4.1/starrail_toolkit.egg-info/requires.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-04 18:30:41.000000 starrail-toolkit-0.4.1/starrail_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:30:27.334499 starrail-toolkit-0.5.0/
+-rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/LICENSE
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4970 2023-05-08 13:30:27.334332 starrail-toolkit-0.5.0/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4463 2023-05-08 13:29:19.000000 starrail-toolkit-0.5.0/README.md
+-rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-08 13:30:27.334546 starrail-toolkit-0.5.0/setup.cfg
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:30:27.328420 starrail-toolkit-0.5.0/starrail/
+-rw-r--r--   0 littlenyima   (501) staff       (20)      724 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1763 2023-05-08 13:18:40.000000 starrail-toolkit-0.5.0/starrail/config.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:30:27.329106 starrail-toolkit-0.5.0/starrail/entry/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/entry/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1803 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/entry/cli.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      965 2023-05-07 04:25:56.000000 starrail-toolkit-0.5.0/starrail/entry/gui.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1301 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/entry/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:30:27.330488 starrail-toolkit-0.5.0/starrail/gacha/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/gacha/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3636 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/gacha/autodet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/gacha/database.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      806 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/gacha/fetch.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5178 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/gacha/fileio.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5078 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/gacha/parse.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3572 2023-05-08 11:35:55.000000 starrail-toolkit-0.5.0/starrail/gacha/service.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/gacha/type.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/gacha/url.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:30:27.330767 starrail-toolkit-0.5.0/starrail/gui/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/gui/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5870 2023-05-07 10:02:46.000000 starrail-toolkit-0.5.0/starrail/gui/application.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:30:27.331291 starrail-toolkit-0.5.0/starrail/gui/common/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:18:00.000000 starrail-toolkit-0.5.0/starrail/gui/common/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      260 2023-05-07 10:02:46.000000 starrail-toolkit-0.5.0/starrail/gui/common/icon.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      563 2023-05-08 06:27:44.000000 starrail-toolkit-0.5.0/starrail/gui/common/stylesheet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      333 2023-05-08 13:22:41.000000 starrail-toolkit-0.5.0/starrail/gui/common/utils.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:30:27.332101 starrail-toolkit-0.5.0/starrail/gui/interfaces/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:17:51.000000 starrail-toolkit-0.5.0/starrail/gui/interfaces/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1842 2023-05-07 10:02:59.000000 starrail-toolkit-0.5.0/starrail/gui/interfaces/base.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)    13038 2023-05-08 13:22:17.000000 starrail-toolkit-0.5.0/starrail/gui/interfaces/gacha_sync.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2520 2023-05-07 05:24:37.000000 starrail-toolkit-0.5.0/starrail/gui/interfaces/home.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2373 2023-05-07 09:07:50.000000 starrail-toolkit-0.5.0/starrail/gui/interfaces/setting.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      372 2023-05-07 10:02:48.000000 starrail-toolkit-0.5.0/starrail/gui/interfaces/users.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:30:27.332479 starrail-toolkit-0.5.0/starrail/utils/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/utils/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)        6 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/utils/auto_update.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:30:27.333336 starrail-toolkit-0.5.0/starrail/utils/babelfish/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2155 2023-05-08 12:49:28.000000 starrail-toolkit-0.5.0/starrail/utils/babelfish/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      144 2023-05-07 05:10:36.000000 starrail-toolkit-0.5.0/starrail/utils/babelfish/constants.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4541 2023-05-08 12:49:28.000000 starrail-toolkit-0.5.0/starrail/utils/babelfish/dictionary.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      373 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/utils/babelfish/locale.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      586 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/utils/babelfish/multilingual.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/utils/babelfish/translate.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/utils/loggings.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)       22 2023-05-08 13:13:31.000000 starrail-toolkit-0.5.0/starrail/version.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:30:27.334134 starrail-toolkit-0.5.0/starrail_toolkit.egg-info/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4970 2023-05-08 13:30:27.000000 starrail-toolkit-0.5.0/starrail_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1341 2023-05-08 13:30:27.000000 starrail-toolkit-0.5.0/starrail_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-08 13:30:27.000000 starrail-toolkit-0.5.0/starrail_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-08 13:30:27.000000 starrail-toolkit-0.5.0/starrail_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       46 2023-05-08 13:30:27.000000 starrail-toolkit-0.5.0/starrail_toolkit.egg-info/requires.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-08 13:30:27.000000 starrail-toolkit-0.5.0/starrail_toolkit.egg-info/top_level.txt
```

### Comparing `starrail-toolkit-0.4.1/LICENSE` & `starrail-toolkit-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.1/PKG-INFO` & `starrail-toolkit-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.4.1
+Version: 0.5.0
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,32 +12,37 @@
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 《崩坏：星穹铁道》工具箱
 
 <div align="center">
-<img src="https://s1.ax1x.com/2023/04/30/p98Cv26.png" alt="logo" />
+<img src="https://s1.ax1x.com/2023/05/06/p9atspD.png" alt="logo" />
 </div>
 
+
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 |
 | :--------: | :----------: | :-------: |
-|   0.4.0    |    0.4.1     |   0.4.1   |
+|   0.5.0    |    0.5.0     |   0.5.0   |
 
 - [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
 - [x] 支持命令行显示抽卡报告
 - [x] 支持导出 markdown 格式抽卡报告
 - [x] 支持导出网页版抽卡报告
 - [x] 支持中英文多语言导出
 - [x] 支持 Windows 平台游戏中自动检测 API URL
 - [ ] 实现用户界面并编译到 Windows 与 macOS 平台
 - [ ] 支持自动检查更新
 
+***BREAKING：目前用户界面的第一个版本已经实现完成，稍后将会编译到 Windows 平台，界面预览：***
+
+![gui_preview](https://s1.ax1x.com/2023/05/08/p90QWex.png)
+
 ## 安装方式
 
 目前仅提供命令行版本（*我会尽快编译一个可以直接下载运行的应用程序版本*），用户交互界面版本正在开发中。
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
@@ -60,15 +65,15 @@
 
 ### 获取抽卡查询 API URL
 
 请参考[【这个教程】](docs/how-to-get-api-url.md)获取查询链接。
 
 由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间（大约 24 小时）后过期，过期后需要重新获取。
 
-**注：若为 Windows 平台，可以使用本工具自动检测 API URL。** 首先登陆游戏，进入抽卡查询页面，当显示出一页抽卡查询结果后，运行本工具，即可检测到抽卡查询 URL。如果需要切换账号，建议使用上述教程中的方法获取每个账号的 API URL，以便精确控制导出的账号。
+**注：若为 Windows 平台，可以使用本工具自动检测 API URL。** 首先登陆游戏，进入抽卡查询页面，当显示出一页抽卡查询结果后，退出游戏（由于 Windows 系统文件占用问题，若不退出，可能导致缓存无法读取），运行本工具，即可检测到抽卡查询 URL。如果需要切换账号，建议使用上述教程中的方法获取每个账号的 API URL，以便精确控制导出的账号。
 
 ### 导出抽卡记录
 
 #### 命令行导出
 
 可以使用如下命令导出：
 
@@ -81,20 +86,17 @@
 
 **参数说明：**
 
 - `--api`：（Windows 平台可选）API URL 地址。若为 Windows 平台，可以不填这个参数，而使用自动检测功能。
 - `--export`：（可选）导出格式选项。默认为导出全部格式，若仅需导出部分格式，可以替换对应参数。目前支持的格式有 `csv`、`html`、`json`、`md`、`xlsx`。例如，若只需要 json 与 xlsx 格式数据，可以替换为 `--export json xlsx`。
 - `--locale`：（可选）控制输出语言。默认为输出简体中文，可选值为 `en`（英语）、`chs`（简体中文）。
 - `--log-level`：（可选）日志等级。控制日志的输出等级，默认为 `DEBUG`。若感觉输出的日志过多影响观感，建议将日志等级更改为 `INFO`，例如：`--log-level INFO`。（注意：若设置的日志等级过高，可能导致基本的信息无法显示，例如导出进度、导出位置、命令行版抽卡报告等）从高到低的可选值为 `CRITICAL`、`ERROR`、`WARNING`、`INFO`、`DEBUG`。
+- `--request-interval`：（可选）请求间隔。两次请求之间的最小间隔，默认为 `0.1`。若某些情况下因请求过于频繁导致 IP 被 ban，可以适度把这个值调大一点。
 
-本项目目前正处于快速迭代阶段，使用方式可能会发生改变，更新时请留意本部分关于使用方式的说明。
-
-### Troubleshooting
-
-- 遇到 `PermissionError: [Errno 13] Permission denied`：应该是因为缓存文件被占用，建议退出游戏后重试。
+本项目目前正处于快速迭代阶段，使用方式可能会发生改变，请及时更新程序，更新时请留意本部分关于使用方式的说明。
 
 ## 导出结果示例
 
 - Excel 结果示例（为保护隐私已隐藏部分信息）
 
   <img src="https://s1.ax1x.com/2023/05/02/p9GJKts.png" alt="xlsx" style="width: 600px;" />
```

### Comparing `starrail-toolkit-0.4.1/README.md` & `starrail-toolkit-0.5.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # 《崩坏：星穹铁道》工具箱
 
 <div align="center">
-<img src="https://s1.ax1x.com/2023/04/30/p98Cv26.png" alt="logo" />
+<img src="https://s1.ax1x.com/2023/05/06/p9atspD.png" alt="logo" />
 </div>
 
+
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 |
 | :--------: | :----------: | :-------: |
-|   0.4.0    |    0.4.1     |   0.4.1   |
+|   0.5.0    |    0.5.0     |   0.5.0   |
 
 - [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
 - [x] 支持命令行显示抽卡报告
 - [x] 支持导出 markdown 格式抽卡报告
 - [x] 支持导出网页版抽卡报告
 - [x] 支持中英文多语言导出
 - [x] 支持 Windows 平台游戏中自动检测 API URL
 - [ ] 实现用户界面并编译到 Windows 与 macOS 平台
 - [ ] 支持自动检查更新
 
+***BREAKING：目前用户界面的第一个版本已经实现完成，稍后将会编译到 Windows 平台，界面预览：***
+
+![gui_preview](https://s1.ax1x.com/2023/05/08/p90QWex.png)
+
 ## 安装方式
 
 目前仅提供命令行版本（*我会尽快编译一个可以直接下载运行的应用程序版本*），用户交互界面版本正在开发中。
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
@@ -45,15 +50,15 @@
 
 ### 获取抽卡查询 API URL
 
 请参考[【这个教程】](docs/how-to-get-api-url.md)获取查询链接。
 
 由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间（大约 24 小时）后过期，过期后需要重新获取。
 
-**注：若为 Windows 平台，可以使用本工具自动检测 API URL。** 首先登陆游戏，进入抽卡查询页面，当显示出一页抽卡查询结果后，运行本工具，即可检测到抽卡查询 URL。如果需要切换账号，建议使用上述教程中的方法获取每个账号的 API URL，以便精确控制导出的账号。
+**注：若为 Windows 平台，可以使用本工具自动检测 API URL。** 首先登陆游戏，进入抽卡查询页面，当显示出一页抽卡查询结果后，退出游戏（由于 Windows 系统文件占用问题，若不退出，可能导致缓存无法读取），运行本工具，即可检测到抽卡查询 URL。如果需要切换账号，建议使用上述教程中的方法获取每个账号的 API URL，以便精确控制导出的账号。
 
 ### 导出抽卡记录
 
 #### 命令行导出
 
 可以使用如下命令导出：
 
@@ -66,20 +71,17 @@
 
 **参数说明：**
 
 - `--api`：（Windows 平台可选）API URL 地址。若为 Windows 平台，可以不填这个参数，而使用自动检测功能。
 - `--export`：（可选）导出格式选项。默认为导出全部格式，若仅需导出部分格式，可以替换对应参数。目前支持的格式有 `csv`、`html`、`json`、`md`、`xlsx`。例如，若只需要 json 与 xlsx 格式数据，可以替换为 `--export json xlsx`。
 - `--locale`：（可选）控制输出语言。默认为输出简体中文，可选值为 `en`（英语）、`chs`（简体中文）。
 - `--log-level`：（可选）日志等级。控制日志的输出等级，默认为 `DEBUG`。若感觉输出的日志过多影响观感，建议将日志等级更改为 `INFO`，例如：`--log-level INFO`。（注意：若设置的日志等级过高，可能导致基本的信息无法显示，例如导出进度、导出位置、命令行版抽卡报告等）从高到低的可选值为 `CRITICAL`、`ERROR`、`WARNING`、`INFO`、`DEBUG`。
+- `--request-interval`：（可选）请求间隔。两次请求之间的最小间隔，默认为 `0.1`。若某些情况下因请求过于频繁导致 IP 被 ban，可以适度把这个值调大一点。
 
-本项目目前正处于快速迭代阶段，使用方式可能会发生改变，更新时请留意本部分关于使用方式的说明。
-
-### Troubleshooting
-
-- 遇到 `PermissionError: [Errno 13] Permission denied`：应该是因为缓存文件被占用，建议退出游戏后重试。
+本项目目前正处于快速迭代阶段，使用方式可能会发生改变，请及时更新程序，更新时请留意本部分关于使用方式的说明。
 
 ## 导出结果示例
 
 - Excel 结果示例（为保护隐私已隐藏部分信息）
 
   <img src="https://s1.ax1x.com/2023/05/02/p9GJKts.png" alt="xlsx" style="width: 600px;" />
```

### Comparing `starrail-toolkit-0.4.1/setup.py` & `starrail-toolkit-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.1/starrail/__init__.py` & `starrail-toolkit-0.5.0/starrail/__init__.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.1/starrail/entry/setup.py` & `starrail-toolkit-0.5.0/starrail/entry/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.1/starrail/gacha/autodet.py` & `starrail-toolkit-0.5.0/starrail/gacha/autodet.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.1/starrail/gacha/database.py` & `starrail-toolkit-0.5.0/starrail/gacha/database.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.1/starrail/gacha/fetch.py` & `starrail-toolkit-0.5.0/starrail/gacha/fetch.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.1/starrail/gacha/fileio.py` & `starrail-toolkit-0.5.0/starrail/gacha/fileio.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.1/starrail/gacha/parse.py` & `starrail-toolkit-0.5.0/starrail/gacha/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         total_items = len(self.data)
         if not total_items or not count:
             return dict(
                 rank_type=rank_type,
                 count='0',
                 basic_prob='',
                 compr_prob='',
-                since_last='0',
+                since_last='',
                 attempts=[],
                 average='',
             )
         if rank_type == '3':
             return dict(
                 rank_type=rank_type,
                 count=f'{count}',
@@ -98,16 +98,16 @@
 class GachaDataManager:
 
     def __init__(self, uid):
         self.uid = uid
         self.gacha = self.load_cache(uid)
 
     def load_cache(self, uid: str):
-        cache_dir = cfg.cache_dir
-        self.cache_path = os.path.join(cache_dir, f'{uid}.sqlite3')
+        db_dir = cfg.db_dir
+        self.cache_path = os.path.join(db_dir, f'{uid}.sqlite3')
         if os.path.isfile(self.cache_path):
             return parse_cache_from_sql(self.cache_path)
         return init_empty_gacha_record()
 
     def log_stats(self):
         # a simple version
         fileds = ['Type', 'Count', 'Basic Prob.', ' True Prob.', 'Since Last']
```

### Comparing `starrail-toolkit-0.4.1/starrail/gacha/service.py` & `starrail-toolkit-0.5.0/starrail/gacha/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import time
 from datetime import datetime
 
 import starrail.gacha.fileio as fileio
 from starrail.gacha.autodet import detect_api_url
 from starrail.gacha.fetch import fetch_json
 from starrail.gacha.parse import GachaDataManager
 from starrail.gacha.type import GachaType
@@ -36,34 +37,39 @@
             f'Length of payload.data.list: '
             f'{len(payload["data"]["list"])}',
         )
         return False
     return True
 
 
-def export_gacha_type(api_template: str, gacha_type: GachaType):
+def export_gacha_type(
+    api_template: str,
+    gacha_type: GachaType,
+    request_interval: float,
+):
     r = []
     end_id = '0'
     for page in integers():
         logger.info(f'Downloading page {page} of type {gacha_type.name}')
         api_url = get_api_url(
             api_template, end_id, str(gacha_type.value),
             str(page), '5',
         )
         logger.debug(f'Requesting {api_url}')
         response, code = fetch_json(api_url)
+        time.sleep(request_interval)
         if not check_response(response, code):
             break
         data_list = response['data']['list']
         r.extend(data_list)
         end_id = data_list[-1]['id']
     return r
 
 
-def export_gacha_from_api(api_url, export):
+def export_gacha_from_api(api_url, export, request_interval):
     if not api_url:
         api_url = detect_api_url()
     response, code = fetch_json(api_url)
     valid = check_response(response, code)
     if not valid:
         logger.fatal('Error while checking response from api URL, exitting')
         raise ValueError('Invalid or expired api, please check your input')
@@ -72,15 +78,19 @@
 
     uid = response['data']['list'][0]['uid']
     manager = GachaDataManager(uid)
     logger.info(f'Successfully connected to cache of uid {uid}')
     manager.log_stats()
 
     for gacha_type in GachaType:
-        records = export_gacha_type(api_template, gacha_type)
+        records = export_gacha_type(
+            api_template,
+            gacha_type,
+            request_interval,
+        )
         manager.add_records(gacha_type.value, records)
         manager.gacha[gacha_type.value].sort()
         logger.info(f'Finish downloading records of {gacha_type.name}')
 
     fileio.export_as_sql(manager, manager.cache_path)
 
     manager.log_stats()
```

### Comparing `starrail-toolkit-0.4.1/starrail/gacha/url.py` & `starrail-toolkit-0.5.0/starrail/gacha/url.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     Returns:
         str: A new URL string with the cleaned query parameters
     """
 
     parse = urlparse(url)
     query_dict = parse_qs(parse.query)
     query_dict = get_clean_query_dict(query_dict)
+    pop_if_exist(query_dict, 'begin_id')
     pop_if_exist(query_dict, 'end_id')
     pop_if_exist(query_dict, 'gacha_type')
     pop_if_exist(query_dict, 'page')
     pop_if_exist(query_dict, 'size')
     new_query = urlencode(query_dict, doseq=True)
     return urlunparse((
         parse.scheme, parse.netloc, parse.path, parse.params,
```

### Comparing `starrail-toolkit-0.4.1/starrail/utils/babelfish/multilingual.py` & `starrail-toolkit-0.5.0/starrail/utils/babelfish/multilingual.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.1/starrail/utils/loggings.py` & `starrail-toolkit-0.5.0/starrail/utils/loggings.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.1/starrail_toolkit.egg-info/PKG-INFO` & `starrail-toolkit-0.5.0/starrail_toolkit.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.4.1
+Version: 0.5.0
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,32 +12,37 @@
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 《崩坏：星穹铁道》工具箱
 
 <div align="center">
-<img src="https://s1.ax1x.com/2023/04/30/p98Cv26.png" alt="logo" />
+<img src="https://s1.ax1x.com/2023/05/06/p9atspD.png" alt="logo" />
 </div>
 
+
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 |
 | :--------: | :----------: | :-------: |
-|   0.4.0    |    0.4.1     |   0.4.1   |
+|   0.5.0    |    0.5.0     |   0.5.0   |
 
 - [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
 - [x] 支持命令行显示抽卡报告
 - [x] 支持导出 markdown 格式抽卡报告
 - [x] 支持导出网页版抽卡报告
 - [x] 支持中英文多语言导出
 - [x] 支持 Windows 平台游戏中自动检测 API URL
 - [ ] 实现用户界面并编译到 Windows 与 macOS 平台
 - [ ] 支持自动检查更新
 
+***BREAKING：目前用户界面的第一个版本已经实现完成，稍后将会编译到 Windows 平台，界面预览：***
+
+![gui_preview](https://s1.ax1x.com/2023/05/08/p90QWex.png)
+
 ## 安装方式
 
 目前仅提供命令行版本（*我会尽快编译一个可以直接下载运行的应用程序版本*），用户交互界面版本正在开发中。
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
@@ -60,15 +65,15 @@
 
 ### 获取抽卡查询 API URL
 
 请参考[【这个教程】](docs/how-to-get-api-url.md)获取查询链接。
 
 由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间（大约 24 小时）后过期，过期后需要重新获取。
 
-**注：若为 Windows 平台，可以使用本工具自动检测 API URL。** 首先登陆游戏，进入抽卡查询页面，当显示出一页抽卡查询结果后，运行本工具，即可检测到抽卡查询 URL。如果需要切换账号，建议使用上述教程中的方法获取每个账号的 API URL，以便精确控制导出的账号。
+**注：若为 Windows 平台，可以使用本工具自动检测 API URL。** 首先登陆游戏，进入抽卡查询页面，当显示出一页抽卡查询结果后，退出游戏（由于 Windows 系统文件占用问题，若不退出，可能导致缓存无法读取），运行本工具，即可检测到抽卡查询 URL。如果需要切换账号，建议使用上述教程中的方法获取每个账号的 API URL，以便精确控制导出的账号。
 
 ### 导出抽卡记录
 
 #### 命令行导出
 
 可以使用如下命令导出：
 
@@ -81,20 +86,17 @@
 
 **参数说明：**
 
 - `--api`：（Windows 平台可选）API URL 地址。若为 Windows 平台，可以不填这个参数，而使用自动检测功能。
 - `--export`：（可选）导出格式选项。默认为导出全部格式，若仅需导出部分格式，可以替换对应参数。目前支持的格式有 `csv`、`html`、`json`、`md`、`xlsx`。例如，若只需要 json 与 xlsx 格式数据，可以替换为 `--export json xlsx`。
 - `--locale`：（可选）控制输出语言。默认为输出简体中文，可选值为 `en`（英语）、`chs`（简体中文）。
 - `--log-level`：（可选）日志等级。控制日志的输出等级，默认为 `DEBUG`。若感觉输出的日志过多影响观感，建议将日志等级更改为 `INFO`，例如：`--log-level INFO`。（注意：若设置的日志等级过高，可能导致基本的信息无法显示，例如导出进度、导出位置、命令行版抽卡报告等）从高到低的可选值为 `CRITICAL`、`ERROR`、`WARNING`、`INFO`、`DEBUG`。
+- `--request-interval`：（可选）请求间隔。两次请求之间的最小间隔，默认为 `0.1`。若某些情况下因请求过于频繁导致 IP 被 ban，可以适度把这个值调大一点。
 
-本项目目前正处于快速迭代阶段，使用方式可能会发生改变，更新时请留意本部分关于使用方式的说明。
-
-### Troubleshooting
-
-- 遇到 `PermissionError: [Errno 13] Permission denied`：应该是因为缓存文件被占用，建议退出游戏后重试。
+本项目目前正处于快速迭代阶段，使用方式可能会发生改变，请及时更新程序，更新时请留意本部分关于使用方式的说明。
 
 ## 导出结果示例
 
 - Excel 结果示例（为保护隐私已隐藏部分信息）
 
   <img src="https://s1.ax1x.com/2023/05/02/p9GJKts.png" alt="xlsx" style="width: 600px;" />
```

### Comparing `starrail-toolkit-0.4.1/starrail_toolkit.egg-info/SOURCES.txt` & `starrail-toolkit-0.5.0/starrail_toolkit.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -15,18 +15,29 @@
 starrail/gacha/fileio.py
 starrail/gacha/parse.py
 starrail/gacha/service.py
 starrail/gacha/type.py
 starrail/gacha/url.py
 starrail/gui/__init__.py
 starrail/gui/application.py
+starrail/gui/common/__init__.py
+starrail/gui/common/icon.py
+starrail/gui/common/stylesheet.py
+starrail/gui/common/utils.py
+starrail/gui/interfaces/__init__.py
+starrail/gui/interfaces/base.py
+starrail/gui/interfaces/gacha_sync.py
+starrail/gui/interfaces/home.py
+starrail/gui/interfaces/setting.py
+starrail/gui/interfaces/users.py
 starrail/utils/__init__.py
 starrail/utils/auto_update.py
 starrail/utils/loggings.py
 starrail/utils/babelfish/__init__.py
+starrail/utils/babelfish/constants.py
 starrail/utils/babelfish/dictionary.py
 starrail/utils/babelfish/locale.py
 starrail/utils/babelfish/multilingual.py
 starrail/utils/babelfish/translate.py
 starrail_toolkit.egg-info/PKG-INFO
 starrail_toolkit.egg-info/SOURCES.txt
 starrail_toolkit.egg-info/dependency_links.txt
```

